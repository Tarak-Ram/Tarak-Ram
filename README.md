# Hi, I'm Taraka Ramarao Varanasi 👋

**Senior Full Stack Software Engineer · Team Lead · AI/LLM Engineer** — Hyderabad, India

I build production AI and microservices platforms with **Python/FastAPI** and **Node.js**. For 7+ years I've worked on recruitment and HRMS products at Akrivia Automation, where I now lead a team of 10–15 engineers. The platforms I've architected serve **60K+ daily users and 1M+ API requests a day**.

Lately I've been focused on **Generative AI**: RAG, agentic workflows with LangGraph, LLM evaluation and guardrails. I like AI systems that are measured, tested in CI, and safe to ship.

---

## 🚀 Featured projects

### [RAG HR Policy Assistant](https://github.com/Tarak-Ram/rag-hr-assistant)
An agentic RAG assistant, built as a LangGraph state machine, that answers employee policy questions with section-level citations.
- Hybrid retrieval (Qdrant vector search + BM25 with Reciprocal Rank Fusion) and heading-aware chunking: **100% retrieval hit@4** on a labelled eval set
- Relevance grading, a bounded query-rewrite loop and citation verification turn unsupported answers into safe refusals (**100% refusal precision/recall**, prompt-injection attempts included)
- An eval suite (routing, hit@k, correctness, LLM-as-a-Judge faithfulness) runs as a **CI quality gate on every PR**: 96% answer correctness
- Works with any LLM provider: OpenAI, Azure OpenAI, vLLM, Ollama

`Python` `LangGraph` `FastAPI` `Qdrant` `BM25` `Docker` `GitHub Actions`

### [Multilingual AI Customer Assistant](https://github.com/Tarak-Ram/multiLang_calling_agent)
A multi-tenant WhatsApp assistant for clinic bookings and customer support in **Telugu, Hindi and English**, code-mixed text included.
- A cost-tiered LLM router (rules → FAQs → semantic cache → small LLM → RAG → stronger LLM → human handoff): **~80% of conversations need zero LLM calls**
- Grounded RAG on pgvector with deterministic checks, plus a state machine that re-validates booking slots against live data
- Switches LLM models at runtime without a redeploy (LiteLLM), with a circuit breaker and fallback, zero-downtime re-embedding and per-tenant cost reports
- Webhook signature verification, per-tenant isolation, PII masking and SSRF guards; a 54-conversation multilingual eval suite (100% pass) and 330+ tests

`Python` `FastAPI` `PostgreSQL` `pgvector` `Redis` `LiteLLM` `WhatsApp Cloud API` `Docker`

---

## 🛠️ Tech stack

| Area | Tools |
|---|---|
| **AI / LLM** | Generative AI, RAG, Agentic AI, LangChain, LangGraph, Tool Calling, Embeddings, Hybrid Search, Semantic Caching, Guardrails |
| **LLM Evals** | Eval-Driven Development, LLM-as-a-Judge, Retrieval metrics (hit@k), Faithfulness, Prompt-Injection Defence |
| **LLM Providers** | OpenAI, Azure OpenAI, vLLM, Ollama, LiteLLM |
| **Backend** | Python, FastAPI, Pydantic, SQLAlchemy, Node.js, Express.js, NestJS, GraphQL |
| **Frontend** | Angular, React, TypeScript |
| **Data** | PostgreSQL, pgvector, Qdrant, MySQL, MongoDB, Redis, Kafka |
| **Cloud & DevOps** | AWS (Lambda, S3, RDS), Azure App Service, Azure DevOps, Docker, GitHub Actions, CI/CD |

---

## 💼 At work

- Architected **Realm**, a RAG-based recruitment and HRMS assistant (Python/FastAPI + LangGraph, integrated with a Node.js platform), with prompt evaluation and Human-in-the-Loop validation before rollout
- Built a video-interview analytics pipeline (speech-to-text + NLP) that produces transcript summaries and skill-coverage insights
- Designed microservices for high-concurrency Recruitment and HRMS workflows; Redis caching and API optimisation made the platform **25–35% faster**
- Built a document generation engine that serves **100+ clients**

---

## 📫 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Taraka%20Ramarao%20Varanasi-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/taraka-rama-rao-varanasi-0581241a3)
