# Lab 4: Role Assignment and Persona

← [Lesson 4](lesson.md) | [Home](../../README.md) | [Next: Lab 5 →](../05-context-examples/lab.md)

---

## Overview

**Chapter**: 4 - Role Assignment and Persona  
**Level**: Beginner  
**Estimated Time**: 25 minutes  
**Prerequisites**: Complete Lesson 4

## Learning Objectives

By completing this lab, you will:
- Experiment with different roles for the same task
- Match appropriate roles to business scenarios
- Craft effective role descriptions
- Understand how roles change outputs

## Business Scenario

You're a business professional who regularly works with various types of content: marketing materials, data analysis, customer communications, and internal documents. You need to learn how assigning different roles to Gemini can help you get expert-level outputs tailored to each specific task. This lab will help you master role assignment for real-world business situations.

## Materials Needed

- Access to Google Gemini
- Sample product description (you can use one from your work or create a simple one)
- Sample business proposal or document for review (optional for Exercise 3)

---

## Exercise 1: Role Experimentation

**Objective**: See how different roles produce different outputs

**Scenario**: You need to review a product description.

### Your Task

Write the same review request with 3 different roles:

**Role 1: Marketing Expert**
```
You are an experienced marketing professional who writes compelling copy.
Review this product description and suggest improvements for:
- Persuasiveness
- Clarity of benefits
- Call-to-action strength

Product description: [paste description]
```

**Role 2: Customer Advocate**
```
You are a customer advocate who ensures messaging is trustworthy and clear.
Review this product description from a customer's perspective:
- Is it believable?
- Does it address real needs?
- Are claims supported?

Product description: [paste description]
```

**Role 3: Editor**
```
You are an editor focused on clarity and readability.
Review this product description for:
- Grammar and style
- Sentence structure
- Overall flow

Product description: [paste description]
```

### Test and Compare

1. Use the same product description with all 3 roles
2. Note how each role focuses on different aspects
3. Identify which role is most useful for your goal

**Expected Output**:
Each role should provide feedback focused on their area of expertise:
- Marketing Expert: Focus on persuasiveness, benefits, and conversion
- Customer Advocate: Focus on trust, credibility, and customer needs
- Editor: Focus on grammar, clarity, and readability

**Validation Prompt**:
```
I'm learning about role assignment in prompt engineering. I just completed an exercise
where I used 3 different roles to review the same product description.

Role 1 (Marketing Expert) output: [paste output]
Role 2 (Customer Advocate) output: [paste output]
Role 3 (Editor) output: [paste output]

Please assess:
1. Does each output reflect the assigned role's perspective?
2. Are the differences between roles clear and meaningful?
3. Which role provided the most valuable feedback for improving the product description?
```

### Success Criteria
- [ ] Created 3 distinct role-based prompts
- [ ] Each role has specific expertise
- [ ] Understood how roles shape perspective
- [ ] Outputs clearly differ based on role

**Troubleshooting**:
- **Issue**: All three outputs look similar
  **Solution**: Make the role descriptions more specific. Add details about what each role should focus on and their area of expertise.
- **Issue**: Outputs are too generic
  **Solution**: Add more specific instructions about what aspects each role should evaluate. Be explicit about the perspective they should take.

---

## Exercise 2: Marketing Campaign Analysis

**Objective**: Use expert role for business analysis

**Scenario**: Analyze campaign performance data.

### Your Task

Write a prompt with a marketing strategist role:

```
You are a marketing strategist with 10 years of experience in B2B SaaS.
Analyze this campaign performance data and provide strategic recommendations.

Campaign data:
- Email campaign: 5,000 sent, 22% open rate, 3.2% click rate, 12 conversions
- Social media: 50,000 impressions, 800 clicks, 8 conversions
- Paid search: $2,000 spent, 150 clicks, 15 conversions

Provide:
1. Performance assessment for each channel
2. Cost per conversion analysis
3. Top 3 strategic recommendations for next quarter
4. Which channel to prioritize and why

Format as executive summary suitable for leadership review.
```

