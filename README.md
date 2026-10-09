# Hi, I'm Nastya 👋

**Full-stack developer, strongest on the frontend.** Five years of commercial React and TypeScript on a B2B SaaS platform, together with the Node.js services behind it. Ten years as a graphic designer before that.

I build products end to end: database schema, API, interface, deployment. The design background means I also care how the result feels. Loading states, transitions, feedback and accessibility are part of the product to me, not polish added at the end.

Open to full-stack and frontend roles across Europe, remote or hybrid.

---

## 🌐 Built solo, end to end

**[⚓ Kambuz](https://kambuz-lilac.vercel.app/)** ([source](https://github.com/BoikoAnastasiia/kambuz)) — «Что приготовить?»: pick a meal and a cuisine, get a recipe. The recipes come from a multi-agent Claude pipeline that turns YouTube cooking videos into structured recipes: a scout splits a vlog into its dishes, an extractor writes each one up in Russian with timestamps into the video, a verifier checks every ingredient and amount against the transcript, and a judge spots duplicates. It reads speech in any language, silent videos' chapters and the author's description. I benchmarked models per agent and moved the pipeline from Sonnet to Haiku 5.5, about 30× cheaper at 2–3 cents a video. Recipes live in MongoDB; new videos are queued from the site, admin-only behind Google sign-in, for a worker on my machine.
`Claude API` `TypeScript` `Next.js` `MongoDB` `Auth.js` `Zod`

**[🏋️ Podhod](https://podhod-workout.cc/)** ([source](https://github.com/BoikoAnastasiia/podhod)) — a bilingual (EN/RU) workout program builder and tracker. A Hono API on Cloudflare Workers with D1 and Drizzle ORM, a 1,324-exercise library, per-exercise progression computed by a pure engine, Google sign-in, and a CI pipeline that migrates the database before every deploy.
`React` `TypeScript` `Hono` `Cloudflare Workers` `D1` `Drizzle ORM`

**[🎸 Guess the Band](https://guesstheband.fun/)** ([source](https://github.com/BoikoAnastasiia/guess-the-band)) — a music quiz. Vercel Functions proxy the Deezer API server-side instead of exposing it to the browser, and every round and answer is recorded in Postgres to compute per-track difficulty. Anonymous play always works and syncs the moment you sign in.
`React` `Vite` `TypeScript` `Supabase` `Vercel Functions`

**[📚 Slovníček](https://slovnicek-alpha.vercel.app/)** ([source](https://github.com/BoikoAnastasiia/slovnicek)) — an offline-first PWA that teaches Slovak vocabulary to Russian speakers, with FSRS spaced repetition and a frequency-ordered bank of 2,000 words. IndexedDB is the source of truth, not a cache. The hard part is a hand-written bidirectional sync engine: last-write-wins with per-table watermarks, and pull ordered before push so a stale offline edit can never overwrite a newer server row.
`Next.js` `TypeScript` `Dexie` `Supabase` `PWA`

**[🇭🇷 Rječniček](https://rjecnicek.vercel.app/)** ([source](https://github.com/BoikoAnastasiia/rjecnicek)) — Slovníček's Croatian sibling, built for family: a B1–B2 word bank extended with an electrician's trade vocabulary, running on the same offline-first engine.
`Next.js` `TypeScript` `Dexie` `Supabase` `Vitest`

**🤖 [jobfeeder](https://github.com/BoikoAnastasiia/jobfeeder)** — a job aggregator over five sources behind a pluggable source interface. Runs on a GitHub Actions cron every four hours with persistent dedupe state and notifies through a Telegram bot. My first Python project.
`Python` `GitHub Actions` `Telegram Bot`

---

## 🏢 Commercial work: Gipper (2021–2026)

Five years on [Gipper](https://platform.gogipper.com/), a B2B SaaS platform for creating graphics, newsletters and websites, used by thousands of organizations.

**AI-powered generation pipeline.** A Claude agent interprets a text prompt, React renders templates offscreen and measures text slots via `getBoundingClientRect`, and Fabric.js assembles the design. It made graphic creation about 5x faster. Built on the platform's Mastra / Node.js / PostgreSQL AI engine; I also wrote the agents' evaluations and tests, and a color-matching algorithm that applies workspace branding to generated objects.

**Server-side rendering from scratch.** A Node.js server that renders React to HTML and assembles full documents for customer-published sites, with data preloading, CSS and font injection, Sentry monitoring and cross-browser fixes.

**Real-time and media services.** A Socket.io service tracking live device state, with token auth, automatic reconnection and a freeze watchdog for stalled connections. AWS S3 presigned uploads and Lambda integrated into a production media pipeline.

**14-module microfrontend platform.** Vite and Module Federation: 2 host apps, 9 feature modules, 3 shared libraries, 34 routes, each deployed independently through Bitbucket Pipelines. Later migrated to a pnpm + Turborepo monorepo, with custom branch-sync tooling.

**Shared UI kit.** 150+ Storybook-documented components, accessible to WCAG 2.1 (ARIA, full keyboard navigation, screen-reader support), used by every feature module.

**Testing and tooling.** Playwright end-to-end tests on critical user flows, and the team's AI development harness on Claude Code, taking Jira tickets to tested, review-ready PRs.

---

## 🛠️ Tech stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Hono](https://img.shields.io/badge/Hono-E36002?style=flat&logo=hono&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white)
![Drizzle](https://img.shields.io/badge/Drizzle_ORM-C5F74F?style=flat&logo=drizzle&logoColor=black)

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![MobX](https://img.shields.io/badge/MobX-FF9955?style=flat&logo=mobx&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat&logo=redux&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?style=flat&logo=sass&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat&logo=cloudflareworkers&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat&logo=vitest&logoColor=white)
![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=flat&logo=storybook&logoColor=white)

- **Languages:** TypeScript, JavaScript (ES6+), Python, SQL, HTML5, CSS3
- **Backend & data:** Node.js, REST APIs, SSR, Hono, serverless functions, WebSockets (Socket.io), OAuth 2.0, PostgreSQL (schema design, indexing, row-level security), MongoDB, Drizzle ORM
- **Cloud & DevOps:** AWS (S3, Lambda), Google Cloud, Vercel, Cloudflare Workers, Supabase, CI/CD (Bitbucket Pipelines, GitHub Actions)
- **Frontend:** React, Next.js (App Router), MobX, Redux Toolkit, TanStack Query, Tailwind CSS, SCSS, Fabric.js
- **Architecture & testing:** Microfrontends (Module Federation), monorepos (pnpm workspaces, Turborepo), design systems, Playwright (E2E), Vitest, Storybook
- **AI:** Claude API & Agent SDK, Mastra, agent evaluations, Claude Code, prompt engineering

---

## 🎓 Certifications

- **Anthropic Academy — Building with the Claude API** (2026)

---

## 📫 Get in touch

[![Portfolio](https://img.shields.io/badge/a--boiko.dev-111111?style=flat&logo=googlechrome&logoColor=white)](https://a-boiko.dev)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:boiko.nastasiia@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anastasiia-boiko-026238198/)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=flat&logo=telegram&logoColor=white)](https://t.me/Anastasyah)
