# ResearchForge Agents

ResearchForge is a multi-agent crypto research intelligence console. It demonstrates how specialized AI agents collaborate to analyze tokens, track narratives, model unlock risk, and monitor whale flows — then produce a scored conviction output with an exportable evidence bundle.

Live demo: `https://arzillaputriutami-sketch.github.io/agent-researchforge/`

## Problem

Crypto research requires synthesizing data from dozens of sources: on-chain metrics, developer activity, social signals, token schedules, whale movements, and institutional flows. Manual research is slow, biased, and rarely produces structured evidence that a third party can audit.

## Solution

ResearchForge coordinates four specialized agents:

- **Analyst** — sources and synthesizes raw data
- **Risk** — scores downside scenarios
- **Thesis** — builds a directional narrative
- **Critic** — challenges assumptions and surfaces contradictions

Each agent produces structured output. The system merges these into a conviction score with a reasoning trace and evidence bundle.

## Demo features

- Four interactive research profiles:
  - Token Thesis Builder
  - Narrative Tracker
  - Unlock Risk Radar
  - Whale Flow Monitor
- Conviction score with position sizing recommendation
- Agent reasoning trace (5-step process)
- Evidence bundle with severity labels
- Category distribution chart (doughnut)
- Confidence breakdown chart (radar)
- Terminal-style agent log transcript
- Exportable proof report (plain text)
- No API keys, wallets, or backend services required

## AI model framing

In production, each agent role could be backed by a long-context model like MiMo:

- Analyst: multi-source data retrieval and synthesis
- Risk: quantitative modeling and Monte Carlo simulation
- Thesis: narrative construction from structured signals
- Critic: adversarial reasoning and historical comparison

The browser demo uses deterministic fixtures to demonstrate the complete workflow safely.

## Reviewer usage path

1. Open the live demo.
2. Click each research profile in the left panel.
3. Press **Run research simulation** to cycle profiles.
4. Inspect the thesis, agent trace, evidence bundle, and charts.
5. Press **Export proof report** to download a structured text report.

## Tech stack

- Static HTML
- Tailwind CDN
- Chart.js (doughnut + radar)
- Vanilla JavaScript
- GitHub Pages deployment

## Safety

This repository contains no private credentials, wallet material, server-side code, or live API endpoints. All data is synthetic and deterministic.
