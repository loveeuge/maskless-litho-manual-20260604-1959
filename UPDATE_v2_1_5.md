# v2.1.5 메뉴얼 업데이트 기록

기준 소스: `4077c33` (Release v2.1.5 display safety and LED startup fixes).

- 현재 일반 버전 기준 24개 섹션으로 개정
- 빠른 시작에 Initialize 및 실제 노광 전 TEST Mode OFF 명시
- DLP Display / Apply 전용 섹션: 1920x1080/100%, pending 선택,
  검정 화면/LED OFF/current 0 readback 확인, 실패 후 복구
- 첫 수동 ON: 준비창, Pattern visible, 30초 미확인 종료,
  같은 초기화 세션 재사용, 재초기화/장비 변경 후 재확인
- 5초 준비 제한과 DLL blocking, 명령 응답과 광 출력의 차이 설명
- Motorized Focus 일반 버전 제외 및 내부 실행 옵션 거부
- Fast Portable 및 `_internal` 보존, 외부 카메라 프로그램 안내
- GDS 실제 도형과 crop frame, preview zoom과 CAD scale 구분
- 렌즈/DLP별 Keystone 호환성, Compensation/Sequence 파일 오류,
  OFF/current/FAN 오류 및 CAD 저장 취소 설명 보강
- 기능 탭, 키보드 이동, 인쇄 시 전체 탭 표시, 원본 이미지 링크

현재 소스 위젯 19종을 Windows Qt 렌더링으로 캡쳐했습니다.
임시 사용자 데이터와 하드웨어 명령 차단을 적용했습니다.
LED/UV 상태는 UI 예시이며 실제 장비 실행 결과가 아닙니다.

HTML, 목차/탭 연결, 이미지, PC/모바일 표시 및 배포 반영을 검증합니다.
실장비의 UV 출력, 전류, 지연 시간, 선량, 정확도의 검증을 뜻하지 않습니다.
