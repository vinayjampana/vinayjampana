# Vinay Jampana — Senior Frontend Engineer

Building frontend systems that scale — React · TypeScript · Nx Monorepo · Next.js · CI/CD

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

## What I'm Good At

- **Nx Monorepo Architecture** — migrated 3 React apps (80K+ LOC), cut build time 35%, reduced dependency duplication 25%
- **Design Systems** — built 40+ component library adopted by 5 microapps and 15+ engineers, cut feature UI time 5 days to 3
- **Bundle Performance** — 9MB to 5MB (35%), FCP 2.8s to 1.8s, CI budget gates to prevent regression
- **CI/CD Pipelines** — GitHub Actions: lint → typecheck → Jest 80% coverage → bundle regression → preview deploy → production

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

**Frontend:** React 18/19 · TypeScript · Next.js · Redux Toolkit · Context API  
**Architecture:** Nx Monorepo · Modular Frontend · Vite · Webpack  
**Performance:** Code splitting · Bundle analysis · Lighthouse · Performance budgets  
**Testing:** Jest · React Testing Library  
**DevOps:** GitHub Actions · CI/CD · Vercel · Preview deployments

---

**Open to Senior Frontend / SDE2-SDE3 roles — Hyderabad, Bangalore, or Remote**

vinayvarma541@gmail.com · [linkedin.com/in/vinay-jampana](https://linkedin.com/in/vinay-jampana) · [vinayjampana.dev](https://vinayjampana.dev)
