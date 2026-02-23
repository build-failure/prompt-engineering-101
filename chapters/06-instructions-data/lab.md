# Lab 6: Separating Instructions from Data

← [Lesson 6](lesson.md) | [Home](../../README.md) | [Next: Lab 7 →](../07-output-formatting/lab.md)

---

## Overview

**Chapter**: 6 - Separating Instructions from Data  
**Level**: Intermediate  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 6

## Learning Objectives

By completing this lab, you will:
- Practice separating instructions from data in prompts
- Learn effective formatting techniques for data inclusion
- Handle different data types (text, tables, lists)
- Apply separation techniques to real business scenarios

## Business Scenario

You frequently need to analyze data, summarize documents, and process information from various sources. When instructions and data are mixed together, AI can get confused about what to analyze versus what to do. You'll learn how to clearly separate your instructions from the data you want processed, leading to more accurate and reliable results.

## Materials Needed

- Access to Google Gemini
- Sample data provided in exercises
- Optional: Your own business data to practice with

---

## Exercise 1: Before and After Comparison

**Objective**: See the impact of separating instructions from data

**Scenario**: You need to analyze customer feedback comments.

### Your Task

Compare these two approaches:

**Version 1: Mixed Instructions and Data (Confusing)**
```
Analyze these customer comments and identify the top 3 issues. Look for patterns
in the feedback. Here are the comments: "The app crashes when I upload photos" and
"I love the new interface but the app is slow" and "Crashes constantly, very frustrating"
and "Great features but needs to be faster" and "App freezes on my phone". Create a
summary with the issues and how many times each appears.
```

**Version 2: Separated Instructions and Data (Clear)**
```
INSTRUCTIONS:
Analyze the customer feedback below and:
1. Identify the top 3 issues mentioned
2. Count how many times each issue appears
3. Present as a table with: Issue | Count | Severity

DATA:
"""
- "The app crashes when I upload photos"
- "I love the new interface but the app is slow"
- "Crashes constantly, very frustrating"
- "Great features but needs to be faster"
- "App freezes on my phone"
"""
```

### Test and Compare

1. Run both versions in Gemini
2. Compare the clarity and accuracy of outputs
3. Note which version is easier to modify

**Expected Output**:
- Version 1: May miss some issues, harder to parse
- Version 2: Clear analysis, accurate counts, proper table format

**Validation Prompt**:
```
I'm learning about separating instructions from data. I tested two versions:

Version 1 (mixed) output: [paste output]
Version 2 (separated) output: [paste output]

Please assess:
1. Which version produced more accurate results?
2. How did separation improve clarity?
3. Which would be easier to modify if I had more data?
```

### Success Criteria
- [ ] Understood the difference between mixed and separated approaches
- [ ] Recognized how separation improves accuracy
- [ ] Saw how formatting makes data clearer

**Troubleshooting**:
- **Issue**: Both outputs look similar
  **Solution**: Try with more complex data where the difference becomes more apparent
- **Issue**: Version 2 seems overly complex
  **Solution**: Remember, clarity is worth the extra structure, especially with larger datasets

---

## Exercise 2: Email Thread Summarization

**Objective**: Separate instructions from multi-part text data

**Scenario**: You need to summarize a long email thread for your team.

### Your Task

Create a prompt that clearly separates instructions from the email content:

```
INSTRUCTIONS:
Summarize this email thread about the product launch delay.

Extract and organize:
- Reason for the delay
- New launch date
- Action items with owners
- Any concerns raised

Format as:
- Brief overview (2 sentences)
- Key points (bullets)
- Action items table (Task | Owner | Deadline)

Keep it concise, maximum 250 words.

---

EMAIL THREAD:
"""
From: Sarah Chen <sarah@company.com>
To: Product Team
Date: March 15, 2024
Subject: Product Launch Update

Team, we need to push the launch date. The QA team found critical bugs in the
payment integration that need to be fixed before we can go live.

---

From: Mike Rodriguez <mike@company.com>
To: Sarah Chen, Product Team
Date: March 15, 2024
Subject: RE: Product Launch Update

How much time do we need? I've already scheduled the marketing campaign for March 25.
Can we still hit that date?

---

From: Sarah Chen <sarah@company.com>
To: Product Team
Date: March 15, 2024
Subject: RE: Product Launch Update

Engineering estimates 2 weeks for fixes and testing. New target date is April 8.

Action items:
- Mike: Reschedule marketing campaign
- Dev team: Fix payment bugs by March 29
- QA: Complete testing by April 5
- Sarah: Update stakeholders

I know this is frustrating, but we can't launch with payment issues.

---

From: Jennifer Lee <jen@company.com>
To: Product Team
Date: March 15, 2024
Subject: RE: Product Launch Update

Agreed. Better to delay than launch broken. I'm concerned about customer expectations
though - we've been promoting the March date. How do we handle communications?
"""
```

**Expected Output**:
A clear summary with:
- Overview of the delay situation
- Organized key points
- Action items in table format
- Professional, concise presentation

