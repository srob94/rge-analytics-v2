# Agent Instructions: Rge-analytics-v2

## Architecture Rules
- Backend: Python 3.11 with FastMCP.
- Hosting: Google Cloud Run.
- Security Proxy: AgyFlow sidecar (localhost:8080).

## Execution Rules
- Always write a unit test in `/tests` before completing a task.
- Never hardcode secrets; use GCP Secret Manager or environment variables.
- Keep terminal outputs concise to prevent context bloat.

## Complete Task Protocol
1. Run `pytest` or `npm test` and ensure all tests pass.
2. Commit changes using Conventional Commits (`feat: ...`, `fix: ...`).
3. Open a PR using `gh pr create`.
