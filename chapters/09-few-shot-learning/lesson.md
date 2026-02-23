# Chapter 9: Few-Shot Learning with Examples

← [Previous: Chapter 8 - Step-by-Step Reasoning](../08-step-by-step/lesson.md) | [Home](../../README.md) | [Next: Chapter 10 - Accuracy and Hallucinations →](../10-accuracy-hallucinations/lesson.md)

---

## Overview

**Level:** Intermediate  
**Duration:** 30 minutes  
**Prerequisites:** Chapters 1-8

## Learning Objectives

- Understand how examples teach AI patterns
- Learn to select effective examples
- Master few-shot prompting techniques
- Apply pattern learning to business tasks

---

## What is Few-Shot Learning?

Few-shot learning is teaching AI by showing examples of what you want. Instead of just describing the desired output, you demonstrate it.

### The Learning Spectrum

**Zero-Shot:** No examples, just instructions
```
Write a product description in our brand voice.
```

**One-Shot:** One example to show the pattern
```
Here's an example of our brand voice:
[example]

Now write a product description in the same style.
```

**Few-Shot:** Multiple examples (typically 2-5)
```
Here are 3 examples of our brand voice:
[example 1]
[example 2]
[example 3]

Now write a product description in the same style.
```

---

## Why Examples Work

Examples help AI understand:
- **Style and tone** - How to write
- **Format and structure** - How to organize
- **Level of detail** - How much to include
- **Patterns and conventions** - What's expected

### The Power of Pattern Recognition

**Without examples:**
```
Write a professional email signature.
```
Result: Generic, may not match your style.

**With examples:**
```
Create an email signature following this pattern:

Example 1:
John Smith | Senior Marketing Manager
Acme Corp | john.smith@acme.com | (555) 123-4567
LinkedIn: linkedin.com/in/johnsmith

Example 2:
Sarah Johnson | Product Designer
Acme Corp | sarah.j@acme.com | (555) 234-5678
Portfolio: sarahjohnson.design

Now create one for:
Mike Chen | Data Analyst
mike.chen@acme.com | (555) 345-6789
```
Result: Matches your exact format and style.

---

## How Many Examples?

### Zero-Shot (No Examples)
**When to use:**
- Task is straightforward
- Standard format is fine
- You don't have specific style requirements

**Example:**
```
Summarize this article in 3 bullet points.
```

### One-Shot (1 Example)
**When to use:**
- Pattern is simple
- You have one good example
- Want to show general direction

**Example:**
```
Transform technical jargon into simple language.

Example:
Technical: "Utilize the API endpoint to authenticate"
Simple: "Use the login button to sign in"

Now transform: "Implement the authentication protocol"
```

### Few-Shot (2-5 Examples)
**When to use:**
- Pattern is complex
- Style is specific
- Consistency is critical
- Format has nuances

**Example:**
```
Write customer responses in our support style.

Example 1:
Customer: "The app crashed"
Response: "Thanks for reporting this! I'm sorry the app crashed. Can you tell me what you were doing when it happened? This helps us fix it faster."

Example 2:
Customer: "How do I export data?"
Response: "Great question! Here's how to export: Click Settings > Data > Export. You'll get a CSV file. Let me know if you need help with any step!"

Example 3:
Customer: "This feature doesn't work"
Response: "I appreciate you letting us know! To help troubleshoot, could you share: 1) What feature, 2) What happens when you try it? We'll get this sorted out."

Now respond to: "I can't find my saved files"
```

---

## Selecting Effective Examples

### Quality Over Quantity

**Good examples are:**
- ✅ Representative of desired output
- ✅ Clear and well-executed
- ✅ Diverse enough to show range
- ✅ Consistent in quality
- ✅ Relevant to the task

**Avoid examples that:**
- ❌ Are mediocre or flawed
- ❌ Are too similar to each other
- ❌ Don't represent your best work
- ❌ Are outdated or off-brand
- ❌ Are too complex or simple

### Example Selection Checklist

