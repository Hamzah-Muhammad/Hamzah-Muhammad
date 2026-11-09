# Hamzah Muhammad

Founder of [Minni AI](https://minniai.com) in Toronto. Former Amazon software engineer.

Minni AI makes AI agents use fewer tokens without giving worse answers. Every agent has three layers, memory, the interface around the model, and the model itself. The model is a commodity, so the saving comes from the first two.

## Minni AI

Our main service is the MinniMemoryInterface, our token reduction research applied to a team's agents. These products deliver it.

| Product | What it does |
|---|---|
| [MinniMemoryMCP](https://minniai.com/minnimemorymcp/docs) | Splits the memory files Claude Code and Codex load every turn into a small part that always loads and files that load only when a task needs them. Then it measures the saving. On [npm](https://www.npmjs.com/package/minnimemory) and as a [Claude Code plugin](https://github.com/MinniAI-com/minnimemory-plugin). |
| MinniMemoryAgent | In development. Keeps a company's agent memory files healthy across its whole fleet and opens a pull request per repo. |
| [MinniCode](https://minniai.com/minnicode) | A terminal coding agent in the shape of Claude Code, built for open LLMs and low token use. |
| [MinniTuner](https://minniai.com/minnituner) | A Windows PC tuner that asks before it changes anything. |

Every claim we make is measured. A blind judge checks answer quality, and failed runs stay on the record. [See the results](https://minniai.com/evidence).

Talk to us at [minniai.com](https://minniai.com).

## Also building

[Prime Investing Capital](https://primeinvestingcapital.org) is an AI trading floor with paying users. Prediction engines scan for stock setups, and each user gets their own AI trading persona, portfolio review and options flow.

## Open source

| Project | What it does |
|---|---|
| [SafeDataBaseMCP](https://github.com/Hamzah-Muhammad/SafeDataBaseMCP) | An MCP server for databases. Reads run right away. A write is previewed in a transaction that gets rolled back, and only that preview can be committed. SQLite, Postgres or AWS RDS. |
| [OpenCodingAgent](https://github.com/Hamzah-Muhammad/OpenCodingAgent) | An open source terminal coding agent on DeepSeek V4 through NVIDIA. Edits files, runs shell and git, opens PRs. Locked to one folder and refuses to read secrets files. |
| [Ticket2PR](https://github.com/Hamzah-Muhammad/Ticket2PR) | Give it a GitHub issue, get a pull request back. Built on the Claude Agent SDK. It never merges, and the tests make sure of that. Desktop app and CLI. |
| [LangGraphAgentTemplate](https://github.com/Hamzah-Muhammad/LangGraphAgentTemplate) | A starting point for agents on LangChain and LangGraph 1.x. Five workflow modes, human approval, long term memory, context compaction, evals and CI come built in. You add the prompt, tools and eval cases. |
| [PricingWebapp](https://github.com/Hamzah-Muhammad/PricingWebapp) | A stock price simulator using Geometric Brownian Motion and Black Scholes pricing, in a trading terminal style UI. Node and React. |
| [PCTuner](https://github.com/Hamzah-Muhammad/PCTuner-Optimization-Tool) | A Windows desktop app that applies PC performance tweaks. It logs every change so it can be undone, and makes a restore point first. |
| [The Edge overview](https://github.com/Hamzah-Muhammad/TheEdge-Overview) | How The Edge, Prime Investing Capital's trading floor, was built and how it fits together. The source is closed. |

## Stack

| Area | Tools |
|---|---|
| Agents | Claude Agent SDK, OpenAI SDK, LangChain, LangGraph, MCP |
| Backend | Python, FastAPI, Node.js, Java, PostgreSQL |
| Frontend | TypeScript, React, Next.js |
| Infra | AWS, Docker, Kubernetes, GitHub Actions |
