# AutoGPT

A powerful platform to **build, deploy, and run continuous AI agents** that automate complex workflows — a mirrored copy of the [Significant-Gravitas/AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) open-source project (v0.6.8 platform beta).

> Built by Girish Lade — [ladestack.in](https://ladestack.in)

## Features

- **Agent Builder** — low-code, block-based interface to design custom AI agents: connect blocks where each block performs a single action.
- **Ready-to-use agents** — pick from a library of pre-configured agents and put them to work immediately.
- **Workflow management** — build, modify, and optimize automation workflows with ease.
- **Deployment controls** — manage the full agent lifecycle from testing to production.
- **Agent interaction** — run and interact with your agents through a user-friendly interface.
- **Monitoring & analytics** — track agent performance and gain insights to continually improve.

## Tech Stack

- **Frontend:** Next.js / React (TypeScript)
- **Backend:** Python (FastAPI-style services), Docker Compose for self-hosting
- **AI:** LLM-powered agent orchestration (works with OpenAI and compatible providers)

## Quick Start (self-hosting with Docker)

```bash
# Clone the repo
git clone https://github.com/girishlade111/AutoGPT.git
cd AutoGPT

# Copy and fill in your environment (API keys etc.)
cp .env.example .env

# Start the platform
docker compose up -d
```

Then open the frontend URL printed by Docker Compose and sign in to build your first agent.

> Note: This mirror contains the top-level project files; upstream submodules are not included. For the complete source with full history, see the [original repository](https://github.com/Significant-Gravitas/AutoGPT).

## Project Structure

```
.
├── .deepsource.toml        # Static analysis config
├── .dockerignore           # Docker build exclusions
├── .pre-commit-config.yaml # Pre-commit hooks
├── CITATION.cff            # Citation metadata
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md         # Contribution guidelines
├── LICENSE                 # MIT license
├── SECURITY.md             # Security policy
└── README.md
```

## Environment Variables

| Variable | Purpose |
|---|---|
| `OPENAI_API_KEY` | LLM provider API key for agent execution |
| `AUTH_SECRET` / secrets | Session and service secrets for the platform services |

Refer to the [official self-hosting guide](https://docs.agpt.co/platform/getting-started/) for the complete, up-to-date setup documentation.

## Deploy Notes

This is a mirror of a full-stack, Docker-based platform (backend services + database + frontend). It is **not deployed as a static website** — run it via Docker Compose on a VPS or local machine as described above.

## License

MIT — see [LICENSE](./LICENSE).

---

**Built by Girish Lade** · [ladestack.in](https://ladestack.in)
