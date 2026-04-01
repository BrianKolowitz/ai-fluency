# AI Fluency for Healthcare

## Purpose
Open-source micro-learning framework for building AI competency in healthcare organizations. Designed to be forked, customized, and deployed via GitHub Pages.

## Stack
- **Content:** Markdown with Jekyll frontmatter
- **Site:** GitHub Pages with `just-the-docs` theme (dark mode)
- **Diagrams:** Mermaid (rendered by just-the-docs built-in support)
- **License:** CC BY-NC-SA 4.0 (non-commercial, share-alike)

## Structure
```
index.md                      → GitHub Pages landing page
README.md                     → Repo landing page (GitHub)
_config.yml                   → Jekyll config (theme, nav, mermaid)
proposal/
  overview.md                 → Executive summary
  guidelines.md               → Healthcare AI safety framework
  measurement.md              → KPIs, fluency slope, success criteria
  implementation.md           → Rollout plan and delivery strategy
  levels/
    beginner.md               → Level 1: Foundations
    capable.md                → Level 2: Applied use (minimum bar)
    proficient.md             → Level 3: Workflow redesign
    expert.md                 → Level 4: Innovation & leadership
process-flow.md               → Mermaid diagrams (6 total)
CONTRIBUTING.md               → Contribution guidelines
LICENSE                       → CC BY-NC-SA 4.0
```

## Key Decisions
- **just-the-docs theme** over hacker/minima — professional nav + built-in Mermaid + dark mode for the CLI-forward audience.
- **CC BY-NC-SA 4.0** instead of MIT — allows org forks (including private) but prevents commercialization/resale of the framework.
- **Fluency slope** as primary metric over pass/fail — measures growth rate, not just completion. Key differentiator.
- **AI agents as maintenance layer** — Content Review, Feedback, and Personalization agents keep the framework current without manual content management.
- **Generalized delivery** — No platform lock-in (Teams, Slack, etc.). Works with whatever the org already uses.

## Current Status
- **Done:** Full framework content, all 4 levels with exercises, measurement system, implementation plan, 6 Mermaid diagrams, Jekyll config, license.
- **Next:** Deploy to GitHub Pages on personal account. Pitch to CIO/VP Clinical Apps workgroup on 2026-04-02.
