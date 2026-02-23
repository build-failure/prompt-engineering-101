# Quick Reference: Prompt Engineering Cheat Sheet

A condensed guide to prompt engineering techniques for quick lookup.

---

## The TCFC Framework

Every effective prompt should include:

| Component | Description | Example |
|-----------|-------------|---------|
| **T**ask | What you want AI to do | "Summarize this report" |
| **C**ontext | Background information | "For executive review" |
| **F**ormat | Desired output structure | "As 3 bullet points" |
| **C**onstraints | Limitations or requirements | "Maximum 100 words" |

**Example:**
```
Summarize this quarterly sales report for executive review. 
Provide 3 bullet points highlighting key trends. 
Maximum 100 words total.
```

---

## Essential Techniques

### 1. Be Specific
❌ "Write an email"
✅ "Write a professional follow-up email to a client after a project proposal meeting, thanking them for their time and summarizing the next steps"

### 2. Assign a Role
```
You are an experienced marketing strategist. 
Analyze this campaign data and provide recommendations.
```

### 3. Provide Context
```
Context: Our company sells B2B software to mid-size companies.
Our target audience is IT managers with limited budgets.
Task: Draft a product introduction email.
```

### 4. Use Examples (Few-Shot)
```
Here are examples of our brand voice:
Example 1: [sample text]
Example 2: [sample text]

Now write a similar message about [topic].
```

### 5. Separate Instructions from Data
```
Instructions: Analyze the following customer feedback and identify the top 3 concerns.

Data:
"""
[paste customer feedback here]
"""
```

### 6. Request Step-by-Step Thinking
```
Analyze this business decision step-by-step:
1. First, identify the key factors
2. Then, evaluate pros and cons
3. Finally, provide a recommendation with reasoning
```

### 7. Specify Output Format
```
Provide your analysis in this format:
- Summary: [one paragraph]
- Key Findings: [bullet list]
- Recommendations: [numbered list]
- Next Steps: [action items with owners]
```

---

## Common Prompt Patterns

### Email Drafting
```
Draft a [type] email to [recipient] about [topic].
Tone: [professional/friendly/formal]
Key points to include:
- [point 1]
- [point 2]
- [point 3]
Length: [X] paragraphs
```

### Document Summarization
```
Summarize the following [document type] for [audience].
Focus on: [key aspects]
Format: [bullet points/paragraphs/executive summary]
Length: [word count or page limit]

Document:
"""
[paste document here]
"""
```

### Data Analysis
```
Analyze this data and provide insights:

Data:
"""
[paste data here]
"""

Please identify:
1. Key trends
2. Notable patterns
3. Areas of concern
4. Recommendations

Format as a structured report.
```

### Presentation Outline
```
Create a presentation outline on [topic] for [audience].
Duration: [X] minutes
Key messages:
- [message 1]
- [message 2]
- [message 3]

Include: title slide, main sections, and conclusion.
```

### Meeting Agenda
```
Create a meeting agenda for [meeting type] with [participants].
Duration: [X] minutes
Objectives:
- [objective 1]
- [objective 2]

Include time allocations for each item.
```

---

## Troubleshooting Guide

| Problem | Solution |
|---------|----------|
| Output too vague | Add more specific constraints and examples |
| Wrong tone | Explicitly specify tone and provide examples |
| Too long/short | Add word count or length constraints |
| Missing information | Provide more context and background |
| Inconsistent results | Use few-shot examples to show desired pattern |
| Hallucinations | Request citations, add "only use provided information" |
| Wrong format | Explicitly describe desired structure with example |
| Off-topic | Clarify the task and add constraints about scope |

---

## Power Words for Prompts

### Action Verbs
- Summarize, Analyze, Compare, Evaluate, Explain
- Draft, Create, Generate, Write, Compose
- Identify, Extract, List, Categorize, Organize
- Review, Critique, Assess, Validate, Check

### Constraint Words
- Maximum, Minimum, Exactly, Approximately
- Only, Exclusively, Specifically, Particularly
- Must include, Should avoid, Do not mention
- Focus on, Emphasize, Prioritize, Highlight

