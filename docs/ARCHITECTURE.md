# ResearchForge Agents Architecture

## Purpose

Research swarm that extracts claims, challenges evidence, scores conviction, and produces analyst-ready briefs.

## Runtime loop

1. **Observe** — collect domain signals: source_quality, claim_overlap, contradiction_count, market_attention, evidence_age_days.
2. **Orient** — map the active scenario to specialist agent responsibilities.
3. **Decide** — score severity, confidence, and operator urgency.
4. **Act** — emit next actions that a human operator can verify.
5. **Reflect** — attach trace IDs and deterministic evidence for review.

## Components

- `backend/swarm.py` — pure Python reasoning core, safe for CI and static demos.
- `backend/app.py` — FastAPI wrapper for product integration.
- `cli.py` — terminal demo path for reviewers.
- `index.html` — front-facing dashboard surface.

## Agent responsibilities

- `Claim Extractor`: owns one part of the analysis loop.
- `Contradiction Hunter`: owns one part of the analysis loop.
- `Citation Graph Builder`: owns one part of the analysis loop.
- `Narrative Risk Analyst`: owns one part of the analysis loop.
- `Briefing Compiler`: owns one part of the analysis loop.

## Production extension points

- Replace deterministic signals with live connectors.
- Persist reports in Postgres or SQLite.
- Add auth and organization workspaces.
- Add export hooks for Slack, Discord, Telegram, or email.
