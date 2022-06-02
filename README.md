# 🚦 Visual Studio Code 접근성 설정

### 이 문서를 읽는 방법

* 키보드 H 키 (헤딩간의 이동 키), Shift + H 키(이전 헤딩간의 이동 키)로 주 타이틀을 먼저 탐색하세요.
* 헤딩간의 이동 이후 화살표 상하좌우 키로 콘텐츠 내용을 탐색하시기 바랍니다.
* Visual Studio Code(이하 VSCode) : 영어로 "브스코드"
* 센스리더와 충돌나는 키는 모두 VScode 내부에서 <mark style="color:yellow;">**단축키 수정(Ctrl + K S)**</mark> 으로 바꿀 수 있습니다.
* VScode가 말을 잘 안들을 때 가상커서 해제(Ctrl + Shift + F12 키)를 한두번 천천히 반복하세요.

## 코딩의 문자열을 읽기  (Alt + Shift + Z : 단축키와 동일 )

VSCode 내의 코딩 특수 문자열을 모두 읽어주도록 하는 설정을 합니다.

마우스 오른쪽 키보드 키(오른쪽 Ctrl 키 옆의 왼쪽 첫번째 키)로 정의

1. <mark style="color:yellow;">**VSCode를 반드시 실행 상태**</mark>에서 <mark style="color:yellow;">**Ctrl + \\**</mark> 를 누룹니다.(센스리더 <mark style="color:yellow;">**환경설정 수정창**</mark>)
2. 도구(T) > 구두점 읽기목록(N) 메뉴를 실행합니다. (<mark style="color:yellow;">**Alt + T, N 키 실행**</mark>)
3. <mark style="color:yellow;">**화살표 위 / 아래**</mark> 키보드를 눌러서 이동해 보세요.
4. 일단 내용을 들어보시고 <mark style="color:yellow;">**마우스 오른쪽 키**</mark>(<mark style="color:yellow;">**오른쪽 Ctrl 키 바로 옆의 왼쪽 첫번째 키**</mark>)를 누르세요.
5. 화살표 위 / 아래 키보드를 눌러서 이동해 보세요.
6. 변경, 삭제, 추가 중에 <mark style="color:yellow;">**"추가"를 선택**</mark>합니다.
7. 다중선택 목록상자의 <mark style="color:yellow;">**모든 구두점**</mark>을 선택합니다. (선택은 Space 키)
8. 화살표 위 / 아래 키를 모두 눌러서 선택된 내용을 확인 합니다. (선택안됨이 없도록)
9. Tab 키 다음에는 이름(N) 입력 부분에 <mark style="color:yellow;">**"코딩읽기"**</mark>를 입력합니다.
10. <mark style="color:yellow;">**Enter 키**</mark>를 누르면 다중선택 목록상자에 추가됩니다.&#x20;
11. **Enter 키**를 누르면 구두점 읽기목록이 닫히고 센스리더 메인화면 이동합니다.
12. 음성설정(S) > 세부설정(D)으로 이동합니다.(<mark style="color:yellow;">**Alt + S, D 키 실행**</mark>)
13. "<mark style="color:yellow;">**선택 전체(A) 1 / 5 라디오버튼**</mark> = Alt+a" 상태에서 Tab 키 실행합니다.
14. 목록 중에 '구두점 읽기" 항목을 선택하고 스페이스 바를 눌러서 <mark style="color:yellow;">**"코딩읽기"**</mark>로 값을 변경합니다.
15. 파일(G) > 환경 다른 이름으로 저장(A)을 누룹니다.(<mark style="color:yellow;">**Alt + G, A 키 실행**</mark>)
16. 이름 편집 창에 <mark style="color:yellow;">**"\_\_\_VSCode"**</mark>로 입력하고 <mark style="color:yellow;">**"저장" 버튼을 클릭**</mark>하여 완성합니다.
17. 축하합니다.  박수 한번 치시고, 자신만의 소프트웨어 환경을 만들어 보세요.

## VSCode 주요 단축키 수정방법

#### "설정" 키 수정 (<mark style="color:yellow;">**Ctrl+,를 Ctrl+Alt+,**</mark>로 변경)

