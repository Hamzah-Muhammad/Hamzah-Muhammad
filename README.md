# Hamzah Muhammad

Founder of [Minni AI](https://minniai.com) in Toronto. Ex-Amazon software engineer.

Minni AI makes AI agents use fewer tokens without giving worse answers. Every agent has three layers: memory, the interface around the model, and the model itself. The model is a commodity. The saving comes from the first two.

## Minni AI

Our main service is the MinniMemoryInterface, our token-reduction research applied to a team's agents. These products deliver it:

| Product | What it does |
|---|---|
| [MinniMemoryMCP](https://www.npmjs.com/package/minnimemory) | Splits the memory files Claude Code and Codex load every turn into a small always-loaded part and files that load only when a task needs them. Then it measures the saving. `npm install -g minnimemory` |
| MinniMemoryAgent | Keeps a company's agent memory files healthy across its whole fleet and opens a pull request per repo. |
| MinniCode | The Open-LLM coding agent: a terminal coding agent in the shape of Claude Code, tuned for low token use. |
| MinniTuner | A consent-first Windows PC tuner. |

Every claim we make is measured. Answer quality is checked by a blind judge, and failed runs stay on the record.

## Also building

- [Prime Investing Capital](https://primeinvestingcapital.org): an AI-powered trading floor with paying users. Prediction engines that scan for stock setups, a per-user AI trading persona, portfolio review and options flow.

## Open source

| Project | What it does |
|---|---|
| [SafeDataBaseMCP](https://github.com/Hamzah-Muhammad/SafeDataBaseMCP) | An MCP server for databases. Reads run right away. A write has to be previewed in a rolled-back transaction first, and only that preview can be committed. SQLite, Postgres or AWS RDS. |
| [OpenCodingAgent](https://github.com/Hamzah-Muhammad/OpenCodingAgent) | A terminal coding agent on an open-weight model (DeepSeek V4 via NVIDIA). Edits files, runs shell and git, opens PRs. Locked to one directory and refuses to read secrets files. |
| [Ticket2PR](https://github.com/Hamzah-Muhammad/Ticket2PR) | Give it a GitHub issue, get a pull request back. Built on the Claude Agent SDK. It never merges, and the tests make sure of that. Desktop app and CLI. |
| [LangGraphAgentTemplate](https://github.com/Hamzah-Muhammad/LangGraphAgentTemplate) | A starting point for building agents on LangChain 1.x and LangGraph 1.x. Five workflow modes, human approval, long-term memory, context compaction, evals and CI already built. You add the prompt, tools and eval cases. |
| [PricingWebapp](https://github.com/Hamzah-Muhammad/PricingWebapp) | A stock price simulator (Geometric Brownian Motion, Black-Scholes) in a trading-terminal UI. Node and React. |
| [PCTuner-Optimization-Tool](https://github.com/Hamzah-Muhammad/PCTuner-Optimization-Tool) | A Windows desktop app that applies PC performance tweaks, with undo logging and a restore point before every change. |
| [TheEdge-Overview](https://github.com/Hamzah-Muhammad/TheEdge-Overview) | Architecture write-up of The Edge, Prime Investing Capital's trading floor. The source is closed. |

## Stack

| Area | Tools |
|---|---|
| Agents | Claude Agent SDK, OpenAI SDK, LangChain, LangGraph, MCP |
| Backend | Python, FastAPI, Node.js, Java, PostgreSQL |
| Frontend | TypeScript, React, Next.js |
| Infra | AWS, Docker, Kubernetes, GitHub Actions |
