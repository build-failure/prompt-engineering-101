# Lab 8: Step-by-Step Reasoning

← [Lesson 8](lesson.md) | [Home](../../README.md) | [Next: Lab 9 →](../09-few-shot-learning/lab.md)

---

## Overview

**Chapter**: 8 - Step-by-Step Reasoning  
**Level**: Intermediate  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 8

## Learning Objectives

By completing this lab, you will:
- Practice requesting step-by-step reasoning
- Learn when chain-of-thought improves accuracy
- Apply reasoning techniques to complex problems
- Master structured analysis frameworks

## Business Scenario

Many business decisions require careful analysis of multiple factors. Instead of getting quick answers, you need to see the thinking process to make informed decisions. You'll learn to request and evaluate step-by-step reasoning for complex business problems.

## Materials Needed

- Access to Google Gemini
- Sample scenarios provided
- Notepad to evaluate reasoning quality

---

## Exercise 1: Basic Step-by-Step Request

**Objective**: Compare outputs with and without step-by-step reasoning

**Scenario**: You're deciding whether to hire a new team member.

### Your Task

**Version A: Without Step-by-Step**
```
Should we hire a new marketing manager?

Context:
- Current team: 2 marketing coordinators
- Budget: $80K available
- Revenue: $3M annually, growing 20% per year
- Current challenge: Struggling to execute all planned campaigns
```

**Version B: With Step-by-Step**
```
Should we hire a new marketing manager?

Context:
- Current team: 2 marketing coordinators
- Budget: $80K available
- Revenue: $3M annually, growing 20% per year
- Current challenge: Struggling to execute all planned campaigns

Think through this step by step:
1. Assess the current situation and pain points
2. Evaluate if a marketing manager would solve these issues
3. Consider the costs vs. benefits
4. Explore alternative solutions
5. Make a recommendation with rationale
```

### Test Both Versions

1. Run Version A in Gemini
2. Run Version B in Gemini
3. Compare the outputs

**Expected Difference**:
- Version A: Quick yes/no answer with brief reasoning
- Version B: Detailed analysis showing thought process, considering multiple angles

**Validation Prompt**:
```
I'm comparing outputs with and without step-by-step reasoning:

Version A (no steps): [paste output]
Version B (with steps): [paste output]

Please assess:
1. Which output is more useful for making a decision?
2. What additional insights did step-by-step provide?
3. Can I follow the reasoning in Version B?
4. Which would I trust more and why?
```

### Success Criteria
- [ ] Ran both versions
- [ ] Noticed significant difference in depth
- [ ] Version B showed clear reasoning process
- [ ] Understood when step-by-step adds value

**Troubleshooting**:
- **Issue**: Both outputs look similar
  **Solution**: Make the problem more complex or add conflicting factors
- **Issue**: Step-by-step output is too long
  **Solution**: Add constraint: "Keep each step to 2-3 sentences"

---

## Exercise 2: Vendor Selection Analysis

**Objective**: Use step-by-step reasoning for multi-criteria decisions

**Scenario**: Choose between three project management tools for your team.

### Your Task

Create a step-by-step prompt to analyze this decision:

```
Help me choose between these three project management tools: Asana, Monday.com, and ClickUp.

Team context:
- 15 people across 3 departments
- Budget: $500/month maximum
- Current pain: Using spreadsheets, losing track of tasks
- Technical skill: Mixed (some tech-savvy, some not)
- Key needs: Task management, timeline views, team collaboration

Tool information:
- Asana: $10.99/user/month, strong task management, good mobile app
- Monday.com: $8/user/month, very visual, customizable workflows
- ClickUp: $5/user/month, feature-rich, steeper learning curve

Analyze this decision step by step:

1. Define evaluation criteria
   - What factors matter most for our team?
   - How should we weight each factor?

2. Score each tool
   - Rate each tool on our criteria (1-10 scale)
   - Note standout strengths and weaknesses

3. Calculate costs
   - Total monthly cost for 15 users
   - Any setup or training costs
   - Does it fit our budget?

4. Consider implementation
   - How easy is onboarding?
   - What's the learning curve?
   - Do we need training?

5. Assess risks
   - What could go wrong with each option?
   - How locked-in would we be?
   - What if the team doesn't adopt it?

6. Make recommendation
   - Which tool is best for us?
   - Why is it the best choice?
   - What's the implementation plan?
```

### Execute and Evaluate

1. Run your prompt in Gemini
2. Review each step of the reasoning
3. Check if any important factors were missed

**Expected Output**:
- Clear evaluation criteria
- Systematic scoring of each tool
- Cost analysis showing Monday.com fits budget best
- Implementation considerations
- Risk assessment
- Specific recommendation with rationale

**Validation Prompt**:
```
I used step-by-step reasoning for vendor selection:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Did the analysis cover all important factors?
2. Is the scoring methodology sound?
3. Does the recommendation follow logically from the analysis?
4. What factors might have been overlooked?
5. Would this analysis help me make a confident decision?
```

### Success Criteria
- [ ] Created structured step-by-step framework
- [ ] Each step has clear purpose
- [ ] Analysis is systematic and thorough
- [ ] Recommendation is well-supported
- [ ] Can follow and validate the reasoning