### Format Words
- Bullet points, Numbered list, Table, Paragraph
- Sections, Headings, Categories, Groups
- Summary, Overview, Detail, Breakdown
- Professional, Casual, Formal, Conversational

---

## Do's and Don'ts

### ✅ Do
- Be specific about what you want
- Provide relevant context
- Specify desired format
- Use examples when needed
- Iterate and refine prompts
- Test with variations
- Save successful prompts as templates

### ❌ Don't
- Use vague language ("good," "nice," "some")
- Assume AI knows your context
- Mix multiple unrelated tasks
- Forget to specify format
- Accept first output without review
- Ignore hallucinations or errors
- Give up after one attempt

---

## Prompt Templates by Use Case

### 1. Email Follow-Up
```
Draft a follow-up email to [recipient] after [event/meeting].
Thank them for [specific thing].
Mention these key points:
- [point 1]
- [point 2]
Include a clear call-to-action: [action]
Tone: Professional but warm
Length: 3-4 paragraphs
```

### 2. Report Summary
```
Summarize this [report type] for [audience].
Focus on: [key aspects]
Highlight: [specific metrics or findings]
Format: Executive summary with 3-5 bullet points
Length: Maximum 200 words

Report content:
"""
[paste report]
"""
```

### 3. Data Insights
```
Analyze this data and provide insights:

[paste data or describe data]

Identify:
1. Top 3 trends
2. Notable anomalies
3. Actionable recommendations

Format as a business memo.
```

### 4. Content Creation
```
Create [content type] about [topic] for [audience].
Key messages:
- [message 1]
- [message 2]
Tone: [specify tone]
Style: [specify style]
Length: [specify length]
Include: [specific elements]
```

### 5. Problem Solving
```
Help me solve this problem: [describe problem]

Context:
- [relevant background]
- [constraints]
- [goals]

Please:
1. Analyze the situation
2. Identify possible solutions
3. Recommend the best approach
4. Explain your reasoning
```

---

## Advanced Techniques

### Prompt Chaining
Break complex tasks into steps:
1. **Step 1:** Generate outline
2. **Step 2:** Expand each section (use output from Step 1)
3. **Step 3:** Refine and polish (use output from Step 2)

### Validation Prompts
Check your work:
```
Review this [output type] and assess:
1. Does it meet the stated objectives?
2. Is the tone appropriate?
3. Are there any errors or inconsistencies?
4. What could be improved?

[paste your output]
```

### Iterative Refinement
```
Based on this output: [paste previous output]
Please refine it by:
- [specific improvement 1]
- [specific improvement 2]
- [specific improvement 3]
```

---

## Google Workspace Integration

### Gmail
- Draft emails, replies, and announcements
- Summarize email threads
- Create email templates

### Google Docs
- Summarize long documents
- Generate reports and proposals
- Create structured content

### Google Sheets
- Analyze data and identify trends
- Generate insights and recommendations
- Create data summaries

### Google Slides
- Generate presentation outlines
- Create slide content
- Write speaker notes

### Google Meet
- Create meeting agendas
- Summarize meeting notes
- Extract action items

---

## Measuring Success

Good outputs should be:
- ✅ **Accurate** - Factually correct and relevant
- ✅ **Complete** - Includes all requested elements
- ✅ **Appropriate** - Right tone and style for audience
- ✅ **Formatted** - Matches specified structure
- ✅ **Actionable** - Useful for intended purpose

---

## Quick Wins

Start with these high-impact use cases:
1. **Email summarization** - Save time on long threads
2. **Meeting agendas** - Structure productive meetings
3. **Report summaries** - Create executive overviews
4. **Email drafting** - Speed up routine communication
5. **Data analysis** - Get quick insights from spreadsheets

---

## Learning Resources

- **Full Course**: [README.md](README.md)
- **Glossary**: [GLOSSARY.md](GLOSSARY.md)
- **Templates**: [templates/](templates/)
- **Troubleshooting**: [resources/troubleshooting-guide.md](resources/troubleshooting-guide.md)
- **Best Practices**: [resources/best-practices.md](resources/best-practices.md)

---

## Remember

> "The quality of AI output is directly proportional to the quality of your prompt."

Practice makes perfect. Save your best prompts, iterate on what works, and build your personal prompt library.

---

[← Back to Home](README.md)
