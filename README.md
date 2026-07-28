<h1 align="center">Hi, I'm Paramveer 👋</h1>
<h3 align="center">Building multi-agent systems, RAG pipelines, and low-level tools from scratch</h3>

<p align="center">
  <a href="https://paramveer.me"><img src="https://img.shields.io/badge/portfolio-paramveer.me-black?style=flat-square" /></a>
  <a href="https://www.linkedin.com/in/paramveer-singh-2b619a296/"><img src="https://img.shields.io/badge/LinkedIn-Paramveer%20Singh-blue?style=flat-square&logo=linkedin" /></a>
  <a href="https://paramveer.hashnode.dev/"><img src="https://img.shields.io/badge/blog-hashnode-2962FF?style=flat-square&logo=hashnode" /></a>
  <a href="https://x.com/Your_PARAM"><img src="https://img.shields.io/badge/twitter-@Your__PARAM-1DA1F2?style=flat-square&logo=x" /></a>
</p>

---

### ⚡ About

CS Engineering student building things that don't have obvious tutorials for them — agent pipelines with real eval loops, a git implementation from the object model up, distributed inference infra on bare Terraform. I'd rather understand *why* something works than call an SDK that hides it.

- 🔭 Currently building: multi-agent systems, a Rust CLI media player, and a git clone from scratch
- 🌱 Digging into: low-level systems programming, distributed infra, DevOps
- 🎯 Looking for: internships/roles where I can ship real systems, not just wire up APIs

---

### 🚀 Featured builds

| Project | What it actually does |
|---|---|
| **[Nexus](https://github.com/PARAM-ship/nexus-review)** | Multi-agent PR reviewer running as a GitHub Action. Diff parser → planner → 4 parallel specialist reviewers (style/security/perf/tests) → critic agent → aggregator. Built in TS/Bun on Groq, with LLM-as-judge evals and a writer/critic self-correction loop. |
| **[ATLAS](https://github.com/paramcodes/rag-agent-api)** | Production-grade RAG knowledge agent. Docling ingestion, Jina v3 embeddings, RAPTOR hierarchical indexing (UMAP + HDBSCAN + recursive summarization), hybrid BM25+vector retrieval with RRF fusion, Prometheus/Grafana observability. |
| **rgit** | Git, reimplemented from scratch in Rust — the four-object model, SHA-1 content-addressable storage, zlib compression, building up to full tree encoding. |
| **SolIntent** | Solana agent that executes on-chain transactions from plain English, using Jupiter's Ultra Swap API + Claude — built for the Colosseum hackathon. |
| **devops-infra** | Distributed multi-VM inference system on AWS (private subnets, RPC-based worker comms, Terraform provisioning) for Alchemyst AI. |
| **junior-doctor** | AI clinical document pipeline — scanned patient records → structured discharge summaries, with provenance tracking, conflict detection, and a no-fabrication guardrail. |

---

### 🛠️ Stack

<p>
  <img src="https://skillicons.dev/icons?i=ts,js,rust,py,cpp,java,solidity,react,nextjs,nodejs,express,fastapi,postgres,redis,docker,aws,terraform,linux,git,githubactions&theme=dark" />
</p>

---

### 📌 A few lessons from shipping these

- Interpolating arrays into template strings silently gives you `[object Object]` — always stringify explicitly.
- LLM judges hallucinate confidently when their input slots are empty. Guard the data, not just the prompt.
- Critic agents need rules targeted at *logic patterns*, not exact phrasing, or they miss paraphrased bugs.

---

<p align="center"><i>Open to internships and collaborations — reach out on LinkedIn or via my portfolio.</i></p>
