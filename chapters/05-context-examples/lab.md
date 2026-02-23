# Lab 5: Providing Context and Examples

← [Lesson 5](lesson.md) | [Home](../../README.md) | [Next: Lab 6 →](../06-instructions-data/lab.md)

---

## Overview

**Chapter**: 5 - Providing Context and Examples  
**Level**: Intermediate  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 5

## Learning Objectives

By completing this lab, you will:
- Practice adding appropriate context to prompts
- Learn to balance context quantity (not too little, not too much)
- Use examples to guide AI output style and format
- Apply context strategies to real business scenarios

## Business Scenario

You're a business professional who needs to create various communications and documents for different audiences. The same information needs to be presented differently depending on who will read it and why. You'll learn how providing the right context and examples helps Gemini tailor outputs to your specific needs, whether you're writing for executives, clients, or team members.

## Materials Needed

- Access to Google Gemini
- Sample quarterly report data (provided below or use your own)
- Sample email from your work (optional for Exercise 4)

---

## Exercise 1: Context Comparison

**Objective**: See how context changes outputs

**Scenario**: You need to summarize a quarterly business report.

### Your Task

Write the same summarization request with three different levels of context:

**Version 1: Minimal Context (Too Little)**
```
Summarize this quarterly report.

Report: Our Q1 revenue was $2.5M, up 15% from Q4. Customer acquisition cost decreased
to $450. We launched two new features and expanded to the European market. Support
tickets increased 30% but resolution time improved by 20%. Team grew from 45 to 52 people.
```

**Version 2: Excessive Context (Too Much)**
```
Summarize this quarterly report. I'm writing this on Tuesday morning and I need it by
noon because I have a meeting at 1 PM in the conference room on the third floor. The
report was compiled by our finance team using data from Salesforce, QuickBooks, and
our internal analytics dashboard. The data was reviewed by three people and approved
last Friday. We use a fiscal calendar that starts in January. Our company was founded
in 2020 and we're in the SaaS industry...

Report: Our Q1 revenue was $2.5M, up 15% from Q4. Customer acquisition cost decreased
to $450. We launched two new features and expanded to the European market. Support
tickets increased 30% but resolution time improved by 20%. Team grew from 45 to 52 people.
```

**Version 3: Balanced Context (Just Right)**
```
Context:
- Audience: Board of directors (need high-level insights, not operational details)
- Purpose: Quarterly board meeting to assess company health and approve Q2 strategy
- Focus: Growth metrics, market expansion success, and any concerns requiring attention
- Format: 3-4 key bullet points, executive-level language

Summarize this quarterly report for the board meeting:

Report: Our Q1 revenue was $2.5M, up 15% from Q4. Customer acquisition cost decreased
to $450. We launched two new features and expanded to the European market. Support
tickets increased 30% but resolution time improved by 20%. Team grew from 45 to 52 people.
```

### Test and Compare

1. Run all three versions in Gemini
2. Compare the outputs
3. Note which version produces the most useful summary

**Expected Output**:
- Version 1: Generic summary, may miss what's important to board
- Version 2: Summary may be confused by irrelevant details
- Version 3: Focused summary highlighting board-level insights with appropriate language

**Validation Prompt**:
```
I'm learning about providing context in prompts. I created three versions of the same
summarization request with different amounts of context:

Version 1 (minimal) output: [paste output]
Version 2 (excessive) output: [paste output]
Version 3 (balanced) output: [paste output]

Please assess:
1. Which version produced the most useful output for a board meeting?
2. How did the different context levels affect the summaries?
3. What made the balanced version more effective?
```

### Success Criteria
- [ ] Created three versions with different context levels
- [ ] Understood how too little context produces generic outputs
- [ ] Recognized how too much context adds confusion
- [ ] Identified the balanced approach as most effective

**Troubleshooting**:
- **Issue**: All three outputs look similar
  **Solution**: Make the context differences more dramatic. In Version 3, be very specific about audience needs and focus areas.
- **Issue**: Version 2 output isn't affected by excessive context
  **Solution**: Add more irrelevant details to Version 2 to show how it can distract from the core task.

---

## Exercise 2: Audience-Specific Context

**Objective**: Tailor the same information for different audiences

**Scenario**: The same quarterly results need to be communicated to three different audiences.

