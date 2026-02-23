# Chapter 11: Multi-Step Workflows and Prompt Chaining

← [Previous: Chapter 10 - Accuracy and Hallucinations](../10-accuracy-hallucinations/lesson.md) | [Home](../../README.md) | [Next: Chapter 12 - Troubleshooting →](../12-troubleshooting/lesson.md)

---

## Overview

**Level:** Advanced  
**Duration:** 35 minutes  
**Prerequisites:** Chapters 1-10

## Learning Objectives

- Understand when to break tasks into multiple prompts
- Learn prompt chaining strategies
- Master workflow design patterns
- Apply multi-step approaches to complex business tasks

---

## When One Prompt Isn't Enough

Some tasks are too complex for a single prompt. Signs you need multiple steps:

### Complexity Indicators

**Break into steps when:**
- ✅ Task has multiple distinct phases
- ✅ Each phase requires different expertise
- ✅ Output from one step informs the next
- ✅ Quality improves with iteration
- ✅ You need to review intermediate results

**Examples:**
- Research → Analysis → Recommendations → Action Plan
- Data → Insights → Presentation → Email Announcement
- Draft → Review → Revise → Finalize
- Brainstorm → Evaluate → Select → Implement

---

## Prompt Chaining Basics

**Prompt chaining:** Using the output of one prompt as input for the next.

### Simple Chain Example

**Step 1: Extract**
```
Extract the key points from this meeting transcript:
[paste transcript]

Format as bullet points.
```

**Step 2: Organize**
```
Organize these meeting points into categories:
[paste Step 1 output]

Categories: Decisions, Action Items, Discussion Topics, Next Steps
```

**Step 3: Communicate**
```
Create an email summary from these organized points:
[paste Step 2 output]

Audience: Team members who missed the meeting
Tone: Professional but friendly
Length: 200 words maximum
```

---

## Workflow Patterns

### 1. Sequential Pattern

Each step builds on the previous:

```
Step 1 → Step 2 → Step 3 → Final Output
```

**Example: Report Creation**
```
Step 1: "Analyze this data and identify top 3 trends"
Step 2: "For each trend, explain why it's happening"
Step 3: "Based on these trends, provide 3 recommendations"
Step 4: "Create an executive summary combining all insights"
```

### 2. Iterative Pattern

Refine through multiple passes:

```
Draft → Review → Revise → Review → Finalize
```

**Example: Document Refinement**
```
Step 1: "Draft a proposal for [project]"
Step 2: "Review this draft for clarity and persuasiveness"
Step 3: "Revise the draft based on this feedback: [paste review]"
Step 4: "Final polish: check grammar, tone, and formatting"
```

### 3. Branching Pattern

One input, multiple parallel outputs:

```
        → Output A
Input → → Output B
        → Output C
```

**Example: Multi-Audience Communication**
```
Source: Quarterly results data

Branch 1: "Create executive summary for board"
Branch 2: "Create team announcement for employees"
Branch 3: "Create customer-facing update"
```

### 4. Convergent Pattern

Multiple inputs combine into one output:

```
Input A →
Input B → → Combined Output
Input C →
```

**Example: Comprehensive Analysis**
```
Input 1: Customer feedback
Input 2: Sales data
Input 3: Market research

Combine: "Synthesize insights from all three sources into strategic recommendations"
```

---

## Designing Effective Workflows

### Step 1: Map the Process

**Identify phases:**
1. What's the end goal?
2. What are the major steps to get there?
3. What's the logical order?
4. Where do you need to review/decide?

**Example: Product Launch Announcement**
```
Goal: Announce new product to customers

Phases:
1. Identify key messages
2. Draft announcement
3. Create FAQ
4. Write email version
5. Create social media posts
```

### Step 2: Define Each Prompt