- [ ] Does this example show the pattern clearly?
- [ ] Is this the quality I want to replicate?
- [ ] Does it demonstrate key characteristics?
- [ ] Is it similar enough to the new task?
- [ ] Would I be happy if AI copied this style?

---

## Formatting Examples in Prompts

### Basic Format

```
Here are examples of [what you want]:

Example 1:
[example content]

Example 2:
[example content]

Now create [new item] following the same pattern.
```

### Input-Output Format

```
Transform [input type] into [output type].

Example 1:
Input: [example input]
Output: [example output]

Example 2:
Input: [example input]
Output: [example output]

Now transform:
Input: [new input]
```

### Labeled Components Format

```
Create [item] with these components:

Example 1:
[Component A]: [content]
[Component B]: [content]
[Component C]: [content]

Example 2:
[Component A]: [content]
[Component B]: [content]
[Component C]: [content]

Now create for: [new scenario]
```

---

## Real-World Applications

### Email Response Style

**Scenario:** Maintain consistent customer service tone

```
Respond to customer inquiries in our friendly, helpful style:

Example 1:
Q: "When will my order ship?"
A: "Great question! Your order is scheduled to ship tomorrow (March 15th). You'll get a tracking number via email as soon as it's on its way. Anything else I can help with?"

Example 2:
Q: "Can I change my subscription?"
A: "Absolutely! You can upgrade or downgrade anytime. Just go to Account > Subscription > Change Plan. Takes about 30 seconds. Let me know if you'd like me to walk you through it!"

Example 3:
Q: "I got charged twice"
A: "Oh no, I'm so sorry about that! Let me look into this right away. Can you send me your order number? I'll make sure we get this corrected and refunded within 24 hours."

Now respond to: "How do I cancel my trial?"
```

### Report Formatting

**Scenario:** Generate reports with company-specific structure

```
Create a project status report following our format:

Example 1:
**Project:** Website Redesign
**Status:** 🟢 On Track
**Progress:** 65% complete
**This Week:** Completed homepage mockups, started mobile designs
**Next Week:** Finalize mobile designs, begin development
**Blockers:** None
**Budget:** $45K spent of $60K (75%)

Example 2:
**Project:** CRM Migration
**Status:** 🟡 At Risk
**Progress:** 40% complete
**This Week:** Data mapping completed, testing phase started
**Next Week:** Continue testing, address data quality issues
**Blockers:** Waiting on IT approval for server access
**Budget:** $30K spent of $50K (60%)

Now create for:
Project: Mobile App Launch
Status: On track, 80% complete
This week: Beta testing, bug fixes
Next week: Final QA, app store submission
No blockers
Budget: $72K of $80K spent
```

### Social Media Posts

**Scenario:** Match brand voice across platforms

```
Write social media posts in our brand voice:

Example 1 (Product Launch):
"🎉 Say hello to our newest feature! Now you can schedule posts across all platforms in one click. Because your time is precious. Try it free for 14 days → [link]"

Example 2 (Tip):
"💡 Pro tip: The best time to post? When your audience is actually online. Check your analytics → find your peak hours → schedule accordingly. Simple but effective."

Example 3 (Customer Story):
"❤️ 'This tool saved me 10 hours a week' - Sarah, Marketing Manager. Stories like this fuel our team. What's your favorite feature? Drop a comment below!"

Now write a post about: New integration with Google Workspace
```

---

## Common Use Cases

### 1. Maintaining Brand Voice

Use examples to ensure consistency:
- Marketing copy
- Customer communications
- Social media content
- Blog posts
- Product descriptions

### 2. Standardizing Formats

Use examples to replicate structure:
- Report templates
- Email signatures
- Meeting agendas
- Status updates
- Documentation

### 3. Teaching Transformations

Use examples to show conversions:
- Technical → Simple language
- Long → Short summaries
- Formal → Casual tone
- Data → Insights
- Features → Benefits

### 4. Demonstrating Quality

