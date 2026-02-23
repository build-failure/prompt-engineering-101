# Lab 2: Basic Prompt Structure

← [Lesson 2](lesson.md) | [Home](../../README.md) | [Next: Lab 3 →](../03-clarity-specificity/lab.md)

---

## Overview

**Chapter**: 2 - Basic Prompt Structure  
**Level**: Beginner  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 2

## Learning Objectives

By completing this lab, you will:
- Apply the TCFC framework to real business scenarios
- Build well-structured prompts consistently
- Identify missing components in prompts
- Create reusable prompt templates

## Business Scenario

You're managing multiple projects and need to communicate effectively with your team, clients, and stakeholders. Today you'll practice structuring prompts using the TCFC framework for common business communications.

## Materials Needed

- Access to Google Gemini
- This lab document
- 30 minutes of focused time

---

## Exercise 1: Identify the TCFC Components

**Objective**: Learn to recognize TCFC elements in existing prompts

**Scenario**: Analyze these prompts and identify which TCFC components are present or missing.

### Prompt A
```
Summarize this quarterly sales report for the executive team.
Focus on revenue trends and regional performance.
Provide 5 bullet points, maximum 150 words.
Use professional language suitable for C-level review.
```

### Prompt B
```
Write an email to the client.
```

### Prompt C
```
Analyze the customer feedback data and identify the top 3 complaints.
Present as a table with: Issue, Frequency, Severity, Recommended Action.
```

### Your Task

For each prompt, identify:
1. Which TCFC components are present?
2. Which are missing?
3. How would you improve it?

### Answers

<details>
<summary>Click to reveal analysis</summary>

**Prompt A - Complete TCFC:**
- ✅ Task: Summarize
- ✅ Context: Quarterly sales report, executive team audience
- ✅ Format: 5 bullet points
- ✅ Constraints: 150 words max, professional language, focus areas

**Prompt B - Missing Most Components:**
- ✅ Task: Write an email
- ❌ Context: No recipient, purpose, or background
- ❌ Format: No structure specified
- ❌ Constraints: No tone, length, or content guidance

**Improvement:**
```
[T] Draft a follow-up email to client ABC Corp
[C] After yesterday's project proposal meeting, thanking them and confirming next steps
[F] Subject line + 3 paragraphs (thanks, summary, next steps)
[C] Professional but warm tone, maximum 200 words
```

**Prompt C - Partial TCFC:**
- ✅ Task: Analyze and identify
- ⚠️ Context: Minimal (what data? what timeframe?)
- ✅ Format: Table with specific columns
- ❌ Constraints: No guidance on data handling or tone

**Improvement:** Add context about data source and timeframe, add constraint about how to prioritize issues.

</details>

### Success Criteria
- [ ] Correctly identified TCFC components in all three prompts
- [ ] Recognized what was missing
- [ ] Understood how to improve incomplete prompts

---

## Exercise 2: Build a TCFC Prompt from Scratch

**Objective**: Create a complete, well-structured prompt using TCFC

**Scenario**: You need to create a weekly status report for your manager about the website redesign project.

### Information Provided

- Project: Website redesign
- Week: Feb 19-23, 2024
- Team: 4 people (2 designers, 1 developer, 1 content writer)
- Progress: Design mockups 80% complete, development 30% complete
- Blocker: Waiting for client feedback on homepage design
- Next week: Finalize designs, start development on 3 key pages
- Manager prefers: Brief, bullet-point format, highlight any risks

### Your Task

Write a complete TCFC prompt that will generate this status report.

### Template to Fill In

```
[TASK] _______________________________________________

[CONTEXT]
- Project: _______________________________________________
- Audience: _______________________________________________
- Purpose: _______________________________________________
- Current situation: _______________________________________________

[FORMAT]
- Structure: _______________________________________________
- Sections: _______________________________________________

[CONSTRAINTS]
- Length: _______________________________________________
- Tone: _______________________________________________
- Focus: _______________________________________________
```

### Example Solution

<details>
<summary>Click to see example prompt</summary>

```
[TASK] Create a weekly project status report for the website redesign project

[CONTEXT]
- Project: Website redesign, week of Feb 19-23, 2024
- Team: 4 people (2 designers, 1 developer, 1 content writer)
- Audience: My manager who oversees multiple projects
- Purpose: Weekly update to track progress and flag issues

[FORMAT]
Structure as:
- Progress This Week (with % complete for each workstream)
- Blockers/Issues (if any)
- Planned for Next Week
- Overall Status: Green/Yellow/Red

[CONSTRAINTS]
- Bullet-point format, maximum 3-5 bullets per section
- Professional but concise tone
- Highlight the client feedback blocker
- Maximum 200 words total
```

</details>

### Validation Prompt

```
I'm practicing the TCFC framework. Please review my prompt:

**Exercise Goal**: Create a weekly status report prompt using TCFC

**My TCFC Prompt**:
[Paste your complete prompt here]

**Output I Received**:
[Paste Gemini's output here]

**Please assess**:
1. Did I include all four TCFC components?
2. Is each component specific enough?
3. Would the output be useful for my manager?
4. What could I improve?
```