**For each step, specify:**
- Input (what you're starting with)
- Task (what to do)
- Output (what you need)
- Format (how to structure it)

**Example:**
```
Step 1: Key Messages
Input: Product features and benefits
Task: Identify 3 key messages for customers
Output: 3 compelling messages with supporting points
Format: Bullet list with explanations

Step 2: Draft Announcement
Input: 3 key messages from Step 1
Task: Write announcement email
Output: Complete email draft
Format: Subject line + 3-4 paragraphs
```

### Step 3: Plan Handoffs

**Between steps:**
- What information passes forward?
- What gets left behind?
- Do you need to review before continuing?
- Can steps run in parallel?

---

## Real-World Workflows

### Workflow 1: Data Analysis → Presentation

**Goal:** Turn raw data into executive presentation

```
Step 1: Data Summary
"Summarize this sales data:
- Total revenue
- Top 3 products
- Best performing region
- Notable trends

Data: [paste data]"

Step 2: Insights Generation
"Based on this summary, identify:
- What's working well (and why)
- What needs attention (and why)
- Opportunities to pursue

Summary: [paste Step 1 output]"

Step 3: Presentation Outline
"Create a 10-slide presentation outline:
- Slide 1: Title
- Slides 2-4: Key findings (one per slide)
- Slides 5-7: Insights and implications
- Slides 8-9: Recommendations
- Slide 10: Next steps

Content: [paste Step 2 output]"

Step 4: Slide Content
"For each slide in this outline, create:
- Slide title (compelling, not generic)
- 3-4 bullet points
- Key visual suggestion

Outline: [paste Step 3 output]"

Step 5: Speaker Notes
"Create speaker notes for each slide:
- What to say (conversational)
- Key points to emphasize
- Potential questions to address

Slides: [paste Step 4 output]"
```

### Workflow 2: Customer Feedback → Action Plan

**Goal:** Turn feedback into prioritized improvements

```
Step 1: Categorize Feedback
"Categorize this customer feedback into themes.
For each theme, count frequency.

Feedback: [paste all feedback]"

Step 2: Identify Priorities
"Based on these themes, identify top 3 priorities considering:
- Frequency (how many customers mentioned it)
- Impact (how much it affects satisfaction)
- Feasibility (how easy to address)

Themes: [paste Step 1 output]"

Step 3: Generate Solutions
"For each priority, brainstorm 3-5 potential solutions.
Consider quick wins and long-term fixes.

Priorities: [paste Step 2 output]"

Step 4: Evaluate Solutions
"Evaluate each solution on:
- Effort required (low/medium/high)
- Expected impact (low/medium/high)
- Timeline (quick/moderate/long-term)

Solutions: [paste Step 3 output]"

Step 5: Create Action Plan
"Create an action plan with:
- Priority 1: [solution], owner, timeline, success metrics
- Priority 2: [solution], owner, timeline, success metrics
- Priority 3: [solution], owner, timeline, success metrics

Evaluated solutions: [paste Step 4 output]"
```

### Workflow 3: Meeting → Documentation → Communication

**Goal:** From meeting to team communication

```
Step 1: Extract Structure
"From these meeting notes, extract:
- Decisions made (with rationale)
- Action items (with owners and deadlines)
- Open questions
- Next meeting date

Notes: [paste raw notes]"

Step 2: Create Meeting Minutes
"Format these as formal meeting minutes:
- Meeting details (date, attendees, purpose)
- Discussion summary
- Decisions
- Action items
- Next steps

Extracted info: [paste Step 1 output]"

Step 3: Action Item Tracker
"Create an action item tracker table:
| Task | Owner | Deadline | Status | Priority |

From: [paste Step 2 output]"

Step 4: Team Email
"Draft a team email with:
- Brief meeting summary
- Key decisions
- Action items (with owners)
- What team members need to do

Source: [paste Step 2 output]
Tone: Professional but friendly
Length: 250 words max"
```

---

## Managing Context Across Steps

### What to Pass Forward

**Include:**
- ✅ Essential information for next step
- ✅ Decisions made
- ✅ Key outputs
- ✅ Relevant context

**Exclude:**
- ❌ Unnecessary details
- ❌ Intermediate working
- ❌ Redundant information
- ❌ Irrelevant context

### Context Management Example

```
Step 1 Output (Full):
"Analysis of Q1 data shows:
- Revenue: $2.3M (up 15%)
- Customers: 450 (up 12%)
- Churn: 3.2% (down from 4.1%)
- Top product: Enterprise (60% of revenue)
- Regional breakdown: North 45%, South 30%, West 25%
- Monthly trend: Jan $720K, Feb $750K, Mar $830K
[... more details ...]"

Step 2 Input (Curated):
"Based on Q1 performance:
- Revenue grew 15% to $2.3M
- Customer base grew 12% to 450
- Churn improved to 3.2%
- Enterprise product dominates (60%)

Create recommendations for Q2 strategy."
```

---

## Quality Control in Workflows

### Review Points

**Insert reviews:**
- After critical analysis steps
- Before final outputs
- When direction might change
- Before committing resources

**Review Prompt Example:**
```
Review this analysis before we proceed:

[paste intermediate output]

Check for:
- Accuracy of facts and figures
- Logic and reasoning
- Completeness
- Any red flags or concerns

Should we proceed or revise?
```

### Validation Steps

**Add validation:**
```
Step N: Generate output
Step N+1: Validate output

"Review this [output type] for:
1. Accuracy
2. Completeness
3. Appropriateness
4. Quality

Flag any issues before we continue."
```

---

## Efficiency Tips

### 1. Template Your Workflows

Create reusable workflow templates:

```
WORKFLOW: Data Analysis to Presentation

Step 1: Summarize data → [template]
Step 2: Generate insights → [template]
Step 3: Create outline → [template]
Step 4: Develop content → [template]
Step 5: Add speaker notes → [template]

Save this sequence for recurring tasks.
```

### 2. Batch Similar Steps

Group related tasks:

```
Instead of:
- Draft email 1
- Draft email 2
- Draft email 3

Do:
- Draft all 3 emails in one prompt
- Then review all 3
- Then finalize all 3
```

### 3. Parallel Processing

Run independent steps simultaneously:

```
From meeting notes, create in parallel:
- Email summary (for team)
- Action item tracker (for PM)
- Executive brief (for leadership)

All use same source, different outputs.
```

---

## Common Workflow Mistakes

### 1. Too Many Steps

❌ **Over-complicated:**
```
Step 1: Extract data
Step 2: Clean data
Step 3: Format data
Step 4: Analyze data
Step 5: Summarize analysis
Step 6: Format summary
Step 7: Review summary
Step 8: Finalize summary
```

✅ **Streamlined:**
```
Step 1: Analyze this data and summarize key findings
Step 2: Review and refine the summary
Step 3: Format for presentation
```

### 2. Losing Context

❌ **Insufficient handoff:**
```
Step 1: "Analyze data" → [output]
Step 2: "Make recommendations"
(Missing: what data, what analysis showed)
```

✅ **Clear handoff:**
```
Step 1: "Analyze data" → [output]
Step 2: "Based on this analysis: [paste output], provide 3 recommendations addressing the identified trends"
```

### 3. No Review Points

❌ **Straight through:**
```
Draft → Revise → Finalize → Send
(No chance to catch errors)
```

✅ **With reviews:**
```
Draft → Review → Revise → Final Review → Send
(Quality checks built in)
```

---

## Workflow Design Checklist

- [ ] Is the end goal clear?
- [ ] Are steps in logical order?
- [ ] Does each step have a clear purpose?
- [ ] Is context passed between steps?
- [ ] Are there review/decision points?
- [ ] Can any steps be combined?
- [ ] Can any steps run in parallel?
- [ ] Is the workflow repeatable?

---

## Key Takeaways

1. **Complex tasks need multiple steps** - Don't force everything into one prompt
2. **Design the workflow first** - Map out steps before starting
3. **Pass context forward** - Each step needs relevant information
4. **Include review points** - Quality control is essential
5. **Template common workflows** - Reuse successful patterns
6. **Iterate and improve** - Refine workflows based on results

---

## What's Next

You now know how to design and execute complex multi-step workflows!

**Next Steps:**
1. Complete [Lab 11](lab.md) to practice workflow design
2. Map out workflows for your complex recurring tasks
3. Create workflow templates for your team

In **Chapter 12**, we'll cover troubleshooting and debugging - how to fix prompts when they don't work as expected.

---

## Navigation

- **Previous**: [Chapter 10: Accuracy and Hallucinations](../10-accuracy-hallucinations/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 12: Troubleshooting and Debugging](../12-troubleshooting/lesson.md)
- **Lab**: [Lab 11: Multi-Step Workflow Exercises](lab.md)

---

**Chapter 11 Complete!** Ready to practice? → [Start Lab 11](lab.md)
