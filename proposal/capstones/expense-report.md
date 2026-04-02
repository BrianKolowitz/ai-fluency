---
layout: default
title: "Capstone: Expense Report Builder"
---

# Capstone: Expense Report Builder

**Difficulty:** Beginner → Capable | **Time:** ~1.5 hours across exercises | **Deliverable:** A formatted expense report ready for submission

You just got back from a work trip. You have a pile of receipts, some in your email, some photographed on your phone, some scribbled on napkins. Instead of spending an hour wrestling with a spreadsheet, you'll use AI to organize, categorize, format, and prepare a complete expense report.

---

## Exercise 1: Collect and Structure Raw Data (15 min)

Start with messy input — just like real life. Create a rough list of expenses (use a real trip or make one up):

```
Prompt: "I need to organize expenses from a 3-day work trip. Here's 
what I have — it's messy, just like my receipts:

- uber from airport $47.50 tuesday
- dinner with client at Mortons, around $185, tues night, tip included
- hotel Marriott 3 nights, $189/night
- coffee wednesday morning $6.20
- Lyft to client office wed $23
- lunch working session $34.50 wednesday, 3 people
- uber back to airport thursday $52
- airport parking at home $45 for 3 days
- flight was $384 round trip booked last month

Turn this into a structured table with columns: Date, Category 
(Transport, Lodging, Meals, Other), Description, Amount. Sort by 
date, then category."
```

**Checkpoint:** Does the table capture everything? Are the categories logical? Did the AI calculate the hotel total correctly (3 × $189)?

---

## Exercise 2: Categorize and Validate (15 min)

Now refine the categorization and catch errors:

```
Prompt: "Review this expense table for issues:

[paste your table from Exercise 1]

Check for:
1. Are any expenses potentially non-reimbursable? Flag them.
2. Are meal expenses within a typical per-diem range ($75/day)?
3. Is the hotel total calculated correctly?
4. Are there any missing expenses I might have forgotten for a 
   3-day business trip (baggage fees, parking, tips, wifi)?
5. Suggest a category for each flagged item."
```

**Checkpoint:** Did the AI catch the per-diem issue with the $185 dinner? Did it suggest expenses you actually forgot? This is where AI verification skills matter — the AI is checking your data, but you're checking the AI.

---

## Exercise 3: Format for Submission (15 min)

Turn the validated data into a submission-ready format:

```
Prompt: "Format this expense data into a professional expense report. 
Include:

[paste your validated table]

Requirements:
- Header with: Employee name (use 'Your Name'), trip purpose 
  ('Client meeting — [City]'), dates
- Expenses grouped by category with subtotals
- Grand total at the bottom
- Notes column for any items that need explanation (e.g., client 
  dinner over per-diem)
- Format as a clean markdown table I could paste into a document 
  or convert to PDF"
```

**Iterate:** Ask the AI to adjust formatting. Try: "Add a column for receipt status (have/missing)" or "Add the company policy note about meals over $50 requiring manager approval."

---

## Exercise 4: Generate the Summary Memo (15 min)

Most expense reports need a cover memo or summary:

```
Prompt: "Write a brief expense report summary memo for my manager. 
Include:
- Trip purpose and dates
- Total expenses: [your total]
- Breakdown by category (one line each)
- Flag the dinner that exceeded per-diem with a brief justification 
  ('client entertainment — prospect meeting')
- Keep it under 150 words, professional tone

Also generate a one-line email subject for submitting this report."
```

---

## Exercise 5: Build a Reusable Template (15 min)

Turn this into a tool you'll use again:

```
Prompt: "Based on the expense report we just built, create a 
reusable prompt template I can use for any future trip. Include:

- Placeholders for: trip dates, destination, purpose, raw expense list
- The full pipeline: raw data → structured table → validation → 
  formatted report → summary memo
- A checklist of common expenses to jog my memory
- Instructions for someone who's never done this before

Format it so I can copy-paste it and fill in the blanks."
```

**Save this template.** It goes in your [Personal AI Playbook](./playbook.md).

---

## Final Deliverable

Combine your outputs into a complete expense report package:

1. **Formatted expense table** with categories, subtotals, and grand total
2. **Summary memo** for your manager
3. **Reusable template** for future trips

**Reflection:**
- How long would this have taken without AI? How long did it take with AI?
- Where did the AI make mistakes you had to catch?
- What would you add to the template for next time?

> **Industry variant (healthcare):** Use a conference trip to a medical conference (HIMSS, ACHE, etc.) as the scenario. Add categories for CME registration fees and required documentation for education reimbursement.

[← Back to Capstone Projects](./index.md)
