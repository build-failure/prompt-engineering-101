# Chapter 12: Troubleshooting and Debugging Prompts

← [Previous: Chapter 11 - Multi-Step Workflows](../11-multi-step-workflows/lesson.md) | [Home](../../README.md)

---

## Overview

**Level:** Advanced  
**Duration:** 35 minutes  
**Prerequisites:** Chapters 1-11

## Learning Objectives

- Learn systematic troubleshooting approaches
- Understand common prompt problems and solutions
- Master debugging techniques
- Build a personal troubleshooting process

---

## The Debugging Mindset

When prompts don't work, don't give up - debug them!

### Systematic Approach

1. **Identify the problem** - What's wrong specifically?
2. **Diagnose the cause** - Why is it happening?
3. **Apply a fix** - What change will help?
4. **Test the result** - Did it work?
5. **Iterate if needed** - Refine further

**Remember:** Every failed prompt teaches you something. Use failures to improve.

---

## Common Prompt Problems

### Problem 1: Output is Too Vague

**Symptoms:**
- Generic, template-like responses
- Lacks specific details
- Doesn't address your situation

**Diagnosis:**
- Prompt lacks specificity
- Missing context
- No examples provided
- Vague language used

**Fixes:**
```
❌ Before:
"Write a professional email"

✅ After:
"Write a professional follow-up email to Sarah Chen (client) after yesterday's
project proposal meeting. Thank her for her time, reference her interest in
our automation features, and propose a 30-minute call next Tuesday to discuss
pricing for 50 users. Tone: professional but warm. Length: 3 paragraphs."
```

**Key additions:**
- Specific recipient and context
- Exact content to include
- Defined tone and length
- Clear purpose

---

### Problem 2: Wrong Tone or Style

**Symptoms:**
- Too formal when you need casual
- Too casual when you need professional
- Doesn't match your brand voice

**Diagnosis:**
- Tone not specified
- No examples of desired style
- Audience not defined

**Fixes:**
```
❌ Before:
"Draft an announcement about the new policy"

✅ After:
"Draft an announcement about the new remote work policy for our team.
Tone: Positive and reassuring (not corporate or stiff). Write as if you're
talking to colleagues you know well - friendly but professional. Similar to
how we communicate in team meetings. Emphasize benefits and flexibility."
```

**Key additions:**
- Explicit tone description
- Comparison to familiar style
- Audience context
- Emotional direction

---

### Problem 3: Missing Key Information

**Symptoms:**
- Output doesn't include critical points
- Skips important details
- Focuses on wrong aspects

**Diagnosis:**
- Requirements not explicit
- No "must include" list
- Priorities unclear

**Fixes:**
```
❌ Before:
"Summarize the meeting"

✅ After:
"Summarize the project kickoff meeting.

MUST INCLUDE:
- All decisions made (with rationale)
- Action items (with owner and deadline for each)
- Budget discussion outcome
- Timeline milestones
- Next meeting date

Do not skip any of these elements."
```

**Key additions:**
- Explicit requirements list
- "Must include" language
- Clear priorities
- Completeness check

---

### Problem 4: Wrong Format

**Symptoms:**
- Structure doesn't match needs
- Bullets when you wanted paragraphs
- Unorganized when you needed sections

**Diagnosis:**
- Format not specified
- Structure unclear
- No template provided

**Fixes:**
```
❌ Before:
"Compare these three products"

✅ After:
"Compare these three products in a table format:

| Product | Price | Key Features | Best For | Rating |
|---------|-------|--------------|----------|--------|
| [data]  | [data]| [data]       | [data]   | [data] |

Include 3-5 key features per product.
Use 1-5 star rating system.
Keep 'Best For' to one sentence."
```

**Key additions:**
- Exact format specified
- Structure shown visually
- Detail level defined
- Constraints clear

---

### Problem 5: Too Long or Too Short

**Symptoms:**
- Output exceeds needs
- Insufficient detail
- Wrong level of depth

**Diagnosis:**
- No length constraints
- Detail level not specified
- Scope unclear

**Fixes:**
```
❌ Before:
"Summarize this report"

✅ After:
"Summarize this 20-page report in exactly 5 bullet points.
Each bullet: maximum 30 words.
Total summary: maximum 200 words.
Focus on: key findings, recommendations, and next steps only.
Skip: methodology, background, detailed data."
```

**Key additions:**
- Exact length specified
- Per-item constraints
- Focus areas defined
- Exclusions noted

---

### Problem 6: Inconsistent Results

**Symptoms:**
- Same prompt gives different outputs
- Quality varies
- Can't reproduce good results

**Diagnosis:**
- Prompt too open-ended
- Not enough constraints
- Missing examples

