# Hi, I'm Stefan 👋

I'm a software architect focused on reliable software systems, practical automation, and AI that engineers can inspect and control.

My public projects range from self-hosted applications and reusable infrastructure to reproducible experiments. They explore how to give models useful work while keeping permissions, validation, state, and recovery explicit in code.

## Start here

### [Safeplane](https://github.com/stefanrossmeier/safeplane) · Controlled AI-agent workflows

A local-first control plane for assistant and developer workflows, operated through a CLI or Telegram. A deterministic harness owns execution, tool permissions, credentials, validation, and Git operations; agents work within those boundaries.

Developer runs use isolated workspaces, validate proposed changes, and retain review evidence. Accepted changes can become draft pull requests, with the merge decision left to a human. Deployed on a MacBook and a VPS, with operational hardening still evolving.

[Explore the architecture](https://github.com/stefanrossmeier/safeplane/blob/main/docs/ARCHITECTURE.md) · [Try the secret-free workflow](https://github.com/stefanrossmeier/safeplane#neutral-developer-workflow-example)

### [DailyDash](https://github.com/stefanrossmeier/daily-dash) · Automation from source to delivery

A self-hosted market-intelligence system that turns market data, news, prediction-market activity, and community signals into scheduled Telegram briefings. Windmill orchestrates the work; deterministic processing and scoped LLM ranking produce inspectable artifacts that are persisted before delivery.

The engineering extends beyond report generation: typed configuration, versioned prompts and policies, model cost traces, tests that enforce dependency boundaries, and a reproducible deployment setup.

[Follow the pipeline architecture](https://github.com/stefanrossmeier/daily-dash/blob/main/docs/16_ARCHITECTURE_BOUNDARIES.md) · [Quickstart](https://github.com/stefanrossmeier/daily-dash/blob/main/QUICKSTART.md)

### [LLM Gateway](https://github.com/stefanrossmeier/llm-gateway) · Shared inference with clear ownership

A Python service and lean client for OpenAI and OpenRouter access. Each project owns its model aliases, credentials, and budgets; the gateway handles transport, validation, durable accounting, and request recovery.

The interesting architectural work is in failure handling: stable invocation identities, durable attempt receipts, isolated provider credentials, and explicit distinctions between measured cost, estimates, and unknown exposure. Currently an alpha release.

[Explore the architecture](https://github.com/stefanrossmeier/llm-gateway/blob/main/docs/archdoc/ARCHITECTURE.md) · [Try it without provider keys](https://github.com/stefanrossmeier/llm-gateway/blob/main/QUICKSTART.md)

## More to explore

### Applications and engineering tools

| Project | What to look for |
| --- | --- |
| [AI Dash](https://github.com/stefanrossmeier/ai-dash) | AI news briefings from feeds, papers, releases, and community sources, with article evidence, editorial selection, deduplication, and durable Telegram delivery. |
| [Wikiplane](https://github.com/stefanrossmeier/wikiplane) | Source material compiled into a Markdown-and-Git knowledge base for agent memory and human browsing, preserving provenance and conflicting claims. |
| [Safe Web Research](https://github.com/stefanrossmeier/safe-web-research) | A reference implementation for bounded web research: controlled fetching, resource budgets, source provenance, and claim verification, with authority held in Python code. |
| [AI CraftKit](https://github.com/stefanrossmeier/ai-craftkit) | Reusable agent skills for architecture documentation, ADRs, diagrams, and engineering reviews, separating verified implementation facts from decision rationale. |

### Evaluation and local inference

| Project | What to look for |
| --- | --- |
| [Progressive Disclosure Evals](https://github.com/stefanrossmeier/progressive-disclosure-evals) | Controlled comparisons of progressive disclosure, dense and hybrid RAG, and reranking: evidence discovery, answer quality, context use, and latency measured separately. |
| [Decision Model Evals](https://github.com/stefanrossmeier/decision-model-evals) | A vendor-neutral benchmark for choice, binary, and scoring decisions across 5,760 cases and 16 domains, reporting quality, calibration, latency, reliability, and cost. |
| [Local-First LLM](https://github.com/stefanrossmeier/local-first-llm) | Reproducible Apple Silicon coding setups with MLX/oMLX and VS Code Copilot, plus inspection tools and experiments on prompt overhead, caching, and inference performance. |

## How I approach engineering

- Make responsibilities, trust boundaries, and failure behavior explicit.
- Keep model judgments inspectable and consequential actions controlled by code.
- Measure quality, reliability, latency, and cost against reproducible evidence.
- Prefer maintainable systems and useful documentation over unnecessary complexity.

If you work on software architecture, developer automation, or dependable AI systems, I'd enjoy comparing notes. Pick a project above and explore the code, decisions, and experiments behind it.
