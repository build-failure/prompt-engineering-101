# Troubleshooting Guide

Common prompt engineering problems and how to solve them.

---

## Output Quality Issues

### Problem: Output is Too Vague or Generic

**Symptoms:**
- AI gives general information instead of specific answers
- Output lacks detail or concrete examples
- Feels like a template response

**Solutions:**
1. Add more specific context about your situation
2. Include concrete examples of what you want
3. Specify exact format and structure
4. Use numbers (word count, number of items, etc.)
5. Provide background information

**Example Fix:**
```
❌ Before: "Write about our product"

✅ After: "Write a 200-word product description for our project management 
software targeting small business owners. Highlight ease of use, 
time savings, and Google Workspace integration. Tone: professional 
but approachable."
```

---

### Problem: Wrong Tone or Style

**Symptoms:**
- Too formal when you need casual
- Too casual when you need professional
- Doesn't match your brand voice

**Solutions:**
1. Explicitly specify tone in your prompt
2. Provide examples of desired tone
3. Use descriptive tone words (empathetic, authoritative, friendly, etc.)
4. Include audience information
5. Show examples of your brand voice

**Example Fix:**
```
❌ Before: "Draft an email to the client"

✅ After: "Draft an email to the client. Tone: professional but warm, 
like a trusted advisor. Avoid overly formal language. Similar to how 
we'd talk in person - knowledgeable but approachable."
```

---

### Problem: Output is Too Long or Too Short

**Symptoms:**
- AI writes way more than you need
- Output is too brief and lacks substance
- Doesn't fit your format requirements

**Solutions:**
1. Specify exact word count or paragraph count
2. Use "maximum" or "minimum" constraints
3. Provide length examples
4. Specify format (bullets vs. paragraphs affects length)
5. Request specific number of points/items

**Example Fix:**
```
❌ Before: "Summarize this report briefly"

✅ After: "Summarize this report in exactly 5 bullet points, 
maximum 30 words per bullet. Total summary should not exceed 200 words."
```

---

### Problem: Missing Important Information

**Symptoms:**
- Output doesn't include key points you need
- Skips critical details
- Focuses on wrong aspects

**Solutions:**
1. List specific points that must be included
2. Use "must include" language
3. Provide checklist of required elements
4. Specify what to emphasize
5. Give examples of complete outputs

**Example Fix:**
```
❌ Before: "Summarize the meeting"

✅ After: "Summarize the meeting. Must include: 1) All decisions made 
with rationale, 2) Action items with owners and deadlines, 3) Budget 
discussion outcomes, 4) Next meeting date. Do not skip any of these."
```

---

### Problem: Includes Irrelevant Information

**Symptoms:**
- Output has unnecessary details
- Goes off-topic
- Includes things you don't need

**Solutions:**
1. Specify what to exclude
2. Define scope clearly
3. Use "focus only on" language
4. Provide boundaries
5. Specify what's out of scope

**Example Fix:**
```
❌ Before: "Analyze this data"

✅ After: "Analyze Q1 sales data focusing ONLY on revenue trends and 
top-performing products. Exclude: methodology, data collection process, 
and technical details. Audience needs business insights only."
```

---

## Format and Structure Issues

### Problem: Wrong Output Format

**Symptoms:**
- You wanted bullets, got paragraphs
- You wanted a table, got a list
- Structure doesn't match your needs

**Solutions:**
1. Explicitly describe desired format
2. Show an example structure
3. Use format-specific language (table, bullets, sections, etc.)
4. Specify headers and organization
5. Provide a template to follow

**Example Fix:**
```
❌ Before: "Compare these products"

✅ After: "Compare these 3 products in a table format with these columns: 
Product Name | Price | Key Features | Target User | Our Rating. 
Include 3-5 key features per product."
```

---

### Problem: Poor Organization

**Symptoms:**
- Information is jumbled
- No logical flow
- Hard to follow

**Solutions:**
1. Specify the order of information
2. Request numbered sections
3. Define clear structure upfront
4. Use "first...then...finally" language
5. Provide outline to follow

**Example Fix:**
```
❌ Before: "Write a proposal"

✅ After: "Write a proposal with this structure: 1) Executive Summary, 
2) Problem Statement, 3) Proposed Solution, 4) Timeline, 5) Budget, 
6) Expected Outcomes. Each section should be clearly labeled."
```

---

### Problem: Inconsistent Formatting

**Symptoms:**
- Some bullets have periods, others don't
- Inconsistent capitalization
- Mixed formatting styles

**Solutions:**
1. Specify formatting rules
2. Request consistency explicitly
3. Provide style guidelines
4. Show formatting example
5. Use "ensure consistent" language

**Example Fix:**
```
❌ Before: "Create a list of features"

✅ After: "Create a bullet list of 10 features. Format: Each bullet 
starts with a verb, uses title case, ends with a period. Maintain 
consistent style throughout."
```

---

## Content Accuracy Issues

### Problem: Hallucinations or Made-Up Information

**Symptoms:**
- AI invents facts or data
- Creates plausible but false information
- Adds details you didn't provide

**Solutions:**
1. Add "only use information provided" constraint
2. Request citations or sources
3. Ask AI to indicate when it's uncertain
4. Provide all necessary data in prompt
5. Use "do not invent or assume" language