Use examples to set standards:
- Writing quality
- Detail level
- Professionalism
- Completeness
- Accuracy

---

## Advanced Techniques

### Progressive Examples

Show evolution or improvement:

```
Improve this email from good to great:

Version 1 (Good):
"Thanks for your email. I'll look into this and get back to you soon."

Version 2 (Better):
"Thanks for reaching out! I'll investigate this issue and have an update for you by end of day tomorrow."

Version 3 (Great):
"Thanks for bringing this to my attention! I'm looking into it right now and will email you a detailed update by 5 PM tomorrow. In the meantime, here's a workaround you can try: [solution]."

Now improve: "I received your message and will respond later."
```

### Contrasting Examples

Show what to do AND what not to do:

```
Write professional emails (not casual texts):

❌ Bad Example:
"hey can u send me that report? thx"

✅ Good Example:
"Hi Sarah, could you please send me the Q1 sales report when you have a moment? Thank you!"

❌ Bad Example:
"got it"

✅ Good Example:
"Thank you for the update. I've noted the changes and will proceed accordingly."

Now write a professional request for: asking colleague to review document
```

### Contextual Examples

Show how context changes output:

```
Adapt tone based on audience:

For Executives:
"Q1 revenue increased 15% YoY to $2.3M, driven by enterprise sales. Recommend doubling sales team investment."

For Team:
"Great quarter, team! We hit $2.3M in revenue (up 15% from last year). Enterprise sales were the star performer. Leadership is considering expanding our team based on these results."

For Customers:
"We're growing! Thanks to customers like you, we're serving more businesses than ever. This means more features, better support, and continued innovation."

Now write for: Announcing new product feature
Audiences: Executives, Team, Customers
```

---

## Troubleshooting Few-Shot Prompts

### Problem: AI Doesn't Follow Pattern

**Solutions:**
- Add more examples (3-5 instead of 1-2)
- Make examples more similar to target task
- Explicitly state what pattern to follow
- Label key components in examples

### Problem: Output Quality Varies

**Solutions:**
- Ensure all examples are high quality
- Make examples more consistent
- Add explicit quality criteria
- Include more diverse examples

### Problem: AI Copies Too Literally

**Solutions:**
- Add "following the same style/pattern" language
- Show examples with variation
- Emphasize adapting to new context
- Include instruction to be creative within pattern

### Problem: Examples Are Too Different

**Solutions:**
- Choose more similar examples
- Focus on one pattern at a time
- Explain what they have in common
- Simplify to core pattern

---

## Few-Shot Checklist

Before using few-shot learning:

- [ ] Have I selected 2-5 high-quality examples?
- [ ] Do examples clearly show the desired pattern?
- [ ] Are examples consistent in quality and style?
- [ ] Are examples relevant to the new task?
- [ ] Have I formatted examples clearly?
- [ ] Have I explained what pattern to follow?
- [ ] Are examples diverse enough to show range?

---

## Key Takeaways

1. **Examples teach patterns** - Show, don't just tell
2. **Quality matters** - Use your best examples
3. **2-5 is the sweet spot** - Enough to show pattern, not too many
4. **Format clearly** - Make examples easy to understand
5. **Match the task** - Examples should be similar to target
6. **Consistency is key** - Maintain style across examples

---

## What's Next

You now know how to use examples to teach AI your specific patterns and styles!

**Next Steps:**
1. Complete [Lab 9](lab.md) to practice few-shot learning
2. Collect examples of your best work for future prompts
3. Create few-shot templates for recurring tasks

In **Chapter 10**, we'll tackle accuracy and hallucinations - learning how to ensure AI outputs are factually correct and reliable.

---

## Navigation

- **Previous**: [Chapter 8: Step-by-Step Reasoning](../08-step-by-step/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 10: Reducing Hallucinations](../10-accuracy-hallucinations/lesson.md)
- **Lab**: [Lab 9: Few-Shot Learning Exercises](lab.md)

---

**Chapter 9 Complete!** Ready to practice? → [Start Lab 9](lab.md)
