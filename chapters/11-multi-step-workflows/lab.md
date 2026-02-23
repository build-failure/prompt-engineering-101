# Lab 11: Multi-Step Workflows and Prompt Chaining

← [Lesson 11](lesson.md) | [Home](../../README.md) | [Next: Lab 12 →](../12-troubleshooting/lab.md)

---

## Overview

**Chapter**: 11 - Multi-Step Workflows and Prompt Chaining  
**Level**: Advanced  
**Estimated Time**: 35 minutes  
**Prerequisites**: Complete Lesson 11

## Learning Objectives

By completing this lab, you will:
- Practice breaking complex tasks into multiple steps
- Learn to chain prompts effectively
- Master workflow design patterns
- Apply multi-step approaches to real business scenarios

## Business Scenario

Many business tasks are too complex for a single prompt. You need to analyze data, generate insights, create presentations, and communicate results - each requiring different approaches. You'll learn to design and execute multi-step workflows that produce higher quality results than single-prompt approaches.

## Materials Needed

- Access to Google Gemini
- Sample data and scenarios provided
- Notepad or document to track outputs between steps

---

## Exercise 1: Sequential Workflow - Data to Presentation

**Objective**: Chain prompts to transform raw data into presentation content

**Scenario**: You have quarterly sales data that needs to become an executive presentation.

### Your Task

Execute this 4-step workflow:

**Step 1: Data Analysis**
```
Analyze this Q1 sales data and identify key findings:

DATA:
- Total Revenue: $2.5M (Q4 was $2.1M)
- New Customers: 145 (target was 120)
- Customer Retention: 94% (Q4 was 89%)
- Average Deal Size: $17,200 (Q4 was $15,800)
- Sales Cycle: 32 days (Q4 was 38 days)

Product Performance:
- Widget Pro: $890K revenue (35% of total), 52 customers
- Widget Plus: $675K revenue (27% of total), 89 customers
- Widget Lite: $560K revenue (22% of total), 156 customers
- Widget Enterprise: $375K revenue (15% of total), 12 customers

Regional Performance:
- Northeast: $750K (30%), up 25% from Q4
- West: $625K (25%), up 15% from Q4
- South: $575K (23%), up 12% from Q4
- Midwest: $550K (22%), up 8% from Q4

Provide:
1. Top 3 positive findings
2. Top 2 areas of concern
3. Most significant trend
```

**Step 2: Insight Generation**
```
Based on this analysis, generate strategic insights:

[PASTE STEP 1 OUTPUT HERE]

For each finding, explain:
- Why this is happening (likely causes)
- What it means for the business
- What we should do about it

Format as:
Finding → Cause → Implication → Recommendation
```

**Step 3: Presentation Outline**
```
Create a 10-slide presentation outline for executives:

Content to include:
[PASTE STEP 2 OUTPUT HERE]

Structure:
- Slide 1: Title and key message
- Slides 2-4: Top findings (one per slide)
- Slides 5-7: Strategic insights
- Slides 8-9: Recommendations
- Slide 10: Next steps and Q2 outlook

For each slide, provide:
- Slide title (compelling, specific)
- Key message (one sentence)
- 3-4 supporting points
```

**Step 4: Slide Content**
```
For slides 2, 5, and 8 from this outline, create detailed content:

[PASTE RELEVANT SLIDES FROM STEP 3]

For each slide, provide:
- Title
- 3-4 bullet points (max 10 words each)
- Key visual suggestion (chart type and data to show)
- Speaker notes (2-3 sentences)

Keep bullets scannable - phrases not sentences.
```

### Execute the Workflow

1. Run Step 1, save the output
2. Use Step 1 output in Step 2, save that output
3. Use Step 2 output in Step 3, save that output
4. Use Step 3 output in Step 4
5. Review the final presentation content

**Expected Output**:
- Step 1: Clear analysis with findings
- Step 2: Strategic insights with recommendations
- Step 3: Complete 10-slide outline
- Step 4: Detailed content for 3 slides

**Validation Prompt**:
```
I executed a 4-step workflow from data to presentation:

Step 1 (Analysis): [paste output]
Step 2 (Insights): [paste output]
Step 3 (Outline): [paste output]
Step 4 (Detailed slides): [paste output]

Please assess:
1. Does each step build logically on the previous?
2. Is information carried forward appropriately?
3. Is the final output presentation-ready?
4. What improved by using multiple steps vs. one prompt?
5. Could any steps be combined or should any be split?
```

