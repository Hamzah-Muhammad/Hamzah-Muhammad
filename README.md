### Hi, I'm Hamzah Muhammad

Software & AI engineer based in Toronto. Background spans FinTech and FAANG (ex-Amazon). Today I build AI agents that do real work — and the guardrails that make it safe to let them — alongside the financial applications they run inside.

#### Skills

**AI & Agents**
- Building and orchestrating LLM agents with the Claude Agent SDK — tool permissioning, hook-based guardrails, multi-turn task orchestration
- Designing safe boundaries around agent write-access to real codebases and production systems: allow-listed tool surfaces, path jails, and invariants enforced by assertions and tests rather than by prompt instructions
- Shipping agents non-technical users can actually run — packaged desktop apps over the same engine as the CLI, with the auth flow built in
- Multi-provider AI model routing (Anthropic/Claude, NVIDIA NIM, Cerebras, OpenRouter) behind a single internal service
- Prompt & persona engineering for domain-specific assistants

**Backend & APIs**
- Python, FastAPI — async REST API design and implementation
- Node.js, Express
- API integration (market-data feeds, news/RSS, third-party services)
- Auth (JWT), PostgreSQL, relational schema design

**Frontend**
- React (18/19), TypeScript, Next.js (App Router)
- Real-time data visualization — live charting, technical indicators, candlestick views

**Financial Engineering**
- Stochastic price modeling (Geometric Brownian Motion)
- Automated technical-analysis / trade-setup detection systems
- Options-flow and market-positioning analysis

**Systems & DevOps**
- Docker — containerization and image builds for deployment
- Cloud hosting on AWS
- Full CI/CD pipeline creation and management (lint/format/test/build gates, automated deploys, cross-OS test matrices)
- Continuous development workflow — trunk-based branching, PR review gates, staged rollouts
- Windows systems programming — registry, services, scheduled tasks (PowerShell)
- Desktop app packaging (PyInstaller, pywebview, Tkinter)
- Git/GitHub workflow automation

**Also built with:** Godot 4 / GDScript, Python game engines (Ursina/Panda3D)

#### What I'm building

At **[Prime Investing Capital](https://primeinvestingcapital.org)**, I design and build the full stack behind a trading education and live-tools platform:
- **[The Edge](https://primeinvestingcapital.org/TheEdge)** — an AI-Powered Trading Floor (FastAPI + React + PostgreSQL): three Prime Engines that scan the market for day / swing / long-term stock setups, Trade Tracker, TheEdgePortfolio (AI review of your own holdings), AI options-flow verdicts, and a live trading-floor chat with WebRTC screen share where analysts trade live daily. Source is closed — see **[TheEdge-Overview](https://github.com/Hamzah-Muhammad/TheEdge-Overview)** for a public architecture writeup.
- **PrimeInvestingCapital.org** — the platform itself (Next.js, PostgreSQL): live trading tools, education content, account/auth, and Stripe subscription billing for members.
- **PrimeTrader.ai** — the in-app AI trading agent: a per-user persona that learns how you trade, tool access over the platform's own computed data (setups, levels, watchlist, trades, holdings), and write actions that never execute without an explicit user confirmation.

These are closed-source products; the tools below are the open-source side of my work.

#### Open-source tools

**AI agents**

| Project | What it is |
|---|---|
| [**Ticket2PR**](https://github.com/Hamzah-Muhammad/Ticket2PR) | Hand it a GitHub issue, get back a pull request. An autonomous coding agent on the Claude Agent SDK that picks up the issues you label for it, writes and tests the change in a real repo, and opens a PR — **it never merges anything itself**, and that is enforced by assertions and tests, not by asking the model nicely. Ships as a **double-click desktop app** (connect GitHub in-app, pick a repo, click an issue) as well as a CLI. Three agent-authored PRs are left open on its [demo repo](https://github.com/Hamzah-Muhammad/ticket2pr-demo) as a standing exhibit. *v0.2.0 · 67 tests · CI on Windows + Linux* |
| [**OpenCodingAgent**](https://github.com/Hamzah-Muhammad/OpenCodingAgent) | A coding agent for your terminal that runs on a **free, open-weight model** (NVIDIA's DeepSeek V4) instead of a paid key: read/search/write/edit files, run shell commands, use git, with streaming, live token accounting and automatic conversation compaction. Every tool is confined to one sandbox directory — symlink- and junction-safe — and secrets files are refused before they can ever reach the model. *v0.1.1 · 108 tests · CI on Linux* |
| [**SafeDataBaseMCP**](https://github.com/Hamzah-Muhammad/SafeDataBaseMCP) | An MCP server that gives an agent a database and takes away the ability to wreck it. Reads run immediately; a write can't happen in one step — `propose_change` previews the effect inside a rolled-back transaction and hands back a single-use `change_id`, and only that id can commit it, so the preview is structurally unskippable rather than a prompt convention. SQLite by default, with a Postgres/AWS RDS backend (IAM auth, no stored password) behind the same gate. *178 tests · CI on Windows + Linux* |

**Applications & templates**

| Project | What it is |
|---|---|
| [**RestApi-User-Management-Example**](https://github.com/Hamzah-Muhammad/RestApi-User-Management-Example) | A FastAPI REST API template built to be forked and repointed at a real domain: JWT auth, ownership-scoped CRUD, versioned `/v1` routes, a consistent error envelope, liveness/readiness probes, pagination/filtering/sorting, Alembic migrations, 27 pytest tests, Docker/docker-compose, and CI. |
| [**PCTuner-Optimization-Tool**](https://github.com/Hamzah-Muhammad/PCTuner-Optimization-Tool) | A shipped Windows desktop app (Python/FastAPI + React/TypeScript, packaged with PyInstaller + pywebview) that audits and safely applies PC performance tuning, with full undo logging and a System Restore checkpoint before every change. |
| [**PricingWebapp**](https://github.com/Hamzah-Muhammad/PricingWebapp) | A full-stack (Node.js + React) real-time stock price simulator using Geometric Brownian Motion to model price movement, in a trading-terminal UI. |
| [**PythonApps**](https://github.com/Hamzah-Muhammad/PythonApps) | Standalone Python tools, including a free-data options-flow scanner for options market positioning. |
| [**ShellScriptApps**](https://github.com/Hamzah-Muhammad/ShellScriptApps) | Small, auditable Windows PowerShell utilities, shipped as readable source alongside compiled `.exe`s. |

Pinned repos above have more detail in each README.
