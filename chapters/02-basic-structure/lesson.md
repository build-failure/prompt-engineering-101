# Chapter 2: Basic Prompt Structure

← [Previous: Chapter 1 - Introduction](../01-introduction/lesson.md) | [Home](../../README.md) | [Next: Chapter 3 - Clarity and Specificity →](../03-clarity-specificity/lesson.md)

---

## Overview

**Level:** Beginner  
**Duration:** 25 minutes  
**Prerequisites:** Chapter 1 - Introduction to Prompt Engineering

## Learning Objectives

By the end of this chapter, you will:
- Understand the TCFC framework for structuring prompts
- Identify the four key components in any prompt
- Apply the framework to common business tasks
- Write well-structured prompts consistently

---

## The TCFC Framework

In Chapter 1, you learned that good prompts include specific elements. Now we'll give you a systematic framework to structure any prompt: **TCFC**.

**TCFC stands for:**
- **T** = Task
- **C** = Context
- **F** = Format
- **C** = Constraints

Think of TCFC as a checklist. Every time you write a prompt, ask yourself: "Have I included all four elements?"

---

## T = Task (What to Do)

The **Task** is the action you want Gemini to perform. It should be clear and specific.

### Common Task Verbs

- **Create/Generate**: Draft, write, compose, create, generate
- **Transform**: Summarize, condense, expand, rewrite, translate
- **Analyze**: Analyze, evaluate, compare, identify, assess
- **Organize**: Structure, categorize, prioritize, sort, list
- **Respond**: Reply, answer, address, respond

### Examples

**Clear Tasks:**
- ✅ "Draft a follow-up email"
- ✅ "Summarize this quarterly report"
- ✅ "Analyze this sales data"
- ✅ "Create a meeting agenda"

**Unclear Tasks:**
- ❌ "Help with this"
- ❌ "Do something"
- ❌ "Look at this"

### Task Clarity Matters

**Vague:** "Write something about the project"
**Clear:** "Draft a project status update email"

**Vague:** "Deal with this data"
**Clear:** "Analyze this sales data and identify trends"

---

## C = Context (Background Information)

**Context** provides the background Gemini needs to help you effectively. Without context, Gemini can't tailor the output to your specific situation.

### Types of Context

**1. Audience Context**
Who will read or use this?
- "For my manager"
- "For a client presentation"
- "For team members"
- "For executive review"

**2. Situational Context**
What's the situation or background?
- "We met yesterday to discuss..."
- "This is a follow-up to..."
- "The project is behind schedule because..."
- "Our customer complained about..."

**3. Purpose Context**
Why are you creating this?
- "To inform stakeholders of progress"
- "To request approval for budget"
- "To respond to a customer inquiry"
- "To prepare for next week's meeting"

**4. Relationship Context**
What's your relationship to the audience?
- "Long-term client"
- "New prospect"
- "Direct reports"
- "Senior leadership"

### Context Examples

**Without Context:**
```
Summarize this report.
```

**With Context:**
```
Summarize this quarterly financial report for our board of directors
who need to understand revenue trends and any budget concerns before
tomorrow's meeting.
```

**Why it matters:** The board version will focus on high-level trends and strategic implications, while a team version might focus on operational details.

---

## F = Format (How to Structure)

**Format** tells Gemini how to organize and present the information. Without format guidance, you'll get unpredictable structure.


### Common Formats

**Email Formats:**
- Professional email with subject line
- Brief update (3 paragraphs)
- Formal business letter format

**List Formats:**
- Numbered list
- Bullet points
- Checklist with checkboxes
- Prioritized list (high/medium/low)

**Document Formats:**
- Executive summary (overview + key points)
- Report with sections (intro, findings, recommendations)
- Memo format (To/From/Date/Subject)
- Agenda with time allocations

**Data Formats:**
- Table with columns
- Paragraph followed by bullet points
- Summary statistics with examples
- Comparison chart

### Format Examples

**No Format Guidance:**
```
Tell me about the sales data.
```
*Result: Unpredictable structure*

**With Format:**
```
Analyze the sales data and present as:
1. Brief overview paragraph (2-3 sentences)
2. Top 5 findings as bullet points
3. Table showing top 3 products with numbers
```
*Result: Consistent, usable structure*

---

## C = Constraints (Requirements & Limits)

**Constraints** define the boundaries and requirements for your output. They ensure the result fits your needs.

