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
## 📚 핵심 개념 정리

### 1. 절대 경로 vs 상대 경로
- **절대 경로**: 루트 폴더(예: `C:\`)부터 시작하여 파일의 전체 위치를 나타내는 방식 (예: `C:\Users\Documents\test.txt`)
- **상대 경로**: 현재 내가 있는 위치를 기준으로 파일의 위치를 나타내는 방식 (예: `./test.txt` 또는 `../index.html`)

### 2. 파일 권한 (Read, Write, Execute)
- **Read (r)**: 파일을 읽을 수 있는 권한
- **Write (w)**: 파일을 수정하거나 삭제할 수 있는 권한
- **Execute (x)**: 파일을 프로그램으로서 실행할 수 있는 권한
- *참고: 윈도우에서는 `attrib` 명령어로, 리눅스에서는 `chmod` 명령어로 제어합니다.*
### 3. Git의 3가지 공간
- **Working Directory**: 현재 내가 파일을 수정하고 있는 실제 작업 공간
- **Staging Area**: 저장소에 기록하기 전, 저장할 파일들을 잠시 올려두는 준비 영역 (`git add`)
- **Repository**: 버전이 영구적으로 저장되는 공간 (`git commit`)

### 4. Docker 이미지 vs 컨테이너
- **이미지 (Image)**: 프로그램 실행에 필요한 모든 파일과 설정이 담긴 '설계도' (변경 불가능)
- **컨테이너 (Container)**: 이미지를 실행한 '실제 상태'. 설계도로 만든 '실제 건물'과 같으며, 독립된 환경에서 동작함

## 🖥️ 터미널 조작 실습 로그

### 1. 파일 목록 확인 (dir)
- `dir` 명령어를 통해 현재 작업 디렉터리의 파일 목록과 정보를 확인했습니다.

```bash
C:\mission_practice>dir
2026-10-29  오후 02:02    <DIR>          .
2026-10-29  오후 01:43                79 Dockerfile
2026-10-29  오후 02:02                 0 empty_file.txt
2026-10-29  오후 01:42               223 index.html
2026-10-29  오전 11:59                20 note.txt
2026-10-29  오후 12:11               383 README.md

### 2. 파일 관리 실습 (ren, mkdir, move)
- `ren` 명령어로 파일 이름을 변경하고, `mkdir`로 폴더를 생성하여 `move`로 파일을 이동시켰습니다.
- 변경 사항: `empty_file.txt` → `my_log.txt` 이름 변경 및 `archive/` 폴더로 이동 완료