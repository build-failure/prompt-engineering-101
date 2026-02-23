# Lab 12: Troubleshooting and Debugging Prompts

← [Lesson 12](lesson.md) | [Home](../../README.md)

---

## Overview

**Chapter**: 12 - Troubleshooting and Debugging Prompts  
**Level**: Advanced  
**Estimated Time**: 35 minutes  
**Prerequisites**: Complete Lesson 12

## Learning Objectives

By completing this lab, you will:
- Practice systematic troubleshooting approaches
- Learn to diagnose and fix common prompt problems
- Master debugging techniques
- Build your personal troubleshooting process

## Business Scenario

Not every prompt works perfectly the first time. When prompts fail, you need a systematic approach to diagnose and fix them. This lab teaches you to troubleshoot like a pro, turning failed prompts into successful ones through methodical debugging.

## Materials Needed

- Access to Google Gemini
- Broken prompts provided in exercises
- Notepad to track your debugging process

---

## Exercise 1: Diagnosing Vague Output

**Objective**: Fix a prompt that produces generic, unhelpful output

**Scenario**: You need a professional email but keep getting generic templates.

### The Problem

**Broken Prompt:**
```
Write a professional email.
```

**Output You Got:**
```
Dear [Name],

I hope this email finds you well. I am writing to follow up on our previous conversation.

Please let me know if you have any questions or concerns.

Best regards,
[Your Name]
```

**What's Wrong:** Too generic, no specific content, template-like, not useful.

### Your Task

**Step 1: Diagnose**
Using the TCFC framework, identify what's missing:
- Task: Is it clear and specific?
- Context: Is background provided?
- Format: Is structure defined?
- Constraints: Are requirements specified?

**Step 2: Fix the Prompt**
Rewrite the prompt to fix the issues you identified.

**Scenario Details to Include:**
- Recipient: Sarah Chen, potential client
- Purpose: Follow up after proposal meeting yesterday
- Key points: Thank her, reference her interest in automation features, propose next call
- Tone: Professional but warm
- Length: 3 paragraphs

**Step 3: Test Your Fix**
Run your improved prompt and compare the output.

**Expected Improved Output:**
A specific, personalized email that:
- Addresses Sarah by name
- References the specific meeting
- Mentions automation features
- Proposes concrete next steps
- Uses appropriate tone

**Validation Prompt:**
```
I debugged a vague prompt:

Original prompt: "Write a professional email"
Problem: [describe what was wrong]

Improved prompt: [paste your rewritten prompt]
New output: [paste the result]

Please assess:
1. Did I correctly diagnose the problem?
2. Does my improved prompt fix the issues?
3. Is the new output significantly better?
4. What debugging techniques did I use effectively?
```

### Success Criteria
- [ ] Identified specific problems with original prompt
- [ ] Applied TCFC framework to diagnose
- [ ] Rewrote prompt with necessary details
- [ ] New output is specific and useful
- [ ] Understood what made the difference

**Troubleshooting**:
- **Issue**: Still getting generic output
  **Solution**: Add even more specific details - exact names, dates, topics discussed
- **Issue**: Output is too long now
  **Solution**: Add length constraint: "Maximum 150 words, 3 paragraphs"

---

## Exercise 2: Fixing Wrong Tone

**Objective**: Debug a prompt that produces inappropriate tone

**Scenario**: You need a friendly team update but keep getting corporate-speak.

### The Problem

**Broken Prompt:**
```
Write an announcement about the new remote work policy.
```

**Output You Got:**
```
MEMORANDUM

TO: All Personnel
FROM: Management
RE: Remote Work Policy Update

Effective immediately, the organization will implement a revised remote work policy framework. Employees are hereby authorized to utilize remote work arrangements pursuant to departmental guidelines and supervisor approval.

All personnel must ensure compliance with established protocols and maintain productivity metrics in accordance with performance standards.

For questions regarding policy interpretation, please consult your immediate supervisor or the Human Resources department.
```

**What's Wrong:** Too formal, corporate jargon, cold tone, not appropriate for team culture.

### Your Task

**Step 1: Diagnose**
What's causing the wrong tone?
- No tone specified
- No audience defined
- No style guidance
- No examples of desired voice