### Types of Constraints

**1. Length Constraints**
- "Maximum 200 words"
- "3-5 bullet points"
- "One page"
- "Brief (under 100 words)"

**2. Tone Constraints**
- "Professional and formal"
- "Friendly but professional"
- "Empathetic and apologetic"
- "Enthusiastic and positive"
- "Direct and matter-of-fact"

**3. Content Constraints**
- "Focus only on Q4 results"
- "Don't mention pricing"
- "Include specific examples"
- "Avoid technical jargon"

**4. Style Constraints**
- "Use active voice"
- "Write in first person"
- "Use simple language"
- "Include specific numbers"

**5. Time Constraints**
- "For a 5-minute presentation"
- "Quick read (2 minutes)"
- "Detailed analysis"

### Constraint Examples

**Without Constraints:**
```
Write an email about the delay.
```
*Result: Could be any length, any tone, any content*

**With Constraints:**
```
Write an email about the delay.
- Maximum 150 words
- Apologetic but solution-focused tone
- Include new deadline and reason
- Don't go into technical details
```
*Result: Fits your exact needs*

---

## Putting TCFC Together

Let's see how all four elements work together.

### Example 1: Email Thread Summarization

**Without TCFC:**
```
Summarize these emails.
```

**With TCFC:**
```
**Task**: Summarize this email thread

**Context**: This is a 15-message thread between our team and
a client about website requirements. I need to brief my manager
who wasn't included in the conversation.

**Format**: Present as:
- 2-sentence overview
- Key requirements (bullet points)
- Decisions made (bullet points)
- Next steps with owners

**Constraints**:
- Maximum 300 words
- Professional tone
- Focus on decisions and actions, not discussion details
```

### Example 2: Status Report

**Without TCFC:**
```
Create a status report.
```

**With TCFC:**
```
**Task**: Create a weekly project status report

**Context**: Website redesign project, week 6 of 12. Reporting
to project stakeholders who need to know if we're on track.

**Format**: Use this structure:
- Executive summary (2-3 sentences)
- Progress this week (3-4 bullets)
- Upcoming milestones (bullets)
- Risks or blockers (if any)
- Overall status: On Track / At Risk / Behind

**Constraints**:
- One page maximum
- Professional tone
- Highlight any risks prominently
- Include specific completion percentages
```

### Example 3: Meeting Agenda

**Without TCFC:**
```
Make a meeting agenda.
```

**With TCFC:**
```
**Task**: Create a meeting agenda

**Context**: Quarterly planning meeting with department heads
(8 people, 90 minutes). Need to review Q3 results and plan Q4
priorities.

**Format**:
- Meeting header (date, time, attendees, location)
- Agenda items with time allocations
- Each item shows: topic, owner, duration
- Include 10 minutes for Q&A at end

**Constraints**:
- Total time must equal 90 minutes
- Professional format
- Prioritize most important items first
- Leave buffer time between major topics
```

---

## The TCFC Checklist

Before submitting any prompt, check:

- [ ] **Task**: Is it clear what I want Gemini to do?
- [ ] **Context**: Have I provided necessary background?
- [ ] **Format**: Have I specified how to structure the output?
- [ ] **Constraints**: Have I defined length, tone, and requirements?

**Pro Tip:** You don't always need to label them as T/C/F/C in your prompt. Just make sure all four elements are present!

---

## Common TCFC Mistakes

### Mistake 1: Task Without Context

❌ **Missing Context:**
```
Draft an email to the client.
```

✅ **With Context:**
```
Draft an email to our client ABC Corp, following up on yesterday's
meeting where we discussed their concerns about project timeline.
```

### Mistake 2: Context Without Format

❌ **Missing Format:**
```
Analyze this sales data from Q3. We need to present findings
to the executive team next week.
```

✅ **With Format:**
```
Analyze this Q3 sales data for executive presentation. Format as:
1) Executive summary paragraph, 2) Top 5 insights as bullets,
3) Recommendations table.
```

### Mistake 3: Format Without Constraints

❌ **Missing Constraints:**
```
Summarize this report as bullet points.
```

✅ **With Constraints:**
```
Summarize this report as 5-7 bullet points, maximum 200 words total,
focusing on actionable insights. Professional tone for manager review.
```

### Mistake 4: Everything Except Task

