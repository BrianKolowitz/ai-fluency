---
layout: default
title: Feedback
---

# Feedback

This framework improves through your feedback. Every rating, suggestion, and bug report feeds directly into the system — AI agents analyze patterns across feedback to improve content, retire what isn't working, and create what's missing.

## How to Give Feedback

All feedback is collected through [GitHub Issues](https://github.com/BrianKolowitz/ai-fluency/issues/new/choose). Choose the type that fits:

| Type | When to Use |
|:-----|:------------|
| [Content Feedback](https://github.com/BrianKolowitz/ai-fluency/issues/new?template=content-feedback.yml) | Rate and comment on a page, exercise, or lesson you've completed |
| [Exercise Suggestion](https://github.com/BrianKolowitz/ai-fluency/issues/new?template=exercise-suggestion.yml) | Propose a new exercise, topic, or improvement |
| [Industry Variant](https://github.com/BrianKolowitz/ai-fluency/issues/new?template=industry-variant.yml) | Suggest an adaptation for your industry (finance, legal, education, etc.) |
| [Bug Report](https://github.com/BrianKolowitz/ai-fluency/issues/new?template=bug-report.yml) | Report errors, broken links, outdated info, or rendering issues |

You can also [browse existing feedback](https://github.com/BrianKolowitz/ai-fluency/issues) to upvote, comment, or build on ideas others have shared.

## What Happens with Your Feedback

Feedback isn't just collected — it's acted on. Here's the loop:

<div class="mermaid">
flowchart TD
    A[You complete an exercise] --> B[File feedback as a GitHub Issue]
    B --> C[Issue is labeled and categorized]
    C --> D{AI Agent reviews}
    D -->|Content gap| E[Agent drafts improved content]
    D -->|Low ratings| F[Agent flags for rewrite]
    D -->|New suggestion| G[Agent evaluates feasibility]
    D -->|Bug report| H[Agent or maintainer fixes]
    E --> I[Pull Request created]
    F --> I
    G --> I
    H --> I
    I --> J[Human reviews and merges]
    J --> K[Site automatically updates]
    K --> L[You see improved content]
</div>

## What We Collect

Each feedback submission captures structured data that AI agents use to identify patterns:

- **Relevance rating** — Is this content useful for your actual work?
- **Clarity rating** — Is it easy to understand and follow?
- **Difficulty assessment** — Is the challenge level appropriate?
- **Completion status** — Did you finish the exercise?
- **Free-text comments** — What worked, what didn't, what's missing
- **Role and level** (optional) — Helps us understand who the content serves

## How AI Agents Use Feedback

### Pattern Detection

When multiple people report the same issue, the agent surfaces it:

- *"8 of 12 Capable-level feedback entries rate Exercise 2.2a clarity as 2/5 or below"* → Agent drafts a rewrite with clearer instructions
- *"4 suggestions for a budgeting capstone from finance-role users"* → Agent proposes a new capstone project
- *"Exercise 3.1 consistently rated 'too easy' by Proficient-level users"* → Agent suggests increasing complexity or moving it to Capable

### Content Lifecycle

Every piece of content goes through a lifecycle driven by feedback:

```
New → Active → Monitored → Improved or Retired
```

- **New** — Just created, collecting initial feedback
- **Active** — Positive ratings, actively used
- **Monitored** — Mixed or declining ratings, flagged for review
- **Improved** — Rewritten based on feedback patterns
- **Retired** — Consistently low value, replaced with better content

### Role-Specific Adaptation

As feedback accumulates with role data, the agent identifies which exercises work best for which roles:

- *"Operations managers rate the Meeting Pipeline capstone 4.8/5 but the Expense Report capstone 3.1/5"* → Recommend Meeting Pipeline first for ops managers
- *"IT staff consistently skip Beginner exercises but struggle at Proficient 3.3"* → Suggest IT-specific entry path

Over time, this builds a recommendation engine: the right content for the right person at the right time.

## For Organizations (Forked Repos)

When you fork this framework for your organization:

1. **Issues stay in your fork** — Feedback from your team is private to your repo
2. **Customize the templates** — Add org-specific fields (department, team, location)
3. **Configure your own agent** — Point it at your fork's issues to process feedback for your context
4. **Contribute back** — If your team produces great content improvements, submit a PR to the public core

## Feedback Principles

- **All feedback is valuable.** A "this didn't work for me" is as useful as a detailed suggestion.
- **Structured ratings drive automation.** The numeric ratings let AI agents detect patterns at scale. Free text adds the nuance.
- **You own the improvement loop.** Your feedback directly shapes what this framework becomes. Every merged PR from a feedback issue credits the original reporter.
- **No feedback is ignored.** Even if content isn't changed immediately, every issue informs the agent's understanding of what's working and what isn't.
