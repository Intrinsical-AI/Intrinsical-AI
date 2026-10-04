# Welcome to Intrinsical-AI 👋

At the intersection of LLMs and engineering I build **evaluation** frameworks; search, retrieval, and GenAI **systems and tooling**; as well as exploring some research lines and techniques that I find interesting. 

**Focus areas:** Applied ML · Retrieval/RAG/Search · System Architecture · LLM Evaluations

---

## Evaluation & Reliability

> Promptfoo, Ragas, custom evaluators, retrieval metrics, and regression testing.

* **LLM-as-a-judge:** multi-judge, meta-evaluations, calibration and agreement. Rubric design, failure analysis, and iterative progress.
* **Decoupling systems by modules**: split by modules and implement independent evaluations on retrieval, generation, routing, etc.
* **Search and RAG evaluation:** curated test sets, ranking metrics, custom evaluators, benchmarking, and systematic error analysis.
* **Evaluation-driven development:** use quality gates to compare models, retrieval strategies, prompts, and system configurations.
* **Adversarial / stress testing:** red-teaming, jailbreak robustness, edge-case discovery, and bias detection.

---

## Search, Retrieval & RAG

* **Legal Engine Search - LES (2024)**
   An exploratory evaluation pipeline (n=14 queries) for Spanish criminal case law: a CENDOJ sample of ~5,000 records (2020–2024). Relevance graded by consensus among five LLMs with expert review. SentenceTransformer led in Precision@10 (0.92 vs. 0.86 for BM25) and reached an MRR of 1.0; BM25 matched or outperformed it in nDCG (0.915 vs. 0.896). Key takeaway: complementarity rather than a single winner.
  [UPM repository (authentication required)](https://oa.upm.es/87939/)

* **[Modular RAG](https://github.com/Intrinsical-AI/rag-prototype)**
  A modular RAG framework based on Ports and Adapters architecture, with interchangeable retrieval, persistence, model-provider, and evaluation components. Flexible, local, and custom data-management for local agents.
  > Local benchmark: retrieval across 10k chunks (128 tokens): 1.49s index build/load, 4.51s SQLite write, and 99.9ms p50 / 132.0ms p95 across 300 warm-cache queries on BM25 retrieval.

---

## AI Systems & Developer Tooling

* **[RepoGPT](https://github.com/Intrinsical-AI/RepoGPT)**
  Generates structured codebase representations for humans, LLMs, indexing pipelines, and RAG systems. Strict determinism (hash-verified functional idempotency).
  > Local benchmark on synthetic data: parsing performance of ~18.4k LOC/s (.py/.md).

* Agent-oriented developer tooling using structured Command-Line Interfaces (CLIs), local Model Context Protocol (MCP) servers, custom tools, and reproducible development environments.

> **WIP**: governed agent runtimes, event-based execution, explicit tool contracts, approvals, observability, traceability, and recoverable workflows.

---

## Open Source Contributions

**[RRE](https://github.com/SeaseLtd/rated-ranking-evaluator/commits/dataset-generator/?author=Intrinsical-AI)**
  20+ contributions delivering Vespa search integration, Quepid containerization, embedding pipelines, and CI/type-safety hardening. 

**[llm-search-quality-evaluation](https://github.com/SeaseLtd/llm-search-quality-evaluation/commits/main/?author=Intrinsical-AI)**
  Additionally to RRE contributions: research on how to use the new Solr 9.X features to implement retrieval based on embeddings on the RRE framework. Result: no modifications needed in core code, clean workaround using Solr DSL.
  

---

## Research & Experimental

* **[Geometric-Aware Retrieval](https://github.com/Intrinsical-AI/geometric-aware-retrieval-v2)**
  Experimental - research on graph curvature, manifold structure, representation geometry, and non-Euclidean retrieval.

* Current research/learning areas:
  * fairness and Responsible AI, bias in LLMs, latent personas, and EU AI Act compliance;
  * geometry and topology of representation spaces, custom retrieval under anisotropy // local structural distortion, compression efficiency;
  * meta-evaluation of LLM judges, uncertainty estimation
  * agentic systems; local inference, automated decision systems;

---

## Writing

* [Medium - IntrinsicalAI](https://medium.com/@IntrinsicalAI)
* [Substack - Intrinsical-AI](https://substack.com/@intrinsicalai)

---

Always open to discussing search, evals, benchmarks, representation learning, or playing a game of chess or poker