❌ **Missing Clear Task:**
```
This is a customer complaint about late delivery. We value this
customer and want to maintain the relationship. Keep it professional.
```

✅ **With Clear Task:**
```
Draft an apology email to this customer about their late delivery.
We value this long-term customer and want to maintain the relationship.
Include: apology, explanation, compensation offer (10% discount),
assurance it won't happen again. Professional and empathetic tone,
maximum 200 words.
```

---

## TCFC for Different Business Tasks

### Gmail: Email Thread Summarization

**Task**: Summarize this email thread  
**Context**: 20-message thread about project requirements, need to brief new team member  
**Format**: Overview + key points + decisions + action items (all as bullets)  
**Constraints**: Maximum 250 words, focus on outcomes not discussion

### Google Docs: Executive Summary

**Task**: Create an executive summary  
**Context**: From this 10-page quarterly report, for C-level review  
**Format**: 1 page: overview paragraph + key metrics table + 3-5 strategic recommendations  
**Constraints**: Maximum 400 words, focus on strategic implications, highlight risks

### Google Sheets: Data Analysis

**Task**: Analyze this sales data  
**Context**: Monthly sales by region and product, need to identify trends for planning meeting  
**Format**: Brief paragraph + table of top/bottom performers + 3-5 insight bullets  
**Constraints**: Include specific numbers, focus on actionable insights, professional tone

### Google Slides: Presentation Outline

**Task**: Create a presentation outline  
**Context**: 30-minute presentation on Q4 marketing strategy for leadership team  
**Format**: Slide-by-slide outline with titles and 3-4 bullets per slide  
**Constraints**: 10-12 slides total, start with executive summary, end with clear recommendations

### Google Meet: Meeting Agenda

**Task**: Create a meeting agenda  
**Context**: Project kickoff with cross-functional team (10 people, 60 minutes)  
**Format**: Header info + agenda items with time allocations + objectives for each item  
**Constraints**: Total 60 minutes, include 5-minute buffer, prioritize critical items first

---

## Practice: Identify TCFC Components

Let's practice identifying the four components in complete prompts.

### Example Prompt

```
Draft a professional email to Sarah Johnson, our client at TechCorp,
thanking her for yesterday's productive meeting about the website
redesign project. Summarize the three main requirements she mentioned:
mobile-first design, faster load times, and improved SEO. Confirm
our next meeting on Friday at 2pm and mention that I'll send a
detailed proposal by Thursday. Keep it friendly but professional,
maximum 200 words, formatted as a standard business email.
```

### Identify the Components

**Task**: Draft a professional email

**Context**: 
- Recipient: Sarah Johnson at TechCorp (client)
- Situation: Follow-up to yesterday's meeting
- Topic: Website redesign project
- Relationship: Client relationship

**Format**: Standard business email

**Constraints**:
- Tone: Friendly but professional
- Length: Maximum 200 words
- Content: Thank you, 3 requirements, meeting confirmation, proposal timeline

---

## When to Emphasize Each Component

### Emphasize TASK when:
- The action isn't obvious
- Multiple actions are possible
- You need a specific type of output

### Emphasize CONTEXT when:
- Audience matters significantly
- Background is complex
- Relationship affects tone
- Purpose isn't obvious

### Emphasize FORMAT when:
- Structure is critical
- Output will be used in specific way
- Consistency matters
- Multiple sections needed

### Emphasize CONSTRAINTS when:
- Length is critical
- Tone must be specific
- Content boundaries matter
- Style requirements exist

**Remember:** All four are important, but some situations require more detail in certain areas.

---

## Building Your TCFC Muscle

### Start with the Template

```
**Task**: [What do you want Gemini to do?]

**Context**: [Who is this for? What's the situation? Why does it matter?]

**Format**: [How should it be structured?]

**Constraints**: [Length? Tone? Requirements? Limitations?]
```

### Then Write Naturally

Once you're comfortable, you don't need to label each section. Just ensure all four elements are present:

```
Draft a follow-up email to Jennifer Martinez at TechStart Inc.
We met yesterday to discuss their CRM needs, covering integration
requirements, team training, and pricing. Thank her for the meeting,
summarize those three topics briefly, and confirm I'll send a
detailed proposal by Friday. Keep it professional but warm,
maximum 200 words.
```

*All four elements are there, just written naturally!*

---

## TCFC Quick Reference

