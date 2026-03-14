# Opserve Showcase (Code-Free Overview)
- Purpose: Unified observability (metrics + alerting + live status) for services and hosts.
- Outcomes: Shorter MTTR, proactive saturation alerts, cost/usage visibility, shared ops/dev context.
- Built today: FastAPI backend (JWT + refresh, lockout, reset tokens), Prometheus metrics API with WebSocket live updates, React dashboard with token handling and tests, docker-compose dev stack (Postgres, Prometheus, node-exporter, backend, frontend).
- Differentiators: Live stream with HTTP fallback, mock data for offline demos, seeded admin, cross-platform dev launcher, tests (component + Playwright e2e).
