# Muhammad Ridwan

**AI Full Stack Engineer — Agentic Systems & LLM Applications**
Jakarta, Indonesia (UTC+7) · Open to remote — daily overlap with EU hours, evening overlap with US ET

[![Email](https://img.shields.io/badge/Email-ridwanspace.dotcom@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:ridwanspace.dotcom@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-muhammad--ridwan-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-ridwan-0136181a9/)

---

Full-stack engineer with 7+ years across software, data, and ML — the last 3 focused on shipping
production LLM systems end to end: multi-agent orchestration with function calling, RAG pipelines
with evaluation harnesses, multi-provider model routing with cost tracking, and streaming chat UIs.

I build with **Python, TypeScript, and Go** on **Next.js / FastAPI**, and treat evals, guardrails,
token-cost governance, and observability as first-class parts of every AI feature — not an
afterthought bolted on before launch.

Currently **Senior AI Fullstack Engineer at Jatis Mobile**, building a multi-tenant platform for
deploying RAG- and tool-enabled AI agents to WhatsApp.

## What I work on

| | |
|---|---|
| **LLM Engineering** | RAG (hybrid BM25 + vector, reciprocal rank fusion, cross-encoder reranking) · function calling / tool use · structured outputs (Pydantic / Zod) · prompt caching · multi-provider routing & fallback · token-cost metering · prompt-injection defenses |
| **Agents** | LangGraph · Pydantic AI · Mastra · Google ADK · MCP · multi-agent orchestration · agent-loop guardrails (request / token budgets) · agentic coding workflows |
| **Evaluation & Observability** | LLM-as-judge · Langfuse · LangSmith · golden datasets · A/B prompt testing · Sentry · OpenTelemetry |
| **Full Stack** | TypeScript · Python · Go · Next.js 16 (App Router, RSC) · React 19 · Tailwind · shadcn/ui · FastAPI · Node.js · SSE streaming UIs |
| **Data & Infra** | PostgreSQL (RLS, pgvector) · MariaDB · MongoDB · Redis · BigQuery · Kafka · Drizzle · SQLAlchemy · Docker · GCP (Cloud Run, Cloud Tasks, Pub/Sub) · Vercel · GitHub Actions · Terraform |

**Models in production:** Claude Opus 4.8 / Sonnet 5 / Haiku 4.5 · GPT-5.6 · Gemini 3.5 Flash / 3.1 Pro — tiered routing by task complexity.

## Production work

Client and employer systems. Repos are private; happy to walk through architecture and code on request.

### MBS Food Cost — AI-native ERP for a multi-outlet restaurant chain
`Production · GCP Cloud Run` · Next.js 16 · React 19 · TypeScript · Drizzle · MariaDB · Mastra · Gemini + Claude

Multi-tenant food-cost and P&L platform replacing a 40-tab spreadsheet system; corrected the chain's
reported food cost from ~66% to a verified ~45%. Governed AI assistant with **31 read-only
function-calling tools** (discovered via tool-search, not prompt-dumped), a two-agent RAG consultant
with Google Search grounding and cited sources, vision OCR for receipts and bank statements with
Zod-validated multi-stage parsing, and a golden-dataset eval harness. **68-table schema** with
append-only ledgers, idempotent mutations, audit logging, and **~458 test files**.

### KulinerPro — AI-powered ERP for Indonesian F&B businesses
`Deployed · GCP Cloud Run` · FastAPI · Python 3.12 async · MongoDB · Redis · Pydantic AI · Gemini

Solo-built multi-tenant SaaS ERP spanning **36+ modules** (POS, FIFO/FEFO inventory, double-entry
accounting with Indonesian tax compliance, payroll, supplier portal, QR self-service ordering) behind
**1,400+ API endpoints** in a clean/DDD modular monolith. Embedded multi-agent platform: ~10
specialized Pydantic AI agents with delegation graphs, RAG over Gemini embeddings, vector long-term
memory, SSE + voice chat, human-in-the-loop confirmation for write actions, and governance (PII
redaction, tool-call budgets, versioned prompt registry, eval framework with trace assertions).
**1,200+ test files** with an 80% coverage gate and strict mypy.

### RestoGuard — LLM-powered fraud detection for restaurant chains
`Functional MVP` · FastAPI · Pydantic AI · Claude (tiered Haiku → Sonnet → Opus) · PostgreSQL · Redis · arq

Multi-tenant platform pairing a deterministic pandas rule engine (Benford's law, ghost-employee
scoring, vendor-markup and duplicate-invoice detection) with agentic investigation: 7 tenant-scoped
audit tools, prompt caching, SSE streaming, per-tenant token metering with hard budget gates, and
agent-loop request limits. Self-improving CSV ingestion — LLM header-mapping promoted to
deterministic per-tenant adapters after confirmation.

## Open source & demos

| Repo | What it is | Stack |
|---|---|---|
| **[telco-customer-service-agent](https://github.com/ridwanspace/telco-customer-service-agent)** | RAG customer-service agent with confidence-based escalation to a human | FastAPI · Gemini · FAISS · Streamlit |
| **[fastapi-boilerplate-financial](https://github.com/ridwanspace/fastapi-boilerplate-financial)** | Production-grade FastAPI scaffold for financial apps — DDD, clean architecture, idempotency, optimistic locking | FastAPI · async SQLAlchemy · PostgreSQL · Redis |
| **[nutrisnap](https://github.com/ridwanspace/nutrisnap)** | Food photo → FDA-style nutrition label → streaming multimodal chat, no account required | Next.js 16 · TypeScript · Zod · Gemini vision |
| **[code-commit-reviewer](https://github.com/ridwanspace/code-commit-reviewer)** | Automated AI code review over a commit window — no GitHub App, no CI required | Python · Gemini · GitHub REST API |
| **[adk-agent-system-demo](https://github.com/ridwanspace/adk-agent-system-demo)** | Reference multi-agent system on Google ADK — sessions, tools, router-based API design | Python · Google ADK · FastAPI |
| **[ralph-runner](https://github.com/ridwanspace/ralph-runner)** | Agentic CLI for Claude Code workflows — multi-phase tasks, dependency tracking, error-learning | Bash · Claude Code |
| **[restful-fastapi-guidelines](https://github.com/ridwanspace/restful-fastapi-guidelines)** | Living guide to REST API design with FastAPI ([live site](https://restful-fastapi-guidelines.vercel.app)) | Next.js · MDX |
| **[system-tools](https://github.com/ridwanspace/system-tools)** | GUI launcher for Linux system-maintenance bash scripts | Bash · YAD · XFCE |

## Experience

| | |
|---|---|
| **Senior AI Fullstack Engineer** | Jatis Mobile · Jul 2026 – Present |
| **Senior AI Full Stack Engineer** | Paper.id · Jan 2024 – Jul 2026 |
| **Senior Data Engineer** | Paper.id · Jul 2023 – Dec 2023 |
| **Senior Data Scientist** | majoo.id · Jun 2022 – Jul 2023 |
| **IT & Data Science Lead** | PT. Gelora Muda Berjaya · May 2019 – Jun 2022 |

**Certifications:** Google Cloud Professional ML Engineer (2023) · Google Cloud Professional Data Engineer (2022) · AWS Certified Machine Learning – Specialty (2024)

## GitHub

<div align="center">

![Stats](https://github-readme-stats.vercel.app/api?username=ridwanspace&show_icons=true&hide_border=true&theme=transparent&hide_title=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ridwanspace&layout=compact&hide_border=true&theme=transparent&hide_title=true)

</div>

---

**Open to remote AI engineering roles (US / EU).** Reach me at
[ridwanspace.dotcom@gmail.com](mailto:ridwanspace.dotcom@gmail.com) or on
[LinkedIn](https://www.linkedin.com/in/muhammad-ridwan-0136181a9/).
