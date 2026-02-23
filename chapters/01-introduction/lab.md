# Lab 1: Introduction to Prompt Engineering

← [Lesson 1](lesson.md) | [Home](../../README.md) | [Next: Lab 2 →](../02-basic-structure/lab.md)

---

## Overview

**Chapter**: 1 - Introduction to Prompt Engineering  
**Level**: Beginner  
**Estimated Time**: 25 minutes  
**Prerequisites**: Complete Lesson 1

## Learning Objectives

By completing this lab, you will:
- Identify the differences between good and bad prompts
- Recognize missing elements in prompts
- Write improved prompts for common business tasks
- Practice drafting your first effective prompts with Gemini

## Business Scenario

You're starting to use Google Gemini to help with daily work tasks. Today you'll practice the fundamentals: recognizing what makes prompts effective and writing your first improved prompts for real business situations.

## Materials Needed

- Access to Google Gemini
- This lab document
- 25 minutes of focused time

---

## Exercise 1: Good vs. Bad Prompts

**Objective**: Learn to identify what makes a prompt effective or ineffective

**Scenario**: You'll see pairs of prompts for the same task. Identify which is better and why.

### Pair 1: Email Response

**Prompt A:**
```
Write a response
```

**Prompt B:**
```
Draft a professional email response to a customer who asked about
our product pricing. Explain that we offer three tiers (Basic $29/month,
Pro $79/month, Enterprise custom pricing) and suggest scheduling a
call to discuss their needs. Keep it friendly and helpful, maximum
150 words.
```

### Pair 2: Meeting Summary

**Prompt A:**
```
Summarize the meeting notes
```

**Prompt B:**
```
Summarize these project kickoff meeting notes for team members who
couldn't attend. Focus on: decisions made, assigned action items with
owners, and next meeting date. Format as bullet points, maximum 200 words,
professional tone.
```

### Pair 3: Data Analysis

**Prompt A:**
```
Look at this data
```

**Prompt B:**
```
Analyze this monthly sales data and identify: 1) top 3 performing products,
2) any products with declining sales, 3) overall revenue trend. Present
findings as a brief paragraph followed by a table with specific numbers.
```

### Your Task

For each pair:
1. Which prompt is better?
2. What specific elements make it better?
3. What's missing from the weaker prompt?

### Answers

<details>
<summary>Click to reveal analysis</summary>

**All "B" prompts are better. Here's why:**

**Pair 1:**
- ✅ Prompt B specifies: task (draft email), audience (customer), content (pricing tiers), tone (friendly/helpful), length (150 words)
- ❌ Prompt A: No context, no content guidance, no format

**Pair 2:**
- ✅ Prompt B specifies: audience (absent team members), focus areas (decisions/actions/dates), format (bullets), length, tone
- ❌ Prompt A: No audience, no focus, no format

**Pair 3:**
- ✅ Prompt B specifies: specific analysis questions, output format (paragraph + table), what to include
- ❌ Prompt A: No direction, no questions, no format

**Common pattern:** Good prompts include task, context, format, and constraints.

</details>

### Success Criteria
- [ ] Correctly identified the better prompt in each pair
- [ ] Explained what makes each good prompt effective
- [ ] Recognized what's missing from weak prompts

---

## Exercise 2: Spot the Missing Elements

**Objective**: Identify what's missing from incomplete prompts

**Scenario**: These prompts are missing key information. Identify what needs to be added.

### Prompt 1
```
Summarize this report for executives.
```

**What's missing?**
- [ ] Length/format specification?
- [ ] Focus areas or key points?
- [ ] Tone guidance?
- [ ] Purpose or context?

### Prompt 2
```
Write a professional email to the client about the project delay.
```

**What's missing?**
- [ ] Reason for delay?
- [ ] New timeline?
- [ ] Tone (apologetic, matter-of-fact)?
- [ ] Length constraint?

### Prompt 3
```
Create a meeting agenda.
```

**What's missing?**
- [ ] Meeting purpose?
- [ ] Duration?
- [ ] Attendees?
- [ ] Key topics to cover?
- [ ] Format/structure?

### Your Task

For each prompt, check all the missing elements, then write an improved version.

### Example Improvements

<details>
<summary>Click to see improved versions</summary>

**Improved Prompt 1:**
```
Summarize this quarterly financial report for executive review.
Focus on: revenue trends, major expenses, and any budget concerns.
Present as 5 bullet points, maximum 200 words, professional tone
suitable for C-level audience.
```

**Improved Prompt 2:**
```
Write a professional, apologetic email to client ABC Corp about
the 2-week project delay caused by supply chain issues. Explain
the situation briefly, provide the new completion date (March 15),
and offer a 10% discount as compensation. Keep it concise and
solution-focused, maximum 200 words.
```