### Your Task

Write three prompts for the same data, each with audience-specific context:

**Prompt 1: For Executive Team**
```
Context:
- Audience: C-suite executives (CEO, CFO, COO)
- Their focus: Strategic implications, financial health, resource allocation decisions
- What they need: High-level insights, trends, red flags, opportunities
- Tone: Professional, strategic, data-driven

Create an executive summary of Q1 results focusing on strategic insights and decisions needed:

Data: Revenue $2.5M (+15%), CAC $450 (-10%), 2 new features launched, European expansion
completed, support tickets +30%, resolution time -20%, team size 45→52.
```

**Prompt 2: For Sales Team**
```
Context:
- Audience: Sales team members
- Their focus: What affects their ability to sell, customer feedback, competitive position
- What they need: Actionable insights, customer trends, product updates they can use
- Tone: Motivational, practical, team-oriented

Create a Q1 update for the sales team highlighting what matters for their work:

Data: Revenue $2.5M (+15%), CAC $450 (-10%), 2 new features launched, European expansion
completed, support tickets +30%, resolution time -20%, team size 45→52.
```

**Prompt 3: For All-Hands Meeting**
```
Context:
- Audience: Entire company (all departments, all levels)
- Their focus: Company progress, team achievements, how their work contributes
- What they need: Celebration of wins, transparency about challenges, sense of momentum
- Tone: Inclusive, celebratory but honest, inspiring

Create Q1 results announcement for all-hands meeting that celebrates achievements and
builds team pride:

Data: Revenue $2.5M (+15%), CAC $450 (-10%), 2 new features launched, European expansion
completed, support tickets +30%, resolution time -20%, team size 45→52.
```

### Test and Compare

1. Run all three prompts
2. Note how the same data is presented differently
3. Identify what makes each appropriate for its audience

**Expected Output**:
- Executive version: Strategic language, focus on decisions and implications
- Sales team version: Practical insights, emphasis on tools and customer impact
- All-hands version: Celebratory tone, inclusive language, team achievements highlighted

**Validation Prompt**:
```
I'm practicing audience-specific context. I created three versions of Q1 results for
different audiences:

Executive team output: [paste output]
Sales team output: [paste output]
All-hands output: [paste output]

Please assess:
1. Does each output appropriately address its audience's needs?
2. Is the tone appropriate for each audience?
3. Does each version emphasize what matters most to that audience?
```

### Success Criteria
- [ ] Created three audience-specific prompts
- [ ] Each prompt includes relevant audience context
- [ ] Outputs differ in tone, focus, and emphasis
- [ ] Each output is appropriate for its intended audience

**Troubleshooting**:
- **Issue**: All three outputs are too similar
  **Solution**: Be more explicit about what each audience cares about. Add specific instructions about tone and focus areas.
- **Issue**: Outputs don't match the intended tone
  **Solution**: Add examples of the tone you want or be more specific (e.g., "Use motivational language" or "Keep it strategic and concise").

---

## Exercise 3: Using Examples to Guide Style

**Objective**: Use examples to establish consistent output style

**Scenario**: You need to write company emails in a consistent style.

### Your Task

Create a prompt that uses examples to guide email style:

**Prompt with Examples**
```
Write a professional email in our company style.

Our style examples:

Example 1 - Meeting invitation:
"Hi team, Let's sync on the Q2 roadmap next Tuesday at 2 PM. I'll share the draft
beforehand so we can dive right into discussion. Coffee and snacks provided! - Alex"

Example 2 - Project update:
"Quick update: The website redesign is 80% complete. Launch is still on track for
March 15. One small delay with the mobile version, but nothing that affects our timeline.
Questions? Ping me anytime. - Alex"

Example 3 - Request for input:
"Hey everyone, I need your thoughts on the new pricing proposal by EOD Friday. It's
a quick read (2 pages). Your input will help us make the final decision next week.
Thanks! - Alex"

Pattern: Friendly but professional, concise, clear action items, casual sign-off

Now write an email announcing a new company policy about remote work. The policy allows
3 days remote per week, requires core hours 10 AM-3 PM for collaboration, and starts
next month.
```

### Test It

1. Run the prompt with examples
2. Check if the output matches the style pattern
3. Try removing the examples and compare the difference

