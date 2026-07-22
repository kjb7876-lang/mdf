# v17 변경 기록

- 모바일 자동 시작 버튼 입력을 click 단일 경로에서 pointer/touch/click 통합 경로로 변경
- UI 재렌더링 중 사라지는 탭을 document pointer-up fallback으로 복구
- 520ms 입력 중복 방지로 자동 시작 직후 재정지되는 이중 이벤트 차단
- 모바일 utility bar z-index 상향 및 설정 패널 safe-area 간격 확대
- 설정 패널이 열린 상태의 자동 시작 시 패널 자동 닫기
- 버튼 aria-label, touch-action, pointer-events 보강