**Fixes:**
```
❌ Before:
"Write a product description"

✅ After:
"Write a product description following this exact structure:

1. Opening hook (1 sentence, focus on main benefit)
2. Problem it solves (2-3 sentences)
3. Key features (exactly 3 bullets, each starting with a verb)
4. Who it's for (1 sentence)
5. Call-to-action (1 sentence)

Total length: 150-200 words.
Tone: Enthusiastic but not salesy.

Example structure:
[paste example following this format]"
```

**Key additions:**
- Exact structure defined
- Numbered steps
- Specific constraints per section
- Example provided

---

## Debugging Process

### Step 1: Identify What's Wrong

**Ask yourself:**
- What did I expect?
- What did I get instead?
- What's the specific gap?

**Be precise:**
- ❌ "It's not good"
- ✅ "It's too formal - I need a conversational tone"

### Step 2: Check the TCFC Components

**Review each component:**

**Task:**
- [ ] Is the action verb clear?
- [ ] Is the subject specific?
- [ ] Is there only one main task?

**Context:**
- [ ] Did I provide necessary background?
- [ ] Is the audience defined?
- [ ] Is the purpose clear?

**Format:**
- [ ] Did I specify structure?
- [ ] Is organization clear?
- [ ] Are sections defined?

**Constraints:**
- [ ] Is length specified?
- [ ] Is tone defined?
- [ ] Are requirements listed?

### Step 3: Apply Targeted Fixes

**Based on diagnosis:**

**If output is vague:**
→ Add specificity and examples

**If tone is wrong:**
→ Explicitly describe desired tone

**If information is missing:**
→ Add "must include" list

**If format is wrong:**
→ Show exact structure wanted

**If length is wrong:**
→ Add specific word/paragraph counts

### Step 4: Test and Iterate

**After fixing:**
1. Run the revised prompt
2. Compare to original output
3. Check if problem is solved
4. If not, diagnose remaining issues
5. Apply additional fixes
6. Repeat until satisfied

---

## Advanced Debugging Techniques

### Technique 1: Incremental Building

**Start simple, add complexity:**

```
Version 1 (Basic):
"Summarize this report"
→ Test

Version 2 (Add format):
"Summarize this report in 5 bullet points"
→ Test

Version 3 (Add constraints):
"Summarize this report in 5 bullet points, max 30 words each,
focusing on key findings and recommendations"
→ Test

Version 4 (Add context):
"Summarize this quarterly sales report in 5 bullet points, max 30 words each,
focusing on key findings and recommendations. Audience: executive team
making budget decisions."
→ Test
```

### Technique 2: Isolation Testing

**Test components separately:**

```
Test 1: Just the task
"Analyze this sales data"

Test 2: Task + format
"Analyze this sales data and present as:
- Summary paragraph
- Top 3 trends (bullets)
- Recommendations (numbered list)"

Test 3: Task + format + constraints
[Add length, tone, focus requirements]
```

### Technique 3: Comparison Testing

**Try variations:**

```
Version A: With role
"You are a data analyst. Analyze this sales data..."

Version B: Without role
"Analyze this sales data..."

Version C: Different role
"You are a sales manager. Analyze this sales data..."

Compare results to see what works best.
```

### Technique 4: Example Injection

**Add examples progressively:**

```
Attempt 1: No examples
→ Output doesn't match style

Attempt 2: One example
→ Better but inconsistent

Attempt 3: Three examples
→ Consistent style achieved
```

---

## When to Simplify vs. Add Detail

### Simplify When:

**Signs you need to simplify:**
- Prompt is over 500 words
- Multiple complex tasks in one prompt
- Conflicting instructions
- AI seems confused
- Results are chaotic

**How to simplify:**
1. Break into multiple prompts
2. Remove unnecessary details
3. Focus on one task at a time
4. Use clearer language
5. Reduce constraints

**Example:**
```
❌ Too complex:
"Analyze this data considering market trends, competitive landscape,
seasonal factors, and customer behavior patterns, then create a
comprehensive report with executive summary, detailed findings,
statistical analysis, visualizations, recommendations, implementation
plan, risk assessment, and ROI projections..."

✅ Simplified (Step 1 of workflow):
"Analyze this sales data and identify the top 3 trends.
For each trend, provide:
- What the trend is
- Supporting data
- Why it matters"
```

### Add Detail When:

**Signs you need more detail:**
- Output is too generic
- Missing key information
- Wrong style or tone
- Inconsistent results
- Not specific enough

**How to add detail:**
1. Specify exact requirements
2. Add examples
3. Define constraints clearly
4. Provide more context
5. Show desired format

---

## Recognizing Model Limitations

### What AI Can't Do Well

**Be realistic about:**