**Step 2: Fix the Prompt**
Rewrite with explicit tone guidance.

**Context to Add:**
- Audience: Your team (colleagues you work with daily)
- Tone: Friendly, conversational, positive
- Style: Like you're talking to friends, not writing a legal document
- Key message: New policy gives more flexibility, trust-based approach
- Length: 200 words

**Step 3: Test Your Fix**
Run your improved prompt and compare the tone.

**Expected Improved Output:**
A friendly announcement that:
- Sounds like a real person talking
- Uses conversational language
- Emphasizes positive aspects
- Feels warm and approachable
- Avoids corporate jargon

**Validation Prompt:**
```
I debugged a tone problem:

Original prompt: [paste original]
Problem: Too formal and corporate

Improved prompt: [paste your rewritten prompt]
New output: [paste the result]

Please assess:
1. Did I correctly identify the tone issue?
2. Does my improved prompt specify the desired tone?
3. Is the new output appropriately friendly?
4. What specific changes made the biggest difference?
```

### Success Criteria
- [ ] Identified tone as the core problem
- [ ] Added explicit tone descriptors
- [ ] Provided audience context
- [ ] New output matches desired tone
- [ ] Avoided corporate jargon

**Troubleshooting**:
- **Issue**: Still too formal
  **Solution**: Add "Write as if you're talking to a friend" or provide an example of your desired tone
- **Issue**: Now too casual
  **Solution**: Add "Professional but friendly" and "Appropriate for workplace"

---

## Exercise 3: Recovering Missing Information

**Objective**: Fix a prompt that skips critical details

**Scenario**: You need a complete meeting summary but keep getting incomplete output.

### The Problem

**Broken Prompt:**
```
Summarize the meeting.

MEETING NOTES:
Discussed Q2 launch plans. Sarah presented timeline. Mike raised concerns about resources. Jen showed designs. Tom talked about marketing. Decided to move forward. Next meeting in 2 weeks.
```

**Output You Got:**
```
The team discussed Q2 launch plans. Sarah presented a timeline, Mike had concerns, Jen showed designs, and Tom discussed marketing. The team decided to move forward with another meeting scheduled.
```

**What's Wrong:** Missing action items, no specific decisions, no owners, no deadlines, vague summary.

### Your Task

**Step 1: Diagnose**
What information is missing from the output?
- Specific decisions made
- Action items with owners
- Deadlines
- Details about concerns
- Next meeting specifics

**Step 2: Fix the Prompt**
Rewrite to explicitly require all necessary information.

**Add These Requirements:**
```
MUST INCLUDE:
- All decisions made (with brief rationale)
- All action items (with owner and deadline for each)
- Any concerns raised (and how they'll be addressed)
- Next meeting date and agenda
- Key discussion points

Do not skip any of these elements.
```

**Step 3: Test Your Fix**
Run your improved prompt and verify all information is included.

**Expected Improved Output:**
A complete summary with:
- Specific decisions listed
- Action items with owners and dates
- Concerns documented
- Next meeting details
- Nothing important missing

**Validation Prompt:**
```
I debugged a completeness problem:

Original prompt: [paste original]
Problem: Missing critical information

Improved prompt: [paste your rewritten prompt]
New output: [paste the result]

Please assess:
1. Did I identify all missing information?
2. Does my improved prompt explicitly require each element?
3. Is the new output complete?
4. Are action items clear with owners and deadlines?
```

### Success Criteria
- [ ] Identified all missing information types
- [ ] Added explicit "MUST INCLUDE" list
- [ ] New output contains all required elements
- [ ] Action items have owners and deadlines
- [ ] Nothing important is skipped

**Troubleshooting**:
- **Issue**: Still missing some items
  **Solution**: Make requirements even more explicit: "List EVERY action item mentioned, even minor ones"
- **Issue**: Output is too long now
  **Solution**: Add "Be concise but complete - bullet points are fine"

---

## Exercise 4: Correcting Format Problems

**Objective**: Fix a prompt that produces wrong structure

**Scenario**: You need a comparison table but keep getting paragraphs.

### The Problem