### Success Criteria
- [ ] Included all four TCFC components
- [ ] Task is clear and specific
- [ ] Context provides necessary background
- [ ] Format specifies structure clearly
- [ ] Constraints define length, tone, and focus
- [ ] Output is a usable status report

### Troubleshooting

- **Issue**: Output is too long
  **Solution**: Add stricter word count constraint: "Maximum 150 words, no more than 4 bullets per section"

- **Issue**: Missing key information
  **Solution**: Add to context: specific progress numbers, blocker details, team composition

- **Issue**: Wrong tone (too casual or too formal)
  **Solution**: Be explicit in constraints: "Professional tone suitable for manager review, direct and factual"

---

## Exercise 3: Email Thread Summarization

**Objective**: Apply TCFC to a common business task

**Scenario**: You have a long email thread about a client project that you need to summarize for your team.

### Email Thread Context

- Topic: Mobile app feature requests from client
- Participants: You, client contact (Jamie), product manager (Alex)
- Length: 12 emails over 3 days
- Key points: Client wants 3 new features, budget discussion, timeline concerns
- Your need: Summarize for team meeting tomorrow

### Your Task

Write a TCFC prompt to summarize this email thread.

### Prompt Checklist

Before writing, plan each component:

**Task**: What action? (Summarize, extract, condense?)

**Context**: 
- What's being summarized?
- Who needs this summary?
- Why are you creating it?

**Format**:
- How should it be organized?
- What sections?
- What structure?

**Constraints**:
- How long?
- What tone?
- What to emphasize?

### Write Your Prompt

```
[Your TCFC prompt here]
```

### Example Solution

<details>
<summary>Click to see example</summary>

```
[TASK] Summarize this email thread about mobile app feature requests

[CONTEXT]
- 12-email conversation over 3 days between me, client (Jamie), and product manager (Alex)
- Topic: Client requesting new features for mobile app
- Audience: My development team who will implement these features
- Purpose: Brief them before tomorrow's planning meeting

[FORMAT]
Organize as:
- Background (1-2 sentences)
- Requested Features (numbered list with brief description)
- Budget & Timeline Discussion (key points only)
- Decisions Made (bullet list)
- Open Questions (bullet list)

[CONSTRAINTS]
- Maximum 300 words
- Technical team audience - can use technical terms
- Highlight any urgent items
- Focus on actionable information only

Email thread:
[paste emails here]
```

</details>

### Validation Prompt

```
I'm using TCFC to structure an email summarization prompt:

**My Prompt**:
[Paste your prompt]

**Output**:
[Paste Gemini's output]

**Please evaluate**:
1. Does my prompt have complete TCFC structure?
2. Is the summary useful for a team meeting?
3. Did I specify the right format for this use case?
4. What would make this prompt even better?
```

### Success Criteria
- [ ] All TCFC components present and specific
- [ ] Context explains the situation clearly
- [ ] Format appropriate for team briefing
- [ ] Constraints ensure actionable output
- [ ] Summary is ready to use in meeting

---

## Exercise 4: Meeting Agenda Creation

**Objective**: Use TCFC for meeting preparation

**Scenario**: You're organizing a project kickoff meeting and need to create a comprehensive agenda.

### Meeting Details

- Project: Customer portal redesign
- Duration: 90 minutes
- Attendees: Project team (6 people), stakeholders (3 people), client representative
- Goals: Align on objectives, review timeline, assign responsibilities, address concerns
- Your manager wants: Professional agenda sent 2 days before meeting

### Your Task

Create a TCFC prompt to generate this meeting agenda.

### Consider These Questions

1. What specific sections should the agenda include?
2. How should time be allocated?
3. What preparation do attendees need?
4. What tone is appropriate?

### Write Your Prompt

Use the TCFC framework:

```
[TASK] 

[CONTEXT]


[FORMAT]


[CONSTRAINTS]

```

### Example Solution

<details>
<summary>Click to see example</summary>

```
[TASK] Create a comprehensive meeting agenda for a project kickoff meeting

[CONTEXT]
- Project: Customer portal redesign
- Meeting: 90 minutes, 10 attendees (6 team, 3 stakeholders, 1 client)
- Purpose: Align on objectives, review timeline, assign roles, address concerns
- Audience: Mix of technical and non-technical participants
- Timing: Agenda will be sent 2 days before meeting

[FORMAT]
Structure as:
- Meeting Header (title, date, time, location, attendees)
- Meeting Objectives (2-3 key goals)
- Agenda Items (with time allocations and owners)
- Pre-Meeting Preparation (what to review beforehand)
- Expected Outcomes (what we'll accomplish)

[CONSTRAINTS]
- Total time: 90 minutes (include 10-min break)
- Allocate time for Q&A and discussion
- Professional format suitable for client review
- Include time buffer for overruns
- Specify who leads each agenda item
```

</details>

### Validation Prompt