**Expected Output**:
An email that:
- Uses friendly but professional tone
- Is concise and clear
- Includes clear action items or key information
- Has a casual sign-off similar to the examples
- Follows the pattern established by the examples

**Validation Prompt**:
```
I'm learning to use examples to guide AI output style. Here's my prompt with examples:

[Paste your prompt]

And here's the output I received:
[Paste output]

Please assess:
1. Does the output match the style pattern from the examples?
2. Is the tone consistent with the examples (friendly but professional)?
3. Does it follow the structural pattern (concise, clear, casual sign-off)?
4. Would this fit naturally with the example emails?
```

### Success Criteria
- [ ] Included 2-3 clear style examples
- [ ] Identified the pattern in the examples
- [ ] Output matches the established style
- [ ] Understood how examples guide AI behavior

**Troubleshooting**:
- **Issue**: Output doesn't match the example style
  **Solution**: Add a clear statement of the pattern (e.g., "Pattern: friendly tone, bullet points, casual sign-off"). Make the pattern more explicit.
- **Issue**: Examples are too different from each other
  **Solution**: Ensure your examples share common characteristics. They should demonstrate a consistent style pattern.

---

## Exercise 4: Business Email with Company Tone

**Objective**: Apply context and examples to real business communication

**Scenario**: Draft a follow-up email to a client after a proposal meeting.

### Your Task

Write a complete prompt with context and examples:

```
Context:
- Recipient: Sarah Chen, IT Director at MedTech Solutions
- Relationship: Potential client, met twice, friendly and professional rapport
- Meeting: Yesterday's proposal presentation for our project management software
- Their situation: Currently using outdated system, frustrated with lack of integration
- Their concerns: Implementation timeline, training requirements, data migration
- Our advantage: Proven healthcare industry experience, smooth migration process
- Goal: Move to next step (technical demo with their team)
- Tone: Professional but warm, confident but not pushy

Company email style examples:

Example 1: "Hi Michael, Great connecting at the conference! I've been thinking about
the integration challenges you mentioned. I'd love to show you how we solved similar
issues for other clients. Are you free for a quick call next week? Best, Jordan"

Example 2: "Hi Lisa, Thanks for the productive meeting yesterday. As promised, I'm
attaching the case study from the retail client we discussed. I think you'll find
the ROI timeline particularly relevant. Let me know if you have questions! Best, Jordan"

Write a follow-up email to Sarah that:
- Thanks her for yesterday's meeting
- Addresses her top concern (implementation timeline)
- References our healthcare experience
- Proposes next step (technical demo)
- Includes a specific call-to-action
```

**Expected Output**:
A complete email that:
- Matches the company style (professional but warm)
- Includes all required elements (thanks, addresses concern, proposes next step)
- Has appropriate tone for the relationship
- Includes clear call-to-action
- Feels natural and not overly formal

**Validation Prompt**:
```
I'm practicing writing business emails with proper context and style examples.
Here's my prompt:

[Paste your complete prompt]

And here's the email Gemini generated:
[Paste the email output]

Please assess:
1. Does the email include all required elements?
2. Is the tone appropriate for the relationship and situation?
3. Does it match the company style from the examples?
4. Is the call-to-action clear and appropriate?
5. Would this email effectively move the sales process forward?
```

### Success Criteria
- [ ] Included comprehensive context (recipient, relationship, situation, goal)
- [ ] Provided style examples showing company tone
- [ ] Specified all required email elements
- [ ] Output is professional, warm, and actionable
- [ ] Email would be effective in real business situation

**Troubleshooting**:
- **Issue**: Email is too formal or stiff
  **Solution**: Emphasize "warm" and "not pushy" in the tone description. Add more casual examples.
- **Issue**: Email doesn't address the client's concerns
  **Solution**: Be more explicit: "Must specifically mention implementation timeline and our experience with smooth migrations."
- **Issue**: Call-to-action is vague
  **Solution**: Specify exactly what you want: "Propose a 30-minute technical demo next week with specific date options."

---

## Exercise 5: Quarterly Report for Different Audiences

**Objective**: Master context for complex business scenarios

**Scenario**: Create two versions of a quarterly report summary for different stakeholders.

### Your Task

Write two prompts with different audience contexts:

**Prompt 1: For Board of Directors**
```
Context:
- Audience: Board of directors (external advisors, investors, non-operational)
- Their knowledge: High-level company strategy, not day-to-day operations
- Their concerns: Financial health, strategic direction, major risks, growth trajectory
- Their time: Very limited, need concise insights
- Decision impact: Approve budget, strategic initiatives, major hires
- Format: Executive summary, 4-5 key points maximum
- Tone: Professional, strategic, data-driven, confident

Summarize this quarterly report for the board meeting:

Q2 Results:
- Revenue: $3.2M (target was $3M)
- New customers: 45 (target was 40)
- Churn rate: 3.5% (down from 5%)
- Product: Launched AI features, 60% adoption by existing customers
- Team: Hired VP of Sales, engineering team grew 20%
- Market: Competitor X raised $50M, Competitor Y launched similar features
- Challenges: Customer support response time increased to 8 hours (target is 4)
- Cash: $8M runway, 16 months at current burn rate

Focus on: What the board needs to know and decide.
```

**Prompt 2: For Department Heads**
```
Context:
- Audience: Department heads (Sales, Engineering, Marketing, Support, Operations)
- Their knowledge: Deep operational knowledge, need cross-functional insights
- Their concerns: How their department performed, dependencies, resource needs
- Their time: Will read in detail, want actionable insights
- Decision impact: Quarterly planning, resource allocation, cross-team coordination
- Format: Detailed summary with department-specific insights
- Tone: Collaborative, operational, action-oriented

Summarize this quarterly report for the department heads meeting:

Q2 Results:
- Revenue: $3.2M (target was $3M)
- New customers: 45 (target was 40)
- Churn rate: 3.5% (down from 5%)
- Product: Launched AI features, 60% adoption by existing customers
- Team: Hired VP of Sales, engineering team grew 20%
- Market: Competitor X raised $50M, Competitor Y launched similar features
- Challenges: Customer support response time increased to 8 hours (target is 4)
- Cash: $8M runway, 16 months at current burn rate

Focus on: Cross-functional insights and operational implications for each department.
```

### Test and Compare

1. Run both prompts
2. Compare how the same data is presented
3. Note what each version emphasizes

**Expected Output**:
- Board version: High-level strategic insights, financial health, major decisions needed, very concise
- Department heads version: Operational details, cross-functional impacts, specific action areas, more detailed

**Validation Prompt**:
```
I'm practicing creating audience-specific reports. Here are my two versions:

Board of directors output: [paste output]
Department heads output: [paste output]

Please assess:
1. Does the board version focus on strategic, high-level insights?
2. Does the department heads version include operational details?
3. Is each version appropriate for its audience's needs and time constraints?
4. Would each version help its audience make the right decisions?
```

### Success Criteria
- [ ] Created two distinct audience contexts
- [ ] Board version is concise and strategic
- [ ] Department heads version is detailed and operational
- [ ] Each version emphasizes what matters to that audience
- [ ] Understood how context shapes the same information differently

**Troubleshooting**:
- **Issue**: Both outputs are too similar
  **Solution**: Make the audience differences more explicit. Emphasize "concise, strategic" for board and "detailed, operational" for department heads.
- **Issue**: Board version is too detailed
  **Solution**: Add "maximum 4-5 key points" and "they have very limited time" to the context.
- **Issue**: Department heads version lacks actionable insights
  **Solution**: Add "include specific implications for each department" and "what actions are needed."

---

## Reflection Questions

1. **How did adding context change the quality of outputs?** Think about specificity, relevance, and usefulness.

2. **What types of context were most important for your work tasks?** Consider audience, purpose, tone, or background.

3. **How did examples help guide AI behavior?** Reflect on the difference between describing style and showing examples.

4. **When is it worth providing extensive context vs. keeping it brief?** Think about task complexity and output importance.

---

## Key Takeaways

- **Context shapes everything** - Same task, different context = different results
- **Balance is crucial** - Enough context to guide, not so much it confuses
- **Audience matters most** - Who will use this determines what context to include
- **Examples teach patterns** - Showing is more effective than telling
- **Purpose drives focus** - Why you're creating something determines what to emphasize

---

## Next Steps

**Ready for more?** → [Chapter 6: Separating Instructions from Data](../06-instructions-data/lesson.md)

---

**Lab 5 Complete!** 🎉

