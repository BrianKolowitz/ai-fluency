---
layout: default
title: "Capstone: Process Documentation & Improvement"
---

# Capstone: Process Documentation & Improvement

**Difficulty:** Proficient → Expert | **Deliverable:** A current-state SOP and an AI-improved process proposal

Every organization has processes that evolved organically — workarounds stacked on workarounds, manual steps nobody questions, documentation that's years out of date. This project picks one real process, documents it properly, and redesigns it with AI integration.

This is the capstone that most directly demonstrates the shift from "using AI" to "thinking AI-first."

---

## Exercise 1: Select and Map the Current Process

Choose a real process you're involved in. Good candidates:
- New employee onboarding
- Monthly reporting
- Vendor or contract review
- Request intake and triage
- Content review and approval
- Incident response or escalation

```
Prompt: "I want to document and improve a process. The process is: 
[describe your process in 2-3 sentences — what triggers it, who's 
involved, what's the output].

Help me map the current state:
1. List every step from trigger to completion
2. For each step, identify: who does it, how long it takes, what 
   tools are used, what the input/output is
3. Identify handoff points between people
4. Flag steps that are manual, repetitive, or frequently cause delays

Format as a numbered process map. Include a 'pain points' section 
at the end."
```

**Checkpoint:** Walk through the output against reality. What did the AI miss? What steps do you do that you didn't think to mention? Add them — the goal is a complete, honest picture.

> **Industry variant (healthcare):** Good candidates for healthcare: patient intake, referral processing, prior authorization, discharge planning, medication reconciliation.

---

## Exercise 2: Generate the Current-State SOP

Turn the process map into a proper Standard Operating Procedure:

```
Prompt: "Convert this process map into a formal Standard Operating 
Procedure (SOP) document:

[paste your process map from Exercise 1]

Include:
- Document header: Title, version (1.0), effective date, owner
- Purpose and scope (when does this process apply?)
- Roles and responsibilities
- Step-by-step procedure with enough detail for someone new to 
  follow
- Decision points written as if/then rules
- References to tools or systems used
- Revision history table (just the template)

Use clear, imperative language ('Submit the form' not 'The form 
should be submitted'). Target someone performing this process for 
the first time."
```

**Iterate:** "Add a RACI matrix (Responsible, Accountable, Consulted, Informed) for each step."

This SOP has standalone value even before improvement — most processes don't have current documentation.

> **Industry variant (healthcare):** Include regulatory references (Joint Commission standards, CMS requirements) as a section in the SOP.

---

## Exercise 3: Identify AI Integration Opportunities

Now analyze the process for AI-first redesign:

```
Prompt: "Analyze this process for AI integration opportunities:

[paste your SOP]

For each step, evaluate:
- Could AI handle this fully? (automate)
- Could AI assist? (draft, summarize, analyze — human reviews)
- Must this remain fully human? (judgment, approval, relationship)

Then categorize into:
[AUTOMATE] — AI handles end-to-end
[ASSIST] — AI drafts/prepares, human reviews/approves
[HUMAN-ONLY] — Requires judgment, accountability, or relationship

Present as a table: Step | Current State | AI Opportunity | 
Category | Estimated Time Savings

Calculate total time savings per cycle."
```

**Follow-up:**
```
"For each [AUTOMATE] and [ASSIST] item, write the specific AI prompt or 
workflow that would handle it. Be concrete — if step 4 is 
'summarize incoming requests,' write the exact prompt someone 
would use."
```

> **Industry variant (healthcare):** Flag any step involving PHI as [HUMAN-ONLY] or requiring additional de-identification safeguards before AI can assist.

---

## Exercise 4: Design the Improved Process

Redesign with AI integrated:

```
Prompt: "Based on the AI integration analysis:

[paste your analysis from Exercise 3]

Design the improved process:
1. Rewrite the step-by-step procedure with AI steps integrated
2. For AI-assisted steps, specify: what tool, what prompt, what 
   the human reviews
3. Identify new steps that didn't exist before (e.g., 'verify AI 
   output' or 'update prompt template based on results')
4. Calculate the new total cycle time vs. current
5. List risks of the new process and mitigations

Also create a before/after comparison:
Current: X steps, Y minutes, Z handoffs
Improved: X steps, Y minutes, Z handoffs"
```

**Iterate:** "Generate a text-based process flow diagram showing the improved workflow. Mark which steps are AI-handled, AI-assisted, or human-only."

> **Industry variant (healthcare):** Include a compliance review gate in any redesigned healthcare workflow — no AI-touched step goes live without compliance sign-off.

---

## Exercise 5: Build the Business Case

Package this for a decision-maker:

```
Prompt: "Create a one-page business case for implementing the 
improved process. Include:

Current process: [steps, time, pain points from Exercise 1]
Proposed process: [improvements from Exercise 4]

Structure:
- Problem statement (2-3 sentences)
- Proposed solution (what changes)
- Impact: time savings per cycle × frequency = annual hours saved
- Cost: Uses free AI tools; additional costs scale with tool choice
- Risk: what could go wrong and how we mitigate
- Implementation: what it takes to switch (training, setup)
- Recommendation: clear ask ('approve pilot for team X')

Write for a director or VP. Data-driven, concise, no jargon."
```

> **Industry variant (healthcare):** Frame ROI in healthcare terms — reduced wait times, improved throughput, staff satisfaction, compliance audit readiness.

---

## Final Deliverable

A complete process improvement package:

1. **Current-state process map** with pain points identified
2. **Formal SOP** documenting the existing process
3. **AI integration analysis** with opportunity assessment
4. **Redesigned process** with AI steps, prompts, and time savings
5. **One-page business case** ready to present

**Reflection:**
- What was the total time savings in the redesigned process?
- Which AI integrations were obvious? Which surprised you?
- Could you apply this same analysis to another process? (You now have a reusable methodology.)

> **Industry variant (healthcare):** Apply this to a clinical workflow: referral processing, prior authorization, or patient intake. Add compliance review as a required step in the AI analysis — any AI-touched step involving patient data needs additional safeguards.

[← Back: Meeting-to-Action Pipeline](./meeting-pipeline.md) | [Next: Personal AI Playbook →](./playbook.md)
