# Quick‑Stack Experimental Build

This folder holds the minimal **FastAPI + Next.js + Docker + Coolify** stack that was selected in this session for rapid prototyping:

- Backend API: `FastAPI` with `SQLModel` (PostgreSQL) and JWT auth.<br>
- Front‑end: `Next.js 14` (React 18 + TypeScript) with Tailwind CSS.
- Scheduler: (optional) `Celery` with `dateutil`.
- Payments: Stripe‑Python SDK, no subscription, only per‑transaction fees.
- Containerization: Single multi‑stage Dockerfile per service.
- Deployment: Configurable via `coolify.yml` for each component.

The structure is a **monorepo** using `pnpm` workspaces: `packages/api`, `packages/ui`, `packages/common`.

This build is *experimental* – we are testing quick iteration, test coverage, and deployment on Coolify.

## Decision Log
> See *quick‑stack‑decisions.md* in the memory folder for a record of the rules your supervisor requested.
