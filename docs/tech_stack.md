# Tech Stack
- Backend: FastAPI, Uvicorn, Pydantic, SQLAlchemy/Alembic, JWT (python-jose), passlib for hashing.
- Frontend: React + TypeScript, React Testing Library, Playwright e2e.
- Metrics: Prometheus, node-exporter.
- DB: PostgreSQL (configurable via DATABASE_URL).
- Infra/Tooling: Docker, docker-compose, scripts/dev_stack.py and scripts/dev_stack.sh.
- Why: FastAPI for async + typing; Prometheus for standard metrics; React/TS for typed UI and ecosystem.
