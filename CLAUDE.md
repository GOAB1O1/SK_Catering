# SK Catering Platform

**Company:** SK Catering — Multi-tenant nutrition compliance & institutional commerce system
**Location:** New Orleans, LA
**Owner:** GOAB (Brandin)

## Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Language:** TypeScript (strict mode)
- **Styling:** Tailwind CSS
- **Components:** shadcn/ui
- **Backend/DB:** Supabase (Postgres, Auth, Edge Functions, Realtime)
- **Hosting:** Vercel

## Business Context

Multi-sided marketplace connecting schools, hospitals, corporations, caterers, parents, and employees around institutional food service and nutrition compliance.

**Revenue model:**
- Transaction fees (5–12% take rate)
- Prepaid meal wallets (breakage revenue)
- Compliance SaaS subscriptions

**Phase 1:** Louisiana school district pilots — 5–10 districts, ~25,000 students

**Regulatory:** Must comply with USDA school nutrition standards and Louisiana state regulations.

**Primary offer:** Pilot program with local school districts

**Comparable models:** Toast, ClassDojo, MealPal

## Coding Rules

- TypeScript strict mode — no `any` types without justification
- Use shadcn/ui components; do not introduce competing UI libraries
- Mobile-first responsive design
- Never hardcode API keys or secrets — use environment variables
- Feature branches only — no direct commits to `main` during development
- Descriptive commit messages
- Compliance data must be handled carefully — audit trails required for all nutrition/regulatory data mutations
- Prefer server components; use `"use client"` only when necessary
- Use Supabase Row Level Security (RLS) for multi-tenant data isolation
