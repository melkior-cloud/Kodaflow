# Kodaflow — TikTok-like App (Next.js)

A minimal, production-ready starter for a TikTok-style vertical video app.
Built with **Next.js App Router** and **TailwindCSS**. Ready to deploy on **Vercel**.

## Features
- Vertical feed with snap scrolling
- Auto play/pause using IntersectionObserver
- Like button (localStorage) and share to Facebook
- Upload page (POST to /api/videos) — demo uses in-memory store
- Mock data seed via `/api/videos`

## Quick Start

```bash
# 1) Install deps
npm install

# 2) Run dev
npm run dev

# 3) Open
http://localhost:3000
```

## Deploy to Vercel
1. Push to GitHub (repo name suggestion: `kodaflow`).
2. On Vercel, import the repo. No special settings required.
3. Build & deploy — you get a domain like `kodaflow.vercel.app`.

## Configure Domain (later)
Use a free domain provider (e.g., Freenom) and point your DNS (A/ALIAS or CNAME) to Vercel.
Then add the domain in Vercel Project Settings.

## Notes
- `/api/videos` uses an in-memory array (for demo only). In real use, connect to storage (Supabase/S3) & DB.
- Video URLs must be direct **.mp4** or compatible streams.
- Tailwind is pre-configured (see `app/globals.css` and `tailwind.config.ts`).

## License
MIT