```
I'm creating a meeting agenda using TCFC:

**My Prompt**:
[Paste your prompt]

**Generated Agenda**:
[Paste output]

**Please assess**:
1. Is the TCFC structure complete and clear?
2. Would this agenda help run an effective meeting?
3. Are time allocations realistic?
4. Is it professional enough for client review?
5. What's missing or could be improved?
```

### Success Criteria
- [ ] Complete TCFC structure
- [ ] Agenda covers all meeting goals
- [ ] Time allocations add up to 90 minutes
- [ ] Professional format appropriate for all attendees
- [ ] Includes preparation requirements
- [ ] Ready to send to participants

### Troubleshooting

- **Issue**: Agenda too detailed or too vague
  **Solution**: Adjust constraints: "Each agenda item should have: topic, duration, owner, and objective"

- **Issue**: Time allocations don't add up
  **Solution**: Add constraint: "Ensure all time allocations total exactly 90 minutes including break"

- **Issue**: Not professional enough
  **Solution**: Add to constraints: "Use formal business meeting format, suitable for client and executive review"

---

## Exercise 5: Create Your Own TCFC Template

**Objective**: Build a reusable template for a task you do regularly

**Scenario**: Choose a task from your actual work that you could use AI to help with regularly.

### Common Tasks to Consider

- Weekly status reports
- Follow-up emails after meetings
- Customer service responses
- Data analysis summaries
- Meeting notes summarization
- Project proposals
- Team announcements

### Your Task

1. **Choose your task**
2. **Identify what varies** each time (recipient, data, dates, etc.)
3. **Create a TCFC template** with placeholders
4. **Test it** with real information

### Template Format

```
[TASK] [Action] [what you're working with]

[CONTEXT]
- [Variable 1]: [placeholder]
- [Variable 2]: [placeholder]
- Audience: [placeholder]
- Purpose: [standard purpose]

[FORMAT]
[Your standard format]

[CONSTRAINTS]
[Your standard constraints]
```

### Example: Follow-Up Email Template

```
[TASK] Draft a follow-up email after [TYPE OF MEETING]

[CONTEXT]
- Recipient: [NAME and TITLE]
- Meeting date: [DATE]
- Key discussion points: [TOPICS]
- Relationship: [CLIENT/PARTNER/INTERNAL]
- Purpose: Thank them, summarize key points, confirm next steps

[FORMAT]
- Subject line
- Greeting
- Thank you paragraph
- Summary of key points (2-3 bullets)
- Next steps paragraph
- Professional closing

[CONSTRAINTS]
- Professional but warm tone
- Maximum 250 words
- Include specific action items with dates
- Clear call-to-action
```

### Validation Prompt

```
I created a reusable TCFC template for my work:

**Task I Do Regularly**: [Describe the task]

**My TCFC Template**:
[Paste your template with placeholders]

**Test Case** (filled in with real info):
[Paste template with actual values]

**Output**:
[Paste Gemini's output]

**Please evaluate**:
1. Is my template structure sound?
2. Are the placeholders clear?
3. Would this save me time on this recurring task?
4. What could make the template more useful?
```

### Success Criteria
- [ ] Chose a realistic, recurring task
- [ ] Created complete TCFC template
- [ ] Identified appropriate placeholders
- [ ] Tested with real information
- [ ] Output is immediately usable
- [ ] Template is reusable for future instances

---

## Reflection Questions

1. **How does TCFC change** the way you think about prompts?

2. **Which component (T, C, F, or C)** do you most often forget?

3. **What task from your work** would benefit most from a TCFC template?

4. **How will you remember** to use TCFC in your daily work?

5. **What was most challenging** about structuring prompts this way?

---

## Key Takeaways

- **TCFC is your checklist** — Task, Context, Format, Constraints
- **Structure improves results** — Organized prompts get better outputs
- **Templates save time** — Create reusable TCFC templates for recurring tasks
- **All components matter** — Don't skip any part of TCFC
- **Practice builds habit** — Soon TCFC becomes automatic

---

## Next Steps

Excellent work! You now have a reliable framework for structuring any prompt.

**To continue improving:**

1. **Use TCFC daily** — Apply it to every prompt this week
2. **Build your template library** — Create TCFC templates for common tasks
3. **Move to Chapter 3** — Learn about clarity and specificity
4. **Share with colleagues** — Teach others the TCFC framework

**Ready for more?** → [Chapter 3: Clarity and Specificity](../03-clarity-specificity/lesson.md)

---

## Additional Practice (Optional)

Create TCFC prompts for these scenarios:

1. **Data analysis**: Analyze monthly website traffic data
2. **Customer response**: Reply to a product inquiry email
3. **Report creation**: Generate a project completion report
4. **Presentation outline**: Create slides for a sales pitch
5. **Team communication**: Announce a new company policy

---

## Navigation

- **Previous**: [Lesson 2: Basic Prompt Structure](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 3: Clarity and Specificity](../03-clarity-specificity/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 2 Complete!** 🎉 You've mastered the TCFC framework!
