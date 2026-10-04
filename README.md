<div align="center">

# Hi, I'm Abhishek Thakur 👋

**Software Engineer · .NET backends · Search, RAG & vector retrieval · Event-driven systems**

I build backend systems that need to be fast at scale, and the search and AI layers that sit on top of them.

<a href="https://thakurabhishek7283.github.io/under-formation/"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-under--formation-0F172A?style=for-the-badge&logo=astro&logoColor=white"></a>
<a href="https://www.linkedin.com/in/abhishek-thakur-072a981b6/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
<a href="https://leetcode.com/u/abhishekthakur7283/"><img alt="LeetCode" src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"></a>
<a href="mailto:thakurabhishek7283@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-Say%20hi-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>

</div>

---

## About me

- 💼 **Software Engineer at [Eurofins IT Delivery Center](https://www.eurofins.com/)**: Elasticsearch hybrid search, RAG, embeddings and **Model Context Protocol** endpoints for an enterprise procurement platform.
- 📹 Before that, 2.5 years at **I2V Systems** on a video analytics platform deployed across **up to 10,000 cameras**: face recognition, ANPR, event pipelines and PostgreSQL/TimescaleDB performance.
- 🛠️ **3.5+ years** of professional experience in total, mostly C# / .NET 8, PostgreSQL and Angular.
- 🧩 Outside work I build **open-source developer tools**: a family of framework-agnostic collaboration kits, an AI circuit tutor in Rust + WebAssembly, and an AI resume tailoring app.
- 🎓 B.Tech in Information Technology, Maharaja Agrasen Institute of Technology (2023).

## Impact at a glance

| | Result | Where |
| :-: | --- | --- |
| ⚡ | **20–30 → 500+ events/sec** through a RabbitMQ / MassTransit / Hangfire pipeline | I2V Systems |
| ⏱️ | **12 min → under 1 min (−92%)** for a 100K+ record analytics export in .NET + PostgreSQL | I2V Systems |
| 🧠 | **−75% ANN index memory** for face recognition with scalar quantization (Milvus HNSW / IVF SQ8, pgvector) | I2V Systems |
| 📈 | **70 → 300+ frames/sec** TimescaleDB ingestion for 400 cameras through indexing and query-plan tuning | I2V Systems |
| 🏗️ | **−90% dependency violations, −20% production issues** after moving a 40+ project .NET 8 monolith toward Clean Architecture | I2V Systems |
| 🎯 | **CI relevance gate** that fails builds when search/RAG ranking drops below **0.85 MRR/NDCG** on a golden-query set | Eurofins |

## Experience

<details open>
<summary><b>Eurofins IT Delivery Center</b>: Software Engineer · <i>Oct 2025 – Present</i></summary>
<br>

- Catalog search on **Elasticsearch** in .NET that combines exact SKU matching, trigram typo tolerance, scientific-term synonyms and dense-vector similarity using **Reciprocal Rank Fusion**, with indexes kept in sync through **Change Data Capture**.
- Extended the **RAG pipeline** for assay documentation: metadata-driven chunking, Azure OpenAI embeddings, ingestion moved to **Hangfire** background jobs and **Redis semantic caching** for repeat queries.
- Exposed procurement capabilities to internal LLM agents through **MCP endpoints in ASP.NET Core**, with typed tool schemas and role-based access control.
- Added **Angular SSR** to a headless Umbraco site, with Redis-cached HTML and **AWS S3 / CloudFront** asset delivery for SEO-critical pages.

</details>

<details>
<summary><b>I2V Systems</b>: Software Engineer · <i>Apr 2023 – Sep 2025</i></summary>
<br>

- Worked on an **event-driven platform** (RabbitMQ, MassTransit, Hangfire) supporting deployments of up to 10,000 cameras.
- Built a **face recognition pipeline** on pgvector and Milvus, with embeddings served through **NVIDIA Triton**.
- Built **ANPR pipelines and dashboards** for traffic violations and entry/exit monitoring, including a Central Monitoring Hub that aggregates events from **100+ servers**, made fast with materialized views, scheduled preprocessing and query tuning.
- Diagnosed database bottlenecks with PostgreSQL query plans and rewrote inefficient EF Core queries.

</details>

## Featured projects

### 🧱 [Tessera](https://github.com/thakurabhishek7283/tessera): build collaborative apps from pieces

Chat, video calls, comments, kanban, notes, a rich-text editor, image annotation and maps as **framework-agnostic Web Components**. You switch each feature on through configuration, and a feature you don't enable never loads its code. The same kits run across browser tabs with no backend, against the reference server, or against your own API.

<table>
  <tr>
    <td width="33%"><a href="https://github.com/thakurabhishek7283/tessera-realtime"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/thakurabhishek7283/tessera-realtime/main/docs/media/chat-dark.png"><img alt="Tessera realtime chat with reactions, read receipts and typing indicator" src="https://raw.githubusercontent.com/thakurabhishek7283/tessera-realtime/main/docs/media/chat-light.png"></picture></a></td>
    <td width="33%"><a href="https://github.com/thakurabhishek7283/tessera-workspace"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/thakurabhishek7283/tessera-workspace/main/docs/media/kanban-dark.png"><img alt="Tessera workspace kanban board with labels, due dates and assignees" src="https://raw.githubusercontent.com/thakurabhishek7283/tessera-workspace/main/docs/media/kanban-light.png"></picture></a></td>
    <td width="33%"><a href="https://github.com/thakurabhishek7283/tessera-visual"><picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/thakurabhishek7283/tessera-visual/main/docs/media/annotate-dark.png"><img alt="Tessera visual image annotator with labelled shapes" src="https://raw.githubusercontent.com/thakurabhishek7283/tessera-visual/main/docs/media/annotate-light.png"></picture></a></td>
  </tr>
  <tr>
    <td align="center"><sub>Realtime: chat · WebRTC video · presence · comments</sub></td>
    <td align="center"><sub>Workspace: kanban · sticky notes · rich-text editor</sub></td>
    <td align="center"><sub>Visual: image annotation · whiteboard · maps</sub></td>
  </tr>
</table>

| Repository | What it is | |
| --- | --- | --- |
| [`tessera`](https://github.com/thakurabhishek7283/tessera) | Plugin host, zod-validated config and wire protocol, transports (BroadcastChannel / WebSocket), storage adapters (IndexedDB, REST, …), 18 accessible UI primitives, React bridge | [Playground](https://thakurabhishek7283.github.io/tessera/playground/) · [Docs](https://thakurabhishek7283.github.io/tessera/) |
| [`tessera-realtime`](https://github.com/thakurabhishek7283/tessera-realtime) | Presence and live cursors, chat with reactions and read receipts, WebRTC mesh video with screen sharing, threaded comments | [Live demo](https://thakurabhishek7283.github.io/tessera-realtime/) |
| [`tessera-workspace`](https://github.com/thakurabhishek7283/tessera-workspace) | Rich-text editor with slash menu and Markdown, sticky notes, kanban with WIP limits, keyboard drag-and-drop and undo/redo | [Live demo](https://thakurabhishek7283.github.io/tessera-workspace/) |
| [`tessera-visual`](https://github.com/thakurabhishek7283/tessera-visual) | Image annotator and whiteboard (W3C Web Annotation import/export), MapLibre maps with clustering, form-associated location picker | [Live demo](https://thakurabhishek7283.github.io/tessera-visual/) |
| [`tessera-server`](https://github.com/thakurabhishek7283/tessera-server) | Self-hostable Fastify backend: WebSocket rooms, chat history, versioned document store with optimistic concurrency, uploads, TURN credentials, bring-your-own JWT/JWKS auth | `docker compose up` |

**Engineering:** TypeScript · pnpm + Turborepo monorepos · Vitest browser mode · Playwright e2e · axe-core with WCAG 2.2 AA colour tokens · CI on every repo · architecture decision records

---

### ⚡ [Circuit Forge](https://github.com/thakurabhishek7283/Analog-Copilot): AI analog-circuit tutor (in progress)

An LLM composes circuits from **verified building blocks** and streams them to the browser, where they are laid out, animated and **simulated live with ngspice compiled to WebAssembly**. The shared core, the editor and the generation pipeline are built; next is a tutor that answers questions by citing the live simulation values.

- **One Rust crate as the source of truth** (IR, op protocol, electrical rule checks, SPICE compiler), compiled to **WASM** (wasm-bindgen) for the React editor and to a **Python** module (PyO3) for the FastAPI backend.
- **Plan → compose → verify → repair** orchestrator: each block is trialled in its test bench on a sandboxed ngspice worker, and the job streams to the browser over SSE from Redis Streams. Recorded LLM replies make the tests deterministic.
- **Cross-runtime parity gate** that checks native, WASM and Python on 1,000 random op logs, and every part and template is simulation-tested.

`Rust` `WebAssembly` `PyO3` `React` `FastAPI` `PostgreSQL` `Redis` `ngspice` `Docker`

---

### 🎯 [Chase](https://github.com/thakurabhishek7283/chase): AI resume tailoring and job matching

Keeps one master LaTeX resume and produces tailored versions for specific jobs, **one reviewed change at a time, without breaking the template**. It also ranks job openings against your career goals with semantic similarity.

- LLM calls go through **Pydantic AI**, so ATS scores, missing keywords and each proposed patch come back as validated, typed objects.
- **pgvector** cosine similarity ranks job postings, and a separate **LaTeX worker** container compiles the PDFs.
- Angular (signals) frontend, async FastAPI + SQLModel + Alembic, JWT auth with owner-scoped data, and 270 backend tests run in CI against real Postgres.

`Python` `FastAPI` `PostgreSQL` `pgvector` `Pydantic AI` `Angular` `Docker`

---

### 📚 [Under Formation](https://github.com/thakurabhishek7283/under-formation): portfolio and interactive visualizations

My personal site, built with **Astro + React islands**. It includes **30 interactive visualizations** of things I've learned, from transformers, self-attention, KV cache, LoRA and quantization to segment trees, HyperLogLog and Bloom filters. → [**Visit the site**](https://thakurabhishek7283.github.io/under-formation/)

## Tech stack

| | |
| --- | --- |
| **Languages** | ![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white) ![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white) |
| **Backend** | ![.NET 8](https://img.shields.io/badge/.NET%208-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![EF Core](https://img.shields.io/badge/EF%20Core-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![SignalR](https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white) ![MassTransit](https://img.shields.io/badge/MassTransit-1E3A8A?style=flat-square) ![Hangfire](https://img.shields.io/badge/Hangfire-2B6CB0?style=flat-square) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) |
| **Data & search** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![TimescaleDB](https://img.shields.io/badge/TimescaleDB-FDB515?style=flat-square&logo=timescale&logoColor=black) ![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) |
| **AI & vectors** | ![RAG](https://img.shields.io/badge/RAG-6D28D9?style=flat-square) ![MCP](https://img.shields.io/badge/Model%20Context%20Protocol-191919?style=flat-square&logo=anthropic&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square) ![Azure OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=flat-square) ![NVIDIA Triton](https://img.shields.io/badge/NVIDIA%20Triton-76B900?style=flat-square&logo=nvidia&logoColor=white) ![Pydantic AI](https://img.shields.io/badge/Pydantic%20AI-E92063?style=flat-square&logo=pydantic&logoColor=white) |
| **Frontend** | ![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white) ![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=flat-square&logo=reactivex&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Web Components](https://img.shields.io/badge/Web%20Components-29ABE2?style=flat-square&logo=webcomponentsdotorg&logoColor=white) ![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white) ![Umbraco](https://img.shields.io/badge/Umbraco-3544B1?style=flat-square&logo=umbraco&logoColor=white) |
| **Cloud & DevOps** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Azure DevOps](https://img.shields.io/badge/Azure%20DevOps-0078D7?style=flat-square) ![AWS](https://img.shields.io/badge/AWS%20S3%20%2F%20CloudFront-232F3E?style=flat-square) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) |
| **Practices** | Clean Architecture · Domain-Driven Design · query-plan analysis and indexing · unit, browser and end-to-end testing (MSTest, Vitest, Playwright, Karma/Jasmine) |

## GitHub & LeetCode

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=thakurabhishek7283&show_icons=true&hide_border=true&theme=github_dark&count_private=true">
    <img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=thakurabhishek7283&show_icons=true&hide_border=true&count_private=true">
  </picture>
  <a href="https://leetcode.com/u/abhishekthakur7283/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://leetcard.jacoblin.cool/abhishekthakur7283?theme=dark&font=Inter&border=0">
      <img height="165" alt="LeetCode stats" src="https://leetcard.jacoblin.cool/abhishekthakur7283?theme=light&font=Inter&border=0">
    </picture>
  </a>
</p>

---

<div align="center">

**Open to conversations about backend, search and applied-AI engineering.**<br>
The quickest way to reach me is [LinkedIn](https://www.linkedin.com/in/abhishek-thakur-072a981b6/) or [email](mailto:thakurabhishek7283@gmail.com).

</div>
