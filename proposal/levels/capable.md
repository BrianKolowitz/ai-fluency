---
layout: default
title: "Level 2: Capable"
---

# Level 2: Capable — Applied Use

**Time:** ~1 hour | **Prerequisites:** [Beginner](./beginner.html) or equivalent experience | **Goal:** Use AI as a daily tool with structured prompting and consistent output quality.

This is the **minimum bar** for the organization. At this level, AI is no longer experimental — it's part of how you work. You can write effective prompts, get reliable results, and apply AI to real tasks with confidence.

---

## 2.1 Structured Prompting (20 min)

The difference between a beginner and a capable AI user is **prompt structure**. Instead of vague questions, you give the AI clear context, a specific role, and defined constraints.

**The prompt framework:**

```
Role:    Who should the AI act as?
Context: What's the situation?
Task:    What specifically do you need?
Format:  How should the output be structured?
Constraints: What should it avoid or include?
```

### Exercise 2.1: Role-Based Prompting

```
Prompt: "Act as a healthcare communications specialist. I need to 
draft a patient-facing FAQ about a new telehealth service. The 
audience is patients aged 60+, many of whom are not tech-savvy. 

Write 8 Q&A pairs. Use simple language (6th grade reading level). 
Each answer should be 2-3 sentences max. Include a question about 
privacy/security."
```

Compare this output to what you'd get from: "Write a telehealth FAQ." The difference is the structure.

**Iterate:** Ask the AI to add a question you think is missing, or adjust the reading level. Notice how specific instructions produce specific results.

---

## 2.2 AI for Research and Synthesis (20 min)

AI excels at synthesizing information from complex topics into actionable summaries. The key skill: knowing what to ask for and how to verify.

### Exercise 2.2: Research Synthesis

```
Prompt: "Summarize the key differences between the following 
approaches to staff training in healthcare: classroom-based, 
e-learning, micro-learning, and on-the-job mentoring. 

Present as a comparison table with columns: Approach, Strengths, 
Weaknesses, Best For, Time Investment. Focus on what's most 
relevant for a mid-size healthcare organization."
```

**Verify:** Pick one claim from the output and check it against a published source. Did the AI get it right? Where was it imprecise?

### Exercise 2.3: From Research to Action

Take the output from 2.2 and chain it:

```
Follow-up: "Based on this comparison, recommend an approach for an 
organization that needs to train 200 employees across clinical and 
administrative roles in AI skills. They have limited budget and 
can't pull people off the floor for full-day sessions. Justify 
your recommendation."
```

This is **prompt chaining** — building on previous context to go deeper. It's how you move from one-off questions to sustained AI-assisted work.

---

## 2.3 Measuring Your Impact (15 min)

At this level, start tracking how AI affects your work:

### Exercise 2.4: Time Audit

Choose a task you completed with AI this week. Estimate:

| Metric | Without AI | With AI |
|:-------|:-----------|:--------|
| Time to complete | | |
| Quality (1-5) | | |
| Number of iterations | | |

```
Prompt: "I just used AI to [describe task]. It took me [time] 
compared to an estimated [time] without AI. Help me identify 3 
other tasks in my weekly routine where I could see similar gains. 
My role is [your role]."
```

This builds the habit of **quantifying AI impact** — which matters when the organization measures adoption.

---

## 2.4 Command-Line AI Interaction (15 min)

AI tools aren't limited to web interfaces. Working from the command line unlocks faster iteration and integration into technical workflows.

### Exercise 2.5: CLI Basics

If you have access to a CLI AI tool (Claude Code, OpenAI CLI, or similar):

```bash
# Ask a direct question
claude "What are the HIPAA Safe Harbor de-identification standards? 
List all 18 identifiers."

# Pipe content into AI for analysis
cat meeting_notes.txt | claude "Summarize the key action items 
from these meeting notes. Format as a checklist."

# Use AI for quick drafting
claude "Draft a 3-sentence project status update. The project is 
an AI training pilot for 50 staff. We completed week 1 with 80% 
enrollment and positive feedback."
```

The command line is where AI becomes a **power tool** — fast, scriptable, and integrated into how technical work gets done.

---

## 2.5 Checkpoint

Before moving to Proficient, you should be able to answer yes to these:

- [ ] I use structured prompts (role, context, task, format, constraints)
- [ ] I can chain prompts to build on previous AI output
- [ ] I've verified AI output against a real source
- [ ] I can estimate the time savings from AI-assisted tasks
- [ ] I use AI at least a few times per week in my actual work

**Fluency slope check:** Compare your AI usage this week to last week. Are you using it more often? For more complex tasks? That's positive slope.

[← Back: Beginner](./beginner.html) | [Next: Level 3 — Proficient →](./proficient.html)
