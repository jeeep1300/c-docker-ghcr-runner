[개발자 PC]
    │
    │ git push
    ▼
[GitHub Repository]
    │
    │ GitHub Actions Workflow
    ▼
[Windows Self-hosted Runner]
    ├─ Git
    ├─ Docker Desktop 또는 Docker Engine
    ├─ GHCR 로그인
    ├─ Docker image build
    ├─ C 프로그램 테스트
    ├─ GHCR push
    └─ docker compose up -d 로 운영 컨테이너 재배포
            │
            ▼
[운영 컨테이너]
    └─ C 실행 파일 포함 이미지


c-docker-ghcr-runner/
├─ src/
│  └─ main.c
├─ Makefile
├─ Dockerfile
├─ docker-compose.yml
├─ .dockerignore
├─ README.md
└─ .github/
   └─ workflows/
      └─ c-ci-cd.yml

