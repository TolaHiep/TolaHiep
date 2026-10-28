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

I am a Software Engineer specialising in full-stack web applications and AI integration. I take a
product from the first idea to day-to-day operation: requirements, architecture, backend and
frontend, deployment and monitoring. The systems I have built include an online meeting room with
real-time interpretation, admin dashboards, an OCR pipeline that fills in paperwork automatically,
and LLM features built into business workflows.

When I build a system, I focus on what keeps it stable once real users arrive: clear APIs,
consistent data, a fallback when a component fails, and automated tests reliable enough that each
update does not break existing features.

Right now I am going deeper into real-time architecture and production LLM integration: model
routing, evaluation, and latency/cost budgets.

<p align="center">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/senai/third-prize.jpg" width="88%" alt="3rd Prize, Vietnam AI Innovation Challenge 2026">
</p>
<p align="center">
  <i>3rd Prize and Vietnam AI Stars Award, Vietnam AI Innovation Challenge 2026 (AI Singapore)</i>
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

### SmartSales: sales platform for small Vietnamese shops · 2026 · *personal project, private repo*

Zalo chat, orders, calls and livestream selling in one place, with AI that suggests replies and
reviews calls. Built on my own, from the architecture to the UI and the AI.

- 7 Node.js modules on one PostgreSQL database: each module writes only to its own schema and joins across the others, so one customer profile pulls in orders, chats and calls
- Shared sign-in and UI frame, so a call in progress stays connected when staff switch modules
- One AI gateway with a model per task set in `.env` and provider fallback; RAG over documents and products with vector + keyword search
- Two-channel call recording, transcribed per speaker and scored on 7 criteria for staff attitude
- **76 test files** plus an end-to-end smoke test; two security reviews found **61 issues, all fixed**

### SenAI: real-time Vietnamese↔English meeting interpreter · 2026

<a href="https://app.senai.online">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/senai/senai-landing.png" width="100%" alt="SenAI landing page">
</a>

Live bilingual meetings with per-speaker ASR, translation, voice cloning and automatic minutes.
I was the main developer on the project team and built the whole Next.js 16 frontend, most of the
FastAPI backend, the LiveKit meeting room, the translation pipeline, CI/CD and deployment.

- Blank repo to public production in **3 weeks**, on a spec-driven loop (16 design specs + 16 plans kept in the repo)
- **~75 ms ASR + ~295 ms MT, under 400 ms end-to-end**; zero errors up to concurrency 8
- Pluggable model router: self-hosted (Qwen3, F5-TTS on vLLM) or commercial APIs, switched at runtime with auto-fallback
- PostgreSQL 16 + pgvector for glossary and document RAG; **37 UAT suites / 147 real non-mocked tests**

Live at **[app.senai.online](https://app.senai.online)**

### Notarex: notary document OCR & digitization · 2026 · *private repo*

<img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/Notarex/e25-admin-dashboard.png" width="100%" alt="Notarex admin dashboard">

AI OCR from scanned notarial records, online editing through JWT-secured OnlyOffice, and automatic
DOCX generation. I handled the full stack, the AI orchestration and the infrastructure.

- Celery + Redis job queue with zombie-job detection and recovery under load
- 3-role permission model scoped per notary office for tenant isolation
- Delivered over 3.5 months, covered by **43 test modules / 418 automated test cases**

### ASC Farm: agricultural production management · 2026

<a href="https://github.com/TolaHiep/asc-farm">
  <img src="https://raw.githubusercontent.com/TolaHiep/portfolio/main/assets/screenshots/akf-farm/akf-farm-heatmap.png" width="100%" alt="ASC Farm satellite heatmap">
</a>

Web admin plus an offline-first mobile PWA, built to stay reliable in low-connectivity fields.

- Headless Frappe v15 backend with an event-driven task engine, covered by **132 passing tests**
- Anti-fraud completion photos (in-app camera + GPS + watermark) and an idempotent offline queue
- Satellite heatmap (Leaflet + Esri), work calendar, notifications and step-by-step SOPs

Code at **[github.com/TolaHiep/asc-farm](https://github.com/TolaHiep/asc-farm)**

---

## How I work with AI

AI agents write a lot of my code, so most of my effort goes into the process around them.

- Each feature goes through a brainstorm, a versioned design spec, an implementation plan, agent implementation and a real test run. Each system has one canonical spec, with no parallel versions.
- Repo-level agent context (`CLAUDE.md` / `AGENTS.md`) pins the architecture, conventions and branch policy, so agents produce merge-ready code without being briefed again.
- Every AI-written feature has to pass real UAT without mocks (live API, WebSocket and LiveKit calls). I run call-graph impact analysis before editing a symbol, and CI runs on every push.

**697 automated / UAT test cases** authored across SenAI, Notarex and ASC Farm.

---

<p align="center">
  <b>BSc Computer Science</b>, Hanoi University of Science and Technology (HUST), 2021-2026<br>
  <a href="https://nguyenmanhhiep.info">nguyenmanhhiep.info</a> · <a href="mailto:Hiep.work@outlook.com">Hiep.work@outlook.com</a>
</p>