| Component | Key Question | Examples |
|-----------|-------------|----------|
| **Task** | What action? | Draft, summarize, analyze, create, compare |
| **Context** | What background? | Audience, situation, purpose, relationship |
| **Format** | What structure? | Email, bullets, table, report, agenda |
| **Constraints** | What limits? | Length, tone, content focus, style |

---

## Real-World TCFC Examples

### Example 1: Customer Service Response

```
Draft a customer service email responding to John Smith's complaint
about his delayed order (#12345). He's a long-term customer (5 years)
who is understandably frustrated. Apologize sincerely, explain the
delay was due to unexpected supply chain issues, provide the new
delivery date (next Tuesday), and offer a 15% discount on his next
order as compensation. Format as a professional email with subject
line. Keep it empathetic and solution-focused, maximum 250 words.
```

**TCFC Breakdown:**
- **T**: Draft customer service email
- **C**: Delayed order, long-term customer, frustrated, supply chain issue
- **F**: Professional email with subject line
- **C**: Empathetic tone, solution-focused, 250 words max, include apology/explanation/solution/compensation

### Example 2: Weekly Status Report

```
Create a weekly status report for the mobile app development project.
This is week 8 of 16, reporting to the project steering committee
who meets monthly. Summarize progress on the three main features
(user authentication, payment integration, push notifications),
note that payment integration is 2 weeks behind due to API issues,
and outline next week's priorities. Format as: Executive summary
(2-3 sentences), Progress by feature (table), Risks/Issues (bullets),
Next week's focus (bullets). Professional tone, one page maximum,
highlight the payment delay prominently.
```

**TCFC Breakdown:**
- **T**: Create weekly status report
- **C**: Mobile app project, week 8/16, steering committee audience, payment integration delayed
- **F**: Executive summary + progress table + risk bullets + next week bullets
- **C**: Professional tone, one page, highlight delay, specific features to cover

### Example 3: Meeting Agenda from Objectives

```
Create a meeting agenda for our Q4 planning session with the
marketing team (6 people, 2 hours). We need to: review Q3 campaign
performance, brainstorm Q4 campaign ideas, allocate budget across
channels, and assign ownership for each campaign. Format with
meeting header (date: Oct 15, time: 2-4pm, location: Conference Room B),
then agenda items with time allocations and objectives for each.
Include a 10-minute break at the midpoint and 15 minutes for Q&A
at the end. Professional format, ensure time allocations total
exactly 2 hours.
```

**TCFC Breakdown:**
- **T**: Create meeting agenda
- **C**: Q4 planning, marketing team, 6 people, 2 hours, four main objectives
- **F**: Header + agenda items with times and objectives + break + Q&A
- **C**: Professional format, exactly 2 hours total, 10-min break, 15-min Q&A

---

## Key Principles to Remember

### 1. All Four Elements Matter
Missing any component reduces output quality. Check for T, C, F, and C every time.

### 2. Context is Often Underused
Most people forget context. Adding "for my manager" or "for a client presentation" dramatically improves results.

### 3. Format Prevents Surprises
Specifying format ensures you get usable structure, not random organization.

### 4. Constraints Keep It Focused
Length and tone constraints ensure the output fits your actual needs.

### 5. Practice Makes Perfect
The more you use TCFC, the more natural it becomes. Soon you'll do it automatically.

---

## What You've Learned

Congratulations! You now understand:

- ✅ The TCFC framework (Task, Context, Format, Constraints)
- ✅ How to identify each component in prompts
- ✅ Why each element matters for output quality
- ✅ How to apply TCFC to common business tasks
- ✅ How to write naturally while including all four elements

---

## What's Next

Ready to go deeper? In **Chapter 3**, you'll learn about **Clarity and Specificity** — how to be specific without being verbose, and how to avoid vague language that confuses Gemini.

**Next Steps:**
1. Complete [Lab 2](lab.md) to practice applying the TCFC framework
2. Try restructuring some of your existing prompts using TCFC
3. Notice how adding context and format improves your results

---

## Navigation

- **Previous**: [Chapter 1: Introduction](../01-introduction/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 3: Clarity and Specificity](../03-clarity-specificity/lesson.md)
- **Lab**: [Lab 2: Basic Structure Exercises](lab.md)

---

**Chapter 2 Complete!** Ready to practice the TCFC framework? → [Start Lab 2](lab.md)
