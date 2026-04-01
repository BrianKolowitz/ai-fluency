---
layout: default
title: "Level 3: Proficient"
---

# Level 3: Proficient — Workflow Redesign

**Time:** ~1-2 hours | **Prerequisites:** [Capable](./capable.html) | **Goal:** Move from using AI for individual tasks to redesigning workflows and processes with AI integration.

At this level, you stop asking "Can AI help with this task?" and start asking "Should this process be AI-first?" You're thinking systemically, not task-by-task.

---

## 3.1 AI-First Process Thinking (25 min)

Most workflows were designed before AI existed. They have manual steps that exist because automation wasn't available. Proficient users identify these steps and redesign around them.

**The audit framework:**

1. Map the current workflow (steps, inputs, outputs, decisions)
2. Identify steps where AI could draft, summarize, analyze, or generate
3. Identify steps that **must** remain human (clinical judgment, final approvals, patient interaction)
4. Redesign with AI handling the drafting/analysis and humans handling the judgment/approval

### Exercise 3.1: Workflow Audit

Pick a real process you're involved in (onboarding, report generation, meeting prep, policy review). Map it out, then:

```
Prompt: "I have a workflow for [describe process] with these steps:
1. [step 1]
2. [step 2]
3. [step 3]
...

For each step, evaluate whether AI could handle it fully, assist 
with it, or whether it must remain fully human. Then suggest a 
redesigned workflow. This is in a healthcare setting — flag any 
steps with compliance implications."
```

**Key insight:** The best AI integrations don't add AI to existing steps — they eliminate steps entirely. A report that took 3 hours of research, 1 hour of drafting, and 1 hour of formatting might take 30 minutes of prompted generation and 30 minutes of human review.

---

## 3.2 Building Reusable Prompt Systems (25 min)

One-off prompts are Capable-level work. Proficient users build **prompt templates** — reusable, tested prompts that produce consistent results for recurring tasks.

### Exercise 3.2: Create a Prompt Template

Identify a task you do repeatedly (weekly reports, meeting summaries, communication drafts). Build a template:

```
Prompt: "Help me create a reusable prompt template for [recurring 
task]. The template should have:
- A clear role definition
- Placeholders for variable inputs (marked with [brackets])
- Consistent output format
- Quality criteria the output should meet
- A verification checklist

I'll be using this template weekly, so it needs to produce 
reliable results with minimal editing."
```

Test the template with real inputs. Refine until the output consistently meets your standard. Save it — this is now a tool in your toolkit.

---

## 3.3 Data Analysis and Synthesis (25 min)

AI can process and interpret data patterns when given the right framing. This isn't about replacing analytics tools — it's about rapid synthesis and hypothesis generation.

### Exercise 3.3: Analyze Hypothetical Data

```
Prompt: "Here's hypothetical patient satisfaction data for a 
healthcare organization:

Department A: 4.2/5 (n=500), trending down from 4.5 over 6 months
Department B: 3.8/5 (n=300), stable
Department C: 4.6/5 (n=200), trending up from 4.1

Wait times: A=25min avg, B=40min avg, C=15min avg
Staff turnover: A=12%, B=22%, C=8%

Analyze the correlations. What story does this data tell? What 
would you investigate further? Present findings in a format 
suitable for a department head meeting."
```

**Follow-up:** "Now generate 3 specific, actionable recommendations based on this analysis. Include metrics we should track to measure whether the interventions are working."

---

## 3.4 For Managers: Driving Team Adoption (20 min)

If you manage people, your fluency multiplies through your team. This exercise focuses on creating the conditions for team-wide AI adoption.

### Exercise 3.4: Team Adoption Plan

```
Prompt: "I manage a team of [size] in [department] at a healthcare 
organization. I want to increase AI adoption on my team. Current 
state: [describe — e.g., 2 of 8 team members use AI regularly].

Design a 30-day plan to increase adoption. Consider:
- Different comfort levels (some resistant, some eager)
- Time constraints (can't add hours to the workday)
- Healthcare compliance requirements
- How to make early wins visible to build momentum

Include specific actions for week 1, 2, 3, and 4. Format as a 
table with columns: Week, Action, Owner (me vs team), Expected 
Outcome."
```

**Then:** Share the output (or your adapted version) with your team for feedback. This models the behavior you want to see.

---

## 3.5 Checkpoint

Before moving to Expert, you should be able to answer yes to these:

- [ ] I've audited and redesigned at least one workflow with AI integration
- [ ] I have at least one reusable prompt template I use regularly
- [ ] I can identify which parts of a process should be AI-first vs. human-only
- [ ] I've used AI for data analysis or synthesis beyond simple Q&A
- [ ] (Managers) I have a plan for increasing team AI adoption

**Fluency slope check:** Are you initiating AI use proactively, or only when reminded? Proactive use is the signal of proficiency.

[← Back: Capable](./capable.html) | [Next: Level 4 — Expert →](./expert.html)
