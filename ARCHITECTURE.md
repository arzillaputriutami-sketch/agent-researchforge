# ResearchForge Agents Architecture

## Goal
Demonstrate a multi-agent research workflow that produces structured, reviewer-verifiable crypto intelligence.

## Architecture

- `index.html`
  - Three-column layout: scenario selector, main content, reasoning trace + evidence.
  - Four research profiles with unique thesis, trace, evidence, and metrics.
  - Chart.js doughnut (category distribution) and radar (confidence breakdown).
  - Export button generates a plain-text proof report.
- `README.md`
  - Reviewer-facing explanation of problem, solution, and demo flow.
- Browser-only runtime
  - All data is deterministic fixtures embedded in JavaScript.
  - No API calls, no server dependencies, no secrets.

## Agent model

| Agent | Role | Output |
|---|---|---|
| Analyst | Source and synthesize raw data | Structured metrics with citations |
| Risk | Score downside scenarios | Risk factors with probability estimates |
| Thesis | Build directional narrative | Conviction score + position sizing |
| Critic | Challenge assumptions | Contradictions and historical counterpoints |

## Interaction flow

1. User selects a research profile.
2. Page loads matching scenario data.
3. User sees:
   - Thesis card with tags
   - Conviction score
   - Agent reasoning trace (5 steps)
   - Evidence bundle (severity-labeled)
   - Category and confidence charts
   - Terminal agent log
4. User exports proof report.

## Design language

- Deep violet/fuchsia palette (distinct from ChainOps cyan and DeFi Sentinel gold).
- Three-column desktop layout with responsive collapse.
- Frosted glass panels with colored orb backgrounds.
- JetBrains Mono for labels and terminal output.
- Space Grotesk for headings.

## Submission value

This project shows a complete research pipeline:

- multi-source data collection
- adversarial agent reasoning
- structured conviction output
- verifiable evidence bundle
- exportable proof

That makes it suitable for incentive programs evaluating AI agent workflows.
