# Development Environment Training Mission 
- [x] 터미널 기본 조작 및 폴더 생성 (pwd, mkdir, cd) 
- [x] 파일 생성, 확인, 복사, 삭제 (echo, type, copy, del) 
- [x] 파일 권한/속성 제어 (attrib +r, attrib -r) 
- [x] Docker 버전 점검 (docker --version) 
- 문제 상황: 공용 PC 환경 제한으로 docker 명령어 인식 불가 
- 확인 결과: 'docker'은(는) 내부 또는 외부 명령이 아님 에러 발생 
## 🔍 트러블슈팅 (Troubleshooting)

### 1. Docker 명령어 인식 불가 문제
- **문제**: 터미널에서 `docker --version` 입력 시 '명령어를 찾을 수 없음' 에러 발생.
- **원인 가설**: 공용 PC 환경으로 인해 Docker Desktop이 설치되어 있지 않음.
- **확인**: 시스템 프로그램 목록을 확인했으나 Docker 관련 프로그램이 없음.
- **해결/대안**: 공용 PC에서는 이론 학습과 문서 구조화를 우선 진행하고, 실제 컨테이너 빌드 및 실행은 개인 PC(집)에서 수행하기로 함.
