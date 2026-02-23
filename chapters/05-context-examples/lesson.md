# Chapter 5: Providing Context and Examples

← [Previous: Chapter 4 - Role Assignment](../04-role-persona/lesson.md) | [Home](../../README.md) | [Next: Chapter 6 - Separating Instructions from Data →](../06-instructions-data/lesson.md)

---

## Overview

**Level:** Intermediate  
**Duration:** 30 minutes  
**Prerequisites:** Chapters 1-4

## Learning Objectives

- Learn what context to include and what to omit
- Understand how examples guide AI behavior
- Practice providing relevant background information
- Master context placement strategies

---

## What is Context?

Context is the background information AI needs to understand your situation and generate appropriate responses. Think of it as setting the stage before asking for help.

### Why Context Matters

**Without context:**
```
Summarize this report.
```
AI doesn't know: Who it's for, why it matters, what to focus on, how detailed to be.

**With context:**
```
Summarize this quarterly financial report for our board of directors who need
to make budget decisions for next quarter. Focus on revenue trends, cost concerns,
and cash flow. They're non-financial executives, so avoid accounting jargon.
```
AI now understands: Audience, purpose, focus areas, and communication style.

---

## Types of Context

### 1. Audience Context

**Who will read/use this?**
- Their role and expertise level
- What they care about
- What they already know
- How they prefer information

**Example:**
```
Audience: New employees in their first week
- No prior knowledge of our systems
- Need step-by-step guidance
- Prefer simple language
- Want to feel confident, not overwhelmed
```

### 2. Purpose Context

**Why are you creating this?**
- What decision does it support?
- What problem does it solve?
- What action should result?
- What outcome do you want?

**Example:**
```
Purpose: Help the sales team decide which leads to prioritize this month
- Need to allocate limited time effectively
- Want to maximize conversion probability
- Must consider deal size and timeline
```

### 3. Background Context

**What's the situation?**
- Relevant history
- Current state
- Constraints or limitations
- Related information

**Example:**
```
Background: We launched this product 6 months ago
- Initial sales were strong but have plateaued
- Competitors have released similar products
- We have limited marketing budget
- Need to differentiate or adjust strategy
```

### 4. Relationship Context

**What's the connection?**
- Your relationship to the recipient
- Previous interactions
- Shared knowledge
- Communication norms

**Example:**
```
Relationship: Long-term client we've worked with for 3 years
- Very satisfied with our service
- Informal, friendly communication style
- They know our team and processes
- Trust is established
```

---

## How Much Context is Enough?

### The Goldilocks Principle

**Too little:**
```
Write an email about the meeting.
```
Missing: Who, what meeting, what about it, what tone?

**Too much:**
```
Write an email about the meeting that happened on Tuesday, March 12th at 2 PM
in Conference Room B on the 3rd floor of our downtown office building at
123 Main Street, where we discussed the Q2 marketing campaign including social
media strategy, content calendar, budget allocation, team responsibilities,
timeline, deliverables, and also briefly touched on the upcoming trade show...
```
Overwhelming and includes irrelevant details.

**Just right:**
```
Write a follow-up email to the marketing team after yesterday's Q2 planning meeting.
Summarize the key decisions (social media focus, $50K budget, April launch),
confirm action items with owners, and set next meeting date. Tone: professional
but friendly, we're a collaborative team.
```
Includes what's needed, nothing more.

---

## Context Placement Strategies

### Front-Loading Context

Put context before the task:
```
Context: I'm preparing a proposal for a healthcare client who values
data security and HIPAA compliance above all else.

Task: Write an introduction paragraph for our proposal that emphasizes
our security credentials and compliance expertise.
```

**When to use:** Complex situations where understanding context is crucial.

### Integrated Context

Weave context into the task description:
```
Write an introduction paragraph for a healthcare proposal that emphasizes
our security credentials and HIPAA compliance expertise, as this client
values data security above all else.
```

**When to use:** Simpler situations where context flows naturally.

### Structured Context

Organize context in sections:
```
Audience: Healthcare CIO and security team
Purpose: Win contract for patient data management system
Key concerns: HIPAA compliance, data security, uptime
Our strengths: 15 years healthcare experience, zero breaches, 99.99% uptime

Task: Write proposal introduction addressing their concerns and highlighting our strengths.
```

**When to use:** Multiple types of context or complex scenarios.

---

## Using Examples to Guide AI

Examples show AI exactly what you want. This is the foundation of "few-shot learning."

### Zero-Shot (No Examples)

Just instructions:
```
Write a professional email declining a meeting invitation.
```

Works for common tasks, but output may vary.

### One-Shot (One Example)

One example to show the pattern:
```
Write a professional email declining a meeting invitation.

Example of our style:
"Hi Sarah, Thanks for the invitation to next week's planning session.
Unfortunately, I have a conflict and won't be able to attend. Could you
share the notes afterward? Thanks! - Alex"

Now write a similar email declining a lunch meeting with a client.
```

Better consistency with your style.

### Few-Shot (Multiple Examples)

Multiple examples to establish pattern:
```
Write a product feature description in our style.

Example 1: "Smart Scheduling: Let AI find the perfect meeting time for everyone.
No more endless email chains." (Feature name: benefit statement. Pain point addressed.)

Example 2: "Real-time Collaboration: Edit documents together, see changes instantly.
Work feels like you're in the same room." (Feature name: benefit statement. Experience described.)

Now write a description for our "Automated Reporting" feature.
```

Most consistent results.

---

## Real-World Examples

### Example 1: Executive Summary

**Without context:**
```
Summarize this report.
```

