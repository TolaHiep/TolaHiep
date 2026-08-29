# Nguyen Manh Hiep

**Software Engineer · Full-stack** — Hanoi, Vietnam (remote-ready)

I build products end to end: UI, backend, database, deployment and testing. Recent work
centres on real-time systems, production LLM integration and document automation — three
systems carried from requirements through architecture, tests and live deployment in the
past year.

Right now I'm going deeper into real-time architecture and production LLM integration:
model routing, evaluation, and latency/cost budgets.

🌐 **[nguyenmanhhiep.info](https://nguyenmanhhiep.info)** · 💼 [LinkedIn](https://linkedin.com/in/hiepnm2003) · ✉️ [Hiep.work@outlook.com](mailto:Hiep.work@outlook.com)

---

## Selected work

**[SenAI](https://app.senai.online) — real-time Vietnamese↔English meeting interpreter** · 2026
> 🏆 **3rd Prize + Vietnam AI Stars Award**, Vietnam AI Innovation Challenge 2026 (AI Singapore)

Live bilingual meetings with per-speaker ASR, translation, voice cloning and automatic
minutes. Main developer on the project team — the whole Next.js 16 frontend, most of the
FastAPI backend, the LiveKit meeting room, the translation pipeline, CI/CD and deployment.

- Blank repo → public production in **3 weeks**, on a spec-driven loop (16 design specs + 16 plans in-repo)
- **~75 ms ASR + ~295 ms MT, under 400 ms end-to-end**; zero errors up to concurrency 8
- Pluggable model router — self-hosted (Qwen3, F5-TTS on vLLM) or commercial APIs, switched at runtime with auto-fallback
- PostgreSQL 16 + pgvector for glossary/document RAG; **37 UAT suites / 147 real non-mocked tests**

**Notarex — notary document OCR & digitization** · 2026 · *private*

AI OCR from scanned notarial records, online editing through JWT-secured OnlyOffice, and
automatic DOCX generation. Full-stack, AI orchestration and infrastructure.

- Celery + Redis job queue with zombie-job detection and recovery under load
- 3-role permission model scoped per notary office for tenant isolation
- Delivered over 3.5 months, covered by **43 test modules / 418 automated test cases**

**[ASC Farm](https://github.com/TolaHiep/asc-farm) — agricultural production management** · 2026

Web admin plus an offline-first mobile PWA, built to stay reliable in low-connectivity fields.

- Headless Frappe v15 backend with an event-driven task engine — **132 passing tests**
- Anti-fraud completion photos (in-app camera + GPS + watermark) and an idempotent offline queue
- Satellite heatmap (Leaflet + Esri), work calendar, notifications and step-by-step SOPs

## How I work with AI

Agents write a lot of my code; the discipline is in what surrounds them.

- **Spec-driven loop** — brainstorm → versioned design spec → implementation plan → agent implementation → real test run. One canonical spec per system, never parallel versions.
- **Context engineering** — repo-level agent context (`CLAUDE.md` / `AGENTS.md`) pinning architecture, conventions and branch policy, so agents produce merge-ready code without re-briefing.
- **Guardrails** — every AI-written feature lands behind real no-mock UAT (live API / WebSocket / LiveKit calls), call-graph impact analysis before editing a symbol, and CI on every push.

**697 automated / UAT test cases** authored across the three products above.

## Stack

| | |
|---|---|
| **Frontend** | React 19, Next.js 16/14, TypeScript, Tailwind v4, Ant Design, Zustand, TanStack Query, PWA / offline-first, i18n |
| **Backend** | FastAPI, Node.js, NestJS, Express, Spring Boot, Python, Java, REST, WebSocket, WebRTC (LiveKit), Celery, Redis, JWT / OAuth, RBAC |
| **Data** | PostgreSQL 16 + pgvector, MySQL, MariaDB, SQLAlchemy 2.0 async, vector search & embeddings, MinIO (S3) |
| **DevOps** | Docker & Compose, Nginx, systemd, TLS, VPS deployment, GitHub Actions, Cloudflare, Amazon SES |
| **AI** | Claude Code (agents, skills, hooks), Cursor, Copilot, MCP servers, RAG, LLM orchestration, vLLM self-hosting |

## Education

**BSc Computer Science**, Hanoi University of Science and Technology (HUST) — 2021–2026