❌ **Access real-time information**
- Can't check current prices, news, or data
- Provide all necessary information in prompt

❌ **Perform complex calculations**
- May make arithmetic errors
- Verify important calculations

❌ **Understand your specific context**
- Doesn't know your company, industry specifics
- Provide relevant context explicitly

❌ **Make subjective judgments**
- Can't truly evaluate quality without criteria
- Define what "good" means

❌ **Remember previous conversations**
- Each prompt is independent (in most cases)
- Include necessary context each time

### Working Within Limitations

**Strategies:**

1. **Provide complete information**
   - Don't rely on AI's general knowledge
   - Include all relevant data

2. **Verify critical outputs**
   - Check facts and figures
   - Validate important claims

3. **Set clear criteria**
   - Define quality standards
   - Specify evaluation metrics

4. **Use appropriate tasks**
   - Leverage AI's strengths
   - Work around weaknesses

---

## Building Your Troubleshooting Toolkit

### Personal Debugging Checklist

Create your own checklist based on common issues:

```
When a prompt fails, I check:
- [ ] Did I use the TCFC framework?
- [ ] Is my task specific enough?
- [ ] Did I provide all necessary context?
- [ ] Is the format clearly specified?
- [ ] Are constraints explicit?
- [ ] Did I include examples if needed?
- [ ] Is the prompt focused on one main task?
- [ ] Have I avoided vague language?
- [ ] Is the audience defined?
- [ ] Are success criteria clear?
```

### Common Fixes Library

**Build a collection of fixes that work for you:**

```
Problem: Too vague
My fix: Add "specifically" and list exact requirements

Problem: Wrong tone
My fix: Add 3 tone descriptors + example

Problem: Missing info
My fix: Add "MUST INCLUDE:" section with checklist

Problem: Wrong format
My fix: Show exact structure with example

Problem: Too long
My fix: Add "Maximum X words" + "Focus only on Y"
```

### Success Pattern Library

**Save prompts that work well:**

```
Task type: Email drafting
What works: Role + recipient context + key points + tone + length

Task type: Data analysis
What works: Specific metrics + comparison request + insight focus + format

Task type: Summarization
What works: Source type + audience + length + focus areas + exclusions
```

---

## Final Troubleshooting Tips

### 1. Start with the Basics

Before complex fixes, check:
- Is the task clear?
- Did I provide enough information?
- Is the format specified?
- Are constraints defined?

### 2. Change One Thing at a Time

Don't revise everything at once:
- Make one change
- Test the result
- Assess improvement
- Make next change

### 3. Learn from Success

When a prompt works well:
- Save it
- Note what made it effective
- Create a template
- Reuse the pattern

### 4. Don't Give Up Too Soon

Good prompts often need 2-3 iterations:
- First attempt: baseline
- Second attempt: targeted fixes
- Third attempt: fine-tuning

### 5. Ask for Help

Use AI to debug itself:
```
"I'm trying to [goal] but getting [problem].

My prompt:
[paste prompt]

Output I got:
[paste output]

What should I change in my prompt to get better results?"
```

---

## Key Takeaways

1. **Debugging is a skill** - Gets easier with practice
2. **Be systematic** - Follow a process, don't guess randomly
3. **Use TCFC as diagnostic** - Check each component
4. **One change at a time** - Isolate what works
5. **Learn from failures** - Every problem teaches something
6. **Build your toolkit** - Create personal checklists and libraries

---

## Course Complete!

🎉 **Congratulations!** You've completed all 12 chapters of Prompt Engineering 101!

### What You've Learned

**Beginner Skills:**
- Prompt engineering fundamentals
- TCFC framework
- Clarity and specificity
- Role assignment

**Intermediate Skills:**
- Context and examples
- Data handling
- Output formatting
- Step-by-step reasoning
- Few-shot learning

**Advanced Skills:**
- Accuracy and verification
- Multi-step workflows
- Troubleshooting and debugging

### Next Steps

1. **Practice daily** - Use these skills in your work
2. **Build your library** - Save successful prompts
3. **Share knowledge** - Teach others what you've learned
4. **Keep learning** - AI tools evolve, stay current
5. **Experiment** - Try new techniques and approaches

### Resources

- [Quick Reference Guide](../../QUICK_REFERENCE.md)
- [Template Library](../../templates/)
- [Troubleshooting Guide](../../resources/troubleshooting-guide.md)
- [Best Practices](../../resources/best-practices.md)

---

## Navigation

- **Previous**: [Chapter 11: Multi-Step Workflows](../11-multi-step-workflows/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Lab**: [Lab 12: Troubleshooting Exercises](lab.md)

---

**🎓 Course Complete!** You're now a prompt engineering practitioner!

**Ready for the final lab?** → [Start Lab 12](lab.md)
