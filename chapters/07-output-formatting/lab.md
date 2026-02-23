# Lab 7: Output Formatting and Structure

← [Lesson 7](lesson.md) | [Home](../../README.md) | [Next: Lab 8 →](../08-step-by-step/lab.md)

---

## Overview

**Chapter**: 7 - Output Formatting and Structure  
**Level**: Intermediate  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 7

## Learning Objectives

By completing this lab, you will:
- Practice specifying different output formats
- Learn to match formats to business needs
- Master format specifications for consistency
- Apply formatting techniques to real scenarios

## Business Scenario

You work with various types of content daily - reports, emails, presentations, and data analysis. The same information needs different formats depending on the audience and platform. You'll learn how to specify exactly the format you need, ensuring AI outputs are immediately usable without reformatting.

## Materials Needed

- Access to Google Gemini
- Sample content provided in exercises
- Optional: Your own business content to practice with

---

## Exercise 1: Format Comparison

**Objective**: See how format changes impact usability

**Scenario**: You need to present quarterly sales results to different audiences.

### Your Task

Create three versions of the same information in different formats:

**Version 1: Bullet Points (for quick team update)**
```
Summarize Q1 sales results in bullet format:
- 5-7 bullet points
- Start each with key metric or finding
- Include specific numbers and percentages
- Order by importance (most significant first)
- Keep each bullet under 15 words

DATA:
Q1 total revenue: $2.5M (up 18% from Q4)
New customers: 145 (target was 120)
Customer retention: 94% (up from 89%)
Top product: Widget Pro ($890K revenue, 35% of total)
Fastest growing: Widget Lite (67% growth)
Regional performance: Northeast +25%, West +15%, South +12%, Midwest +8%
```

**Version 2: Table Format (for executive report)**
```
Present Q1 sales results as a comparison table:

Columns: Metric | Q4 Actual | Q1 Target | Q1 Actual | vs Target | vs Q4
Rows: Total Revenue, New Customers, Retention Rate, Top Product Revenue

Include a brief summary paragraph below the table (2-3 sentences) highlighting the most important insight.

DATA:
[Same data as above]
Q4 revenue was $2.12M
Q4 new customers: 118
Q4 retention: 89%
Q4 top product: $720K
```

**Version 3: Paragraph Format (for board update)**
```
Write Q1 sales results as 2 professional paragraphs:
- Paragraph 1: Overall performance and key metrics (4-5 sentences)
- Paragraph 2: Notable achievements and trends (3-4 sentences)
- Style: Professional, confident, data-driven
- Include specific numbers to support statements
- Maximum 150 words total

DATA:
[Same data as above]
```

### Test and Compare

1. Run all three versions in Gemini
2. Compare which format is easiest to scan
3. Note which format best serves each audience

**Expected Output**:
- Version 1: Quick, scannable bullet points
- Version 2: Structured table with comparison data
- Version 3: Flowing narrative suitable for formal report

**Validation Prompt**:
```
I'm practicing output formatting with the same content in three formats:

Bullet version: [paste output]
Table version: [paste output]
Paragraph version: [paste output]

Please assess:
1. Does each format serve its intended purpose?
2. Are the format specifications clear in my prompts?
3. Which format would work best for: a) quick Slack update, b) formal report, c) presentation slide?
4. What could improve the format specifications?
```

### Success Criteria
- [ ] Created three distinct formats from same data
- [ ] Each format follows specified structure
- [ ] Understood which format serves which purpose
- [ ] Format specifications were clear and specific

**Troubleshooting**:
- **Issue**: Outputs look too similar
  **Solution**: Be more specific about structure - exact number of bullets, table columns, paragraph count
- **Issue**: Table format is messy
  **Solution**: Explicitly specify column names and request markdown table format

---

## Exercise 2: Meeting Agenda Creation

**Objective**: Create a structured meeting agenda with specific formatting

**Scenario**: You need to create a formatted agenda for a project planning meeting.

### Your Task

Create a comprehensive meeting agenda with precise formatting:

```
Create a meeting agenda in this exact format:

**MEETING DETAILS**
- Date: [from info below]
- Time: [from info below]
- Location: [from info below]
- Attendees: [list from info below]
- Duration: [calculate from info]

**MEETING OBJECTIVES**
(2-3 bullet points stating what we aim to accomplish)

**AGENDA ITEMS**
Format as table:
| Time | Topic | Owner | Duration |
(Calculate time slots based on 60-minute meeting)

**PRE-MEETING PREPARATION**
- Bullet list of what attendees should review beforehand
- Include specific documents or data

**EXPECTED OUTCOMES**
- Bullet list of decisions to be made
- Bullet list of deliverables from this meeting

**NEXT STEPS**
- What happens after this meeting

---

MEETING INFORMATION:
Purpose: Plan Q2 product launch
Date: April 5, 2024
Time: 2:00 PM - 3:00 PM
Location: Conference Room B / Zoom link
Attendees: Sarah (Product Manager), Mike (Engineering Lead), Jennifer (Design Lead), Tom (Marketing Manager), Lisa (Sales Director)

Topics to cover:
- Review launch timeline and milestones
- Finalize feature set for launch
- Discuss marketing strategy and messaging
- Review sales enablement needs
- Identify risks and mitigation plans
- Assign action items

Pre-work: Review product roadmap, competitive analysis, and Q1 sales data
```

**Expected Output**:
- Professionally formatted agenda
- Clear time allocations for each topic
- Specific owners for agenda items
- Actionable pre-meeting requirements
- Clear expected outcomes

**Validation Prompt**:
```
I created a meeting agenda with specific formatting:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Does the output follow the exact format specified?
2. Are all required sections present?
3. Is the agenda practical and usable?
4. Would attendees know what to prepare and expect?
```

### Success Criteria
- [ ] All format sections specified clearly
- [ ] Output includes all required sections
- [ ] Time allocations are realistic
- [ ] Agenda is professional and actionable
- [ ] Format is consistent throughout

**Troubleshooting**:
- **Issue**: Time slots don't add up to 60 minutes
  **Solution**: Add instruction: "Ensure all time slots total exactly 60 minutes"
- **Issue**: Missing sections in output
  **Solution**: Use clear section headers in your format specification with "Include:" statements

---

## Exercise 3: Data Analysis Report

**Objective**: Format analytical findings with mixed format types

**Scenario**: Analyze customer support data and present findings in a structured report.

### Your Task

Create a formatted analysis report combining multiple format types:

```
Analyze this customer support data and format as a structured report:

## EXECUTIVE SUMMARY
(1 paragraph, 3-4 sentences, maximum 75 words)
Highlight the single most important finding and its business impact.

## KEY METRICS
Format as table:
| Metric | This Month | Last Month | Change | Status |
(Status: 🟢 Good / 🟡 Attention Needed / 🔴 Critical)

## TOP ISSUES
Format as numbered list (ranked by frequency):
1. [Issue]: [Count] tickets, [% of total]
2. [Issue]: [Count] tickets, [% of total]
(Continue for top 5 issues)

## TRENDS AND PATTERNS
- 4-6 bullet points
- Each identifies a pattern with supporting data
- Focus on actionable insights

## RECOMMENDATIONS
Format as table:
| Priority | Recommendation | Expected Impact | Owner | Timeline |
(Priority: High/Medium/Low)

## NEXT STEPS
- Bullet list of immediate actions
- Include owners and deadlines

---

SUPPORT DATA:
Total tickets this month: 487 (last month: 423)
Average resolution time: 4.2 hours (last month: 3.8 hours)
Customer satisfaction: 4.1/5 (last month: 4.3/5)
First response time: 45 minutes (last month: 38 minutes)

Issue breakdown:
- Login problems: 142 tickets (29%)
- Slow performance: 98 tickets (20%)
- Feature questions: 87 tickets (18%)
- Billing issues: 73 tickets (15%)
- Bug reports: 52 tickets (11%)
- Other: 35 tickets (7%)

Notable patterns:
- Login issues spiked after March 15 update
- Performance complaints mostly from mobile users
- Billing issues concentrated in first week of month
- 68% of tickets resolved on first contact
- 15% of tickets required escalation (up from 10%)
```

**Expected Output**:
- Multi-section report with varied formats
- Executive summary paragraph
- Two formatted tables
- Numbered and bulleted lists
- Professional, actionable presentation

**Validation Prompt**:
```
I created a formatted analysis report:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Are all format types correctly applied?
2. Is the mix of formats effective for presenting this data?
3. Are the insights actionable?
4. Would this report be useful for decision-making?
5. Is the formatting consistent and professional?
```

### Success Criteria
- [ ] Multiple format types specified clearly
- [ ] Each section uses appropriate format
- [ ] Tables are properly structured
- [ ] Lists follow specified format
- [ ] Report is comprehensive and actionable
- [ ] Format enhances readability

**Troubleshooting**:
- **Issue**: Tables are inconsistent
  **Solution**: Specify exact column names and order in your prompt
- **Issue**: Recommendations lack detail
  **Solution**: Add to format spec: "Each recommendation must include specific action and measurable outcome"

---

## Exercise 4: Email Formatting

