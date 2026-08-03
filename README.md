### Hi, I'm Hamzah Muhammad

Software & AI engineer based in Toronto. Background spans FinTech and FAANG (ex-Amazon); today I build financial applications and AI-driven tools for the stock market.

#### Skills

**AI & Agents**
- Building and orchestrating LLM agents with the Claude Agent SDK — tool permissioning, hook-based guardrails, multi-turn task orchestration
- Multi-provider AI model routing (Anthropic/Claude, Groq, NVIDIA, Cerebras, OpenRouter) behind a single internal service
- Prompt & persona engineering for domain-specific assistants
- Designing safe boundaries around agent write-access to real codebases and production systems

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
- Full CI/CD pipeline creation and management (lint/format/test/build gates, automated deploys)
- Continuous development workflow — trunk-based branching, PR review gates, staged rollouts
- Windows systems programming — registry, services, scheduled tasks (PowerShell)
- Desktop app packaging (PyInstaller, pywebview)
- Git/GitHub workflow automation

**Also built with:** Godot 4 / GDScript, Python game engines (Ursina/Panda3D)

#### What I'm building

At **[Prime Investing Capital](https://primeinvestingcapital.com)**, I design and build the full stack behind a trading education and live-tools platform:
- **TheEdge** — a real-time stock analysis dashboard (FastAPI + React): multi-chart technicals, automated setup detection (intraday/swing/invest), sector rotation, and AI-generated market write-ups.
- **PrimeInvestingCapital.com** — the platform itself (Next.js, PostgreSQL): live trading tools, education content, and account/auth for members.
- **PrimeAI / SmartTrader.ai** — a shared FastAPI model-routing service that powers AI trading-assistant features across the product line.

These are closed-source products; the tools below are the open-source side of my work.

#### Open-source tools

| Project | What it is |
|---|---|
| [**PricingWebapp**](https://github.com/Hamzah-Muhammad/PricingWebapp) | A full-stack (Node.js + React) real-time stock price simulator using Geometric Brownian Motion to model price movement. |
| [**PythonApps**](https://github.com/Hamzah-Muhammad/PythonApps) | Standalone Python tools, including a free-data options-flow scanner for options market positioning. |
| [**TicketToPR**](https://github.com/Hamzah-Muhammad/TicketToPR) | An autonomous coding agent that reads a GitHub issue backlog and opens real pull requests to resolve it — with a hard guardrail hook that blocks the model from ever touching `git`/`gh` directly. |
| [**PcTuner-Open-Source**](https://github.com/Hamzah-Muhammad/PcTuner-Open-Source) | A shipped Windows desktop app (Python/FastAPI + React/TypeScript, packaged with PyInstaller + pywebview) that audits and safely applies PC performance tuning, with full undo logging and a System Restore checkpoint before every change. |
| [**ShellScriptApps**](https://github.com/Hamzah-Muhammad/ShellScriptApps) | Small, auditable Windows PowerShell utilities, shipped as readable source alongside compiled `.exe`s. |

Pinned repos above have more detail in each README.