### Success Criteria
- [ ] Completed all 4 steps in sequence
- [ ] Each step used output from previous step
- [ ] Information flowed logically through workflow
- [ ] Final output is higher quality than single-prompt approach
- [ ] Understood when to break vs. combine steps

**Troubleshooting**:
- **Issue**: Lost important details between steps
  **Solution**: Be more selective about what to pass forward - include key findings but not all raw data
- **Issue**: Steps feel disconnected
  **Solution**: Add context in each prompt: "Based on the previous analysis showing..."

---

## Exercise 2: Iterative Workflow - Document Refinement

**Objective**: Use iteration to improve a document through multiple passes

**Scenario**: You need to create a high-quality project proposal through drafting and refinement.

### Your Task

Execute this iterative workflow:

**Step 1: Initial Draft**
```
Draft a project proposal for implementing a new customer feedback system.

Include:
- Problem statement (what issue we're solving)
- Proposed solution (what we'll build)
- Benefits (why it matters)
- Timeline (high-level phases)
- Budget estimate (rough range)

Audience: VP of Product
Length: 400-500 words
Tone: Professional, persuasive

Context:
- Current feedback is scattered across email, support tickets, social media
- No centralized way to track or analyze feedback
- Product team struggles to prioritize features
- Budget available: $50K-$100K
- Timeline: Need to launch in 6 months
```

**Step 2: Critical Review**
```
Review this proposal draft and identify improvements:

[PASTE STEP 1 OUTPUT HERE]

Evaluate:
1. Clarity - Is the problem and solution clear?
2. Persuasiveness - Is the case compelling?
3. Completeness - Is anything missing?
4. Structure - Is it well-organized?
5. Tone - Is it appropriate for VP audience?

For each area, provide:
- Current state (what's there now)
- Issues (what's not working)
- Suggestions (specific improvements)
```

**Step 3: Revision**
```
Revise the proposal based on this feedback:

ORIGINAL DRAFT:
[PASTE STEP 1 OUTPUT]

FEEDBACK:
[PASTE STEP 2 OUTPUT]

Create an improved version that:
- Addresses all feedback points
- Maintains the same structure and length
- Strengthens weak areas
- Keeps what's working well
```

**Step 4: Final Polish**
```
Polish this revised proposal for final submission:

[PASTE STEP 3 OUTPUT]

Check and improve:
- Grammar and punctuation
- Word choice (stronger verbs, clearer nouns)
- Flow and transitions
- Impact of opening and closing
- Professional tone consistency

Make it shine while keeping the same content and structure.
```

### Execute the Workflow

1. Generate initial draft (Step 1)
2. Get critical review (Step 2)
3. Revise based on feedback (Step 3)
4. Final polish (Step 4)
5. Compare final to initial draft

**Expected Output**:
- Step 1: Solid first draft
- Step 2: Constructive feedback
- Step 3: Improved version addressing feedback
- Step 4: Polished, professional final version

**Validation Prompt**:
```
I used an iterative workflow to refine a proposal:

Initial draft: [paste Step 1]
Review feedback: [paste Step 2]
Revised version: [paste Step 3]
Final polished: [paste Step 4]

Please assess:
1. How did the document improve through iterations?
2. Was the feedback in Step 2 actionable?
3. Did Step 3 effectively address the feedback?
4. What's the quality difference between first and final?
5. Is this approach better than trying to write perfectly in one shot?
```

### Success Criteria
- [ ] Each iteration improved the document
- [ ] Feedback was specific and actionable
- [ ] Revisions addressed the feedback
- [ ] Final version is significantly better than first draft
- [ ] Understood value of iterative refinement

**Troubleshooting**:
- **Issue**: Feedback is too vague
  **Solution**: In Step 2, ask for "specific examples and concrete suggestions"
- **Issue**: Revision doesn't address feedback
  **Solution**: In Step 3, explicitly reference each feedback point: "Addressing clarity issue..."

---

## Exercise 3: Branching Workflow - Multi-Audience Communication

**Objective**: Create multiple outputs from one source for different audiences

**Scenario**: You need to communicate new product features to three different audiences.

### Your Task

Execute this branching workflow:

**Step 1: Core Content (Source)**
```
Extract the key information about our new product features:

PRODUCT UPDATE:
We're launching three new features next month:

1. Automated Reporting: System automatically generates weekly performance reports
   - Saves 5 hours per week per user
   - Customizable templates
   - Scheduled delivery
   - Cost: Included in Pro plan

2. Team Collaboration: Real-time co-editing and commenting
   - Multiple users can work simultaneously
   - In-line comments and suggestions
   - Version history
   - Cost: Included in Team plan

3. API Access: Programmatic access to all platform features
   - RESTful API
   - Comprehensive documentation
   - Rate limits: 1000 calls/hour
   - Cost: $500/month add-on

Create a structured summary with:
- Feature name
- What it does (one sentence)
- Key benefits (2-3 bullets)
- Who it's for
- Availability/cost
```

**Step 2a: Executive Communication**
```
Using this feature information, create an executive summary:

[PASTE STEP 1 OUTPUT]

Format: Email to C-suite
Focus on:
- Strategic value
- Business impact
- Competitive advantage
- Revenue implications

Length: 150 words
Tone: Strategic, high-level, business-focused
```

**Step 2b: Customer Communication**
```
Using this feature information, create a customer announcement:

[PASTE STEP 1 OUTPUT]

Format: Email to existing customers
Focus on:
- How it helps them
- What they can do now
- How to get started
- Excitement and value

Length: 200 words
Tone: Friendly, benefit-focused, enthusiastic
```

**Step 2c: Team Communication**
```
Using this feature information, create a team briefing:

[PASTE STEP 1 OUTPUT]

Format: Internal team update
Focus on:
- What's launching
- Support implications
- Common questions to expect
- Resources and training

Length: 250 words
Tone: Informative, practical, supportive
```

### Execute the Workflow

1. Create core content summary (Step 1)
2. Run all three branches in parallel:
   - Executive version (Step 2a)
   - Customer version (Step 2b)
   - Team version (Step 2c)
3. Compare how same information is presented differently

**Expected Output**:
- Step 1: Structured feature summary
- Step 2a: Strategic executive email
- Step 2b: Benefit-focused customer email
- Step 2c: Practical team briefing

**Validation Prompt**:
```
I created three versions of the same product update:

Core content: [paste Step 1]
Executive version: [paste Step 2a]
Customer version: [paste Step 2b]
Team version: [paste Step 2c]

Please assess:
1. Does each version appropriately adapt for its audience?
2. Is the tone right for each audience?
3. Does each focus on what matters to that audience?
4. Is core information consistent across versions?
5. What makes each version effective for its purpose?
```

### Success Criteria
- [ ] Core content captured all key information
- [ ] Each branch adapted appropriately for audience
- [ ] Tone and focus varied correctly
- [ ] Core facts remained consistent
- [ ] Understood value of audience-specific communication

**Troubleshooting**:
- **Issue**: Versions are too similar
  **Solution**: Be more explicit about audience needs and priorities in each branch prompt
- **Issue**: Inconsistent information across versions
  **Solution**: Use exact same Step 1 output in all branches, don't paraphrase

---

## Exercise 4: Convergent Workflow - Comprehensive Analysis

**Objective**: Combine multiple inputs into one synthesized output

**Scenario**: You have feedback from three sources that need to be synthesized into recommendations.

### Your Task

Execute this convergent workflow:

**Step 1a: Analyze Customer Feedback**
```
Analyze this customer feedback and identify top 3 themes:

FEEDBACK:
- "Love the new dashboard but it's slow to load"
- "Mobile app needs dark mode"
- "Reporting features are exactly what we needed"
- "Dashboard takes forever on mobile"
- "Please add dark mode to mobile app"
- "Reports are great but need more export options"
- "Mobile app is slow and needs dark theme"
- "Dashboard performance is poor"
- "Export reports to Excel would be helpful"
- "Mobile app desperately needs dark mode"

For each theme:
- What customers are saying
- How many mentioned it
- Severity/importance
```

**Step 1b: Analyze Sales Team Input**
```
Analyze this sales team input and identify top 3 priorities:

SALES FEEDBACK:
- "Losing deals because we don't have mobile dark mode"
- "Prospects ask about dashboard performance in demos"
- "Excel export is requested in 80% of sales calls"
- "Mobile app speed is a common objection"
- "Dark mode is a deal-breaker for some prospects"
- "Dashboard loading time hurts demos"
- "Need better export options to close enterprise deals"

For each priority:
- What sales team is reporting
- Business impact
- Frequency
```

