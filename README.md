# MASKLESS LITHO v2.1.5 Manual

PLANCK INC 일반 버전 기준 한글 운용 매뉴얼입니다.

- 사이트: https://loveeuge.github.io/maskless-litho-manual-20260604-1959/
- 공식 릴리즈: https://github.com/PLANCK-INC/MASKLESSLITHO/releases/tag/v2.1.5
- 실행 파일: `maskless_v2_1_5.exe`, `maskless_v2_1_5_fast.exe`
- 기준: 소스 commit `4077c33`, `README.md`, 현재 UI 및 컨트롤러 소스

첫 LED 준비와 `Pattern visible` 확인, ON 응답 후 30초 미확인 종료,
Display Apply 검증과 복구, DLP 1920x1080/100% 조건, Fast Portable 설치,
Motorized Focus 일반 버전 제외, GDS raster 검사, Keystone 호환성,
LED OFF/current/FAN 오류 및 CAD 저장 취소 처리를 반영했습니다.

## 파일 / 재생성

- [한글 매뉴얼 PDF 다운로드](downloads/MASKLESS_LITHO_v2_1_5_Manual_ko.pdf): v2.1.5 일반 버전, 32쪽, 2026-10-28 업데이트.
- 첫 화면의 **한글 매뉴얼 PDF 다운로드** 버튼으로 로그인 없이 내려받을 수 있습니다.
- PDF에는 24개 항목과 숨겨진 탭 27개, 화면 캡쳐 22개 배치를 모두 포함했습니다. 검색, 목차 이동, 책갈피를 지원합니다.
- PDF 생성 및 검사 도구는 [다운로드 사이트 저장소](https://github.com/loveeuge/maskless-download-site/tree/main/tools)에 있습니다. `build_manual_pdf.py`에 한글/영문 사이트 폴더를 전달하고, 생성 결과를 시각 검토한 뒤 이 저장소의 `downloads/`에 복사합니다. 웹 문서를 다시 생성할 때 PDF 링크도 유지하세요.

- `index.html`: 배포 가능한 원페이지 사이트
- `assets/img/*-v2_1_5.png`: 현재 소스의 실제 위젯 캡쳐 19개
- `IMAGE_REFERENCE.md`: 캡쳐 배치와 설명
- `UPDATE_v2_1_5.md`: 변경사항과 검증 범위

```powershell
.\venv64\Scripts\python.exe manual_site_v2105\build_manual_site.py
.\venv64\Scripts\python.exe manual_site_v2105_en\build_manual_site_en.py
```

한글/영문 내용은 `manual_site_v2105/manual_content.py`에서 함께 관리합니다.
폴더 이름은 기존 작업 경로 호환성을 위해 유지합니다.
캡쳐 스크립트는 임시 사용자 데이터와 차단된 하드웨어 명령으로 실행합니다.

```powershell
$env:QT_QPA_PLATFORM='windows'
.\venv64\Scripts\python.exe manual_site_v2105\capture_v2105_screens.py
```

첫 LED 확인창과 UV 진행 상태는 실제 UI를 재현한 예시이며
실제 UV 출력, 전류, 광량, 물리적 패턴 정확도의 검증 결과가 아닙니다.
