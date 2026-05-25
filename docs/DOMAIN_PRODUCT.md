# Agent ResearchForge — Domain Product Layer

Research synthesis lab that turns links, papers, and notes into scored briefs with citations and action plans.

## Live Reviewer Endpoints

- `GET /domain/signals` — inspect supported domain signals and actions
- `POST /domain/analyze` — submit scenario + signals, receive risk score, findings, runbook, trace id
- `GET /domain/demo` — four deterministic demo reports
- `POST /agent-run` — MiMo multi-specialist pipeline proof

## Signals

- `source_count`
- `citation_density`
- `novelty_score`
- `conflict_count`
- `confidence`
- `staleness_days`

## Operator Actions

- cluster sources by claim
- flag contradictory evidence
- draft executive brief
- extract benchmark table
- queue follow-up reading set