**Expected Output**:
A strategic analysis that includes:
- Professional assessment of each channel's performance
- Cost-per-conversion calculations
- Data-driven recommendations prioritized by impact
- Clear reasoning for channel prioritization
- Executive-level language and formatting

**Validation Prompt**:

```
Review this role-based prompt:

[Paste your prompt]

Assess:
1. Is the role specific and relevant?
2. Does the expertise match the task?
3. Would this produce expert-level insights?
4. Are the deliverables clearly defined?
```

### Success Criteria
- [ ] Role has specific expertise (marketing strategist with B2B SaaS experience)
- [ ] Expertise matches the task (campaign analysis)
- [ ] Clear deliverables requested (assessment, analysis, recommendations)
- [ ] Appropriate for audience (executive summary format)

**Troubleshooting**:
- **Issue**: Output is too generic or lacks strategic depth
  **Solution**: Add more specificity to the role (years of experience, industry focus). Request specific types of insights (ROI, CAC, channel effectiveness).
- **Issue**: Output doesn't match executive level
  **Solution**: Explicitly request "executive summary format" and specify the audience is leadership.

---

## Exercise 3: Document Review with Editor Role

**Objective**: Use critic role for quality improvement

**Scenario**: You need feedback on a business proposal.

### Your Task

Create a prompt with an editor/reviewer role:

```
You are an experienced business proposal editor who improves clarity and impact.
Review this proposal and provide specific feedback on:

1. Value proposition clarity
2. Evidence and supporting data
3. Persuasiveness of arguments
4. Professional presentation
5. Any gaps or weaknesses

For each area, provide:
- Current assessment (what's working/not working)
- Specific suggestions for improvement
- Priority (high/medium/low)

Proposal:
[paste proposal]

Be constructive but direct about issues.
```

**Expected Output**:
A structured review that includes:
- Specific feedback for each of the 5 areas
- Current state assessment (strengths and weaknesses)
- Actionable improvement suggestions
- Priority levels for each recommendation
- Professional but constructive tone

**Validation Prompt**:
```
I'm learning about using critic/reviewer roles in prompts. I created this prompt
to review a business proposal:

[Paste your prompt]

Please assess:
1. Is the role appropriate for providing critical feedback?
2. Are the review criteria specific and comprehensive?
3. Is the feedback format clearly defined?
4. Does the prompt encourage constructive criticism?
```

### Success Criteria
- [ ] Role is evaluative/critical (editor with improvement focus)
- [ ] Specific review criteria listed (5 areas defined)
- [ ] Feedback format defined (assessment + suggestions + priority)
- [ ] Constructive approach specified

**Troubleshooting**:
- **Issue**: Feedback is too harsh or negative
  **Solution**: Add "Be constructive" to the prompt. Emphasize you want both strengths and areas for improvement.
- **Issue**: Feedback is too vague
  **Solution**: Request "specific suggestions" and examples. Ask for concrete changes rather than general observations.

---

## Exercise 4: Role Matching Challenge

**Objective**: Match the right role to each scenario

### Scenarios

Match each scenario with the best role:

**Scenario A**: Explain technical API documentation to non-technical users
**Scenario B**: Generate creative campaign ideas
**Scenario C**: Analyze financial data for trends
**Scenario D**: Write empathetic customer service responses
**Scenario E**: Review code for best practices

**Roles to choose from**:
1. Technical writer for non-technical audiences
2. Creative brainstorming facilitator
3. Financial analyst
4. Customer service expert with conflict resolution skills
5. Senior software engineer

### Your Matches

- Scenario A: Role ___
- Scenario B: Role ___
- Scenario C: Role ___
- Scenario D: Role ___
- Scenario E: Role ___

### Write One Prompt

Choose one scenario and write a complete prompt with the appropriate role:

```
[Your prompt here]
```

**Expected Output**:
A complete prompt that:
- Assigns the appropriate role with specific expertise
- Clearly states the task
- Provides necessary context
- Specifies desired output format

**Validation Prompt**:
```
I'm practicing matching roles to tasks. Here's my role matching:

Scenario A: Role ___
Scenario B: Role ___
Scenario C: Role ___
Scenario D: Role ___
Scenario E: Role ___

And here's the complete prompt I wrote for one scenario:
[Paste your prompt]

Please assess:
1. Are my role matches appropriate for each scenario?
2. Does my complete prompt use the role effectively?
3. Is the role's expertise relevant to the task?
```