**Broken Prompt:**
```
Compare these three project management tools: Asana, Trello, Monday.com
```

**Output You Got:**
```
Asana is a comprehensive project management tool that offers task management, timeline views, and team collaboration features. It's priced at $10.99 per user per month for the premium plan.

Trello uses a card-based system with boards and lists, making it very visual and intuitive. It's more affordable at $5 per user per month for the standard plan.

Monday.com provides customizable workflows and automation features with a colorful interface. It costs $8 per user per month for the basic plan.
```

**What's Wrong:** Paragraphs instead of table, hard to compare, not scannable, wrong format.

### Your Task

**Step 1: Diagnose**
Why is the format wrong?
- No format specified
- No structure shown
- No comparison framework
- No visual organization

**Step 2: Fix the Prompt**
Rewrite with explicit format specification.

**Add Format Requirements:**
```
Create a comparison table with these exact columns:
| Tool | Price | Key Features | Best For | Pros | Cons |

Include:
- All three tools as rows
- 3-4 key features per tool (bullet points in cell)
- Specific pricing
- One sentence for "Best For"
- 2-3 pros and cons each

Format as markdown table.
```

**Step 3: Test Your Fix**
Run your improved prompt and verify table format.

**Expected Improved Output:**
A properly formatted table with:
- Clear column headers
- All three tools as rows
- Consistent information in each cell
- Easy to scan and compare
- Markdown table format

**Validation Prompt:**
```
I debugged a format problem:

Original prompt: [paste original]
Problem: Got paragraphs instead of table

Improved prompt: [paste your rewritten prompt]
New output: [paste the result]

Please assess:
1. Did I correctly identify the format issue?
2. Does my improved prompt show the exact format wanted?
3. Is the new output in proper table format?
4. Is the table easy to scan and compare?
```

### Success Criteria
- [ ] Identified format as the problem
- [ ] Specified exact table structure
- [ ] Defined what goes in each column
- [ ] New output is properly formatted table
- [ ] Information is easy to compare

**Troubleshooting**:
- **Issue**: Table structure is messy
  **Solution**: Show exact table format with column names and separators
- **Issue**: Inconsistent information across rows
  **Solution**: Specify what information is required for each column

---

## Exercise 5: Debugging Length Issues

**Objective**: Fix prompts that produce too much or too little content

**Scenario**: You need a concise summary but keep getting essays or one-liners.

### Problem A: Too Long

**Broken Prompt:**
```
Summarize this article about AI in healthcare.

[Long article text]
```

**Output You Got:**
A 500-word summary when you needed 100 words.

### Problem B: Too Short

**Broken Prompt:**
```
Explain our new product features.
```

**Output You Got:**
"Our new product has improved performance and better UI."

### Your Task

**Step 1: Diagnose Both Problems**
- Problem A: No length constraint specified
- Problem B: No detail level specified

**Step 2: Fix Both Prompts**

**Fix for Problem A (Too Long):**
```
Summarize this article about AI in healthcare.

Requirements:
- Exactly 3 bullet points
- Each bullet: maximum 30 words
- Total: maximum 100 words
- Focus only on: main findings and implications
- Skip: background, methodology, detailed examples

[Article text]
```

**Fix for Problem B (Too Short):**
```
Explain our new product features in detail.

For each feature, include:
- Feature name
- What it does (2-3 sentences)
- Key benefits (3 bullets)
- Who it's for (1 sentence)
- How to use it (2-3 steps)

Features to cover:
1. Automated reporting
2. Team collaboration
3. API access

Total length: 400-500 words
```

**Step 3: Test Both Fixes**
Run both improved prompts and verify length is appropriate.

**Expected Improved Outputs:**
- Problem A: Concise 100-word summary with 3 bullets
- Problem B: Detailed 400-500 word explanation with all components

**Validation Prompt:**
```
I debugged two length problems:

Problem A - Too Long:
Original: [paste]
Fixed: [paste]
Result: [paste and note word count]

Problem B - Too Short:
Original: [paste]
Fixed: [paste]
Result: [paste and note word count]

Please assess:
1. Did I correctly diagnose both length issues?
2. Do my fixes specify appropriate constraints?
3. Are the new outputs the right length?
4. What techniques worked for controlling length?
```

