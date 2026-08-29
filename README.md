<h1 align="center">Nguyen Manh Hiep</h1>

<p align="center">
  <b>Software Engineer · Full-stack</b><br>
  Hanoi, Vietnam · remote-ready
</p>

<p align="center">
  <a href="https://nguyenmanhhiep.info"><img src="https://img.shields.io/badge/Portfolio-nguyenmanhhiep.info-0D6E8B?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://linkedin.com/in/hiepnm2003"><img src="https://img.shields.io/badge/LinkedIn-hiepnm2003-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:Hiep.work@outlook.com"><img src="https://img.shields.io/badge/Email-Hiep.work%40outlook.com-0078D4?style=flat-square&logo=microsoftoutlook&logoColor=white" alt="Email"></a>
  <a href="https://app.senai.online"><img src="https://img.shields.io/badge/Live%20product-app.senai.online-E23E70?style=flat-square&logo=icloud&logoColor=white" alt="SenAI"></a>
</p>

---

I build products end to end: UI, backend, database, deployment and testing. Recent work centres
on real-time systems, production LLM integration and document automation — three systems carried
from requirements through architecture, tests and live deployment in the past year.

Right now I am going deeper into real-time architecture and production LLM integration: model
routing, evaluation, and latency/cost budgets.

<p align="center">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/senai/third-prize.jpg" width="88%" alt="3rd Prize, Vietnam AI Innovation Challenge 2026">
</p>
<p align="center">
  <i>3rd Prize + Vietnam AI Stars Award — Vietnam AI Innovation Challenge 2026 (AI Singapore)</i>
</p>

## Stack

**Frontend**

![React](https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![PWA](https://img.shields.io/badge/PWA_offline--first-5A0FC8?style=flat-square&logo=pwa&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![LiveKit](https://img.shields.io/badge/WebRTC_·_LiveKit-1E88E5?style=flat-square&logo=webrtc&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

**Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL_·_MariaDB-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO_S3-C72E49?style=flat-square&logo=minio&logoColor=white)

**DevOps & AI**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Amazon SES](https://img.shields.io/badge/Amazon_SES-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM_self--hosting-1A73E8?style=flat-square&logo=huggingface&logoColor=white)

---

## Selected work

### SenAI — real-time Vietnamese↔English meeting interpreter · 2026

<a href="https://app.senai.online">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/senai/senai-landing.png" width="100%" alt="SenAI landing page">
</a>

Live bilingual meetings with per-speaker ASR, translation, voice cloning and automatic minutes.
Main developer on the project team — the whole Next.js 16 frontend, most of the FastAPI backend,
the LiveKit meeting room, the translation pipeline, CI/CD and deployment.

- Blank repo to public production in **3 weeks**, on a spec-driven loop (16 design specs + 16 plans kept in the repo)
- **~75 ms ASR + ~295 ms MT, under 400 ms end-to-end**; zero errors up to concurrency 8
- Pluggable model router — self-hosted (Qwen3, F5-TTS on vLLM) or commercial APIs, switched at runtime with auto-fallback
- PostgreSQL 16 + pgvector for glossary and document RAG; **37 UAT suites / 147 real non-mocked tests**

Live at **[app.senai.online](https://app.senai.online)**

### Notarex — notary document OCR & digitization · 2026 · *private repo*

<img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/Notarex/e25-admin-dashboard.png" width="100%" alt="Notarex admin dashboard">

AI OCR from scanned notarial records, online editing through JWT-secured OnlyOffice, and automatic
DOCX generation. Full-stack, AI orchestration and infrastructure.

- Celery + Redis job queue with zombie-job detection and recovery under load
- 3-role permission model scoped per notary office for tenant isolation
- Delivered over 3.5 months, covered by **43 test modules / 418 automated test cases**

### ASC Farm — agricultural production management · 2026

<a href="https://github.com/TolaHiep/asc-farm">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/akf-farm/akf-farm-heatmap.png" width="100%" alt="ASC Farm satellite heatmap">
</a>

Web admin plus an offline-first mobile PWA, built to stay reliable in low-connectivity fields.

- Headless Frappe v15 backend with an event-driven task engine — **132 passing tests**
- Anti-fraud completion photos (in-app camera + GPS + watermark) and an idempotent offline queue
- Satellite heatmap (Leaflet + Esri), work calendar, notifications and step-by-step SOPs

Code at **[github.com/TolaHiep/asc-farm](https://github.com/TolaHiep/asc-farm)**

---

## How I work with AI

Agents write a lot of my code; the discipline is in what surrounds them.

- **Spec-driven loop** — brainstorm, then a versioned design spec, an implementation plan, agent implementation, and a real test run. One canonical spec per system, never parallel versions.
- **Context engineering** — repo-level agent context (`CLAUDE.md` / `AGENTS.md`) pinning architecture, conventions and branch policy, so agents produce merge-ready code without re-briefing.
- **Guardrails** — every AI-written feature lands behind real no-mock UAT (live API / WebSocket / LiveKit calls), call-graph impact analysis before editing a symbol, and CI on every push.

**697 automated / UAT test cases** authored across the three products above.

---

<p align="center">
  <b>BSc Computer Science</b> — Hanoi University of Science and Technology (HUST), 2021–2026<br>
  <a href="https://nguyenmanhhiep.info">nguyenmanhhiep.info</a> · <a href="mailto:Hiep.work@outlook.com">Hiep.work@outlook.com</a>
</p>
