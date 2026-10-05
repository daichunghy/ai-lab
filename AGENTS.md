# AI Agent Guidelines

This repository is designed for autonomous and collaborative AI development. Every AI coding agent working in this repository must adhere to the following conventions:

## 1. Project Scoping
- **Do not pollute the repository root.** Keep root clean (only repo-level configurations, orchestration, and documentation).
- Place standalone applications and feature builds in `projects/<project-name>/`.
- Place one-off scripts, proof-of-concepts, and benchmarks in `experiments/<experiment-name>/`.

## 2. Dependency Management
- **Python:** Prefer `uv` for lightning-fast virtual environment and dependency resolution. Avoid polluting global Python environments.
- **Node.js / Web:** Prefer `pnpm` or `bun` when available, falling back to standard `npm`.
- Ensure each project has its own lockfile and dependency definition.

## 3. Secret & Security Hygiene
- **Never commit credentials.** Never hardcode API keys, service account JSONs, or secrets in code or commits.
- Always provide `.env.example` templates with placeholder values.

## 4. Documentation & Verifiability
- Every new project or experiment must have its own concise `README.md` detailing:
  - What the project does.
  - Prerequisites and environment variables needed.
  - Clear run commands (e.g. `uv run python main.py` or `npm run dev`).
