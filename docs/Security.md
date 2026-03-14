# Security Posture
- Auth: JWT access + refresh, expirations enforced.
- Passwords: Complexity rules; hashing via passlib.
- Lockout: Temporary lockout after repeated failed logins.
- Reset: Token-based password reset flow.
- Roles: Basic role checks on protected endpoints; (roadmap) admin/operator/viewer granularity.
- Transport: Expect HTTPS in production; CORS origins configurable via env.