**Step 1c: Analyze Usage Data**
```
Analyze this usage data and identify top 3 insights:

USAGE DATA:
- Dashboard page: 45% bounce rate (industry average: 25%)
- Dashboard load time: 8.2 seconds (target: <3 seconds)
- Mobile app sessions: 35% of total usage
- Mobile app: 60% of users access between 6PM-10PM
- Report exports: 2,300 requests/month (growing 15%/month)
- Export format requests: Excel (78%), PDF (15%), CSV (7%)
- Mobile app ratings: 3.2/5 (desktop app: 4.5/5)

For each insight:
- What the data shows
- Why it matters
- Trend direction
```

**Step 2: Synthesize All Sources**
```
Synthesize insights from all three sources:

CUSTOMER FEEDBACK:
[PASTE STEP 1a OUTPUT]

SALES INPUT:
[PASTE STEP 1b OUTPUT]

USAGE DATA:
[PASTE STEP 1c OUTPUT]

Create a unified analysis:
1. What are the top 3 priorities across all sources?
2. How do the sources support each other?
3. Are there any conflicts or contradictions?
4. What's the strongest evidence for each priority?

Format as:
Priority 1: [Name]
- Customer evidence: [summary]
- Sales evidence: [summary]
- Data evidence: [summary]
- Overall strength: High/Medium/Low

[Repeat for priorities 2 and 3]
```

**Step 3: Generate Recommendations**
```
Based on this synthesized analysis, create actionable recommendations:

[PASTE STEP 2 OUTPUT]

For each priority, recommend:
- Specific action to take
- Expected impact
- Effort required (low/medium/high)
- Timeline (quick win / 1 month / 1 quarter)
- Success metrics

Format as table:
| Priority | Action | Impact | Effort | Timeline | Success Metric |

Then provide:
- Recommended sequence (what to do first, second, third)
- Rationale for the sequence
```

### Execute the Workflow

1. Analyze each source separately (Steps 1a, 1b, 1c)
2. Synthesize all sources (Step 2)
3. Generate recommendations (Step 3)
4. Review how multiple inputs led to stronger recommendations

**Expected Output**:
- Steps 1a-c: Individual source analyses
- Step 2: Unified synthesis showing patterns
- Step 3: Prioritized, actionable recommendations

**Validation Prompt**:
```
I used a convergent workflow to synthesize multiple inputs:

Customer analysis: [paste Step 1a]
Sales analysis: [paste Step 1b]
Data analysis: [paste Step 1c]
Synthesis: [paste Step 2]
Recommendations: [paste Step 3]

Please assess:
1. Did the synthesis effectively combine all sources?
2. Are priorities supported by multiple sources?
3. Are recommendations actionable and specific?
4. Is the evidence stronger than using just one source?
5. Is the recommended sequence logical?
```

### Success Criteria
- [ ] Analyzed each source independently
- [ ] Synthesis identified cross-source patterns
- [ ] Recommendations based on combined evidence
- [ ] Priorities supported by multiple sources
- [ ] Understood value of multi-source analysis

**Troubleshooting**:
- **Issue**: Synthesis just lists sources separately
  **Solution**: In Step 2, explicitly ask "What patterns appear across all sources?"
- **Issue**: Recommendations don't reflect synthesis
  **Solution**: In Step 3, reference specific evidence from Step 2 for each recommendation

---

## Exercise 5: Complete Workflow Design

**Objective**: Design and execute your own workflow for a complex task

**Scenario**: Design a workflow to turn meeting notes into multiple outputs.

### Your Task

**Phase 1: Design the Workflow**

Given this goal: "Transform raw meeting notes into organized documentation and communications"

Design a workflow that produces:
1. Formal meeting minutes
2. Action item tracker
3. Team email summary
4. Executive brief

Map out:
- How many steps needed?
- What's the sequence?
- What passes between steps?
- Any parallel branches?

**Phase 2: Create the Prompts**

Write the actual prompts for each step in your workflow.

**Phase 3: Execute the Workflow**

Use these meeting notes:

