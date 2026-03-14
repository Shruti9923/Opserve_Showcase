# Architecture
## System Context
- Users → React frontend → FastAPI backend → Prometheus + Postgres; WebSocket for live updates.
- Observability plane: Prometheus scrapes infra (node-exporter), backend enriches/serves to UI.

## Components
- Frontend: React app with token-aware API client and WebSocket hook.
- Backend: FastAPI REST + WebSocket; metrics service (Prometheus client); auth (JWT/refresh/lockout/reset).
- Data: Postgres for auth/session/state; Prometheus for time-series.
- Infra: docker-compose for Prometheus + node-exporter; optional backend/frontend services.

## Key Flows
- Auth: Login → access + refresh tokens; refresh on expiry; password reset token flow; lockout after retries.
- Metrics: Frontend requests overview/time-range → backend queries Prometheus (fallback mock when unavailable).
- Live updates: Frontend subscribes to /ws/updates; falls back to HTTP polling if stream drops.

## Deployment (dev/demo)
- Local: python scripts/dev_stack.py (backend + frontend); or separate uvicorn + npm start.
- Compose: docker-compose up (Prometheus/node-exporter; enable backend/frontend services as needed).
