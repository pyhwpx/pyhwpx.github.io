# Quickstart

이 페이지에서는 아래아한글을 자동화하기 위한 pyhwpx 모듈의 간단한 
사용법을 요약하여 보여드립니다. `pip install pyhwpx`로 모듈을 
설치해주세요.

2025년 3월 5일 수요일!

<note>pyhwpx는 윈도우 버전에서만 작동합니다.</note>

## 1. 코드 작성 및 실행방법

`pyhwpx`로 아래아한글을 실행하는 방법은 굉장히 간단합니다.

```python
from pyhwpx import Hwp
hwp = Hwp()  # 가장 최근에 활성화한 한/글 창에 연결합니다. 한/글이 실행되어 있지 않다면 새 창을 생성합니다.
hwp.open("FileName.hwp")  # 현재 작업디렉토리의 `FileName.hwp` 문서를 불러옵니다.
hwp.open(r"C:\path\to\file.hwpx")  # 경로 문자열에 역슬래시를 사용하기 위해서는 따옴표 왼쪽에 
`r`을 붙여줘야 합니다.
hwp.Quit()  # 한/글을 종료합니다.
```

만약 두 개 이상의 문서를 열어놓고 상호작용해야 한다면
아래와 같은 방법으로 창이나 탭을 추가할 수 있습니다.

```python
from pyhwpx import Hwp

hwp = Hwp()

hwp.add_doc()  # 한/글 창을 하나 더 추가합니다. (두 번째 창이 활성화된 상태입니다.)
hwp.open("first_doc.hwp")  # 두 번째 창에 문서를 불러옵니다.
hwp.switch_to(0)  # 다시 첫 번째 한/글 창을 활성화합니다.
hwp.CopyPage()  # `쪽 복사` 기능을 실행합니다.
hwp.switch_to(1)  # 두 번째 창을 활성화하고
hwp.PastePage()  # `쪽 붙이기` 기능을 실행합니다.
hwp.save_as("result.hwp")  # 다른이름으로 저장합니다.

hwp.FileClose()  # 두 번째 문서창을 닫습니다. (창도 종료됩니다.)
hwp.switch_to(0)  # 첫 번째 창을 활성화하고
hwp.Close()  # 문서편집을 종료하지만, 창은 `빈 문서`로 열린 상태입니다.
hwp.Quit()  # 한/글을 종료합니다.
```

## 2. 한/글 기능 실행방법

한/글에는 `복사`나 `붙여넣기`, `글자 입력`처럼 간단한 기능에서부터, 
`문단모양 설정`이나 `스타일 변경`처럼 다양한 매개변수를 필요로 하는 복잡한 기능까지 
다양하게 제공하고 있습니다.

### 2-1. 메서드 방식

단순하거나 매개변수 갯수가 적은 기능들, 
비교적 자주 사용되는 기능들은 
아래 방식으로 실행 가능합니다.

```Python
hwp.insert_text("Hello world!")  # 문자열 입력
hwp.BreakPara()  # 줄바꿈(엔터)
hwp.create_table(3, 5, treat_as_char=True)  # 3행5열의 표 생성(글자처럼 취급) 
```

> `pyhwpx`의 메서드 명명규칙은 특이하게 `PascalCase`와 `snake_case` 두 가지를 사용하고 있습니다. ~~무식해 보이는 이런 명명규칙에도~~
> ~~나름의 기준이 있기는 한데,~~ 한/글 API 의 기능을 그대로
> 사용한 경우 파스칼케이스를, API 외에 임의로 추가했거나, 커스텀 매개변수나 기능을 부여한 경우에는 스네이크케이스를 쓰고 있습니다.  
> 향후 버전에는 둘 다 사용 가능하게(혹은 한 쪽으로 통일하는 방향으로?) 리팩토링할 예정입니다.

### 2-2. 매크로 방식

매개변수가 많거나, 활용도가 높지 않다고 판단된 기능들은 아래 방식으로 실행 가능합니다. 
(순차적으로 메서드 방식으로 실행 가능할 수 있게 작업중입니다.)

아래 코드는 문단모양을 변경하는 예시입니다. 
변경내용이 많아서 복잡해 보이지만 
실행에 필요한 코드는 첫 두 줄과 마지막 한 줄 뿐입니다. 

```Python
pse = hwp.HParameterSet.HParaShape  # 비어있는 문단모양 파라미터셋 생성
hwp.HAction.GetDefault("ParagraphShape", pset.HSet)  # 현재값으로 파라미터셋 초기화 
pset.AlignType = hwp.HAlign("Center")  # 정렬 방식 : 가운데정렬
pset.RightMargin = hwp.PointToHwpUnit(20.0)  # 문단 왼쪽 여백 10pt
pset.LeftMargin = hwp.PointToHwpUnit(20.0)  # 문단 오른쪽 여백 10pt
hwp.HAction.Execute("ParagraphShape", pset.HSet)  # 변경 파라미터셋을 문서에 적용
```

사실 위의 코드는 아래아한글의 스크립트매크로를 복사한 후 문법만 파이썬에 맞게 변경했을 뿐입니다.
아래 코드는 녹화했던 스크립트매크로의 원본입니다.

```JavaScript
function OnScriptMacro_문단모양변경()
{
	HAction.GetDefault("ParagraphShape", HParameterSet.HParaShape.HSet);
	with (HParameterSet.HParaShape)
	{
		AlignType = HAlign("Center");
		RightMargin = PointToHwpUnit(20.0);
		LeftMargin = PointToHwpUnit(20.0);
	}
	HAction.Execute("ParagraphShape", HParameterSet.HParaShape.HSet);
}
```

메서드나 액션아이디, 파라미터셋의 목록은 아래아한글 공식문서 또는 기능(작성예정) 페이지를 참고해주시기 바랍니다.