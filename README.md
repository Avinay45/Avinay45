# Avinay (Vinay) Kumar — Backend • AI Systems • Data Engineering

I design and ship production-grade backend systems and AI-enabled products: retrieval-augmented LLM services, reproducible ETL pipelines, and API-first platforms that deliver measurable outcomes. My work focuses on architecture, reliability, and operational reproducibility — not demos.

Repository highlights (evidence)
- RAG & LLM products: election-companion, ai-resume-screening-tool, Resume-Screening-RAG-Pipeline
- Data engineering & APIs: cloud-data-analytics-pipeline (FastAPI, SQLAlchemy, Postgres)
- Backend fundamentals: todoapp (Spring Boot + React)

Links
- GitHub: https://github.com/Avinay45
- Feature repos: election-companion · ai-resume-screening-tool · Resume-Screening-RAG-Pipeline · cloud-data-analytics-pipeline · langchain-course · todoapp

---

## Professional summary
I build backend-first systems that combine durable engineering and applied AI. I design retrieval-powered LLM systems, production ETL pipelines, and REST/edge APIs that are reproducible, testable, and deployable. Typical responsibilities I take on: system design, API contract and schema design, vector index strategy for RAG, deployment automation (Docker / Compose / CI), and operational runbooks.

What I deliver
- Deterministic retrieval + LLM pipelines for domain assistants
- Reproducible ETL workflows and analytics APIs
- Clean, layered backend services with observable behavior
- Minimal, focused frontends and UX for product validation

---

## Engineering domains

### AI Systems
What I build
- Retrieval-Augmented Generation (RAG) systems with explicit retrieval logic, provenance, and source attribution.
- Embedding pipelines and scale-aware vector indexing (FAISS / pgvector).
- Production prompts, LLM orchestration, and deterministic evaluation for business workflows.

How I create value
- Turn unstructured documents into searchable knowledge with clear relevance metrics.
- Design retrieval strategies (small-to-big chunking, hybrid retrievers) to reduce hallucination and improve explainability.

### Backend Engineering
What I build
- API-first services with versioned endpoints, input validation, and contract tests.
- Layered backend architecture (Controller → Service → Repository) and robust error handling.

How I create value
- Reduce integration friction with clear OpenAPI/Swagger contracts and example requests.
- Protect data flows (auth, RLS where appropriate) and document service SLAs for on-call teams.

### Data Engineering
What I build
- Reproducible ETL: ingestion → validation → transformation → storage → analytics.
- Analytics endpoints that return business KPIs (aggregations, cohort analyses).

How I create value
- Provide teams with reliable, queryable datasets and APIs for dashboards and ML pipelines.
- Automate data quality checks and make pipelines re-runnable (Dockerized + versioned schemas).

### Cloud & DevOps
What I build
- Containerized services (Docker + Compose) and CI pipelines for linting, tests, and builds.
- Serverless edges for low-latency LLM integration and secure database access patterns.

How I create value
- Reduce time-to-deploy and ensure reproducible environments for reviewers and hiring managers.
- Add basic observability (logs, OpenAPI, health checks) so projects are interview-review ready.

### Full-Stack (practical)
What I build
- Minimal, purposeful frontends (Next.js / React / Streamlit) that surface product flows and debugging views.

How I create value
- Ship a small UI for stakeholder validation; keep the backend as the source of truth.

---

## Technical expertise (evidence-based)
Languages
- Python · TypeScript · Java · JavaScript · SQL · HTML/CSS

Backend
- FastAPI · Spring Boot · Node.js / Edge Functions · REST · OpenAPI/Swagger

Frontend
- Next.js · React · Streamlit · Tailwind CSS · Vite

Databases & Indexing
- PostgreSQL (Supabase) · pgvector · FAISS · H2 (dev)

AI & Machine Learning
- LangChain patterns · embeddings (sentence-transformers, gte-small) · spaCy · scikit-learn · RAG design

Data Engineering
- Pandas · NumPy · SQLAlchemy · synthetic data generation

Cloud & DevOps
- Docker · Docker Compose · GitHub Actions · AWS S3 (object storage)

Developer tools
- Git · Postman/Swagger · basic CI workflows

(Only technologies with repository evidence are listed.)

---

## Featured engineering case studies

### 1) ElectionGuide AI — election-companion
Project overview
- Production-oriented RAG assistant for Indian election information: eligibility, registration steps, polling booth search, and timeline visualization.

Business problem
- Reduce misinformation and friction for first-time or infrequent voters; provide state-aware guidance and resources.

Technical architecture
- Next.js (App Router, UI) → Serverless edge functions (chat & retrieval) → Supabase (Postgres + pgvector) → Embeddings service → LLM gateway.
- Security: Supabase Auth + Row-Level Security (RLS) patterns for user-scoped features.

Key engineering challenges
- Multilingual retrieval and prompt conditioning
- Low-latency retrieval pipeline with 384-dim embeddings + tuned Top-K
- Secure serverless access to the vector store without exposing keys to the client

Impact
- Product-ready architecture that demonstrates RAG production patterns and civic impact.

Repository
- https://github.com/Avinay45/election-companion

---

### 2) AI Resume Screening Tool — ai-resume-screening-tool
Project overview
- End-to-end system to parse resumes, build semantic indexes, and provide recruiter-facing ranking and chat.

Business problem
- Automate first-pass candidate screening and produce consistent, explainable ranking for hiring teams.

