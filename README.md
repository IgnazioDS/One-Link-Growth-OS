# One-Link Growth OS

A multi-tenant SaaS that helps creators operate a simple growth system:
- Define your Rule of One (one primary product, one primary channel, one destination link)
- Turn one weekly pillar into a 7-day content pack (posts, hooks, scripts, emails)
- Route every asset through a One-Link Hub and funnel pages
- Track click-to-lead and click-to-purchase attribution

## Tech Stack

- Web: Next.js
- API: FastAPI
- Worker: Celery
- DB: Postgres + pgvector
- Queue/Cache: Redis
- Containers: Docker Compose

## Repo Structure

- `apps/api` — FastAPI service + domain + migrations
- `apps/web` — Next.js dashboard + public pages (hub/funnel)
- `services/worker` — Celery worker + AI pipelines
- `docker-compose.yml` — dev/prod profiles

## Prerequisites

- Docker Desktop (recommended)

## Local Development

1) Create env file:
```bash
cp .env.example .env
