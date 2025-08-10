# 📚 PYQ-Hub — Previous-Year Papers + AI Solver

A web app to **organize previous-year college exam papers** and instantly generate **AI-powered step-by-step solutions**.  
Designed for **fast search**, clean viewing, and smarter revision before Mid/End Sem exams.

## ✨ Key Features
- Browse by **Department**, **Subject**, **Semester**, **Exam Type**
- In-browser **PDF/Image viewer** (zoom, paginate)
- AI Solver:
  - *Mid Sem*: concise steps
  - *End Sem*: full derivations/proofs
- Login-gated AI usage (magic link or social login)
- Caching of solutions to save cost & time
- Mobile-friendly layout + issue reporting

## 🎯 Why It Helps
- All PYQs in one place (no messy WhatsApp forwards)
- Instant, structured solutions with depth control
- Clear, readable PDFs/images
- Planned: Similar questions & formula summaries

## 🛠 Tech Stack
- **Frontend:** Next.js (React), TypeScript, Tailwind CSS, react-pdf
- **Backend:** Next.js API Routes, Auth (NextAuth/Clerk/Supabase)
- **AI:** Provider API (pluggable), optional Redis cache
- **Storage:** Public folder (MVP), S3/R2 later
- **Hosting:** Vercel

## 🚀 Quick Start
```bash
git clone YOUR_REPO_URL
cd YOUR_REPO_NAME
npm install
cp .env.example .env.local  # add keys
npm run dev
