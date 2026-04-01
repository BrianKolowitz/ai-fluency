# AI Fluency

## Purpose
Open-source micro-learning framework for building AI competency across organizations. Industry-agnostic by design — healthcare is used as an example vertical throughout. Designed to be forked, customized, and deployed via GitHub Pages.

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
  guidelines.md               → AI safety & compliance guidelines
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
- **Industry-agnostic framing** — Framework is for any organization. Healthcare used as one example vertical. Exercises are general-first with industry variant callouts.
- **Zapier attribution** — Inspired by Zapier's AI Fluency Rubric. Cited once in README, index, and overview.
- **just-the-docs theme** over hacker/minima — professional nav + built-in Mermaid + dark mode for the CLI-forward audience.
- **CC BY-NC-SA 4.0** instead of MIT — allows org forks (including private) but prevents commercialization/resale of the framework.
- **Fluency slope** as primary metric over pass/fail — measures growth rate, not just completion. Key differentiator.
- **AI agents as maintenance layer** — Content Review, Feedback, and Personalization agents keep the framework current without manual content management.
- **Generalized delivery** — No platform lock-in (Teams, Slack, etc.). Works with whatever the org already uses.

## Current Status
- **Done:** Full framework content, all 4 levels with exercises, measurement system, implementation plan, 6 Mermaid diagrams, Jekyll config, license. Reframed from healthcare-specific to organizational adoption framework (2026-04-01).
- **Next:** Deploy to GitHub Pages on personal account. Pitch to CIO/VP Clinical Apps workgroup on 2026-04-02.