**Validation Prompt**:
```
I'm practicing separating instructions from data for email summarization:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Is the separation between instructions and data clear?
2. Did the output include all requested elements?
3. Is the summary useful for team members who missed the thread?
4. What could improve the structure?
```

### Success Criteria
- [ ] Clear separation between instructions and email data
- [ ] Used delimiters (""") to mark data boundaries
- [ ] Instructions specify exact output format
- [ ] Summary is accurate and complete
- [ ] Easy to add more emails if needed

**Troubleshooting**:
- **Issue**: Output misses some action items
  **Solution**: In instructions, emphasize "Extract ALL action items mentioned in any email"
- **Issue**: Format doesn't match request
  **Solution**: Be more specific about table structure: "Create a markdown table with exactly these columns"

---

## Exercise 3: Spreadsheet Data Analysis

**Objective**: Handle structured data with clear separation

**Scenario**: Analyze monthly sales data from Google Sheets.

### Your Task

Create a prompt that separates analysis instructions from tabular data:

```
INSTRUCTIONS:
Analyze the monthly sales data below and provide:

1. Top 3 performing products by revenue
2. Products with declining sales (month-over-month decrease)
3. Overall revenue trend
4. One key recommendation based on the data

Present findings as:
- Executive summary (3 sentences)
- Top performers table (Product | Revenue | Growth %)
- Concerns section (bullet points)
- Recommendation (1 paragraph)

---

DATA:
| Product | January | February | March |
|---------|---------|----------|-------|
| Widget A | $45,000 | $52,000 | $58,000 |
| Widget B | $38,000 | $35,000 | $32,000 |
| Widget C | $29,000 | $31,000 | $34,000 |
| Widget D | $51,000 | $53,000 | $55,000 |
| Widget E | $22,000 | $20,000 | $18,000 |
| Widget F | $15,000 | $18,000 | $21,000 |

Total: $200,000 | $209,000 | $218,000
```

**Expected Output**:
- Clear executive summary
- Table showing top 3 performers with growth percentages
- Identification of declining products (Widget B and E)
- Actionable recommendation based on trends

**Validation Prompt**:
```
I'm practicing data analysis with separated instructions:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Did the separation make the data analysis clearer?
2. Are all requested elements present in the output?
3. Is the analysis accurate based on the data?
4. Is the recommendation actionable?
```

### Success Criteria
- [ ] Instructions clearly separated from data table
- [ ] Data formatted as a proper table
- [ ] Analysis instructions are specific and numbered
- [ ] Output format is clearly defined
- [ ] Results are accurate and actionable

**Troubleshooting**:
- **Issue**: AI misreads the table data
  **Solution**: Ensure table formatting is clean with clear column headers and alignment
- **Issue**: Analysis is too shallow
  **Solution**: Add to instructions: "Provide specific numbers and percentages in your analysis"

---

## Exercise 4: Survey Response Processing

**Objective**: Process multiple data items with consistent formatting

**Scenario**: Analyze customer survey responses from Google Forms.

### Your Task

Create a prompt to analyze survey data with clear separation:

```
INSTRUCTIONS:
Analyze these customer satisfaction survey responses.

For each question, provide:
- Summary of responses
- Key themes or patterns
- Percentage breakdown where applicable
- Notable quotes (if relevant)

Present as a structured report with sections for each question.
Highlight any urgent issues that need immediate attention.

---

SURVEY DATA:
"""
Question 1: How satisfied are you with our product? (1-5 scale)
Responses: 5, 4, 5, 3, 4, 5, 2, 4, 5, 4, 3, 5, 4, 5, 1, 4, 5, 5, 4, 5

Question 2: What do you like most about our product?
- "Easy to use and intuitive interface"
- "Great customer support team"
- "Solves my problem perfectly"
- "Fast and reliable"
- "Love the mobile app"
- "Integration with other tools"
- "Regular updates and improvements"
- "Good value for money"

Question 3: What needs improvement?
- "Loading time is too slow"
- "Mobile app crashes sometimes"
- "Need better reporting features"
- "Slow loading times"
- "More integrations needed"
- "App stability issues"
- "Better documentation"
- "Faster performance"

Question 4: Would you recommend us to others? (Yes/No)
Responses: Yes, Yes, Yes, No, Yes, Yes, Yes, No, Yes, Yes, Yes, Yes, No, Yes, Yes, Yes, Yes, Yes, Yes, Yes
"""
```

**Expected Output**:
- Structured analysis for each question
- Satisfaction score average and distribution
- Themes from open-ended responses
- Clear identification of the performance/stability issue pattern
- Recommendation percentage
- Urgent issues highlighted

**Validation Prompt**:
```
I'm analyzing survey data with separated instructions:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Is the data clearly separated and easy to read?
2. Did the analysis identify key patterns (performance issues)?
3. Are percentages and summaries accurate?
4. Would this report be useful for product decisions?
```

### Success Criteria
- [ ] Clear separation between instructions and survey data
- [ ] Survey data organized by question
- [ ] Instructions specify analysis approach for each question type
- [ ] Output identifies the performance/stability pattern
- [ ] Report is actionable for product team

**Troubleshooting**:
- **Issue**: Analysis misses the pattern in "needs improvement"
  **Solution**: Add instruction: "Look for repeated themes across responses"
- **Issue**: Percentages are incorrect
  **Solution**: Verify data formatting is clear, consider adding: "Show your calculation"

---

## Exercise 5: Meeting Notes to Action Items

**Objective**: Extract structured information from unstructured text

**Scenario**: Convert raw meeting notes into organized action items.

### Your Task

Create a prompt that separates extraction instructions from meeting notes:

```
INSTRUCTIONS:
Process these meeting notes and extract:

1. Decisions made (what was decided and why)
2. Action items (task, owner, deadline)
3. Open questions (what needs to be resolved)
4. Next meeting date and agenda

Format as:
- Decisions: Numbered list with brief rationale
- Action Items: Table with columns (Task | Owner | Deadline | Priority)
- Open Questions: Bullet list
- Next Steps: Date, time, and agenda topics

Ensure every action item has a clear owner and deadline.
Flag any items missing owners or deadlines.

---

MEETING NOTES:
"""
Project Planning Meeting - March 20, 2024
Attendees: Sarah (PM), Mike (Dev), Jennifer (Design), Tom (Marketing)

Sarah opened by reviewing the project timeline. We're targeting a May 15 launch.
Everyone agreed this is achievable if we stay on track.

Mike raised concerns about the API integration complexity. After discussion, we
decided to use the third-party solution instead of building custom. This saves
3 weeks of development time. Mike will research vendors by next Friday.

Jennifer presented three design concepts. Team preferred Option B for its clean
interface. She'll create detailed mockups by April 5.

Tom needs final messaging approved before creating marketing materials. Sarah
will draft key messages and share by March 25. Tom will then create campaign
materials.

Question came up about budget for paid advertising. Sarah needs to check with
finance and report back.

We still need to decide on the pricing model. Should we discuss this with the
sales team first?

Next meeting: March 27 at 2 PM. Agenda: Review vendor options, approve messaging,
discuss pricing model.
"""
```

**Expected Output**:
- Clear list of decisions with rationale
- Complete action items table with all details
- Open questions identified
- Next meeting information
- Any flagged items missing details

**Validation Prompt**:
```
I'm extracting action items from meeting notes:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Are instructions clearly separated from the meeting notes?
2. Did the output capture all action items with owners and deadlines?
3. Were decisions and open questions properly identified?
4. Is the output format useful for follow-up?
5. Were any missing details flagged?
```

### Success Criteria
- [ ] Clear separation between instructions and notes
- [ ] Extraction instructions are comprehensive
- [ ] Output format is specified in detail
- [ ] All action items captured with owners and deadlines
- [ ] Decisions and open questions identified
- [ ] Next meeting information included
- [ ] Missing information flagged

**Troubleshooting**:
- **Issue**: Some action items are missed
  **Solution**: Add instruction: "Read through the entire notes carefully and extract every commitment or task mentioned"
- **Issue**: Deadlines are vague
  **Solution**: Add: "If deadline is not explicit, note as 'TBD' and flag for clarification"
- **Issue**: Output format is inconsistent
  **Solution**: Provide a template or example of the exact format you want

---

## Reflection Questions

1. **How did separating instructions from data improve your prompts?** Think about clarity, accuracy, and ease of modification.

2. **What formatting techniques worked best for different data types?** Consider text blocks, tables, lists, and delimiters.

3. **When is separation most critical?** Reflect on data complexity, volume, and task requirements.

4. **How will you apply this technique to your work?** Think about emails, reports, data analysis, and document processing.

---

## Key Takeaways

- **Separation prevents confusion** - AI knows what to do vs. what to analyze
- **Formatting matters** - Use delimiters, sections, and clear boundaries
- **Consistency helps** - Use the same separation pattern across prompts
- **Scalability improves** - Easy to add more data without rewriting instructions
- **Accuracy increases** - Less chance of AI misinterpreting instructions as data

---

## Next Steps

Excellent work! You now know how to structure prompts with clear data separation.

**To continue improving:**

1. **Apply to your work** - Use separation for any data analysis tasks this week
2. **Build templates** - Create reusable formats for common data types
3. **Move to Chapter 7** - Learn about output formatting and structure
4. **Practice with real data** - Try with your actual business documents and spreadsheets

**Ready for more?** → [Chapter 7: Output Formatting and Structure](../07-output-formatting/lesson.md)

---

## Additional Practice (Optional)

Try separating instructions from data for these scenarios:

1. **Customer feedback**: Analyze 20 product reviews
2. **Financial data**: Summarize quarterly expense report
3. **Email analysis**: Extract key points from 10-email thread
4. **Survey results**: Process employee satisfaction survey
5. **Meeting series**: Summarize notes from 4 weekly meetings

---

## Navigation

- **Previous**: [Lesson 6: Separating Instructions from Data](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 7: Output Formatting and Structure](../07-output-formatting/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 6 Complete!** 🎉 You've mastered instruction-data separation!