**With context:**
```
Context:
- Audience: Executive team (CEO, CFO, COO) - very busy, need quick insights
- Purpose: Monthly business review, they make strategic decisions based on this
- Background: Last month we launched new product, expanded to new region
- Focus: What's working, what's not, what needs attention

Summarize this 20-page operational report as a 1-page executive summary.
Highlight: revenue trends, new product performance, regional expansion results,
and any red flags requiring immediate action.

Report: [paste report]
```

### Example 2: Customer Email

**Without context:**
```
Write a response to this customer.
```

**With context:**
```
Context:
- Customer: Premium subscriber for 2 years, generally happy
- Issue: Experienced service outage during critical presentation
- Our fault: Yes, server issue on our end, now resolved
- Relationship: Want to maintain, they're a good customer
- Company policy: Can offer 1 month credit for significant issues

Write an empathetic response that:
- Acknowledges their frustration and our responsibility
- Explains what happened (briefly, not technical)
- States what we've done to prevent recurrence
- Offers 1 month service credit
- Reinforces our commitment to their success

Tone: Genuinely apologetic, professional, solution-focused

Customer email: [paste email]
```

### Example 3: Presentation Content

**Without context:**
```
Create slides about our product.
```

**With context:**
```
Context:
- Audience: Potential enterprise clients (IT directors, CIOs)
- Their concerns: Security, scalability, integration with existing systems
- Presentation: 20 minutes, followed by Q&A
- Our advantages: Enterprise-grade security, proven scalability, 50+ integrations
- Competition: They're evaluating 2 other vendors
- Goal: Get invited to next round (technical demo)

Create content for 8 slides covering:
1. Problem we solve (their pain points)
2. Our solution overview
3. Security features (their top concern)
4. Scalability proof (case study)
5. Integration capabilities
6. Customer success stories (similar companies)
7. Implementation process
8. Next steps (call to action)

For each slide: title, 3-4 bullet points, suggested visual

Tone: Professional, confident but not arrogant, focused on their needs
```

---

## Context for Different Business Tasks

### Data Analysis

**Essential context:**
- What the data represents
- Time period covered
- Business question to answer
- What decision this supports
- Any known issues with data

**Example:**
```
Context: This is monthly sales data for Q1 2026 across 4 regions.
We're trying to understand why overall sales are flat despite new product launch.
Sales team thinks it's regional variation, marketing thinks it's seasonal.
This analysis will determine where we focus resources in Q2.

Analyze this data to identify: regional performance differences, new product
adoption rates, and any patterns that explain flat overall growth.
```

### Email Drafting

**Essential context:**
- Recipient and relationship
- Purpose of email
- Previous communication
- Desired outcome
- Tone requirements

**Example:**
```
Context: Emailing a prospect we met at a conference 2 weeks ago.
Had good conversation about their challenges with project management.
They seemed interested but didn't commit. Want to follow up without being pushy.
Goal: Get a 30-minute discovery call scheduled.

Draft a follow-up email that references our conversation, offers value
(share relevant case study), and suggests a low-pressure call to explore fit.
```

### Document Creation

**Essential context:**
- Document purpose
- Target readers
- How it will be used
- Required sections
- Formality level

**Example:**
```
Context: Creating a process document for new hires to follow when onboarding clients.
Readers: New account managers with varying experience levels.
Use: Step-by-step reference during their first few client onboardings.
Must be: Clear, comprehensive, but not overwhelming.
Company style: Friendly and supportive, not rigid corporate.

Create a client onboarding process document with: overview, step-by-step
procedure, common issues and solutions, and resources/contacts.
```

---

## Common Context Mistakes

### 1. Assuming AI Knows Your Situation

❌ "Write the usual update"
✅ "Write our weekly project status update for stakeholders: progress, blockers, next steps"

### 2. Including Irrelevant Details

❌ "I'm writing this on my laptop in the office on a Tuesday afternoon..."
✅ Focus on context that affects the output

### 3. Forgetting Audience

❌ "Explain this technical concept"
✅ "Explain this technical concept to non-technical executives who need to approve budget"

### 4. No Purpose Statement

❌ "Analyze this data"
✅ "Analyze this data to determine if we should expand to the West Coast region"

### 5. Missing Relationship Context

❌ "Write an email to John"
✅ "Write an email to John, our long-time client with whom we have a friendly, informal relationship"

---

## Context Checklist

Before submitting a prompt, verify you've included:

- [ ] **Audience**: Who is this for? What's their knowledge level?
- [ ] **Purpose**: Why are you creating this? What's the goal?
- [ ] **Background**: What situation led to this need?
- [ ] **Constraints**: Any limitations or requirements?
- [ ] **Tone/Style**: How should this sound?
- [ ] **Desired outcome**: What should happen as a result?

---

## Key Takeaways

1. **Context shapes output** - Same task, different context = different results
2. **Include what matters** - Audience, purpose, background, constraints
3. **Examples teach patterns** - Show AI what you want
4. **Balance is key** - Enough context, not too much
5. **Structure helps** - Organize context clearly

---

## What's Next

You now understand how to provide effective context and use examples!

**Next Steps:**
1. Complete [Lab 5](lab.md) to practice context and examples
2. Experiment with different amounts of context
3. Build a library of examples for your common tasks

In **Chapter 6**, we'll learn how to separate instructions from data for cleaner, more effective prompts.

---

## Navigation

- **Previous**: [Chapter 4: Role Assignment and Persona](../04-role-persona/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 6: Separating Instructions from Data](../06-instructions-data/lesson.md)
- **Lab**: [Lab 5: Context and Examples Exercises](lab.md)

---

**Chapter 5 Complete!** Ready to practice? → [Start Lab 5](lab.md)