**Improved Prompt 3:**
```
Create a meeting agenda for our 60-minute project planning session
with the development team (6 people). Cover: project goals, timeline
review, task assignments, and Q&A. Include time allocations for each
section and leave 10 minutes for questions. Format professionally.
```

</details>

### Validation Prompt

```
I'm learning to identify missing elements in prompts:

**Original Prompt**: [Paste one of the incomplete prompts]

**My Improved Version**: [Paste your improved prompt]

**Please assess**:
1. Did I identify the key missing elements?
2. Is my improved version more effective?
3. What else could I add to make it even better?
```

### Success Criteria
- [ ] Identified missing elements in all three prompts
- [ ] Wrote improved versions with complete information
- [ ] Understood why each addition improves the prompt

### Troubleshooting

- **Issue**: Not sure what's missing
  **Solution**: Ask yourself: Who is this for? What exactly do I want? How should it look? Any limits or requirements?

- **Issue**: Improved prompt feels too long
  **Solution**: That's okay! Detailed prompts get better results. You can save them as templates for reuse.

---

## Exercise 3: Write Your First Email Prompt

**Objective**: Create a complete prompt for a common business task

**Scenario**: You need to send a follow-up email after meeting with a potential client.

### Meeting Context

- Client: Jennifer Martinez, Marketing Director at TechStart Inc.
- Meeting: Yesterday, discussed their need for a new CRM system
- Key points discussed: Integration with existing tools, team training, pricing
- Next step: You'll send a proposal by Friday
- Your goal: Thank her, summarize key points, confirm next steps

### Your Task

Write a complete prompt that will generate this follow-up email.

### Prompt Template

Use this structure to build your prompt:

```
Draft a [type] email to [recipient] about [topic].

[Provide context about the situation]

Include:
- [Point 1]
- [Point 2]
- [Point 3]

Tone: [specify tone]
Length: [specify length]
```

### Write Your Prompt

```
[Your complete prompt here]
```

### Example Solution

<details>
<summary>Click to see example prompt</summary>

```
Draft a professional follow-up email to Jennifer Martinez,
Marketing Director at TechStart Inc.

We met yesterday to discuss their need for a new CRM system.
The meeting covered three main topics: integration with their
existing tools, team training requirements, and pricing options.

Include:
- Thank you for her time and the productive discussion
- Brief summary of the three key topics we discussed
- Confirmation that I'll send a detailed proposal by Friday
- Offer to answer any questions in the meantime
- Professional closing with my contact information

Tone: Professional but warm and appreciative
Length: Maximum 200 words
```

</details>

### Test Your Prompt

1. Copy your prompt
2. Paste it into Google Gemini
3. Review the generated email
4. Check if it includes all required elements

### Validation Prompt

```
I'm practicing writing effective prompts for business emails:

**My Prompt**:
[Paste your complete prompt]

**Generated Email**:
[Paste Gemini's output]

**Please evaluate**:
1. Does my prompt provide enough context?
2. Is the generated email professional and complete?
3. Would this email be ready to send with minimal editing?
4. What could I improve in my prompt?
```

### Success Criteria
- [ ] Prompt includes recipient and context
- [ ] Specifies all content to include
- [ ] Defines tone and length
- [ ] Generated email is professional and complete
- [ ] Email requires minimal editing before sending

### Troubleshooting

- **Issue**: Email is too generic
  **Solution**: Add more specific details about the meeting and discussion points

- **Issue**: Wrong tone (too formal or too casual)
  **Solution**: Be explicit: "Professional but warm" or "Formal business tone"

- **Issue**: Email is too long
  **Solution**: Add stricter length constraint: "Maximum 150 words, 3 short paragraphs"

---

## Exercise 4: Document Summarization

**Objective**: Write a prompt to summarize business content

**Scenario**: You have a long project status report that needs to be summarized for your manager.

### Report Context

- Document: 5-page project status report
- Project: Website redesign (in progress for 6 weeks)
- Your manager needs: Quick overview of progress, any issues, and next steps
- Manager's preference: Brief, bullet-point format
- Time constraint: Manager will read this in 2 minutes

### Your Task

Write a prompt that will create an effective summary.

### Consider These Questions

1. What should the summary focus on?
2. How long should it be?
3. What format works best?
4. What tone is appropriate?

### Write Your Prompt

```
[Your summarization prompt here]
```

### Example Solution

<details>
<summary>Click to see example</summary>

```
Summarize this 5-page website redesign project status report
for my manager who needs a quick overview.

Focus on:
- Current progress and completion percentage
- Any blockers or issues
- Key milestones achieved this week
- Next steps and upcoming deadlines

Format as:
- Brief overview (1-2 sentences)
- Progress highlights (3-4 bullets)
- Issues/blockers (bullets, if any)
- Next steps (2-3 bullets)

Keep it concise - maximum 250 words total. Use professional
language suitable for manager review. Highlight any urgent
items or risks.

[Report content would go here]
```