**Troubleshooting**:
- **Issue**: Analysis is too superficial
  **Solution**: Add more specific questions in each step: "For each tool, rate on scale of 1-10 with explanation"
- **Issue**: Missing important factors
  **Solution**: Add step: "What other factors should we consider that weren't mentioned?"

---

## Exercise 3: Problem Diagnosis

**Objective**: Use step-by-step reasoning to diagnose business problems

**Scenario**: Your website conversion rate has dropped significantly.

### Your Task

Create a diagnostic prompt with step-by-step reasoning:

```
Our website conversion rate dropped from 3.2% to 1.8% over the past month.

Diagnose this problem step by step:

1. Identify what changed
   - When exactly did the drop occur?
   - What changes did we make to the website?
   - What external factors changed (seasonality, competition, market)?

2. Analyze the data
   - Is the drop across all pages or specific pages?
   - Are certain user segments more affected?
   - What does the funnel analysis show?
   - Where are users dropping off?

3. Generate hypotheses
   - What are the possible causes?
   - Which causes are most likely based on the data?
   - What evidence supports each hypothesis?

4. Prioritize investigation
   - Which hypotheses should we test first?
   - What data would confirm or rule out each hypothesis?
   - What's the quickest way to validate?

5. Recommend next steps
   - What should we investigate immediately?
   - What tests should we run?
   - What fixes should we try?
   - How will we measure if the fix works?

Additional context:
- We redesigned the checkout page on March 15
- Added a new required field (phone number) to the form
- Increased prices by 10% on March 20
- Competitor launched a promotion on March 18
- Traffic volume is unchanged
```

### Execute and Evaluate

1. Run your diagnostic prompt
2. Review the reasoning at each step
3. Check if the diagnosis makes sense

**Expected Output**:
- Timeline of changes identified
- Data analysis showing checkout page is the problem
- Hypothesis that new required field is causing friction
- Prioritized investigation plan
- Specific recommendations (A/B test removing phone field)

**Validation Prompt**:
```
I used step-by-step reasoning to diagnose a problem:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Did the diagnosis follow a logical process?
2. Were all relevant factors considered?
3. Is the root cause identification convincing?
4. Are the recommended next steps actionable?
5. What would make this diagnosis stronger?
```

### Success Criteria
- [ ] Diagnostic framework is systematic
- [ ] Each step builds on previous findings
- [ ] Root cause is identified with evidence
- [ ] Recommendations are specific and testable
- [ ] Can validate the reasoning

**Troubleshooting**:
- **Issue**: Jumps to conclusion too quickly
  **Solution**: Add: "Consider at least 3 possible causes before selecting the most likely"
- **Issue**: Doesn't use the provided context
  **Solution**: Add: "Reference the specific changes mentioned in the context"

---

## Exercise 4: Strategic Planning

**Objective**: Break down a goal into actionable steps

**Scenario**: Your company wants to increase customer retention from 85% to 92%.

### Your Task

Create a planning prompt with step-by-step reasoning:

```
We want to increase customer retention from 85% to 92% over the next 6 months.

Create a strategic plan using step-by-step reasoning:

1. Understand the current state
   - Why are 15% of customers leaving?
   - What are the common reasons for churn?
   - Which customer segments have highest churn?

2. Define the target state
   - What does 92% retention mean in numbers?
   - How many customers do we need to retain?
   - What's the business impact of this improvement?

3. Identify key drivers
   - What factors most influence retention?
   - What do high-retention customers have in common?
   - What can we control vs. what we can't?

4. Generate initiatives
   - What actions could improve retention?
   - Which initiatives address the biggest churn reasons?
   - What resources would each initiative require?

5. Prioritize initiatives
   - Which initiatives have highest impact?
   - Which are quickest to implement?
   - What's the effort vs. impact for each?

6. Create action plan
   - What are the specific steps for top 3 initiatives?
   - Who owns each initiative?
   - What's the timeline?
   - How will we measure success?

Context:
- Current customers: 500
- Monthly churn: 7-8 customers
- Top churn reasons: Price (40%), lack of features (30%), poor support (20%), other (10%)
- Budget: $50K for retention initiatives
- Team: 2 customer success managers, 1 product manager
```

### Execute and Evaluate

1. Run your planning prompt
2. Review the strategic reasoning
3. Assess if the plan is actionable

**Expected Output**:
- Analysis of current churn patterns
- Clear target (retain 35 more customers over 6 months)
- Key retention drivers identified
- Multiple initiatives proposed
- Prioritized action plan with owners and timelines
- Success metrics defined

**Validation Prompt**:
```
I used step-by-step reasoning for strategic planning:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Does the plan logically flow from analysis to action?
2. Are initiatives aligned with the root causes?
3. Is the prioritization sound?
4. Is the action plan specific enough to execute?
5. Are success metrics appropriate?
```

### Success Criteria
- [ ] Plan starts with understanding current state
- [ ] Each step builds toward the goal
- [ ] Initiatives address root causes
- [ ] Action plan is specific and actionable
- [ ] Success metrics are defined

