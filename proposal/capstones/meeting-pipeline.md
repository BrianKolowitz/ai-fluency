---
layout: default
title: "Capstone: Meeting-to-Action Pipeline"
---

# Capstone: Meeting-to-Action Pipeline

**Difficulty:** Capable → Proficient | **Deliverable:** A reusable workflow that turns messy meeting notes into structured follow-ups

Every organization loses hours to the same problem: meetings end, notes get filed, action items get forgotten. This project builds a repeatable pipeline that uses AI to extract, organize, and communicate what actually matters from any meeting.

---

## Exercise 1: Process Raw Meeting Notes

Start with realistic, messy notes — the kind you'd actually take:

```
Prompt: "Here are my raw notes from a team meeting. They're messy 
and incomplete, like real notes:

Attendees: Sarah (dir), Mike (ops mgr), Priya (IT), me
- talked about Q3 planning, Sarah wants draft by June 15
- Mike raised issue w/ vendor contract renewal, expires July 1
  needs legal review before we can renew
- Priya says new system migration pushed to August, was supposed 
  to be July — waiting on security assessment
- budget discussion — we're 12% under on Q2, Sarah says reallocate 
  to training (AI fluency program?)
- Mike volunteered to own vendor negotiation, needs procurement 
  involved
- next meeting in 2 weeks, Priya will have security assessment 
  results by then
- Sarah wants everyone to identify one process for AI integration 
  before next meeting

Extract from these notes:
1. Key decisions made
2. Action items with owner and deadline
3. Open questions / unresolved items
4. Agenda items for next meeting

Format as clean sections with bullet points."
```

**Checkpoint:** Did the AI catch all the action items? Did it correctly assign owners? Did it flag the vendor contract deadline as urgent?

> **Industry variant (healthcare):** Use a clinical operations meeting — staffing ratios, quality metrics review, regulatory prep items. Note: never include patient identifiers in notes processed through AI.

---

## Exercise 2: Generate the Follow-Up Email

Turn the structured output into professional communication:

```
Prompt: "Using these meeting notes:

[paste structured output from Exercise 1]

Draft a follow-up email to all attendees. Include:
- Brief meeting summary (3 sentences max)
- Action items table: Item | Owner | Deadline | Status
- Key decisions documented
- Next meeting date and expected pre-reads
- Professional but not stiff tone — these are teammates

Subject line should be clear and include the date."
```

**Iterate:** Try adjusting for different audiences:
- "Rewrite this as an executive summary for Sarah's boss — cut the details, emphasize decisions and risks"
- "Rewrite just the action items as Slack messages, one per action owner"

> **Industry variant (healthcare):** Frame for a clinical department audience — include compliance action items separately from operational ones.

---

## Exercise 3: Create the Next Meeting Agenda

Chain from the follow-up to proactive planning:

```
Prompt: "Based on the action items and open issues from this meeting:

[paste your structured notes]

Create an agenda for the next meeting (2 weeks from now). Include:
- Time estimates for each agenda item
- Which items need pre-work and from whom
- A 'parking lot' section for items that were raised but deferred
- Total meeting time (target 45 min — flag if the agenda needs 
  more time)

Format as a shareable agenda document."
```

**Follow-up:**
```
"The vendor contract expires July 1 and we're meeting in 2 weeks. 
Add a risk flag to the agenda if the timeline is tight. What should 
we escalate before the next meeting?"
```

This is where AI moves from reactive (processing notes) to proactive (identifying risks and suggesting actions).

> **Industry variant (healthcare):** Include a standing "regulatory/compliance updates" agenda section typical of healthcare ops meetings.

---

## Exercise 4: Build Decision and Action Trackers

Meetings aren't isolated — they're part of an ongoing stream. Build tracking documents:

```
Prompt: "Create two tracking templates based on our meeting:

1. DECISION LOG — A table to track decisions across meetings:
   Columns: Date, Decision, Context, Made By, Status, Review Date

2. ACTION TRACKER — A table to track action items across meetings:
   Columns: ID, Action Item, Owner, Deadline, Status, Notes, 
   Source Meeting Date

Populate both with the items from our meeting. Add example entries 
showing how they'd be updated over time (e.g., an action marked 
complete, a decision revisited)."
```

**Iterate:** "Add conditional formatting rules — describe how I'd color-code overdue items in a spreadsheet, and which items should trigger reminders 3 days before deadline."

> **Industry variant (healthcare):** Add a compliance-specific tracker alongside the decision and action trackers — tracking regulatory deadlines and audit items.

---

## Exercise 5: Systematize the Pipeline

Turn this into a repeatable system:

```
Prompt: "I want to create a reusable 'meeting processing pipeline' 
that I can run after any meeting. Design it as a step-by-step 
workflow:

Step 1: Input raw notes → Output structured notes
Step 2: Structured notes → Follow-up email
Step 3: Structured notes → Action tracker update
Step 4: Action tracker → Next meeting agenda
Step 5: After next meeting → Update decision log

For each step, write the reusable prompt template with placeholders.
Include tips for each step (e.g., 'paste notes within 1 hour while 
context is fresh').

Format as a reference card I can keep at my desk or pin in a doc."
```

**Save this pipeline.** It goes in your [Personal AI Playbook](./playbook.md).

> **Industry variant (healthcare):** Note that the pipeline should include a de-identification check step for any notes that reference patient scenarios.

---

## Final Deliverable

A complete meeting processing system:

1. **Structured meeting notes** from raw input
2. **Follow-up email** ready to send
3. **Next meeting agenda** with time estimates
4. **Decision log and action tracker** templates
5. **Reusable pipeline** with prompt templates for each step

**Reflection:**
- How much time does this save per meeting? Multiply by your meetings per week.
- Where in the pipeline did you need to correct the AI most?
- What would you customize for your specific team's meeting style?

> **Industry variant (healthcare):** Use a clinical operations meeting: staffing reviews, quality metrics, regulatory prep. Add a compliance note about not including patient identifiers in meeting notes processed through AI tools.

[← Back: Expense Report Builder](./expense-report.md) | [Next: Process Documentation →](./process-improvement.md)
