# AI Fluency

## Purpose
Open-source micro-learning framework for building AI competency across organizations. Industry-agnostic by design — healthcare is used as an example vertical throughout. Designed to be forked, customized, and deployed via GitHub Pages.

## Stack
- **Content:** Markdown with Jekyll frontmatter
- **Site:** GitHub Pages with `jekyll-theme-hacker` (dark mode, terminal aesthetic)
- **Diagrams:** Mermaid (rendered via CDN in custom layout)
- **License:** CC BY-NC-SA 4.0 (non-commercial, share-alike)

## Structure
```
index.md                      → GitHub Pages landing page
README.md                     → Repo landing page (GitHub)
_config.yml                   → Jekyll config (theme, url, baseurl)
_layouts/default.html         → Custom layout with nav, mermaid, footer
proposal/
  index.md                    → Proposal section table of contents
  overview.md                 → Executive summary
  guidelines.md               → AI safety & compliance guidelines
  measurement.md              → KPIs, fluency slope, success criteria
  implementation.md           → Rollout plan and delivery strategy
  levels/
    index.md                  → Competency levels overview
    beginner.md               → Level 1: Foundations
    capable.md                → Level 2: Applied use (minimum bar)
    proficient.md             → Level 3: Workflow redesign
    expert.md                 → Level 4: Innovation & leadership
  capstones/
    index.md                  → Capstone projects overview
    expense-report.md         → Capstone: Expense Report Builder
    meeting-pipeline.md       → Capstone: Meeting-to-Action Pipeline
    process-improvement.md    → Capstone: Process Documentation & Improvement
    playbook.md               → Capstone: Personal AI Playbook
process-flow.md               → Mermaid diagrams (6 total)
CONTRIBUTING.md               → Contribution guidelines
LICENSE                       → CC BY-NC-SA 4.0
```

## Key Decisions
- **Industry-agnostic framing** — Framework is for any organization. Healthcare used as one example vertical. Exercises are general-first with industry variant callouts.
- **Zapier attribution** — Inspired by Zapier's AI Fluency Rubric. Cited once in README, index, overview, and levels index.
- **jekyll-theme-hacker** — Terminal aesthetic with custom layout for nav bar, Mermaid CDN integration, centered 80% width content.
- **CC BY-NC-SA 4.0** instead of MIT — allows org forks (including private) but prevents commercialization/resale of the framework.
- **Fluency slope** as primary metric over pass/fail — measures growth rate, not just completion. Key differentiator.
- **AI agents as maintenance layer** — Content Review, Feedback, and Personalization agents keep the framework current without manual content management. Designed but not yet implemented — Phase 2.
- **Generalized delivery** — No platform lock-in (Teams, Slack, etc.). Works with whatever the org already uses.

## Current Status
- **Done:** Full framework content, all 4 levels with exercises (healthcare variants on all), 4 capstone projects, measurement system, implementation plan, 6 Mermaid diagrams, Jekyll config with hacker theme, CC BY-NC-SA license. Deployed to GitHub Pages.
- **Next:** Pitch to CIO/VP Clinical Apps workgroup on 2026-04-02. AI agent implementation is Phase 2.
