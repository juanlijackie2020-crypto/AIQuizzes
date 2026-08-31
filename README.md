# AI Level Quiz

Four short self-assessments that plot you — as an individual, a team, a leader, or an organization — on a clear AI maturity scale. No accounts, no tracking, no server: everything runs and scores in your browser.

**Try it live:** `https://<your-github-username>.github.io/ai-level-quiz/`

## The Four Lenses

| Quiz | What it measures | Output |
|------|------------------|--------|
| **Individual** | Your personal AI collaboration capability — daily usage, prompting, context management, agents, quality control | L1–L5 level + role-specific advice |
| **Team** | Collective AI maturity — from fragmented personal use to a governed, shared AI system | L1–L5 on the team ladder |
| **Leadership** | Readiness to lead an AI-native team — vision, sponsorship, creating conditions for others | Readiness profile + development path |
| **Organization** | AI Nativeness × Organizational Readiness | One of four quadrants: Leader, Explorer, Commando, Onlooker |

The **Individual**, **Team**, and **Leadership** quizzes share a five-rung ladder:

- **L1 — Instructional**: one-sentence prompts, results depend on luck
- **L2 — Structured**: roles, formats, and constraints — but rebuilt from scratch every time
- **L3 — Collaborative**: AI as a thinking partner, with context and role-play
- **L4 — Systematic**: agents and workflows embedded in how you work
- **L5 — Asset-Based**: your methods have become reusable, measurable digital assets

## Features

- **Bilingual** — every quiz runs in English and 中文, switchable at any time
- **Private by design** — scoring happens entirely in your browser; no data leaves your device
- **Zero dependencies** — each quiz is a single self-contained HTML file
- **Instant report** — level, strengths, blockers, and a concrete upgrade path per result

## Run It Locally

Just open `index.html` in a browser. No build step, no install, no server required.

## Deploy to GitHub Pages

1. Push this repository to GitHub.
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Your site goes live at `https://<username>.github.io/ai-level-quiz/` within a minute or two.

## Repository Structure

```
ai-level-quiz/
├── index.html               # Landing hub — pick your lens
├── quizzes/
│   ├── individual.html      # 8 questions · ~2 min · L1–L5
│   ├── team.html            # 8 questions · ~2 min · L1–L5
│   ├── leadership.html      # 8 questions · ~2 min · readiness
│   └── organization.html    # 11 questions · ~3 min · quadrant
├── README.md
└── LICENSE
```

## Customize

All copy lives in a bilingual `i18n` object at the top of each quiz's `<script>` block (`en` / `zh` keys). Edit questions, options, or result reports there — everything else (scoring, navigation, result rendering) adapts automatically. Scoring bands for the ladder quizzes are in `calculateLevel()` if you want to retune them.

## License

[MIT](LICENSE) — free to use, adapt, and build on. If it helps you or your team, a star is appreciated.
