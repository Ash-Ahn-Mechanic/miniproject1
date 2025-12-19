## 개발 환경 설정 문제

`docker` 명령어를 찾을 수 없습니다. 이는 Docker Desktop이 설치되어 있지 않거나 실행 중이 아니거나, 또는 `docker` 실행 파일이 시스템의 PATH 환경 변수에 추가되어 있지 않음을 의미합니다.

이 프로젝트는 Docker를 기반으로 개발 환경을 구성하고 실행하므로, **Docker Desktop을 설치하고 실행한 후 `docker` 명령어가 터미널에서 정상적으로 작동하는지 확인해주셔야 합니다.**

Docker 설치 및 설정이 완료되면, 다시 알려주시면 WP0 작업을 이어서 진행하겠습니다.

---
**Current Progress:**

*   `backend`, `frontend`, `infra` 디렉토리 생성 완료.
*   `infra/docker-compose.yml` 파일 생성 완료.
*   `backend/main.py`, `backend/requirements.txt`, `backend/Dockerfile`, `backend/.env.example` 파일 생성 완료.
*   `backend/.env` 파일 복사 완료.

**Remaining tasks for WP0 (Blocked by Docker):**

*   Alembic 세팅(마이그레이션 가능 상태)
*   lint/format: ruff + black, pre-commit 설정
*   CI: GitHub Actions로 backend 테스트 + 린트 돌리기
*   `docker compose up`을 통한 로컬 환경 구동 확인 (WP0 완료 기준)