1. **바로 가기 키(Ctrl + K S)**를 누룹니다.
2. 검색창에 "2630개 키 바인딩 사전순으로 표시 편집창" 이 뜹니다.
3. 검색 편집창에 키보드로 _Ctrl_ , 를 누룹니다.
4. 탭 키를 두번 누르면 "키 바인딩 목록상자"에서 Enter 키를 누룹니다.
5. 화살표 상하 키로 탐색하시면 "workbench.action.openSettings, 제어+,, 기본값 "에서 정지합니다.
6. 키보드로 Enter키 후 단축키를 설정할 _<mark style="color:yellow;">**Ctrl + Alt + ,**</mark>_ 를 반드시 한번만 칩니다.(주의 해애햐 함)
7. 최종 Enter 키를 누르면 적용되고, "Ctrl + W"로 단축키 바로 가기 키 설정을 닫습니다.
8. 안되면 1번부터 다시 반복하세요.(될때까지 주의해서)

#### "모든 명령 표시" 키 수정(<mark style="color:yellow;">**Ctrl+Shift+P**</mark>를 <mark style="color:yellow;">Ctrl+Alt+P</mark>로 변경)

1. 바로 가기 키(Ctrl + K S)를 누룹니다.
2. 검색창에 "2630개 키 바인딩 사전순으로 표시 편집창" 이 뜹니다.
3. 검색 편집창에 키보드로 _Ctrl_ Shift P 를 누룹니다.
4. 탭 키를 두번 누르면 "키 바인딩 목록상자"에서 Enter 키를 누룹니다.
5. 화살표 상하 키로 탐색하시면 "모든 명령 표시"에서 정지합니다.
6. 키보드로 Enter키 후 단축키를 설정할 _<mark style="color:yellow;">**Ctrl + Alt + P**</mark>_를 반드시 한번만 칩니다.(주의 해애햐 함)
7. 최종 Enter 키를 누르면 적용되고, "Ctrl + W"로 단축키 바로 가기 키 설정을 닫습니다.
8. 안되면 1번부터 다시 반복하세요.(될때까지 주의해서)

#### "탐색기" 키 수정 (<mark style="color:yellow;">Ctrl+Shift+E</mark>를 <mark style="color:yellow;">Ctrl+Alt+E</mark>로 변경)

1. 바로 가기 키(Ctrl + K S)를 누룹니다.
2. 검색창에 "2630개 키 바인딩 사전순으로 표시 편집창" 이 뜹니다.
3. 검색 편집창에 키보드로 _Ctrl_ Shift E 를 누룹니다.
4. 탭 키를 두번 누르면 "키 바인딩 목록상자"에서 Enter 키를 누룹니다.
5. 화살표 상하 키로 탐색하시면 "탐색기 표시, 제어+ Shift+E, 기본값viewContainer.workbench.view.explorer.enabled "에서 정지합니다.
6. 키보드로 Enter키 후 단축키를 설정할 _<mark style="color:yellow;">**Ctrl + Alt + E**</mark>_를 반드시 한번만 칩니다.(주의 해애햐 함)
7. 최종 Enter 키를 누르면 적용되고, "Ctrl + W"로 단축키 바로 가기 키 설정을 닫습니다.
8. 안되면 1번부터 다시 반복하세요.(될때까지 주의해서)

#### "검색" 키 수정 (<mark style="color:yellow;">**Ctrl+Shift+F를 Ctrl+Alt+F로 변경**</mark>)

1. 이전 설정, 모든 명령 표시, 탐색기 키를 수정했던 방식으로 검색 단축키를 "Ctrl + Shift + F"를 "Ctrl + Alt + F"로 바꿉니다.
2. 키 바인딩 목록상자 내부에서는 "검색: 파일에서 찾기, 제어 + Shift + F, 기본값"에서 "검색: 파일에서 찾기, 제어+ Alt + F, 기본값"으로 변경합니다.

#### "링크 열기" 키 수정 (키 링크 없음을 Ctrl+Alt+0으로 변경)

1. "링크 열기" 또는 "action openLink"를 검색 후 "키 바인딩 목록상자"에서 Enter키 입력합니다.
2. <mark style="color:yellow;">**링크를 키보드로 열수 있도록 "Ctrl + Alt + 0"으로 입력**</mark>합니다.
3. "http://" 또는 "https://"로 시작하는 단어는 링크 키로 열 수 있습니다.

### 공통적인 키 조합에 문제점

