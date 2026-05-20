# Hi, I'm Aaditya 👋

**AI Backend Engineer** — I build the systems that sit *behind* AI products: RAG pipelines, multi-agent workflows, and the FastAPI services that serve them.

MS Computer Science @ Syracuse (grad May 2026). I like taking an idea from a rough design doc all the way to a deployed, working system — and I care about the unglamorous parts: keeping the request path fast, gating expensive LLM calls, and making sure things don't fall over under load.

---

### 🛠️ What I work with

**AI / Agentic**  &nbsp; LLMs (OpenAI GPT) · RAG pipelines · Multi-agent systems (LangGraph) · Embeddings & semantic search · Prompt engineering
**Backend**  &nbsp; Python · FastAPI · Django · Flask · async processing · REST APIs
**Data & Vector Stores**  &nbsp; PostgreSQL (pgvector) · Redis · MongoDB · MySQL · query optimization
**Infra & MLOps**  &nbsp; Docker · AWS · Azure · GitHub Actions CI/CD · Celery · Linux
**Testing & Auth**  &nbsp; Pytest · unit/integration testing · JWT · RBAC

---

### 🚀 Things I've built

**🤖 Autonomous Multi-Agent Code Repair System**
A 4-agent LangGraph pipeline — *detector → diagnoser → fixer → validator* — that repairs Python bugs. The validator feeds failure reasons back into the fixer's next attempt, so success rate improves across retries. Tested on 100+ hand-built bugs (type errors, logic faults, infinite loops), tracking pass@1 across iterations. Wrapped as a FastAPI endpoint so it can drop into any CI/CD as a pre-merge check.
`Python · FastAPI · OpenAI GPT · LangGraph · Pytest`

**🔍 AI-Powered Incident Response System (RAG + Agentic)**
A retrieval-first system that embeds incident logs into pgvector and returns the top-3 similar past incidents *before* any LLM call. LLM calls are gated behind a similarity threshold — high-confidence retrievals return the matched incident directly; only low-similarity queries fall through to the model. A Redis cache on the retrieval layer skips re-embedding for semantically similar queries. Built a hand-labeled eval set to measure precision@3 before tuning the threshold.
`FastAPI · OpenAI GPT · Hugging Face · pgvector · Redis`

**😀 Face Emotion Detection**
Full-stack app for real-time emotion classification, with separate REST endpoints for preprocessing, inference, and validation. Structured the inference pipeline around clear response contracts so models could be swapped without touching the frontend.
`React · Flask · Python · Deep Learning`

---

### 💼 Currently

Software Developer @ **iConsult Collaborative** (Syracuse University) — building and maintaining 10+ REST APIs for an AI startup-analysis platform. Recent work: moved long-running inference jobs off the request path with Celery + Redis, set up Docker + GitHub Actions CI/CD on AWS, and redesigned pgvector-backed PostgreSQL indexes to cut latency on retrieval-heavy endpoints.

---

### 📫 Reach me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:aadijoshi11802@gmail.com)

---

<sub>Open to AI/backend engineering roles. Send me a good systems or ML paper and I'll probably want to talk about it.</sub>