```
MEETING NOTES - Product Planning 3/28/24
Attendees: Sarah (PM), Mike (Eng), Jen (Design), Tom (Marketing)

Sarah: Q2 goals - launch mobile app, improve dashboard performance, add dark mode
Mike: Mobile app on track for May 15, dashboard performance needs 3 weeks, dark mode is quick (1 week)
Jen: Have dark mode designs ready, mobile app designs 90% done, need feedback on onboarding flow
Tom: Need 2 weeks lead time for launch marketing, want to coordinate with mobile app launch

Decisions:
- Launch mobile app May 15
- Add dark mode in April (quick win)
- Dashboard performance improvements by May 1
- Marketing campaign starts May 1

Action items:
- Mike: Complete dashboard performance work by May 1
- Jen: Finalize mobile app designs by April 5, share onboarding flow by April 1
- Tom: Prepare marketing campaign, launch May 1
- Sarah: Coordinate with all teams, weekly check-ins

Questions:
- Do we have budget for paid ads? (Sarah to check with finance)
- Should we do beta testing for mobile app? (Team to discuss next meeting)

Next meeting: April 4, 2PM - Review progress and decide on beta testing
```

Execute your workflow and produce all four outputs.

**Expected Output**:
- Workflow design document
- All prompts written
- All four outputs generated
- Reflection on workflow effectiveness

**Validation Prompt**:
```
I designed and executed a custom workflow:

Workflow design: [describe your steps and logic]

Prompts used: [paste all prompts]

Outputs produced:
1. Meeting minutes: [paste]
2. Action tracker: [paste]
3. Team email: [paste]
4. Executive brief: [paste]

Please assess:
1. Is the workflow design logical and efficient?
2. Are the prompts well-structured?
3. Do the outputs meet their purposes?
4. Could the workflow be improved?
5. What did I learn about workflow design?
```

### Success Criteria
- [ ] Designed a logical workflow
- [ ] Created clear prompts for each step
- [ ] Executed the complete workflow
- [ ] Produced all required outputs
- [ ] Reflected on workflow effectiveness
- [ ] Can apply workflow design to other tasks

**Troubleshooting**:
- **Issue**: Not sure how many steps to use
  **Solution**: Start with major phases (extract → organize → format → communicate), then break down if needed
- **Issue**: Outputs are inconsistent
  **Solution**: Ensure each step passes forward the necessary context from previous steps

---

## Reflection Questions

1. **When is a multi-step workflow better than a single prompt?** Think about complexity, quality, and control.

2. **What workflow patterns did you find most useful?** Sequential, iterative, branching, or convergent?

3. **How do you decide what to pass between steps?** What information is essential vs. what can be left behind?

4. **What's the right balance between too many and too few steps?** How do you find it?

---

## Key Takeaways

- **Complex tasks benefit from multiple steps** - Don't force everything into one prompt
- **Design workflows before executing** - Plan the sequence and handoffs
- **Pass context forward strategically** - Include what's needed, exclude what's not
- **Different patterns serve different needs** - Sequential, iterative, branching, convergent
- **Quality improves with workflow approach** - Each step can focus on doing one thing well

---

## Next Steps

Excellent work! You now know how to design and execute complex multi-step workflows.

**To continue improving:**

1. **Map your recurring tasks** - Identify which would benefit from workflows
2. **Create workflow templates** - Document successful patterns for reuse
3. **Move to Chapter 12** - Learn troubleshooting and debugging techniques
4. **Practice workflow design** - The more you do it, the better you'll get

**Ready for the final chapter?** → [Chapter 12: Troubleshooting and Debugging](../12-troubleshooting/lesson.md)

---

## Additional Practice (Optional)

Try designing workflows for these scenarios:

1. **Customer feedback → Product roadmap**: Analyze feedback, prioritize features, create roadmap
2. **Data → Report → Presentation → Email**: Complete reporting workflow
3. **Research → Analysis → Recommendations → Implementation plan**: Strategic planning workflow
4. **Draft → Review → Revise → Approve**: Document approval workflow
5. **Brainstorm → Evaluate → Select → Plan**: Decision-making workflow

---

## Navigation

- **Previous**: [Lesson 11: Multi-Step Workflows and Prompt Chaining](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 12: Troubleshooting and Debugging](../12-troubleshooting/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 11 Complete!** 🎉 You've mastered multi-step workflows!