### Success Criteria
- [ ] Identified length as the core issue
- [ ] Added specific length constraints
- [ ] Specified what to include/exclude
- [ ] New outputs are appropriate length
- [ ] Understood how to control verbosity

**Troubleshooting**:
- **Issue**: Still too long
  **Solution**: Add "Maximum X words" AND "Focus only on Y, skip Z"
- **Issue**: Still too short
  **Solution**: Add "For each item, include: [list specific components]"

---

## Exercise 6: Systematic Debugging Practice

**Objective**: Apply complete debugging process to a complex problem

**Scenario**: This prompt has multiple issues. Debug it systematically.

### The Problem

**Broken Prompt:**
```
Write something about the project.
```

**Output You Got:**
```
The project is progressing well. The team is working hard and making good progress. We expect to complete it soon. There are some challenges but we're addressing them.
```

**What's Wrong:** Everything! Vague task, no context, no format, no constraints, useless output.

### Your Task

**Step 1: Complete Diagnosis**
Use the TCFC framework to identify ALL problems:

**Task Issues:**
- [ ] What specific task? (write what?)
- [ ] What about the project?
- [ ] What's the purpose?

**Context Issues:**
- [ ] What project?
- [ ] Who's the audience?
- [ ] What's the situation?

**Format Issues:**
- [ ] What structure?
- [ ] How to organize?
- [ ] What sections?

**Constraint Issues:**
- [ ] How long?
- [ ] What tone?
- [ ] What to include/exclude?

**Step 2: Gather Requirements**
Before fixing, decide what you actually need:
- Purpose: Status update for stakeholders
- Project: Website redesign project
- Audience: Executive team
- Format: Structured update with sections
- Length: 250 words
- Must include: Progress, milestones, blockers, next steps

**Step 3: Rebuild the Prompt**
Create a completely new prompt addressing all issues:

```
[Your rebuilt prompt here - should be comprehensive and specific]
```

**Step 4: Test and Iterate**
1. Run your rebuilt prompt
2. Evaluate the output
3. If issues remain, diagnose and fix
4. Iterate until output is good

**Expected Final Output:**
A professional status update with:
- Clear project context
- Specific progress details
- Milestone status
- Identified blockers
- Concrete next steps
- Appropriate length and tone

**Validation Prompt:**
```
I systematically debugged a broken prompt:

Original prompt: "Write something about the project"
Original output: [paste]

My diagnosis:
- Task issues: [list]
- Context issues: [list]
- Format issues: [list]
- Constraint issues: [list]

Rebuilt prompt: [paste your complete rewrite]

Final output: [paste]

Iterations needed: [number]

Please assess:
1. Was my diagnosis complete?
2. Did my rebuilt prompt address all issues?
3. Is the final output professional and useful?
4. What was my most effective debugging technique?
5. What did I learn about systematic debugging?
```

### Success Criteria
- [ ] Identified all problems using TCFC
- [ ] Gathered complete requirements
- [ ] Rebuilt prompt from scratch
- [ ] Final output is professional and complete
- [ ] Understood systematic debugging process
- [ ] Can apply this process to any broken prompt

**Troubleshooting**:
- **Issue**: Overwhelmed by multiple problems
  **Solution**: Fix one category at a time - start with Task, then Context, then Format, then Constraints
- **Issue**: Not sure what's needed
  **Solution**: Ask yourself: "If I got the perfect output, what would it look like?" Then work backward

---

## Exercise 7: Build Your Debugging Checklist

**Objective**: Create your personal troubleshooting toolkit

### Your Task

Based on all the exercises, create your own debugging resources:

**1. Personal Debugging Checklist**
```
When a prompt fails, I check:
- [ ] [Add your checklist items based on what you learned]
- [ ] 
- [ ] 
[Continue with 10-15 items]
```

**2. Common Problems & Fixes Library**
```
Problem: Output is too vague
My go-to fix: [Your approach]

Problem: Wrong tone
My go-to fix: [Your approach]

Problem: Missing information
My go-to fix: [Your approach]

[Add more based on your experience]
```

