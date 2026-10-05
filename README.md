<div align="center">

# Vinay Jampana, Senior Software Engineer (AI and Full-Stack)

I build production LLM agents and the products around them: React and Next.js interfaces, NestJS and Python services, and the evals and tracing that keep agents honest.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vinay-jampana)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vinayvarma541@gmail.com)
[![Website](https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vinayjampana.dev)
[![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/package/vite-plugin-bundle-size-tracker)

</div>

---

## What I work on

At [Zotok.ai](https://zotok.ai) (Hyderabad, since May 2023) I lead a team of five on a B2B WhatsApp-commerce platform, and I own the architecture and delivery of its order-agent and the systems around it. Write-ups of the work are on [vinayjampana.dev](https://vinayjampana.dev); customer names and internal details are removed.

- **Order-agent platform.** One opaque LangGraph agent became seven typed steps composed on a visual canvas, so behaviour changes per customer need no redeploy. [Case study](https://vinayjampana.dev/work/order-agent-platform)
- **Alias ranker.** A rarity-weighted matcher over about 15,000 production aliases: leave-one-out hit@1 69% to 78%, and 81% to 95% on real rep phrasings. [Case study](https://vinayjampana.dev/work/alias-ranker)
- **Evals in CI.** 6 eval sets and 64 scenarios graded against ground-truth SKUs, run twice a day with a breach rule that alerts the team. [Case study](https://vinayjampana.dev/work/order-agent-evals)
- **Tracing.** OpenTelemetry and Langfuse across a runtime where every block is its own HTTP call. [Case study](https://vinayjampana.dev/work/tracing-a-block-runtime)
- **UltraTech on WhatsApp.** Led a team of three that moved a plant's offline pour and dispatch forms to a WhatsApp flow in 2.5 weeks. [Case study](https://vinayjampana.dev/work/rmc-dispatch-whatsapp)
- **Frontend load time.** First load from 15 to 30 seconds to about 1.5 seconds on a 19-app Nx monorepo. [Case study](https://vinayjampana.dev/work/frontend-load-time)

---

## Side projects

### vite-plugin-bundle-size-tracker — Published npm Package
> Tracks and compares Vite bundle sizes across builds — warns before regressions ship

Born from real pain: I was tuning the bundle of a large monorepo at Zotok.ai and needed a way to make sure it never crept back. Built this so any Vite project can enforce bundle budgets without writing custom CI scripts.

**What it does:**
- Tracks bundle size history across N builds
- Compares current build against rolling average
- Configurable threshold alerts (default: warn at +10%)
- JSON report output for CI/CD pipelines
- Zero config — works out of the box

**Stack:** TypeScript · Vite Plugin API · Node.js

[npm Package](https://www.npmjs.com/package/vite-plugin-bundle-size-tracker) | [Repo](https://github.com/vinayjampana/vite-plugin-bundle-size-tracker)

---

### Tiny Tracker — Live Habit & Routine Tracker
> [tinytracker.in](https://tinytracker.in) — minimalist daily accountability app

Built the app I wanted but couldn't find: a clean Today view, habit streaks, visual progress heatmap, and no bloat. PWA — installs on any device, works offline.

**Architecture:**
- Next.js 16 App Router + React 19
- Firebase Auth (Email + Google) + Firestore
- Firebase Security Rules for per-user data isolation
- PWA support — installable, offline-capable
- IST timezone — built for Indian users
- Deployed on Vercel with custom domain

**Stack:** Next.js · TypeScript · Firebase · Tailwind CSS · Shadcn/ui · Vercel

[Live App](https://tinytracker.in) | [Repo](https://github.com/vinayjampana/habit-and-routine-tracker)

---

### RoleMiner — Personal Job Discovery Pipeline
> India-first job scraper that scores roles against your profile using a single LLM call

Tired of manually checking 9 job boards. Built an automated pipeline that scrapes Greenhouse, Lever, Ashby, Cutshort, and Workday tenants, filters by freshness/location/salary/role type, pre-ranks with TF-IDF, then sends the top 50 to an LLM (any OpenAI-compatible API) for structured scoring. Full React dashboard with live pipeline logs via SSE — so you can watch every scraper fire in real time and see exactly why each job was filtered or ranked where it was.

**Architecture:**
- Python 3.11 + FastAPI + SQLite (companies, runs, run_events)
- Async HTTPX scrapers for 5 ATS types + per-run structured event logging
- Pipeline: rule filter → role keyword filter → TF-IDF cosine rank → LLM batch score
- SSE `/stream/{run_id}` — live events while running, DB replay for finished runs
- React 18 + Vite + TypeScript + React Query + Recharts dashboard
- Docker Compose for local + VPS deploy
- Cost: < $0.002 per run (< ₹0.17)

**Stack:** Python · FastAPI · SQLite · scikit-learn · React · TypeScript · Tailwind · Docker

[Repo](https://github.com/vinayjampana/role-miner)

---

## Stack

**AI:** LLM agents and tool calling, LangGraph, structured outputs, prompt engineering, LLM evaluation, Langfuse, OpenTelemetry, OCR and vision, OpenSearch kNN retrieval  
**Backend:** TypeScript, Node.js, NestJS, Python (FastAPI), PostgreSQL, Prisma, Hasura  
**Frontend:** React 18/19, Next.js, TypeScript, Redux Toolkit, Module Federation, Vite, Nx  
**Cloud:** AWS (ECS, Lambda, S3, Amplify), Docker, GitHub Actions

---

**Open to senior AI full-stack and applied AI roles. Hyderabad, Bengaluru or remote.**

vinayvarma541@gmail.com · [linkedin.com/in/vinay-jampana](https://linkedin.com/in/vinay-jampana) · [vinayjampana.dev](https://vinayjampana.dev)
