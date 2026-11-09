# Copilot instructions — TradeSquare

## Project
TradeSquare is an AI-powered B2B trade facilitation platform connecting buyers and suppliers across Rwanda and East Africa.

## Architecture

- Exactly two root application directories: `frontend/` and `backend/`.
- `frontend/` contains the Flutter/Dart app using Material 3, Riverpod, go_router, and Dio.
- `backend/` contains the Python/FastAPI application, database logic, integrations, and AI services.
- Production AI services belong under `backend/app/ai/`; ML experimentation belongs under `backend/ml/`.
- Do not add root-level `apps/`, `server/`, `mobile/`, or `api/` directories.

## Coding standards

- Keep modules cohesive and well named.
- Use `snake_case` for Python modules and `lowercase_with_underscores` for Dart files.
- Use `PascalCase` for Dart types and `snake_case` for Python classes/functions when appropriate.
- Keep API endpoints thin and delegate business logic to services and repositories.
- Add tests for meaningful behavior changes.

## Design and localization

- Centralize design tokens and styles in the frontend application theme.
- Use the official font Manrope.
- Support English and Kinyarwanda localization.
- Use the TradeSquare brand palette: primary `#0A66C2`, deep blue `#004182`, light blue `#70B5F9`, background `#F3F6F8`, white `#FFFFFF`, and text `#191919`.

## Security and data handling

- Never commit credentials, tokens, sensitive business records, MINICOM data, or model artifacts.
- Use environment variables and placeholder values only.
- Keep secret material in local `.env` files and out of the repository.
- Ensure raw, interim, processed datasets and model artifacts stay out of version control.

## Change discipline

- Preserve existing code.
- Inspect before replacing files.
- Do not implement features when the task is purely about structure.
- Update architecture or documentation when conventions change.