**Objective**: Format professional emails for different purposes

**Scenario**: Create three different types of business emails with appropriate formatting.

### Your Task

Create formatted emails for three scenarios:

**Email 1: Project Status Update**
```
Format as professional status update email:

**SUBJECT LINE:** [Clear, specific, includes project name and status]

**GREETING:** [Professional, appropriate for team]

**BODY STRUCTURE:**
Paragraph 1: Current status summary (2-3 sentences)

**Progress This Week:**
- Bullet list of completed items (3-5 bullets)

**Next Week Focus:**
- Bullet list of planned items (3-5 bullets)

**Blockers/Needs:**
- Bullet list if any, or state "None at this time"

**Key Metrics:**
Brief table or bullet list of relevant numbers

Closing paragraph: Next steps and any asks (2 sentences)

**CLOSING:** [Professional sign-off]

---

PROJECT INFO:
Project: Website Redesign
Status: On track for May 15 launch
Completed: Homepage design approved, mobile mockups done, content audit finished
In progress: Development of new templates, content migration
Planned: User testing, final QA, launch preparation
Blocker: Waiting for final brand guidelines from marketing
Metrics: 60% complete, 4 weeks remaining, budget 85% utilized
```

**Email 2: Meeting Follow-up**
```
Format as meeting follow-up email:

**SUBJECT LINE:** [Meeting name + date + "Summary and Action Items"]

**GREETING:** [Include all attendees]

**BODY STRUCTURE:**
Opening: Thank attendees, state meeting purpose (1 sentence)

**DECISIONS MADE:**
- Numbered list (3-5 items)
- Each decision with brief rationale

**ACTION ITEMS:**
Format as simple table or structured list:
- [Task] - Owner: [Name] - Due: [Date]
(5-7 action items)

**OPEN QUESTIONS:**
- Bullet list of items needing resolution
- Note who will follow up on each

**NEXT MEETING:**
Date, time, and brief agenda

Closing: Invitation for questions/clarifications (1 sentence)

**CLOSING:** [Professional]

---

MEETING INFO:
Meeting: Q2 Marketing Planning
Date: March 28, 2024
Attendees: Tom (Marketing), Sarah (Product), Lisa (Sales), Mike (Engineering)
Decisions: Approved $50K campaign budget, selected Agency B for creative, confirmed May 1 launch date
Actions: Tom to brief agency by April 5, Sarah to provide product messaging by April 1, Lisa to create sales materials by April 10, Mike to prepare demo environment by April 8
Open questions: Final pricing not decided, need to confirm trade show attendance
Next meeting: April 11, 2PM - Review campaign creative and finalize pricing
```

**Email 3: Customer Response**
```
Format as customer service response email:

**SUBJECT LINE:** [Re: their subject - professional and solution-focused]

**GREETING:** [Personalized, warm but professional]

**BODY STRUCTURE:**
Paragraph 1: Acknowledge their issue with empathy (2 sentences)

Paragraph 2: Explain the solution or next steps (3-4 sentences)
- Include specific actions being taken
- Provide timeline
- Set clear expectations

**WHAT YOU CAN DO NOW:**
- Numbered list of immediate steps customer can take (if applicable)

**WHAT WE'RE DOING:**
- Bullet list of actions on our end

Closing paragraph: Reassurance and invitation to follow up (2 sentences)

**CLOSING:** [Warm, professional, include contact info]

---

CUSTOMER ISSUE:
Customer: Jane Smith
Issue: Unable to access account after password reset, tried 3 times
Impact: Can't access important documents for meeting tomorrow
Customer tone: Frustrated but professional
Solution: Password reset link was going to spam folder, we've whitelisted her domain and sent new link, also offering phone support
```

### Test All Three

1. Create all three emails with specified formatting
2. Compare how format serves each purpose
3. Note which format elements are most important for each type

**Expected Output**:
- Three professionally formatted emails
- Each with appropriate structure for its purpose
- Clear, scannable formatting
- Actionable content

**Validation Prompt**:
```
I created three formatted business emails:

Status update: [paste output]
Meeting follow-up: [paste output]
Customer response: [paste output]

Please assess:
1. Does each email follow its specified format?
2. Is the formatting appropriate for each purpose?
3. Are the emails professional and clear?
4. Would recipients know exactly what to do next?
5. What formatting elements work best in each?
```

### Success Criteria
- [ ] All three emails follow specified formats
- [ ] Format matches purpose and audience
- [ ] Content is clear and actionable
- [ ] Professional tone maintained
- [ ] Easy to scan and understand
- [ ] Next steps are obvious