**Example Fix:**
```
❌ Before: "Summarize our Q1 performance"

✅ After: "Summarize our Q1 performance using ONLY the data provided below. 
Do not add statistics, percentages, or facts not explicitly stated. 
If information is missing, note it as '[Data not provided]'."

Data: [paste actual data]
```

---

### Problem: Misinterpretation of Instructions

**Symptoms:**
- AI does something different than intended
- Misunderstands the task
- Focuses on wrong aspect

**Solutions:**
1. Break complex tasks into steps
2. Use very explicit language
3. Provide examples of desired output
4. Clarify ambiguous terms
5. State what NOT to do

**Example Fix:**
```
❌ Before: "Improve this email"

✅ After: "Improve this email by: 1) Making the subject line more 
compelling, 2) Shortening paragraphs to 2-3 sentences each, 
3) Adding a clear call-to-action at the end. Do NOT change the core 
message or tone."
```

---

## Iteration and Refinement

### Problem: First Output Isn't Quite Right

**Symptoms:**
- Close but not exactly what you need
- Some parts good, others need work
- Right direction but needs adjustment

**Solutions:**
1. Use follow-up prompts to refine
2. Specify what to keep and what to change
3. Provide feedback on the output
4. Ask for specific modifications
5. Iterate incrementally

**Example Refinement:**
```
"Based on the previous output, please make these changes:
- Make the tone more formal
- Add specific metrics to support each point
- Reduce length by 30%
- Keep the overall structure and main arguments"
```

---

### Problem: Inconsistent Results

**Symptoms:**
- Same prompt gives different outputs each time
- Quality varies
- Can't reproduce good results

**Solutions:**
1. Make prompts more specific
2. Add more constraints
3. Use examples to show desired pattern
4. Specify format more precisely
5. Include success criteria

**Example Fix:**
```
Add to your prompt:
"Format requirements:
- Exactly 5 paragraphs
- Each paragraph 3-4 sentences
- Start each paragraph with a topic sentence
- Include one specific example per paragraph
- End with a clear conclusion"
```

---

## Task-Specific Issues

### Problem: Data Analysis Lacks Insight

**Symptoms:**
- Just restates the data
- No interpretation or meaning
- Doesn't answer "so what?"

**Solutions:**
1. Ask explicitly for insights, not just summary
2. Request "what this means" or "implications"
3. Specify business context
4. Ask for recommendations
5. Request "why this matters"

**Example Fix:**
```
❌ Before: "Analyze this sales data"

✅ After: "Analyze this sales data and provide: 1) What the trends mean 
for our business, 2) Why these patterns are occurring, 3) What actions 
we should take, 4) What risks or opportunities this reveals."
```

---

### Problem: Email Sounds Robotic

**Symptoms:**
- Too stiff or formal
- Doesn't sound human
- Lacks personality

**Solutions:**
1. Request conversational tone
2. Add "write as if speaking to a colleague"
3. Include personality descriptors
4. Provide example of your writing style
5. Ask to avoid corporate jargon

**Example Fix:**
```
❌ Before: "Draft an email to the team"

✅ After: "Draft an email to the team in a conversational, friendly tone. 
Write as if you're talking to them in person - warm, clear, and genuine. 
Avoid corporate buzzwords. Sound like a real person, not a press release."
```

---

### Problem: Summary Misses Key Points

**Symptoms:**
- Important information left out
- Focuses on minor details
- Doesn't capture main message

**Solutions:**
1. Specify what must be included
2. Define "key points" explicitly
3. Provide criteria for importance
4. Request focus on specific aspects
5. Give context about what matters

**Example Fix:**
```
❌ Before: "Summarize this document"

✅ After: "Summarize this document focusing on: decisions that need to be 
made, financial implications, and timeline impacts. These are the most 
critical aspects for our stakeholders. Include specific numbers and dates."
```

---

## Quick Diagnostic Checklist

When a prompt isn't working, check:

- [ ] Is the task clearly stated?
- [ ] Have I provided enough context?
- [ ] Is the desired format specified?
- [ ] Are there clear constraints (length, tone, etc.)?
- [ ] Have I included all necessary information?
- [ ] Are there any vague or ambiguous terms?
- [ ] Have I specified what to include/exclude?
- [ ] Is the audience defined?
- [ ] Have I stated the purpose?
- [ ] Are success criteria clear?

---

## When to Start Over

Sometimes it's better to rewrite the prompt completely:

**Start over if:**
- You've tried 3+ refinements without success
- The output is completely off-track
- You realize your original prompt was unclear
- The task is more complex than you initially thought
- You need to add substantial context

**How to start over:**
1. Review what didn't work
2. Use the TCFC framework (Task, Context, Format, Constraints)
3. Be more specific in each component
4. Add examples if helpful
5. Test the new prompt

---

## Getting Help

**If you're still stuck:**

1. **Review the course materials**
   - Check relevant chapter lessons
   - Review the Quick Reference guide
   - Look at template examples

2. **Use validation prompts**
   - Ask Gemini to review your prompt
   - Get feedback on what's unclear
   - Request suggestions for improvement

3. **Simplify the task**
   - Break complex tasks into smaller steps
   - Do one thing at a time
   - Chain multiple simpler prompts

4. **Try examples**
   - Look at similar prompts in templates
   - Adapt working examples to your needs
   - Study prompts that produced good results

---

[← Back to Home](../README.md) | [Best Practices →](best-practices.md)
