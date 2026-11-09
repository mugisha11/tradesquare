# Contributing to TradeSquare

## Scope

This repository is currently focused on establishing a professional, scalable repository structure. Keep changes narrow, preserve the separation between `frontend/` and `backend/`, and avoid implementing features during architecture work.

## Architecture conventions

- Keep all Flutter code under `frontend/`.
- Keep all FastAPI, database logic, AI services, and integrations under `backend/`.
- Keep production AI inference in `backend/app/ai/` and experimentation/training in `backend/ml/`.
- Use modular service and repository layers and avoid unnecessary abstraction.
- Never commit secrets, credentials, confidential datasets, or model artifacts.

## Code quality

- Prefer descriptive names and typable interfaces.
- Add tests for meaningful behavior changes.
- Inspect existing files before overwriting and preserve working code when one already exists.
