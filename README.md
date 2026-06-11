# MASKLESS LITHO v2.1 Manual Site

MASKLESS LITHO v2.1 기준 GitHub Pages 원페이지 운용 매뉴얼입니다.

- 기준 소스: `README.md`, `ui/main_window.py`, `ui/pattern_settings_section_builder.py`, `ui/setting_window.py`, `ui/gds_layer_dialog.py`, `ui/uv_keystone_window.py`
- 릴리즈 빌드 파일명: `maskless_v2_1.exe`
- 주요 반영 내용: manual `LED ON` 안정화, UV Keystone 자동 적용 상태, GDS Import crop frame, Motorized Focus 단일 exe 내부 모드, Draw CAD/Expose Setup 운용 흐름
- 화면 구성: 왼쪽 고정 목차, 모바일 선택 목차, 기능별 탭 섹션, v2.1 UI 캡쳐

중요 변경점:

- v2.1 UI에는 별도 `Keystone Preview / Expose` 버튼이 없습니다.
- `LED ON`은 UV Keystone이 `APPLIED (ON)`이면 보정 이미지를 먼저 적용하고, UV Keystone이 꺼져 있거나 profile이 없으면 raw 이미지로 출력합니다.
- 수동 LED ON 직후 `Manual LED starting...`, 실제 LED ON 성공 후 `Manual exposing... 0.000s` 상태가 표시됩니다.
- UV Keystone Calibration은 시작 전 DLP monitor와 main/camera monitor의 native 해상도를 확인합니다.

정적 사이트이므로 `index.html`과 `assets/img`만으로 동작합니다.