**Troubleshooting**:
- **Issue**: Plan is too generic
  **Solution**: Add: "Be specific about actions, owners, and timelines. No vague statements."
- **Issue**: Doesn't address the context provided
  **Solution**: Add: "Base your plan on the specific churn reasons and resources mentioned"

---

## Exercise 5: Multi-Criteria Decision

**Objective**: Evaluate a complex decision with competing factors

**Scenario**: Decide whether to launch a new product feature now or wait.

### Your Task

Create a decision analysis prompt:

```
Should we launch the new AI-powered recommendation feature now or wait 3 months?

Context:
- Feature is 80% complete, core functionality works
- Known issues: Recommendations sometimes miss the mark (70% accuracy, target is 85%)
- Competitor announced similar feature launching in 2 months
- Current customers are asking for this feature
- Engineering team says 3 more months would get to 85% accuracy
- Marketing has campaign ready to go
- Sales team says this feature would help close 5 pending deals worth $200K

Analyze this decision step by step:

1. Define what we're optimizing for
   - Speed to market vs. quality?
   - Competitive advantage vs. customer satisfaction?
   - Revenue vs. reputation?

2. Evaluate "launch now" option
   - Pros: Beat competitor, help close deals, satisfy customer requests
   - Cons: Lower accuracy might disappoint users, potential negative reviews
   - Risks: What if accuracy issues cause churn?

3. Evaluate "wait 3 months" option
   - Pros: Higher quality, better user experience, stronger launch
   - Cons: Competitor launches first, lose pending deals, disappoint waiting customers
   - Risks: What if competitor captures market?

4. Consider middle ground
   - Could we do a limited beta launch?
   - Could we launch with clear "beta" labeling?
   - Could we launch to select customers first?

5. Assess the stakes
   - What's the cost of getting this wrong?
   - Is this decision reversible?
   - What's the long-term impact?

6. Make recommendation
   - What should we do?
   - Why is this the best choice given the tradeoffs?
   - What conditions or safeguards should we include?
```

### Execute and Evaluate

1. Run your decision analysis
2. Review how competing factors are weighed
3. Assess if the recommendation balances all concerns

**Expected Output**:
- Clear definition of decision criteria
- Thorough analysis of both options
- Consideration of middle-ground alternatives
- Risk assessment
- Recommendation with conditions (e.g., "Launch now but as beta with select customers")

**Validation Prompt**:
```
I used step-by-step reasoning for a complex decision:

My prompt: [paste your prompt]

Output: [paste Gemini's output]

Please assess:
1. Were all competing factors considered?
2. Is the tradeoff analysis balanced?
3. Does the recommendation make sense given the factors?
4. Are risks adequately addressed?
5. Would this analysis help leadership make a decision?
```

### Success Criteria
- [ ] All competing factors identified
- [ ] Both options thoroughly analyzed
- [ ] Tradeoffs explicitly discussed
- [ ] Recommendation addresses key concerns
- [ ] Decision includes conditions or safeguards

**Troubleshooting**:
- **Issue**: Analysis favors one option too heavily
  **Solution**: Add: "Present a balanced analysis. Both options have merit - explain the tradeoffs clearly"
- **Issue**: Doesn't consider middle ground
  **Solution**: Explicitly add step asking for alternative approaches

---

## Reflection Questions

1. **When did step-by-step reasoning add the most value?** Think about which exercises benefited most.

2. **How did seeing the reasoning process change your confidence?** Compare to getting just an answer.

3. **What makes good step-by-step reasoning?** What characteristics did the best outputs have?

4. **How will you use this in your work?** What decisions or problems would benefit from this approach?

---

## Key Takeaways

- **Step-by-step improves complex decisions** - Shows thinking, not just conclusions
- **Provide a framework** - Guide the reasoning process with specific steps
- **Validate the logic** - Review each step, don't blindly accept the conclusion
- **Use selectively** - Not every task needs detailed reasoning
- **Combine with context** - Background information makes reasoning more relevant

---

## Next Steps

Excellent work! You now know how to request and evaluate step-by-step reasoning.

**To continue improving:**

1. **Apply to real decisions** - Use step-by-step for an actual decision you're facing
2. **Create reasoning templates** - Build frameworks for your common decision types
3. **Move to Chapter 9** - Learn few-shot learning with examples
4. **Practice validation** - Get good at spotting flawed reasoning

**Ready for more?** → [Chapter 9: Few-Shot Learning with Examples](../09-few-shot-learning/lesson.md)

---

## Additional Practice (Optional)

Try step-by-step reasoning for these scenarios:

1. **Budget allocation**: Distribute $100K across 5 initiatives
2. **Process improvement**: Reduce customer onboarding time from 2 weeks to 1 week
3. **Hiring decision**: Choose between 3 candidates with different strengths
4. **Market expansion**: Decide which geographic market to enter next
5. **Technology choice**: Select between build, buy, or partner for a capability

---

## Navigation

- **Previous**: [Lesson 8: Step-by-Step Reasoning](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 9: Few-Shot Learning with Examples](../09-few-shot-learning/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 8 Complete!** 🎉 You've mastered step-by-step reasoning!
