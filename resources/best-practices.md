# Prompt Engineering Best Practices

Guidelines and checklists for writing effective prompts consistently.

---

## The Golden Rules

### 1. Be Specific, Not Vague
❌ "Write something professional"  
✅ "Write a 200-word professional email to a client confirming our meeting on March 15th"

### 2. Provide Context
❌ "Summarize this"  
✅ "Summarize this quarterly report for executives who need to make budget decisions"

### 3. Specify Format
❌ "Give me information about competitors"  
✅ "Create a comparison table of our top 3 competitors showing pricing, features, and target market"

### 4. Set Clear Constraints
❌ "Keep it short"  
✅ "Maximum 150 words, 3 paragraphs, professional tone"

### 5. Iterate and Refine
Don't expect perfection on the first try. Refine based on results.

---

## Pre-Prompt Checklist

Before submitting any prompt, verify:

### Task Component
- [ ] Is the action verb clear? (summarize, analyze, draft, create, etc.)
- [ ] Is the subject specific? (what you're working with)
- [ ] Is there only one main task? (or properly broken down)

### Context Component
- [ ] Have I explained the situation/background?
- [ ] Is the audience defined?
- [ ] Is the purpose clear?
- [ ] Have I included relevant constraints?

### Format Component
- [ ] Have I specified the structure? (bullets, paragraphs, table, etc.)
- [ ] Are sections/organization defined?
- [ ] Is the presentation style clear?

### Constraints Component
- [ ] Is length specified? (word count, paragraph count)
- [ ] Is tone defined? (professional, casual, empathetic, etc.)
- [ ] Are requirements listed? (must include, must avoid)
- [ ] Are boundaries set? (scope, focus areas)

---

## Writing Effective Prompts

### Start with the TCFC Framework

Every prompt should have:
- **T**ask: What you want AI to do
- **C**ontext: Background information
- **F**ormat: How to structure output
- **C**onstraints: Limitations and requirements

### Use Clear, Direct Language

**Do:**
- Use active voice: "Analyze this data"
- Be explicit: "Create exactly 5 bullet points"
- Specify numbers: "Maximum 200 words"
- Define terms: "Professional tone means formal but approachable"

**Don't:**
- Use passive voice: "This data should be analyzed"
- Be vague: "Make it good"
- Use relative terms: "Keep it brief"
- Assume understanding: "You know what I mean"

### Provide Examples When Helpful

Show AI what you want:
```
Here's an example of our brand voice:
[example text]

Now write similar content about [topic].
```

### Break Down Complex Tasks

Instead of one massive prompt:
```
❌ "Analyze this data, write a report, create a presentation, and draft an email about it"
```

Use a sequence:
```
✅ Step 1: "Analyze this data and identify top 3 trends"
✅ Step 2: "Based on these trends, write an executive summary"
✅ Step 3: "Create a presentation outline from this summary"
✅ Step 4: "Draft an email announcing these findings"
```

---

## Quality Guidelines

### Clarity
- Use simple, direct language
- Avoid ambiguous terms
- Define any jargon or acronyms
- Be explicit about requirements

### Completeness
- Include all necessary information
- Don't assume AI knows your context
- Provide data when needed
- Specify all requirements upfront

### Consistency
- Use consistent terminology
- Maintain consistent formatting in your prompts
- Apply the same standards across similar tasks
- Build on successful patterns

### Conciseness
- Be specific but not verbose
- Remove unnecessary words
- Focus on essential information
- Don't over-explain obvious points

---

## Testing and Iteration

### Test Your Prompts

1. **Run the prompt** - See what you get
2. **Evaluate output** - Does it meet your needs?
3. **Identify gaps** - What's missing or wrong?
4. **Refine prompt** - Add specificity or constraints
5. **Test again** - Verify improvements

### Iteration Strategies

**If output is too vague:**
- Add more specific context
- Include examples
- Specify exact format
- Define success criteria

**If output is wrong tone:**
- Explicitly state desired tone
- Provide tone examples
- Describe audience
- Use tone descriptors

**If output is wrong length:**
- Add exact word/paragraph count
- Use "maximum" or "minimum"
- Specify format (affects length)
- Give length examples

**If output misses key points:**
- List required elements
- Use "must include" language
- Provide checklist
- Specify priorities

### Save What Works

Build your personal prompt library:
- Save successful prompts
- Note what made them work
- Create templates for recurring tasks
- Document your patterns

---

## Common Scenarios

### Email Drafting

**Best practices:**
- Specify recipient and relationship
- State email purpose clearly
- Define tone explicitly
- Include key points to cover
- Set length constraints
- Request specific structure

**Template:**
```
Draft a [TYPE] email to [RECIPIENT] about [TOPIC].
Context: [RELATIONSHIP/SITUATION]
Include: [KEY POINTS]
Tone: [STYLE]
Length: [PARAGRAPHS/WORDS]
Structure: [GREETING/BODY/CLOSING]
```

### Document Summarization

**Best practices:**
- Specify document type and length
- Define target audience
- State summary purpose
- Indicate focus areas
- Set length limits
- Request specific format

**Template:**
```
Summarize this [DOC TYPE] for [AUDIENCE].
Focus on: [KEY ASPECTS]
Ignore: [WHAT TO SKIP]
Format: [STRUCTURE]
Length: [WORD COUNT]
Purpose: [WHY THEY NEED THIS]
```

### Data Analysis

**Best practices:**
- Provide data context
- Specify analysis type
- Define metrics of interest
- Request insights, not just summary
- Specify output format
- Include business context

**Template:**
```
Analyze this [DATA TYPE] to [SPECIFIC GOAL].
Context: [BUSINESS SITUATION]
Focus on: [METRICS/DIMENSIONS]
Provide: [INSIGHTS/RECOMMENDATIONS]
Format: [STRUCTURE]
Include: [SPECIFIC NUMBERS/EXAMPLES]
```

### Content Creation

**Best practices:**
- Define content type and purpose
- Specify target audience
- Provide topic and key messages
- Set tone and style
- Include length requirements
- Request specific elements

**Template:**
```
Create [CONTENT TYPE] about [TOPIC] for [AUDIENCE].
Purpose: [GOAL]
Key messages: [MAIN POINTS]
Tone: [STYLE]
Length: [WORD COUNT]
Include: [REQUIRED ELEMENTS]
```

---

## Dos and Don'ts

### ✅ Do

- **Be specific** about what you want
- **Provide context** about the situation
- **Specify format** for the output
- **Set constraints** on length, tone, content
- **Use examples** when helpful
- **Iterate** based on results
- **Save successful prompts** for reuse
- **Test variations** to find what works
- **Break down** complex tasks
- **Define your audience** clearly

### ❌ Don't

- **Be vague** with terms like "good," "nice," "some"
- **Assume context** AI doesn't have
- **Skip format** specifications
- **Use relative terms** like "brief," "detailed"
- **Mix multiple tasks** in one prompt
- **Ignore tone** requirements
- **Accept first output** without review
- **Give up** after one attempt
- **Forget to specify** what to exclude
- **Use jargon** without definition

---

## Efficiency Tips

### Build Template Library

Create reusable templates for:
- Common email types
- Regular reports
- Recurring analyses
- Standard documents
- Frequent requests

### Use Prompt Chaining

For complex workflows:
1. Break into logical steps
2. Use output from step 1 in step 2
3. Refine progressively
4. Build toward final result

### Leverage Few-Shot Learning

Show AI the pattern:
```
Example 1: [INPUT] → [DESIRED OUTPUT]
Example 2: [INPUT] → [DESIRED OUTPUT]

Now do the same for: [NEW INPUT]
```

### Create Validation Prompts

Check your work:
```
Review this [OUTPUT TYPE] and assess:
1. [CRITERION 1]
2. [CRITERION 2]
3. [CRITERION 3]

Provide specific feedback.
```

---

## Quality Assurance

### Before Sending/Using AI Output

Check:
- [ ] Accuracy - Is information correct?
- [ ] Completeness - Includes all required elements?
- [ ] Tone - Appropriate for audience?
- [ ] Format - Matches specifications?
- [ ] Length - Within constraints?
- [ ] Clarity - Easy to understand?
- [ ] Relevance - On-topic and focused?
- [ ] Professionalism - Suitable for purpose?

### Red Flags to Watch For

- **Hallucinations** - Made-up facts or data
- **Off-topic content** - Irrelevant information
- **Wrong tone** - Too formal/casual
- **Missing elements** - Incomplete output
- **Inconsistencies** - Contradictory information
- **Vague language** - Lacks specificity
- **Poor organization** - Hard to follow

---

## Continuous Improvement

### Track What Works

Keep a log of:
- Successful prompts
- What made them effective
- Patterns that emerge
- Common refinements needed

### Learn from Failures

When prompts don't work:
- Analyze what went wrong
- Identify missing components
- Note what to add next time
- Update your templates

### Stay Current

- Review new Gemini features
- Learn advanced techniques
- Adapt to platform changes
- Share knowledge with colleagues

### Practice Regularly

- Use AI for daily tasks
- Experiment with variations
- Try new techniques
- Build your skills progressively

---

## Team Best Practices

### Standardization

- Use consistent frameworks (TCFC)
- Share successful templates
- Document common patterns
- Create team guidelines

### Knowledge Sharing

- Share prompt libraries
- Discuss what works
- Learn from each other
- Build collective expertise

### Quality Standards

- Define output criteria
- Review AI-generated content
- Maintain consistency
- Ensure accuracy

---

## Ethical Considerations

### Transparency

- Disclose when content is AI-generated (if required)
- Don't claim AI work as entirely your own
- Be honest about AI assistance

### Accuracy

- Verify facts and data
- Don't spread misinformation
- Check for hallucinations
- Validate important information

### Privacy

- Don't include confidential information in prompts
- Be careful with personal data
- Follow company policies
- Respect privacy regulations

### Responsibility

- Review AI outputs before using
- Take responsibility for final content
- Don't blindly trust AI
- Apply human judgment

---

## Quick Reference

### The Perfect Prompt Formula

```
[TASK] [Specific action] [what you're working with]

[CONTEXT]
- Audience: [who this is for]
- Purpose: [why you're creating this]
- Background: [relevant situation]

[FORMAT]
- Structure: [how to organize]
- Sections: [what to include]
- Style: [presentation approach]

[CONSTRAINTS]
- Length: [word/paragraph count]
- Tone: [voice and style]
- Requirements: [must-haves]
- Exclusions: [what to avoid]
```

### Success Checklist

- [ ] Task is clear and specific
- [ ] Context provides necessary background
- [ ] Format specifies structure
- [ ] Constraints define boundaries
- [ ] All required information included
- [ ] No vague or ambiguous terms
- [ ] Audience is defined
- [ ] Purpose is stated
- [ ] Success criteria are clear

---

[← Troubleshooting Guide](troubleshooting-guide.md) | [Home](../README.md) | [Additional Learning →](additional-learning.md)
