# Hwp Instance Methods

아래와 같이 `Hwp` 클래스를 임포트하여 한/글 인스턴스를 생성할 수 있습니다.

```Python
from pyhwpx import Hwp

hwp = Hwp()
```

## 기본제공 메서드 목록

### hwp.get_image_info(ctrl)
이미지 ctrl의 원본 그림의 이름과
원본 그림의 크기 정보를 추출하는 메서드

#### 파라미터

ctrl
: 이미지의 컨트롤 객체(`IDHwpCtrlCode`). 커서를 이미지 앞으로 옮기거나, 선택상태와 무관하게 컨트롤 객체만 특정할 수 있다면 이미지의 크기와 삽입 당시의 파일명을 추출할 수 있다.

#### 활용사례 {collapsible="true"}

<tabs>
    <tab title="소스코드">
<code-block lang="py">
from pyhwpx import Hwp

hwp = Hwp()
hwp.get_image_info(hwp.ctrl_list[0])
</code-block>
    </tab>
    <tab title="실행화면">
        <img src="001.png" alt="get_image_info result" />
</tab>
</tabs>

### `hwp.goto_style(style: Union[int, str])`

특정 스타일이 적용된 위치로 찾아가는 메서드.  
탐색은 문서아랫방향으로만 수행하며 현재위치 이후 해당 스타일이 없거나,
스타일이름/인덱스번호가 잘못된 경우 `False`를 리턴. 찾아가기 성공시 `True`를 리턴.

#### 파라미터

style: int|str
: 스타일인덱스(바탕글이 `0`)를 정수로 입력하거나, 스타일이름 문자열 입력 가능.

#### 사용방법 {collapsible="true"}

<tabs>
    <tab title="예시코드">
<code-block lang="Python">
# 모든 "개요 3" 스타일을 "개요 2" 스타일로 변경하는 코드
while hwp.goto_style("개요 3"):
    hwp.set_style("개요 2")
</code-block>
    </tab>
    <tab title="실행화면">
        <img src="style_change.gif" alt="get_image_info result" />
</tab>
</tabs>