Technical architecture
- PDF parsing (pdfplumber) → NLP extraction (spaCy) → Sentence embeddings → FAISS vector index → RAG retrieval → LLM evaluation → Streamlit dashboard.

Key engineering challenges
- Robust text extraction from noisy PDFs
- Deterministic ranking pipeline to enable recruiter trust
- Integrating FAISS with downstream LLM evaluation and report generation

Impact
- Prototype that standardizes screening and can be productized into HR tooling.

Repository
- https://github.com/Avinay45/ai-resume-screening-tool

---

### 3) Resume Screening RAG Pipeline — Resume-Screening-RAG-Pipeline
Project overview
- Research-oriented RAG pipeline implementing adaptive retrieval patterns and RAG-fusion strategies.

Business problem
- Improve LLM reliability on document-grounded tasks by conditioning on curated resume chunks.

Technical architecture
- Chunking → embeddings → FAISS → hybrid retrieval (query classification + small-to-big retrieval) → LLM conditioning and evaluation → Streamlit demo.

Key engineering challenges
- Chunk retrieval traceability and provenance for each LLM response
- Adaptive toggling of retrieval modes based on prompt type
- Demonstrating RAG fusion techniques end-to-end

Impact
- Provides a template for reliable, auditable LLM-assisted candidate evaluation.

Repository
- https://github.com/Avinay45/Resume-Screening-RAG-Pipeline

---

### 4) Cloud Data Analytics Pipeline — cloud-data-analytics-pipeline
Project overview
- Reproducible cloud-native ETL pipeline that ingests synthetic transactional data and exposes analytics via a FastAPI service.

Business problem
- Demonstrate a production-style data pipeline: ingestion, validation, transformation, storage, and analytics API surface.

Technical architecture
- CSV Generator → S3 raw layer → validation & transformation scripts (Pandas) → SQLAlchemy → Supabase/Postgres → FastAPI analytics endpoints (Swagger).

Key engineering challenges
- Building reproducible local/dev environments (Docker) for data engineers
- Designing SQL-friendly schemas and analytic queries for performant aggregation
- Exposing analytics via stable API contracts

Impact
- Demonstrates full data lifecycle and API patterns for analytics consumers.

Repository
- https://github.com/Avinay45/cloud-data-analytics-pipeline

---

### 5) LangChain Course — langchain-course
Project overview
- Project-based learning resource that walks through LangChain and agent patterns with practical code examples and exercises.

Value
- Demonstrates familiarity with LangChain concepts and agent architectures, useful when discussing design trade-offs in interviews.

Repository
- https://github.com/Avinay45/langchain-course

---

### 6) TodoApp (Spring Boot + React) — todoapp
Project overview
- Layered backend example demonstrating DTOs, validation, exception handling, and a React frontend.

Engineering value
- Solid evidence of classical backend design and clean separation of concerns.

Repository
- https://github.com/Avinay45/todoapp

---

## System design & engineering principles

System design
- Design for clear contracts: define OpenAPI first for services and keep backwards-compatible changes.
- Prioritize observable behaviour: health checks, structured logs, and small smoke tests.

Reliability
- Favor deterministic pipelines and idempotent operations for ETL and retrieval.
- Add provenance to retrieval results; expose sources in API responses.

Scalability
- Separate compute and storage: vector indexes and databases scale independently.
- Use efficient indexes (HNSW / FAISS / pgvector) and tune top-K/thresholds.

Maintainability
- Keep code modular and well-typed (where applicable), with small, focused tests and reproducible dev environments (Docker + Compose).

Documentation
- README should state: problem, architecture, run instructions, demo link, and "my role".
- Provide minimal runbooks for reproduction and basic troubleshooting.

Developer experience
- One-command local bootstrap: sample data + docker-compose → run smoke test → see demo.
- CI enforces linting and smoke tests before merging.

---

## Open source & professional growth
- Public contributions (recommended next steps): identify 2–3 upstream projects you rely on (LangChain, FAISS integrations, Supabase SDK) and contribute targeted fixes or docs.
- Technical writing: create concise engineering notes: "Designing production RAG: retrieval, provenance, and costs" and link them in the repo READMEs.
- Research artifacts: convert experiment notebooks into reproducible demos with pinned dependencies and Dockerfiles.

(If you want, I will draft contribution ideas and PR templates.)

---

## GitHub metrics (place in README for recruiters)
<div align="center">
  ![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Avinay45&theme=tokyonight&show_icons=true&hide_border=true)
  &nbsp;&nbsp;
  ![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Avinay45&theme=tokyonight&hide_border=true&layout=compact)
  <br/>
  ![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=Avinay45&theme=tokyonight)
  &nbsp;&nbsp;
  ![Trophy](https://github-profile-trophy.vercel.app/?username=Avinay45&theme=tokyonight)
</div>

---

## Contact
- LinkedIn: (add your LinkedIn URL)
- Portfolio / demos: (add hosted demo URLs)
- Email: you@domain.com
- GitHub: https://github.com/Avinay45

---

Minimal operational checklist for each featured repo (apply across pinned repos)
- Add LICENSE (MIT or Apache-2.0)
- Top-of-README: one-line problem, one-line impact, demo GIF or link
- Add reproduce script: docker-compose up → run demo script
- Add basic CI: lint + smoke test
- Add "my role" and "what I solved" bullets
