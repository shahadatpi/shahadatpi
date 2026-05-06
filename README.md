# Hey, I'm Shahadat 👋

**Self-taught full-stack engineer from Sylhet, Bangladesh.**  
I build things that solve real problems — not tutorial clones.

---

## What I've Built

### ⚛ [AtomicTest](https://atomictest.app) — Live in Production
> *An exam prep platform for Bangladesh HSC & university admission students — the only platform that renders real LaTeX and TikZ diagrams with native Bengali font support.*

I was a private tutor. Every existing platform rendered math as blurry images or dropped diagrams entirely. So I built the one I needed.

**What makes it non-trivial:**
- 🐳 **Custom Docker microservice** — TeX Live + XeLaTeX + ImageMagick running on Render, compiling raw LaTeX at request time. TeX Live is ~4 GB; serverless wasn't an option.
- ⚡ **3-tier caching** — DB → module-level Map → SHA-256 server cache. First compile is the only compile. Every subsequent render across all users hits a pre-compiled PNG.
- 🤖 **AI batch import** — Gemini Vision API extracts questions, options, correct answers, difficulty, and full LaTeX solutions directly from uploaded exam paper images.
- 🔍 **9-filter real-time search** — subject, topic, subtopic, difficulty, institution, type, text search, free/pro gate, pagination — all state serialised to URL via `history.replaceState()` (zero RSC round-trips, survives hard refresh, fully shareable links).
- 🔐 **Single-device session enforcement** — Better Auth revokes all previous sessions on new login. Exam integrity requirement.
- 🧪 **Vitest test suite** — unit tests for LaTeX tokeniser, MCQ block builder, TikZ stripper, question parser, plus an end-to-end paper pipeline integration test.

**Stack:** Next.js 16 (App Router) · React 19 · TypeScript · Tailwind CSS 4 · Supabase (PostgreSQL + Storage) · Better Auth · KaTeX · Docker · Gemini API · Vercel + Render

[→ Live site](https://atomictest.app) · [→ Source code](https://github.com/shahadatpi/atomic-test)

---

## Tech I Work With

```
Languages      TypeScript · JavaScript · SQL
Frontend       Next.js · React · Tailwind CSS · shadcn/ui · KaTeX
Backend        Next.js API Routes · Node.js · Express
Database       Supabase · PostgreSQL
Auth           Better Auth · OAuth (Google, Facebook)
DevOps         Docker · Vercel · Render
AI/ML          Google Gemini Vision API
Testing        Vitest · @vitest/coverage-v8
```

---

## How I Got Here

No CS degree. No bootcamp. I taught myself to code because I had a problem worth solving.

I spent two years as a private tutor watching students struggle because the tools were broken — math rendered as garbled text, diagrams missing entirely, no way to track what a student actually needed to practice. I decided to fix it.

AtomicTest is the result: 824+ LaTeX-rendered problems, a custom LaTeX compiler pipeline, AI-powered content import, and a progress tracking system — all built and shipped solo.

I'm now looking for a **remote full-stack engineering role** where I can build things that matter.

---

## Currently

- 🚀 Shipping features on AtomicTest
- 📚 Deepening system design knowledge
- 🌏 Open to **remote full-stack roles** (TypeScript / Next.js / React)
- 📬 Reach me: [here.is.shahadat@gmail.com](mailto:here.is.shahadat@gmail.com)

---

## GitHub Activity

> Consistency over intensity. I commit daily — features, fixes, refactors, tests.

---

*Built in Sylhet. Deployed worldwide.*
