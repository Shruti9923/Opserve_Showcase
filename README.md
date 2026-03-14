# Opserve Showcase
**Unified IT Observability and Infrastructure Monitoring Platform**

## Project Overview
Opserve is a high-performance observability dashboard designed to provide a single pane of glass for IT infrastructure health. It integrates a FastAPI backend with Prometheus-powered metrics to deliver real-time observability, helping reduce Mean Time to Recovery (MTTR) and proactively detect system saturation.

## System Integration and Architecture
This project focuses on the integration of time-series data engines and real-time communication protocols:

* **Data Engineering Pipeline:** Orchestrates a Prometheus and node-exporter stack to ingest and process system metrics including CPU, Memory, Latency, and Error Rates.
* **Networking and Real-time Telemetry:** Implemented a dual-channel communication layer using WebSockets (`/ws/updates`) for live streams with an automated HTTP polling fallback for network resilience.
* **Infrastructure as Code:** Utilizes Docker Compose to manage a full-stack development environment, including PostgreSQL for session management and Prometheus for time-series data.
* **Security Integration:** Features a robust JWT Access and Refresh token system, server-side password hashing, account lockout policies, and role-based access checks.

## Tech Stack
* **Backend:** Python (FastAPI), SQLAlchemy, Pytest.
* **Frontend:** React, TypeScript, React Testing Library, Playwright.
* **Observability:** Prometheus, Node-exporter.
* **Persistence:** PostgreSQL.
* **DevOps:** Docker, Docker Compose.

## Key Capabilities
* **Live Health Monitoring:** Real-time visibility into uptime and resource utilization.
* **Resilient Demo Mode:** Built-in mock data fallback to ensure dashboard functionality even if the Prometheus instance is offline.
* **Secure Access:** Comprehensive authentication suite including password complexity rules, lockout mechanisms, and secure reset tokens.
* **Administrative Control:** Role-gated user management views and administrative dashboards.

## Testing and Quality Assurance
* **Frontend:** Component testing via React Testing Library and E2E testing with Playwright.
* **Backend:** Comprehensive suite of Pytest cases covering authentication and metrics endpoints.
* **Roadmap:** Integration of alert policy flows and WebSocket resilience stress-testing.

## Roadmap
* **Log Aggregation:** Integrating Grafana Loki to pair metrics with root-cause logs.
* **Anomaly Detection:** Implementing moving averages and SLA widgets for predictive maintenance.
* **Granular RBAC:** Advanced Admin, Operator, and Viewer permissions and layout control.

## Contact
**Shruti Deshmane**
- Email: shrutideshmane93@gmail.com
- LinkedIn: https://www.linkedin.com/in/shruti-deshmane-ba7897358