</details>

### Validation Prompt

```
I'm writing a prompt to summarize a project report:

**My Prompt**:
[Paste your prompt]

**Generated Summary**:
[Paste output]

**Please assess**:
1. Does the prompt specify what to focus on?
2. Is the format appropriate for a busy manager?
3. Would this summary be useful for quick decision-making?
4. What would make the prompt more effective?
```

### Success Criteria
- [ ] Prompt specifies focus areas
- [ ] Defines appropriate format for audience
- [ ] Sets reasonable length constraint
- [ ] Summary is actionable and clear
- [ ] Manager could read and understand in 2 minutes

---

## Exercise 5: Your Own Business Task

**Objective**: Apply what you've learned to your actual work

**Scenario**: Choose a real task from your work where Gemini could help.

### Common Tasks to Consider

- Drafting a specific type of email you send regularly
- Summarizing meeting notes or reports
- Analyzing data from spreadsheets
- Creating agendas or action items
- Writing announcements or updates
- Responding to customer inquiries

### Your Task

1. **Choose your task**: Pick something you actually need to do
2. **Gather context**: What information does Gemini need?
3. **Write your prompt**: Include all necessary elements
4. **Test it**: Use Gemini to generate the output
5. **Refine**: Adjust your prompt if needed

### Prompt Checklist

Before writing, ensure you can answer:

- [ ] What exactly do I want Gemini to do? (Task)
- [ ] What background information is needed? (Context)
- [ ] How should the output be structured? (Format)
- [ ] What are the requirements? (Constraints: length, tone, etc.)

### Write Your Prompt

```
[Your real-world prompt here]
```

### Test and Refine

1. Use your prompt with Gemini
2. Evaluate the output
3. If it's not quite right, identify what to adjust:
   - Need more context?
   - Format not clear enough?
   - Tone not right?
   - Missing constraints?
4. Revise and try again

### Validation Prompt

```
I wrote a prompt for a real task from my work:

**My Task**: [Describe what you need to accomplish]

**My Prompt**:
[Paste your prompt]

**Output**:
[Paste Gemini's output]

**Please evaluate**:
1. Is my prompt clear and complete?
2. Is the output useful for my actual work?
3. What would make this prompt even more effective?
4. Could I reuse this prompt as a template?
```

### Success Criteria
- [ ] Chose a realistic work task
- [ ] Wrote a complete prompt with all elements
- [ ] Tested with Gemini
- [ ] Output is useful for your actual work
- [ ] Identified how to improve if needed

### Troubleshooting

- **Issue**: Output doesn't match what you need
  **Solution**: Add more specific details about desired outcome

- **Issue**: Output is in wrong format
  **Solution**: Be explicit about structure: "Format as email with subject line and 3 paragraphs"

- **Issue**: Tone is off
  **Solution**: Specify exact tone: "Friendly but professional" or "Formal business communication"

---

## Reflection Questions

1. **What surprised you** about the difference between good and bad prompts?

2. **Which element** (task, context, format, constraints) do you think is most important?

3. **What task from your work** will you try with Gemini first?

4. **What was most challenging** about writing effective prompts?

5. **How will prompt engineering** help you in your daily work?

---

## Key Takeaways

- **Specificity matters** — Clear, detailed prompts get better results
- **Context is crucial** — Gemini needs background to help effectively
- **Format guides output** — Specify how you want information structured
- **Constraints ensure fit** — Define length, tone, and requirements
- **Practice improves skill** — You'll get better with each prompt

---

## What's Next

Excellent work! You've completed your first hands-on practice with prompt engineering.

**To continue improving:**

1. **Use Gemini daily** — Practice with real work tasks this week
2. **Notice patterns** — Pay attention to what makes prompts work
3. **Save good prompts** — Build your own library of effective prompts
4. **Move to Chapter 2** — Learn the TCFC framework for systematic prompt structure

**Ready for more structure?** → [Chapter 2: Basic Prompt Structure](../02-basic-structure/lesson.md)

---

## Additional Practice (Optional)

Try writing prompts for these scenarios:

1. **Customer service**: Respond to a complaint about a delayed order
2. **Team communication**: Announce a new company policy
3. **Data analysis**: Analyze monthly sales trends
4. **Meeting prep**: Create an agenda for a project kickoff
5. **Content creation**: Draft a LinkedIn post about a company achievement

---

## Navigation

- **Previous**: [Lesson 1: Introduction](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 2: Basic Prompt Structure](../02-basic-structure/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Getting Started](../../GETTING_STARTED.md)

---

**Lab 1 Complete!** 🎉 You're on your way to becoming a prompt engineering pro!
