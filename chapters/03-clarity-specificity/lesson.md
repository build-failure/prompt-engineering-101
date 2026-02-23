# Chapter 3: Clarity and Specificity

← [Previous: Chapter 2 - Basic Prompt Structure](../02-basic-structure/lesson.md) | [Home](../../README.md) | [Next: Chapter 4 - Role Assignment →](../04-role-persona/lesson.md)

---

## Overview

**Level:** Beginner  
**Duration:** 25 minutes  
**Prerequisites:** Chapters 1-2

## Learning Objectives

- Learn how to be specific without being verbose
- Understand the impact of vague language on AI outputs
- Master techniques for adding helpful detail
- Balance specificity with flexibility

---

## The Specificity Spectrum

```
Too Vague ←→ Just Right ←→ Too Rigid
```

### Too Vague
```
Analyze the data
```
Problem: AI doesn't know what data, what analysis, or what format.

### Just Right
```
Analyze this Q1 sales data to identify the top 3 performing product categories
and any declining trends. Present as a brief summary with key metrics.
```
Sweet spot: Clear task, specific focus, defined output.

### Too Rigid
```
Analyze rows 1-47 of the attached spreadsheet, calculate the sum of column C,
divide by column D, multiply by 1.5, then create exactly 3 sentences each
containing exactly 15 words describing the result using only these words: [list]
```
Problem: Over-constrained, inflexible, hard to get useful results.

---

## Vague Words to Avoid

### Replace Vague Terms with Specific Ones

| Vague | Specific |
|-------|----------|
| "Some information" | "The project timeline, budget, and key milestones" |
| "Soon" | "By end of day Friday" or "Within 2 business days" |
| "A few" | "3-5 examples" or "Approximately 10 items" |
| "Good quality" | "Professional tone, error-free, with specific examples" |
| "Brief" | "Maximum 200 words" or "2-3 paragraphs" |
| "Important points" | "Revenue trends, cost concerns, and growth opportunities" |
| "Nice format" | "Bullet-point list with headers and subpoints" |
| "Professional" | "Formal business tone, suitable for executive review" |

---

## Techniques for Adding Helpful Detail

### 1. Specify Quantities

❌ "List some competitors"
✅ "List our top 5 direct competitors in the B2B SaaS space"

❌ "Summarize briefly"
✅ "Summarize in exactly 3 bullet points, maximum 50 words each"

### 2. Define Scope

❌ "Analyze sales performance"
✅ "Analyze Q1 2026 sales performance for the North American region only"

❌ "Review this document"
✅ "Review this document for grammar errors, clarity issues, and tone consistency"

### 3. Clarify Purpose

❌ "Write about our product"
✅ "Write a product description for our website homepage to attract small business owners"

❌ "Explain the process"
✅ "Explain the onboarding process to new employees in simple, step-by-step terms"

### 4. Specify Audience

❌ "Create a summary"
✅ "Create a summary for non-technical executives who need to make a budget decision"

❌ "Draft an email"
✅ "Draft an email to a frustrated customer who needs reassurance and a clear solution"

### 5. Define Success Criteria

❌ "Make it better"
✅ "Improve clarity by: simplifying complex sentences, adding transition words, and removing jargon"

❌ "Analyze this"
✅ "Identify: 1) Top 3 trends, 2) Any anomalies, 3) Actionable recommendations"

---

## Real-World Examples

### Example 1: Data Analysis

**Vague:**
```
Look at the sales numbers
```

**Specific:**
```
Analyze the monthly sales data for Q1 2026 (January-March).
Identify:
- Which product category had the highest growth
- Any months with declining sales
- Regional performance differences

Present findings as a brief executive summary with specific percentages.
```

### Example 2: Email Drafting

**Vague:**
```
Write a follow-up email
```

**Specific:**
```
Draft a follow-up email to Maria Santos, the procurement manager at TechCorp,
three days after our product demo. Thank her for her time, reference her
specific interest in our automation features, and propose a 30-minute call
next week to discuss pricing for 100 users. Tone: professional but warm,
2-3 paragraphs maximum.
```

### Example 3: Document Summarization

**Vague:**
```
Summarize this report
```

**Specific:**
```
Summarize this 25-page market research report for our marketing team.
Focus on: target customer demographics, competitor positioning, and
market opportunities. Ignore the methodology section. Format as 5-7
bullet points, each with a brief explanation. Maximum 300 words total.
```

---

## When to Be Specific vs. Flexible

### Be Specific About:

✅ **Quantities**: Word counts, number of items, data ranges
✅ **Scope**: Time periods, geographic regions, specific topics
✅ **Format**: Structure, organization, presentation style
✅ **Audience**: Who will read/use this, their knowledge level
✅ **Purpose**: Why you're creating this, what decision it supports
✅ **Constraints**: What to include/exclude, tone, length

### Stay Flexible About:

✅ **Exact wording**: Let AI choose natural phrasing
✅ **Creative elements**: Allow AI to suggest approaches
✅ **Examples**: AI can generate relevant examples
✅ **Organization details**: Trust AI for logical flow
✅ **Style variations**: Within your specified tone

---

## The "5 W's" Technique

Use journalism's 5 W's to add specificity:

### Who?
- Who is this for?
- Who is involved?
- Who will use this?

### What?
- What exactly do you need?
- What should be included/excluded?
- What format?

### When?
- What time period?
- What deadline?
- What sequence?

### Where?
- What location/region?
- What platform/medium?
- What context?

### Why?
- What's the purpose?
- What decision does this support?
- What problem does this solve?

**Example Application:**
```
[WHO] Draft an email to our enterprise clients
[WHAT] announcing our new security features
[WHEN] for immediate distribution this week
[WHERE] via our monthly newsletter
[WHY] to reduce churn and highlight our commitment to data protection

Format: Newsletter section, 150-200 words, professional but enthusiastic tone
```

---

## Common Clarity Mistakes

### 1. Assuming Context

❌ "Summarize the usual way"
✅ "Summarize as we do for board meetings: executive summary paragraph + 3-5 key points + recommendations"

### 2. Using Jargon Without Definition

❌ "Analyze the KPIs"
✅ "Analyze these key performance indicators: customer acquisition cost (CAC), lifetime value (LTV), and churn rate"

### 3. Ambiguous Pronouns

❌ "Review it and make it better"
✅ "Review this proposal and improve: clarity of value proposition, strength of call-to-action, and professional tone"

### 4. Unclear Comparisons

❌ "Compare them"
✅ "Compare Product A vs. Product B on: price, features, target market, and customer reviews"

### 5. Vague Timeframes

❌ "Recent data"
✅ "Data from the past 3 months (December 2025 - February 2026)"

---

## Specificity Checklist

Before submitting a prompt, ask:

- [ ] Have I specified exact quantities (word count, number of items)?
- [ ] Is the time period/scope clear?
- [ ] Have I defined the audience?
- [ ] Is the purpose explicit?
- [ ] Have I specified the format/structure?
- [ ] Are there any vague words I should replace?
- [ ] Would someone else understand exactly what I want?

---

## Practice: Adding Specificity

### Transform These Vague Prompts

**Vague Prompt 1:**
```
Write about the meeting
```

**Add Specificity:**
- What meeting? (Project kickoff, client review, team standup?)
- What about it? (Summary, agenda, follow-up?)
- For whom? (Attendees, absent colleagues, manager?)
- What format? (Email, document, bullet points?)
- How long? (Word count, paragraph count?)

**Vague Prompt 2:**
```
Analyze customer feedback
```

**Add Specificity:**
- What feedback? (Survey, reviews, support tickets?)
- What time period? (Last month, Q1, past year?)
- What analysis? (Sentiment, themes, trends?)
- What output? (Report, summary, recommendations?)
- What focus? (Product issues, service quality, feature requests?)

---

## Key Takeaways

1. **Specificity improves results** — Clear prompts get better outputs
2. **Avoid vague language** — Replace "some," "good," "brief" with exact terms
3. **Use the 5 W's** — Who, What, When, Where, Why
4. **Balance is key** — Specific enough to guide, flexible enough to allow quality
5. **Check before submitting** — Review for vague terms and ambiguity

---

## What's Next

You now know how to write clear, specific prompts that get exactly what you need!

**Next Steps:**
1. Complete [Lab 3](lab.md) to practice clarity and specificity
2. Review your recent prompts and add specificity
3. Build a list of your commonly used specific terms

In **Chapter 4**, we'll explore role assignment and personas — how to get AI to adopt specific expertise and perspectives.

---

## Navigation

- **Previous**: [Chapter 2: Basic Prompt Structure](../02-basic-structure/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 4: Role Assignment and Persona](../04-role-persona/lesson.md)
- **Lab**: [Lab 3: Clarity and Specificity Exercises](lab.md)

---

**Chapter 3 Complete!** Ready to practice? → [Start Lab 3](lab.md)
