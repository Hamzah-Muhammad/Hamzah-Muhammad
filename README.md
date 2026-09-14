# Hi, I'm Hamzah

Software & AI engineer in Toronto, 6+ years across fintech and enterprise software, ex-Amazon. I build LLM agents, while working with Claude Agent SDK, LangChain, MCP, and the financial apps they power.

## What I'm building

- [The Edge](https://primeinvestingcapital.org/TheEdge) at [Prime Investing Capital](https://primeinvestingcapital.org): an AI-powered trading floor. Prediction engines that scan for stock setups, a per-user AI trading persona, a portfolio review tab, options flow, and a live chat floor. FastAPI, React, Next.js, PostgreSQL.
- [Minni AI](https://minniai.com): tools that cut token usage for AI agents through better interfaces and curated memory.

## Projects

| Project | What it does |
|---|---|
| [SafeDataBaseMCP](https://github.com/Hamzah-Muhammad/SafeDataBaseMCP) | An MCP server for databases. Reads run right away. A write has to be previewed in a rolled-back transaction first, and only that preview can be committed. SQLite, Postgres or AWS RDS. Installs as a Claude Code plugin or a claude.ai connector. |
| [OpenCodingAgent](https://github.com/Hamzah-Muhammad/OpenCodingAgent) | A terminal coding agent on a free open-weight model (DeepSeek V4 via NVIDIA). Edits files, runs shell and git, opens PRs. Locked to one directory and refuses to read secrets files. CI on Windows and Linux. |
| [Ticket2PR](https://github.com/Hamzah-Muhammad/Ticket2PR) | Give it a GitHub issue, get a pull request back. Built on the Claude Agent SDK. It never merges, and the tests make sure of that. Ships as a desktop app and a CLI. Three of its PRs are left open on the [demo repo](https://github.com/Hamzah-Muhammad/ticket2pr-demo). |
| [PricingWebapp](https://github.com/Hamzah-Muhammad/PricingWebapp) | A stock price simulator (Geometric Brownian Motion, Black-Scholes) in a trading-terminal UI. Node and React. |
| [PCTuner-Optimization-Tool](https://github.com/Hamzah-Muhammad/PCTuner-Optimization-Tool) | A Windows desktop app that applies PC performance tweaks, with undo logging and a restore point before every change. |
| [TheEdge-Overview](https://github.com/Hamzah-Muhammad/TheEdge-Overview) | Architecture write-up of The Edge: what was built and how it fits together. The source is closed. |

## Stack

Python (FastAPI), TypeScript (React, Next.js, Node), PostgreSQL, Docker, AWS, GitHub Actions. Claude Agent SDK, MCP and LangChain for agent work. PowerShell for Windows tooling.