1. <mark style="color:red;">**"Ctrl + Shift + 별도의 키"를 다운했을때 공통적으로 센스리더와 충돌**</mark>됨.
   * 해결방법은 "Ctrl + Shift + 별도의 키"를 <mark style="color:yellow;">**"Ctrl + Alt + 별도의 키"로 키조합을 수정**</mark>합니다.

### VSCode의 접근설 설정

접근성 설정을 안하면 모든 에디터 문서 내부의 줄에 \*\*"빈 줄"\*\*로만 읽습니다. 제대로 읽으려면 반드시 셋팅이 필요합니다. 설정의 단축키(컨트롤 + 콤마)가 센스리더의 영향으로 실행이 불가능하여 수동메뉴로 접근하여 접근성을 셋팅합니다.

1. 파일(**Alt + F 키**) 에서 2. 기본 설정(P 키)을 치고 Enter 키 누름니다.
2. 설정 검색 편집창에서 "화면 읽기"를 치고 Enter키를 치시면 접근성관련 설정이 조회됩니다.
3. 탭키를 눌러서 "Editor Accessibility Support. 수정됨 편집기를 화면 읽기 프로그램에 최적화된 모드로 실행할지 여부를 제어합니다. 사용하도록 설정하면 자동 줄 바꿈이 사용하지 않도록 설정됩니다."에 접근합니다.
4. <mark style="color:yellow;">**editor.accessibilitySupport on 콤보상자에서 "on"**</mark>값이 오면 Enter키를 누룹니다.
5. 접근성 설정이 완료되면 에디터의 모든 글을 센스리더에서 읽을 수 있습니다.
6. 축하합니다. ^^

### 접근성 키보드 이동의 기본

1. <mark style="color:yellow;">**풀다운 메뉴는 하위 메뉴가 있음으로 Enter 키로 하위 메뉴 접근**</mark>합니다.
2. 풀다운 하위 메뉴 내에서는 Home 키 (제일 첫번째메뉴로 이동), End 키(끝부분 메뉴로 이동), 상하 키로 다음/이전으로 이동합니다.
3. 상하 탭 메뉴는 방향키 위, 아래 화살표로 이동합니다. Home 키는 제일 첫번째, End 키는 마지막 메뉴로 이동합니다.
4. 좌우 탭 메뉴는 방향키 좌, 우 화살표로 이동합니다. Home 키는 제일 첫번째, End 키는 마지막 메뉴로 이동합니다.

### 주요 메뉴 이동시 접근이 안되는 현상(<mark style="color:yellow;">**단축키 변경을 안했을 때**</mark>)

1. 다음과 같이 하면 매번 키 를 두세번 눌러야 함으로 매우 불편합니다.  "VSCode 주요 단축키 수정방법"의 헤딩 부분을 참조하여 변경합니다.
2. 탐색기 탭(Ctrl + Shift + E 키) 메뉴는 Control + Shift + N 키 (기능키 무시)를 치고 다시 탐색기(Control + Shift + E 키)를 실행해야 접근 가능 합니다.(한번만 키보드 실행해야 함)
3. 검색(Ctrl + Shift + F 키) 페이지 탭 메뉴는 Control + Shift + N 키 (기능키 무시)를 치고 다시 검색(Control + Shift + F 키)를 실행해야 접근 가능 합니다.(한번만 키보드 실행해야 함)
4. 확장(Ctrl + Shift + X 키) 페이지 탭 메뉴는 Control + Shift + N 키 (기능키 무시)를 치고 다시 확장(Control + Shift + X 키)를 실행해야 접근 가능 합니다.(한번만 키보드 실행해야 함) 이후 "마켓플레이스에서 확장 검색 편집창"으로 읽습니다.

### 센스리더에서 전혀 다른 내용을 읽을 때

1. 메뉴에서 ESC 키 또는 특정 키를 누르면 이상한 동작을 보일때가 있습니다.
2. 긴장하지 마시고 Alt + 1로 기본 문서 편집창으로 돌아 옵니다.
3. 편집창에 여러 문서가 켜져 있는 경우 첫번째 문서는 Alt + 1 키는 1번 문서, Alt + 2 키는 2번 문서, Alt + 3 키는 3번 등으로 이동 가능합니다.
4. 편집창에 창이 나눠져 있는 경우 Ctrl + 1 은 1번 그룹, Ctrl + 2는 2번 그룹 등으로 순차적으로 이동가능합니다.

