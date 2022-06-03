# 크롬 개발자 툴의 단축키

[크롬 개발자 툴의 단축키 항목 바로가기](https://developer.chrome.com/docs/devtools/shortcuts/)
[크롬 단축키로 시간 벌기](https://www.google.com/chrome/tips/#shortcuts)

이 페이지는 Chrome DevTools의 키보드 단축키에 대한 참조입니다.

# DevTools 열기를 위한 키보드 단축키
DevTools를 열려면 브라우저 뷰포트에 커서가 있는 동안 다음 키보드 단축키를 누르십시오.
센스리더에서는 충돌되는 키는 Control + Shift + N (기능키 무시)를 한번 누른 후에 단축키를 실행해야 합니다. 
별도의 환경설정 chrome.Chrome_WidgetWin_1에서 키를 수정해도 될 것 같습니다.

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
마지막 사용한 패널 열기 | Command + Option + I | F12 또는 Control + Shift + I
콘솔 패널 열기 | Command + Option + J | Control + Shift + J
요소 패널 열기 | Command + Shift + C  또는 Command + Option + C | Control + Shift + C

# 전역 키보드 단축키
다음 키보드 단축키는 대부분의 DevTools 패널에서 사용할 수 있습니다.

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
설정 표시 | ? 또는 Function + F1 | ? 또는 F1
다음 패널에 초점 맞추기 | Command + ] | Control + ]
이전 패널에 초점 맞추기 | Command + [ | Control + [
마지막으로 사용한 도킹 위치로 다시 전환 함. <br>DevTools가 전체 세션의 기본 위치에 있는 경우 이 바로 가기는 DevTools를 별도의 창에 도킹 해제함. | Command + Shift + D | Control + Shift + D
장치 모드 전환 | Command + Shift + M | Control + Shift + M
요소 검사 모드 전환 | Command + Shift + C | Control + Shift + C
명령 메뉴 열기 | Command + Shift + P | Control + Shift + P
서랍 토글 | Escape | Escape
새로고침 | Command + R | F5 또는 Control + R
<strong style="color:crimson; font-weight:600;">강력 새로고침<strong> | Command + Shift + R | Control + F5 또는 Control + Shift + R
현재 패널 내에서 텍스트를 검색함. 감사 , 애플리케이션 및 보안 패널 에서 지원되지 않음 | Command + F | Control + F
로드된 모든 리소스에서 텍스트를 검색할 수 있는 서랍 에서 검색 탭을 엽니다. | Command + Option + F | Control + Shift + F
소스 패널 에서 파일 열기 | Command + O 또는 Command + P | Control + O 또는 Control + P
확대 | Command + Shift + + | Control + Shift + + 
축소 | Command + - | Control + -
기본 확대 / 축소 수준 복원 | Command + 0 | Control + 0
스니펫 실행 | Command + O를 눌러 명령 메뉴! 를 열고 스크립트 이름을 입력 한 다음Enter | Control + O를 눌러 명령 메뉴! 를 열고 스크립트 이름을 입력 한 다음Enter

# 요소 패널 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
변경 취소 | Command + Z | Control + Z
변경 다시 실행 | Command + Shift + Z | Control + Y
현재 선택된 요소 위 / 아래 요소 선택 | UpArrow / DownArrow | UpArrow / DownArrow
현재 선택된 노드를 확장함. 노드가 이미 확장된 경우 이 바로 가기는 그 아래에 있는 요소를 선택함. | RightArrow | RightArrow
현재 선택된 노드를 축소함. 노드가 이미 축소된 경우 이 바로 가기는 그 위에 있는 요소를 선택함. | Left Arrow | Left Arrow
현재 선택된 노드와 모든 하위 노드를 확장하거나 축소함. | 누른 Option상태에서 요소 이름 옆에 있는 화살표 아이콘을 클릭함. |  + 를 Control누른 Alt상태에서 요소 이름 옆에 있는 화살표 아이콘을 클릭함.
현재 선택된 요소에서 속성 편집 모드 전환 | Enter | Enter
속성 편집 모드로 들어간 후 다음 / 이전 속성 선택 | Tab / Shift + Tab | Tab / Shift + Tab
현재 선택된 요소 숨기기 | H | H
현재 선택된 요소에서 HTML 모드로 편집 토글 | Function + F2 | F2

# 스타일 창 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
속성 값이 선언된 줄로 이동 | 누른 Command상태에서 속성 값 클릭 | 누른 Control상태에서 속성 값 클릭
색상 값의 RBGA, HSLA 및 Hex 표현을 순환함. | 누른 상태에서 값 옆에 있는 색상 미리보기 Shift 상자 를 클릭함. | 누른 상태에서 값 옆에 있는 색상 미리보기 Shift 상자 를 클릭함.
다음 / 이전 속성  또는 값 선택 | Tab속성 이름  또는 값 클릭 후  / Shift + Tab를 누릅니다. | Tab속성 이름  또는 값 클릭 후  / Shift + 를 누릅니다.Tab
속성 값을 0.1씩 증가 / 감소 | Option값 클릭 후  + UpArrow / Option +DownArrow 를 누릅니다. | Alt값 클릭 후  + UpArrow / Alt + 를 누릅니다.DownArrow
속성 값을 1씩 증가 / 감소 | UpArrow값 클릭 후  / 를 누릅니다.DownArrow | UpArrow값 클릭 후  / 를 누릅니다.DownArrow
속성 값을 10씩 증가 / 감소 | Shift값 클릭 후  + UpArrow / Shift + 를 누릅니다.DownArrow | Shift값 클릭 후  + UpArrow / Shift + 를 누릅니다.DownArrow
속성 값을 100만큼 증가 / 감소 | Command값 클릭 후  + UpArrow / Command + 를 누릅니다.DownArrow | Control값 클릭 후  + UpArrow / Control + 를 누릅니다.DownArrow
각도 값의 도(deg), 그라디안(grad), 라디안(rad) 및 회전(회전) 표시를 순환함. | 누른 상태에서 값 옆에 있는 각도 미리보기Shift 상자 를 클릭함. | 누른 상태에서 값 옆에 있는 각도 미리보기Shift 상자 를 클릭함.
각도 값을 1씩 증가 / 감소 | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 UpArrow / DownArrow | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 UpArrow / DownArrow
각도 값을 10만큼 증가 / 감소 | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 Shift + UpArrow / Shift + 를 누릅니다.DownArrow | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 Shift + UpArrow / Shift + 를 누릅니다.DownArrow
각도 값을 15만큼 증가 / 감소 | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 을 누르고 각도 시계 오버레이Shift 를 클릭 / 마우스 슬라이드함. | 값 옆에 있는 각도 미리보기 상자를 클릭한 다음 을 누르고 각도 시계 오버레이Shift 를 클릭 / 마우스 슬라이드함.

# 소스 패널 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
스크립트 실행 일시 중지(현재 실행 중인 경우)  또는 재개(현재 일시 중지된 경우) | F8 또는 Command + \ | F8 또는 Control + \
다음 함수 호출 건너뛰기 | F10 또는 Command + ' | F10 또는 Control + '
다음 함수 호출로 이동 | F11 또는 Command + ; | F11 또는 Control + ;
현재 기능에서 벗어나기 | Shift + F11 또는 Command + Shift + ; | Shift + F11 또는 Control + Shift + ;
일시 중지된 동안 특정 코드 줄로 계속 | 누른 상태 Command에서 코드 줄을 클릭함. | 누른 상태 Control에서 코드 줄을 클릭함.
현재 선택된 프레임 아래 / 위에서 호출 프레임을 선택함. | Control + . / Control + , | Control + . / Control + ,
로컬 수정 사항에 대한 변경 사항 저장 | Command + S | Control + S
모든 변경 사항 저장 | Command + Option + S | Control + Alt + S
라인으로 이동 | Control + G | Control + G
현재 열려 있는 파일의 줄 번호로 점프 | Command + O를 눌러 명령 메뉴: 를 열고 줄 번호를 입력 한 다음Enter | Control + O를 눌러 명령 메뉴: 를 열고 행 번호를 입력 한 다음Enter
현재 열려 있는 파일의 열로 이동(예: 5행, 9열) | Command + O를 눌러 명령 메뉴: 를 열고 , 줄 번호, 또 다른 :, 열 번호를 차례로 입력한 다음Enter | Control + O를 눌러 명령 메뉴: 를 열고 , 줄 번호, 또 다른 :, 열 번호를 차례로 입력한 다음Enter
함수 선언(현재 열려 있는 파일이 HTML  또는 스크립트인 경우)  또는 규칙 세트(현재 열려 있는 파일이 스타일시트인 경우)로 이동 | Command + Shift + O을 누른 다음 선언 / 규칙 집합의 이름을 입력하거나 옵션 목록에서 선택함. | Control + Shift + O 를 누른 다음 선언 / 규칙 집합의 이름을 입력하거나 옵션 목록에서 선택함.
**<strong style="color:crimson; font-weight:600;">활성 탭 닫기</strong>** | Option + W | **Alt + W**

# 코드 편집기 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
커서까지 마지막 단어의 모든 문자 삭제 | Option + Delete | Control + Delete
코드 줄 중단점 추가  또는 제거 | 커서를 라인에 놓은 다음 Command + 를 누릅니다.B | 커서를 라인에 놓은 다음 Control + 를 누릅니다.B
일치하는 괄호로 이동 | Control + M | Control + M
한 줄 주석을 전환함. 여러 줄을 선택한 경우 DevTools는 각 줄의 시작 부분에 주석을 추가함. | Command +  / | Control +  / 
커서가 있는 단어의 다음 발생을 선택 / 선택 취소함. 각 발생은 동시에 강조 표시됩니다. | Command + D / Command + U | Control + D / Control + U

# 성능 패널 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
녹음 시작 / 중지 | Command + E | Control + E
녹음 저장 | Command + S | Control + S
녹음 로드 | Command + O | Control + O

# 메모리 패널 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
녹음 시작 / 중지 | Command + E | Control + E

# 콘솔 패널 키보드 단축키

동작 | 맥 | 윈도우 / 리눅스
-- | -- | --
자동 완성 제안 수락 | RightArrow 또는 Tab | RightArrow 또는 Tab
자동 완성 제안 거부 | Escape | Escape
이전 명세서 가져오기 | UpArrow | UpArrow
다음 명령문 가져오기 | DownArrow | DownArrow
**콘솔 에 집중** | Control + \` | Control + \`
<strong style="color:crimson; font-weight:600;">콘솔 지우기</strong> | Command + K 또는 Option + L | Control + L
**여러 줄 입력을 강제 실행** | Shift + Return | Shift + Enter
실행하다 | Return | Enter
콘솔에 기록된 개체의 모든 하위 속성을 확장함. | 누른 상태에서 확장Alt 을 클릭 함. | 누른 상태에서 확장Alt 을 클릭 함.