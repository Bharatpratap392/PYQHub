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

## Add sample papers
Put PDFs/images into public/papers/
Edit data/metadata.json:
[
  {
    "id": "cse-prob-8-end-2023",
    "department": "CSE",
    "subject": "Probability",
    "semester": 8,
    "examType": "END",
    "year": 2023,
    "file": "/papers/cse_prob_end_2023.pdf",
    "pages": 8
  }
]

Roadmap
v1 (MVP):
Filters + viewer + login + AI
JSON metadata + public PDFs
Report issue
v1.1:
Admin upload with OCR
Formula sheet + common mistakes summary
Queue + retries + caching
v2:
Provider failover
Similar questions & alternate methods
PostgreSQL + S3/R2
v3:

Self-hosted open model

Discussions per question

Export custom practice sets

Known Limitations
Blurry scans reduce OCR & AI accuracy

Free AI tiers have rate limits

JSON + public files not scalable

Step correctness varies by topic/model

Contributing
Fork repo, create branch, open PR

Report bugs via Issues

For new papers, follow metadata & folder structure


