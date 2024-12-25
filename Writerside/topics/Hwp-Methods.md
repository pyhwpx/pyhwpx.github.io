# Hwp Instance Methods

아래와 같이 `Hwp` 클래스를 임포트하여 한/글 인스턴스를 생성할 수 있습니다.

```Python
from pyhwpx import Hwp

hwp = Hwp()
```

## 기본제공 메서드 목록

### `hwp.get_image_info(ctrl)`
이미지 ctrl의 원본 그림의 이름과
원본 그림의 크기 정보를 추출하는 메서드

#### 파라미터
- ctrl : 이미지의 컨트롤 객체(`IDHwpCtrlCode`). 커서를 이미지 앞으로 옮기거나, 선택상태와 무관하게 컨트롤 객체만 특정할 수 있다면 이미지의 크기와 삽입 당시의 파일명을 추출할 수 있다. 
#### 사용방법 {collapsible="true"}
<tabs>
    <tab title="예시코드">
<code-block lang="py">
from pyhwpx import Hwp

hwp = Hwp()
hwp.get_image_info(hwp.ctrl_list[0])
</code-block>
    </tab>
    <tab title="실행 후 화면">
        <img src="001.png" alt="get_image_info result" />
</tab>
</tabs>

