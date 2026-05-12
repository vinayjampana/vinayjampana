<div align="center">

# Vinay Jampana — Senior Software Engineer

Building frontend systems that scale — React · TypeScript · Nx Monorepo · Next.js · CI/CD

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vinay-jampana)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:vinayvarma541@gmail.com)
[![Website](https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vinayjampana.dev)
[![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/package/vite-plugin-bundle-size-tracker)

</div>

<div align="center">

<img height="160" src="https://github-readme-streak-stats.herokuapp.com/?user=vinayjampana&theme=tokyonight&hide_border=true" />

</div>

<div align="center">

<img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=vinayjampana&theme=react-dark&hide_border=true&area=true" />

</div>

---

## Featured Work

### vite-plugin-bundle-size-tracker — Published npm Package
> Tracks and compares Vite bundle sizes across builds — warns before regressions ship

Born from real pain: I reduced a 9MB JS bundle to 5MB at Zotok.ai and needed a way to make sure it never crept back. Built this so any Vite project can enforce bundle budgets without writing custom CI scripts.

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

## What I'm Good At

- **Nx Monorepo Architecture** — migrated 3 React apps (80K+ LOC), cut build time 35%, reduced dependency duplication 25%
- **Design Systems** — built 40+ component library adopted by 5 microapps and 15+ engineers, cut feature UI time 5 days to 3
- **Bundle Performance** — 9MB to 5MB (35%), FCP 2.8s to 1.8s, CI budget gates to prevent regression
- **CI/CD Pipelines** — GitHub Actions: lint → typecheck → Jest 80% coverage → bundle regression → preview deploy → production
- **Full-Stack Tools** — FastAPI + SQLite backends, async Python scrapers, SSE streams, Docker Compose deploys

---

## Experience

**Senior Software Engineer @ Zotok.ai** *(May 2023 – Present)*
- Led Nx monorepo migration for 3 React applications, 80K+ LOC
- Built versioned design system: 40+ components, 5 microapps, 15+ engineers
- Reduced JS bundle 9MB → 5MB, FCP 2.8s → 1.8s
- Built full GitHub Actions CI/CD pipeline from scratch
- Reduced post-release regressions 20% via PR guidelines + architecture reviews

**Senior Developer @ Sumeru Software** *(Aug 2022 – Jan 2023)*

**SDE1 @ Aerchain** *(Apr 2021 – Jan 2022)*

---

## Stack

<div align="center">

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)

</div>

**Frontend:** React 18/19 · TypeScript · Next.js · Redux Toolkit · Context API  
**Architecture:** Nx Monorepo · Modular Frontend · Vite · Webpack  
**Performance:** Code splitting · Bundle analysis · Lighthouse · Performance budgets  
**Testing:** Jest · React Testing Library  
**Backend:** Python · FastAPI · SQLite · scikit-learn · HTTPX  
**DevOps:** GitHub Actions · CI/CD · Docker Compose · Vercel · Preview deployments

---

**Open to Senior Frontend / SDE2-SDE3 roles — Hyderabad, Bangalore, or Remote**

vinayvarma541@gmail.com · [linkedin.com/in/vinay-jampana](https://linkedin.com/in/vinay-jampana) · [vinayjampana.dev](https://vinayjampana.dev)