<details>
<summary>Click for answers</summary>

- Scenario A: Role 1 (Technical writer)
- Scenario B: Role 2 (Creative facilitator)
- Scenario C: Role 3 (Financial analyst)
- Scenario D: Role 4 (Customer service expert)
- Scenario E: Role 5 (Software engineer)

</details>

### Success Criteria
- [ ] Matched roles correctly to scenarios
- [ ] Understood role-task alignment principles
- [ ] Wrote effective role-based prompt with clear expertise

**Troubleshooting**:
- **Issue**: Unsure which role fits which scenario
  **Solution**: Think about what expertise is needed for each task. Match the specialized knowledge required to the role's area of expertise.
- **Issue**: Prompt doesn't leverage the role effectively
  **Solution**: Make sure your task aligns with the role's expertise. Reference the role's perspective in what you're asking for.

---

## Exercise 5: Create Your Role Library

**Objective**: Build reusable roles for your work

### Your Task

Create 5 role descriptions for tasks you do regularly:

**Role 1**: [Your role description]
**Use for**: [What tasks]

**Role 2**: [Your role description]
**Use for**: [What tasks]

**Role 3**: [Your role description]
**Use for**: [What tasks]

**Role 4**: [Your role description]
**Use for**: [What tasks]

**Role 5**: [Your role description]
**Use for**: [What tasks]

### Example

```
Role 1: "You are a business communications expert who writes clear, professional emails"
Use for: Email drafting, announcements, formal communications

Role 2: "You are a data analyst who turns numbers into actionable insights"
Use for: Sales data analysis, performance reports, trend identification

Role 3: "You are a helpful executive assistant who organizes information efficiently"
Use for: Meeting notes, task lists, scheduling, coordination
```

**Expected Output**:
A personalized library of 5 role descriptions that:
- Are specific to your actual work tasks
- Include relevant expertise for each role
- Can be reused in future prompts
- Cover different types of tasks you do regularly

**Validation Prompt**:
```
I'm building a personal library of roles for my work. Here are my 5 roles:

Role 1: [Your role] - Use for: [tasks]
Role 2: [Your role] - Use for: [tasks]
Role 3: [Your role] - Use for: [tasks]
Role 4: [Your role] - Use for: [tasks]
Role 5: [Your role] - Use for: [tasks]

Please assess:
1. Are these roles specific enough to be useful?
2. Do they cover a good range of my work tasks?
3. Is the expertise in each role relevant to its intended use?
4. Any suggestions for improving these role descriptions?
```

### Success Criteria
- [ ] Created 5 relevant roles for your actual work
- [ ] Each role has specific expertise
- [ ] Roles match your actual work tasks
- [ ] Can reuse these roles regularly in your prompts

**Troubleshooting**:
- **Issue**: Roles are too generic (e.g., "You are a professional")
  **Solution**: Add specific expertise, experience level, or focus area. Think about what specialized knowledge would help with each task.
- **Issue**: Can't think of 5 different roles
  **Solution**: Review your typical work week. What different types of tasks do you do? Writing, analyzing, planning, communicating? Each needs a different role.

---

## Reflection Questions

1. **How did different roles change the outputs you received?** Think about the specific differences in perspective, focus, and recommendations.

2. **Which role was most useful for your typical work tasks?** Consider which expertise aligns best with what you do daily.

3. **When might you use multiple roles for the same task?** Think about scenarios where different perspectives would be valuable.

4. **How specific should a role description be?** Reflect on the balance between detailed expertise and keeping prompts concise.

---

## Key Takeaways

- **Roles shape perspective** - Different expertise produces different outputs
- **Match role to task** - Choose relevant expertise
- **Be specific** - Detailed roles work better
- **Build a library** - Reuse effective roles
- **Experiment** - Try different roles for same task

---

## Next Steps

**Ready for more?** → [Chapter 5: Providing Context and Examples](../05-context-examples/lesson.md)

---

**Lab 4 Complete!** 🎉
