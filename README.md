<div align="center">

```text
 ╔═══════════════════════════════════════════════════════════════════════╗
 ║   ____                                          _                     ║
 ║  |  _ \ __ _ _ __ __ _ _ __ ___   ___ ___   __| | ___  ___            ║
 ║  | |_) / _` | '__/ _` | '_ ` _ \ / __/ _ \ / _` |/ _ \/ __|           ║
 ║  |  __/ (_| | | | (_| | | | | | | (_| (_) | (_| |  __/\__ \           ║
 ║  |_|   \__,_|_|  \__,_|_| |_| |_|\___\___/ \__,_|\___||___/           ║
 ║                                                                       ║
 ║   Autonomous Agents • Terminal TUIs • RAG • Systems Engineering       ║
 ╚═══════════════════════════════════════════════════════════════════════╝
```

<p align="center">
  <a href="https://paramveer.me"><img src="https://img.shields.io/badge/Portfolio-paramveer.me-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/paramveer-singh-2b619a296/"><img src="https://img.shields.io/badge/LinkedIn-Paramveer_Singh-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:sparamveer1001@gmail.com"><img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

</div>

```bash
$ cat ~/.profile.json
{
  "engineer": "Paramveer Singh",
  "focus": ["Autonomous Coding Agents", "Hierarchical RAG", "Distributed Systems & TUIs"],
  "philosophy": "Understand the runtime from scratch rather than wrapping black-box SDKs"
}
```

---

### ⚡ Quick Scan: Featured Builds

```bash
$ ls -la ~/projects/featured --sort=recent
```

| System / Tool | Core Architecture & Problem Solved | Stack |
|---|---|---|
| **[Maggie](https://github.com/paramcodes/maggie)** | **Autonomous terminal coding agent**. Dual `PLAN`/`BUILD` modes, multi-provider LLM gateway, human-in-the-loop security confirmation gates, reactive `@` file mentions, and persistent SQLite WAL sessions. | Bun • OpenTUI • SQLite |
| **[Nexus](https://github.com/PARAM-ship/nexus-review)** | **Multi-agent PR reviewer**. Native GitHub Action running AST diff parsing → planner → 4 parallel specialist reviewers (style, security, perf, tests) → critic agent → aggregator with LLM-as-judge evals. | TS • Bun • Groq |
| **[ATLAS](https://github.com/paramcodes/rag-agent-api)** | **Production-grade hierarchical RAG**. Docling ingestion, Jina v3 embeddings, RAPTOR tree clustering (UMAP + HDBSCAN), hybrid BM25 + pgvector HNSW search with RRF fusion, and Prometheus observability. | Bun • Fastify • pgvector • Prometheus |
| **[Night Code](https://github.com/paramcodes/brightbot)** | **Open-source terminal coding harness**. Local code inspection, AST edits, and token-by-token streaming via a stateless relay with local execution authority. | TypeScript • OpenTUI |
| **[BackendSaga](https://github.com/paramcodes/backendsaga)** | **Interactive systems failure explorer**. Incident triage engine, failure modes knowledge graph, and evidence library for distributed backend systems. | Next.js • TypeScript • GraphViz |
| **[Ben](https://github.com/paramcodes/ben)** | **Systems agent runtime in Rust**. Learning-oriented terminal coding agent harness exploring low-level process management and tool orchestration. | Rust |
| **[Junior Doctor](https://github.com/paramcodes/junior-doctor)** | **AI clinical document pipeline**. Scanned patient records → structured discharge summaries with provenance tracking, conflict detection, and anti-hallucination guardrails. | Python • LLM Evals |
| **[devops-infra](https://github.com/paramcodes/devops-infra)** | **Distributed inference architecture**. Multi-VM inference cluster on AWS with private subnet routing, RPC worker communication, and Terraform provisioning. | Python • Terraform • AWS |

---

### 🔬 Architecture Deep Dives

<details open>
<summary><b>🪄 Maggie — Autonomous TUI Coding Assistant</b></summary>
<br>

[![Maggie Demo](https://raw.githubusercontent.com/paramcodes/maggie/main/docs/maggie_demo.gif)](https://github.com/paramcodes/maggie)

- **Dual Execution Modes**: Instant `Shift+Tab` toggle between **PLAN** (read-only architectural analysis & codebase reconnaissance) and **BUILD** (autonomous file modifications and command execution).
- **Security Confirmation Gate**: Destructive actions (`write`, `edit`, `bash`) trigger human-in-the-loop confirmation gates before execution.
- **Universal Clipboard & Reactive Mentions**: Native OSC 52 mouse drag text selection copies directly to system clipboard across SSH/local sessions; reactive `@` file search with fuzzy scoring.
- **Persistence**: Bun SQLite in WAL mode with cascading session indexing and cross-session resume.

</details>

<details>
<summary><b>🛡️ Nexus — Multi-Agent PR Reviewer Action</b></summary>
<br>

- **Specialist Fan-Out**: Diff parser slices changes by AST boundary and fans them out to 4 parallel specialist reviewer agents (Style, Security, Performance, Test Coverage).
- **Writer / Critic Loop**: A dedicated Critic agent validates each finding against the original file context before aggregation to eliminate hallucinated issues.
- **LLM-as-Judge Evals**: Benchmarked against synthesized PR datasets with ground truth validation to track precision/recall over prompt and model iterations.

</details>

<details>
<summary><b>🧠 ATLAS — Production-Grade Hierarchical RAG Agent</b></summary>
<br>

- **RAPTOR Hierarchical Indexing**: Replaces flat chunking by recursively clustering document vectors (UMAP dimensionality reduction + HDBSCAN) and summarizing clusters with Gemini to answer high-level thematic queries.
- **Hybrid Retrieval & RRF**: Combines pgvector cosine similarity (HNSW index) and PostgreSQL BM25 full-text search using Reciprocal Rank Fusion ($k=60$).
- **Precision Reranking**: Passes candidate documents through Jina Reranker v2 before final prompt synthesis.
- **Observability**: Prometheus `/metrics` endpoint with Grafana dashboards for latency, token spend, and retrieval cache hits.

</details>

---

### 🛠️ Tech Stack & Systems

```ini
[Core Languages]       TypeScript  •  Rust  •  Python  •  C++  •  Go  •  SQL
[Agents & Retrieval]   OpenTUI  •  Jina v3  •  pgvector  •  RAPTOR  •  Docling  •  BM25
[Backend Runtimes]     Bun  •  Node.js  •  Fastify  •  FastAPI  •  Express
[Databases & Caching]  PostgreSQL  •  Redis  •  SQLite (WAL)  •  Neo4j
[Infra & DevOps]       Linux  •  Docker  •  Terraform  •  AWS (VPC/Private Subnets)  •  GitHub Actions
```

---

### 📌 Hard-Won Engineering Lessons

- **Validate schemas, not just prompts**: LLM evaluators and critic judges hallucinate confidently when template variables or context slots are empty or malformed.
- **Target logic patterns, not syntax**: Critic agents need rules targeted at structural bug patterns rather than exact phrasing, otherwise paraphrased bugs slip right through.
- **Hierarchical retrieval beats flat chunking**: For multi-page technical documents, recursive clustering (RAPTOR) preserves cross-document context that standard RAG chunks miss completely.

---

<div align="center">

```text
Let's build systems that matter.
```

<sub>Open to systems engineering, autonomous agent infrastructure, and low-level tooling roles.</sub>

</div>
