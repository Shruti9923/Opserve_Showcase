# Operations (Dev/Demo)
- One-liner: python scripts/dev_stack.py (env overrides supported).
- Compose: docker-compose up (Prometheus + node-exporter; toggle backend/frontend services for full stack).
- Direct: uvicorn app.main:app --reload --host 0.0.0.0 --port 8000; npm start in react-frontend.
- Health/readiness: exposed in backend (for compose/orchestrators).
- Seeds: scripts in fastapi-backend/app/scripts (e.g., seed_admin.py) to bootstrap admin.
- Config: .env for SECRET_KEY, DATABASE_URL, PROMETHEUS_URL, ALLOWED_ORIGINS.
