---
layout: default
title: Process Flows
---

# Process Flows & Architecture

## Learner Journey

How an individual moves through the framework:

<div class="mermaid">
flowchart TD
    A[Join Program] --> B[Read Safety Guidelines]
    B --> C[Self-Assess Starting Level]
    C --> D{Entry Level}
    D -->|Zero experience| E[Beginner: Foundations]
    D -->|Some experience| F[Capable: Applied Use]
    D -->|Regular user| G[Proficient: Workflow Redesign]
    D -->|Power user| H[Expert: Innovation & Leadership]
    E --> I[Daily Micro-Lessons]
    F --> I
    G --> I
    H --> I
    I --> J[Practice Exercises]
    J --> K[Weekly Fluency Slope Check-in]
    K --> L{Slope Positive?}
    L -->|Yes| M[Progress to Next Level]
    L -->|Flat/Declining| N[Adjusted Content + Support]
    M --> I
    N --> I
</div>

## Micro-Learning Delivery

How daily lessons reach learners and adapt:

<div class="mermaid">
flowchart LR
    A[Content Repo<br/>GitHub] --> B[AI Personalization Agent]
    C[Learner Profile<br/>Level + Role + Slope] --> B
    B --> D[Daily Micro-Lesson<br/>Tailored to Learner]
    D --> E[Communication Channel]
    E --> F[Learner Completes Exercise]
    F --> G[Feedback + Slope Data]
    G --> C
</div>

## AI Agent Maintenance Cycle

How the framework stays current:

<div class="mermaid">
flowchart TD
    A[Learner Feedback<br/>Exercises, Slope Data, Comments] --> B[Feedback Agent<br/>Aggregate & Analyze]
    B --> C{Patterns Identified?}
    C -->|Content gap| D[Content Review Agent<br/>Draft Updates]
    C -->|Tool change| D
    C -->|Low engagement| E[Personalization Agent<br/>Adjust Delivery]
    C -->|No issues| F[No Action Needed]
    D --> G[Proposed Changes<br/>PR in Repo]
    G --> H[Admin Review & Approve]
    H --> I[Merge & Deploy<br/>GitHub Pages Auto-Updates]
    I --> J[Notify Learners of Changes]
    E --> K[Update Learner Profiles<br/>Adjust Lesson Difficulty/Type]
    K --> L[Next Micro-Lesson Adapted]
</div>

## Technology Stack

<div class="mermaid">
flowchart TB
    subgraph Public["Open Source Core"]
        A[GitHub Repository<br/>Content + Config]
        B[GitHub Pages<br/>Web Delivery]
        A --> B
    end

    subgraph Org["Organization Fork (Private)"]
        C[Forked Repo<br/>Customized Content]
        D[GitHub Pages<br/>Internal Access]
        C --> D
    end

    subgraph AI["AI Layer"]
        E[Content Review Agent<br/>Quarterly Updates]
        F[Feedback Agent<br/>Pattern Analysis]
        G[Personalization Agent<br/>Learner Adaptation]
    end

    subgraph Tools["AI Tools (Free Tier)"]
        H[ChatGPT]
        I[Claude]
        J[Grok]
        K[CLI Tools]
    end

    subgraph Delivery["Communication"]
        L[Team Channel<br/>Daily Micro-Lessons]
        M[Feedback Forms<br/>Slope Tracking]
    end

    A --> C
    AI --> C
    M --> AI
    Tools --> L
    D --> L
</div>

## Fluency Slope Tracking

How growth is measured and acted upon:

<div class="mermaid">
flowchart LR
    A[Weekly Check-in<br/>3 Questions] --> B[Slope Calculation<br/>Breadth + Depth + Experimentation]
    B --> C{Trend}
    C -->|Steep Positive| D[Accelerate<br/>Next level exercises]
    C -->|Gradual Positive| E[Continue<br/>Reinforce current level]
    C -->|Flat| F[Intervene<br/>Adjust content, check blockers]
    C -->|Declining| G[Support<br/>Direct outreach, identify issues]
    D --> H[Update Learner Profile]
    E --> H
    F --> H
    G --> H
    H --> I[Next Lesson Personalized]
</div>

## Fork & Customize Model

How organizations adopt the framework:

<div class="mermaid">
flowchart TD
    A[Public Core Repo<br/>AI Fluency<br/>CC BY-NC-SA 4.0] --> B[Organization Forks Repo]
    B --> C[Make Private if Needed]
    C --> D[Customize Content<br/>Add internal guidelines<br/>Adjust exercises<br/>Brand for org]
    D --> E[Deploy via GitHub Pages]
    E --> F[Configure AI Agents<br/>Point to org channel & forms]
    F --> G[Launch Program]
    G --> H[Upstream Updates Available]
    H --> I{Merge Upstream?}
    I -->|Yes| J[Pull updates from public core]
    I -->|No| K[Continue with org version]
    J --> D
</div>

## Feedback-Driven Improvement

How learner feedback flows through GitHub Issues to improve the framework:

<div class="mermaid">
flowchart TD
    A[Learner completes exercise] --> B{Was it helpful?}
    B -->|Yes| C[File feedback via GitHub Issue<br/>Rate: relevance, clarity, difficulty]
    B -->|No| C
    B -->|Has suggestion| D[File suggestion via GitHub Issue<br/>New exercise or improvement]
    C --> E[Issue labeled & categorized<br/>by content area and type]
    D --> E
    E --> F[AI Agent scans issues<br/>on review cycle]
    F --> G{Pattern detected?}
    G -->|Low ratings cluster| H[Agent drafts content rewrite<br/>Creates Pull Request]
    G -->|Multiple similar suggestions| I[Agent drafts new content<br/>Creates Pull Request]
    G -->|Bug or error| J[Agent or maintainer<br/>fixes directly]
    G -->|Isolated feedback| K[Logged for future review]
    H --> L[Human reviews PR]
    I --> L
    J --> L
    L --> M[Merge & deploy<br/>GitHub Pages auto-updates]
    M --> N[Learners see improved content]
    N --> A
</div>

---

[← Back to Home](./index.md)