**3. Quick Diagnostic Questions**
```
When output isn't right, I ask:
1. [Your question]
2. [Your question]
3. [Your question]
[Add 5-10 questions]
```

**4. Success Pattern Library**
```
For [task type], what works:
- [Pattern elements]

For [task type], what works:
- [Pattern elements]

[Add patterns for your common tasks]
```

### Share and Validate

**Validation Prompt:**
```
I created my personal debugging toolkit:

My debugging checklist: [paste]
My common fixes library: [paste]
My diagnostic questions: [paste]
My success patterns: [paste]

Please assess:
1. Is my checklist comprehensive?
2. Are my fixes practical and actionable?
3. Are my diagnostic questions effective?
4. Will this toolkit help me debug future prompts?
5. What should I add to make it more useful?
```

### Success Criteria
- [ ] Created comprehensive debugging checklist
- [ ] Documented common problems and fixes
- [ ] Listed diagnostic questions
- [ ] Captured success patterns
- [ ] Toolkit is personalized to your needs
- [ ] Ready to use for future debugging

---

## Reflection Questions

1. **What's your debugging process now?** How has it evolved from when you started?

2. **Which debugging technique is most valuable?** TCFC diagnosis, incremental building, isolation testing?

3. **How do you know when to simplify vs. add detail?** What signals guide your decision?

4. **What patterns have you noticed in your own prompt failures?** Are there recurring issues?

---

## Key Takeaways

- **Debugging is systematic, not random** - Follow a process
- **TCFC framework is your diagnostic tool** - Check each component
- **One change at a time** - Isolate what works
- **Build your personal toolkit** - Learn from every failure
- **Every broken prompt teaches something** - Failures are learning opportunities
- **Practice makes perfect** - Debugging gets easier with experience

---

## Course Complete! 🎓

**Congratulations!** You've completed all 12 chapters and labs of Prompt Engineering 101!

### Your Journey

**Beginner Skills Mastered:**
- ✅ Prompt engineering fundamentals
- ✅ TCFC framework
- ✅ Clarity and specificity
- ✅ Role assignment and persona

**Intermediate Skills Mastered:**
- ✅ Context and examples
- ✅ Instruction-data separation
- ✅ Output formatting
- ✅ Step-by-step reasoning
- ✅ Few-shot learning

**Advanced Skills Mastered:**
- ✅ Accuracy and verification
- ✅ Multi-step workflows
- ✅ Troubleshooting and debugging

### What's Next?

**1. Apply Daily**
Use these skills in your work every day. The more you practice, the better you'll get.

**2. Build Your Library**
- Save successful prompts
- Document what works
- Create templates for common tasks
- Build your personal toolkit

**3. Share Knowledge**
- Teach colleagues what you've learned
- Share your best prompts
- Help others debug their prompts
- Build a community of practice

**4. Keep Learning**
- AI tools evolve constantly
- Stay current with new features
- Experiment with new techniques
- Join prompt engineering communities

**5. Experiment and Innovate**
- Try new approaches
- Combine techniques creatively
- Push boundaries
- Discover what works for you

### Resources

- [Quick Reference Guide](../../QUICK_REFERENCE.md) - Cheat sheet of all techniques
- [Template Library](../../templates/) - Reusable prompt templates
- [Troubleshooting Guide](../../resources/troubleshooting-guide.md) - Common problems and solutions
- [Best Practices](../../resources/best-practices.md) - Quality guidelines

### Final Thoughts

You now have the skills to:
- Write effective prompts for any task
- Debug and fix failing prompts
- Design complex multi-step workflows
- Maintain consistency and quality
- Continuously improve your prompting

**Remember:** Prompt engineering is a skill that improves with practice. Every prompt you write, every problem you debug, every workflow you design makes you better.

**You're not just a user of AI tools - you're a prompt engineering practitioner!**

---

## Navigation

- **Previous**: [Lesson 12: Troubleshooting and Debugging](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/) | [Best Practices](../../resources/best-practices.md)

---

**🎉 Lab 12 Complete! Course Complete! 🎓**

**You did it!** You're now equipped to use AI effectively in your work. Go forth and prompt with confidence!
