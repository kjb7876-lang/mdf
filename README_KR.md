# 사이버 성역 방어 2.5D v18 모바일 로컬파일 터치 수정판

## Android에서 가장 확실한 실행법
1. ZIP을 완전히 압축 해제합니다. ZIP 안에서 `index.html`을 바로 열지 마세요.
2. 일반 파일 미리보기/HTML Viewer 대신 **Acode의 Preview**, **Spck Preview**, 또는 로컬 HTTP 서버 앱으로 여세요.
3. 첫 화면에서 `초기 성역 자동 건설 시작`을 누른 뒤 상단의 `자동 시작`을 누릅니다.
4. Chrome에서 직접 로컬 파일 열기가 막히거나 흰 화면이 나오면 Acode에서 폴더를 열고 `index.html → Preview`로 실행합니다.

## iPhone/iPad
Files 앱의 빠른 미리보기보다 로컬 웹서버/웹호스팅 방식이 안정적입니다. 압축을 푼 뒤 HTML 실행을 지원하는 앱에서 열거나 itch.io/GitHub Pages 같은 HTTPS 호스팅에 올려 실행하세요.

## v18 수정 내용
- 문서 전체의 `touch-action:none`을 제거하고 게임 캔버스에만 적용했습니다.
- 첫 진입 시작 버튼을 도움말 맨 위에 고정해 스크롤 없이 게임을 시작할 수 있습니다.
- 자동 시작/수동 전환, 설정 버튼을 포함한 모든 버튼에 모바일 탭 누락 보정기를 추가했습니다.
- pointerup/touchend 뒤 native click이 오지 않는 Android HTML Viewer/WebView에서는 synthetic click을 한 번만 보냅니다.
- native click이 늦게 도착할 때 중복 실행되는 문제를 차단합니다.
- 버튼 위에서 스크롤한 경우는 탭으로 처리하지 않습니다.
- 도움말·설정 패널은 세로 스크롤, 하단/상단 버튼 바는 가로 스크롤이 가능하도록 터치 영역을 분리했습니다.

## 주의
HTML을 ZIP 내부에서 바로 미리보기하면 JavaScript나 터치 이벤트가 제한될 수 있습니다. 반드시 압축 해제 후 실제 브라우저 엔진의 Preview 또는 HTTP 주소로 실행하세요.
