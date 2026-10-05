# AI Lab 🧪

A modular workspace for AI-assisted prototypes, autonomous agent tools, benchmarks, and experimental applications.

---

## 📁 Repository Structure

```text
ai-lab/
├── projects/        # Production-ready prototypes and standalone sub-projects
├── experiments/     # Fast POCs, model evaluations, and research scripts
├── shared/          # Reusable utilities, helper scripts, and base configurations
├── AGENTS.md        # Conventions and execution rules for AI assistants
└── README.md
```

---

## 🚀 Workspace Conventions

### 1. Adding a New Project
Create a self-contained directory inside `projects/<project-name>` or `experiments/<experiment-name>`.

Each project should include:
- A dedicated `README.md` explaining the purpose, setup, and run commands.
- Its own dependency manifest (e.g. `pyproject.toml` / `requirements.txt` using `uv`, or `package.json`).
- An `.env.example` file documenting required environment variables (never commit actual `.env` files).

### 2. Environment & Secrets
Store API keys (`OPENAI_API_KEY`, `GEMINI_API_KEY`, `ANTHROPIC_API_KEY`, etc.) inside a local `.env` file at the root or project-level. These are automatically excluded by `.gitignore`.

---

## 🤖 Working with AI Agents

When instructing AI agents (Antigravity, Claude Code, Cursor, Copilot) to build projects in this repository, reference [AGENTS.md](AGENTS.md) for architectural and dependency management standards.