**Troubleshooting**:
- **Issue**: Emails are too long
  **Solution**: Add word/sentence limits to each section in format spec
- **Issue**: Format is inconsistent between emails
  **Solution**: Create a template format and specify variations for each type

---

## Exercise 5: Presentation Slide Content

**Objective**: Format content specifically for presentation slides

**Scenario**: Create formatted content for a presentation about Q1 results.

### Your Task

Format content for 5 presentation slides with strict formatting rules:

```
Create content for 5 presentation slides about Q1 results.

For each slide, provide:

**SLIDE [NUMBER]: [TITLE]**
(Title: Maximum 6 words, clear and specific)

**CONTENT:**
- 3-5 bullet points maximum
- Each bullet: 1 line, maximum 10 words
- Use strong action words
- Include specific numbers where relevant

**SPEAKER NOTES:**
(2-3 sentences expanding on the bullets)

**VISUAL SUGGESTION:**
(One sentence describing chart, image, or graphic to include)

---

FORMATTING RULES:
- Titles in title case
- Bullets start with action verbs or key terms
- No complete sentences in bullets (phrases only)
- Numbers should stand out
- Keep it scannable - audience should grasp in 3 seconds

---

PRESENTATION DATA:
Topic: Q1 Business Results
Audience: Company all-hands meeting
Key messages:
- Strong growth: 18% revenue increase
- Customer success: 145 new customers, 94% retention
- Product wins: Widget Pro leading, Widget Lite fastest growing
- Regional performance: All regions grew, Northeast leading
- Looking ahead: On track for annual goals, launching 2 new products in Q2

Slides needed:
1. Title/overview slide
2. Revenue and growth slide
3. Customer metrics slide
4. Product performance slide
5. Q2 outlook slide
```

**Expected Output**:
- 5 slides with concise, scannable content
- Strict adherence to bullet point limits
- Clear visual suggestions
- Useful speaker notes
- Professional, presentation-ready format

**Validation Prompt**:
```
I created formatted presentation slide content:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Does each slide follow the strict formatting rules?
2. Are bullets concise enough for slides (not too wordy)?
3. Would the content be readable from the back of a room?
4. Do speaker notes provide helpful expansion?
5. Are visual suggestions practical and relevant?
6. Could this content be used directly in Google Slides?
```

### Success Criteria
- [ ] All 5 slides formatted consistently
- [ ] Bullet points are concise (not full sentences)
- [ ] Titles are clear and under 6 words
- [ ] Speaker notes provide context
- [ ] Visual suggestions are specific
- [ ] Content follows presentation best practices
- [ ] Format is immediately usable

**Troubleshooting**:
- **Issue**: Bullets are too long
  **Solution**: Add stricter limits: "Maximum 8 words per bullet, use phrases not sentences"
- **Issue**: Too much content per slide
  **Solution**: Specify: "Maximum 4 bullets per slide, prefer 3"
- **Issue**: Titles are vague
  **Solution**: Add: "Titles must include specific metric or outcome"

---

## Reflection Questions

1. **How does format specification improve output quality?** Think about clarity, usability, and time saved.

2. **Which format types are most useful for your work?** Consider your daily tasks and communication needs.

3. **What happens when format isn't specified?** Reflect on outputs you've received without format guidance.

4. **How can you create reusable format templates?** Think about your recurring tasks and standard formats.

---

## Key Takeaways

- **Format specifications prevent reformatting work** - Get it right the first time
- **Different purposes need different formats** - Match format to audience and platform
- **Be specific about structure** - Define sections, lengths, and organization
- **Consistency matters** - Specify formatting rules for professional results
- **Templates save time** - Create reusable format specifications for common tasks

---

## Next Steps

Excellent work! You now know how to specify output formats for any business need.

**To continue improving:**

1. **Create format templates** - Build a library for your common tasks
2. **Apply to your work** - Use format specifications in all your prompts this week
3. **Move to Chapter 8** - Learn step-by-step reasoning techniques
4. **Experiment** - Try the same content in different formats to see what works best

**Ready for more?** → [Chapter 8: Step-by-Step Reasoning](../08-step-by-step/lesson.md)

---

## Additional Practice (Optional)

Try creating format specifications for these scenarios:

1. **Product comparison**: Compare 3 products in table format
2. **Weekly newsletter**: Format company updates for email
3. **Training document**: Create structured how-to guide
4. **Performance review**: Format employee feedback professionally
5. **Project proposal**: Structure a business case document

---

## Navigation

- **Previous**: [Lesson 7: Output Formatting and Structure](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 8: Step-by-Step Reasoning](../08-step-by-step/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 7 Complete!** 🎉 You've mastered output formatting!
