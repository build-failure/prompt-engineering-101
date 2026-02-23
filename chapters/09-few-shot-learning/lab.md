# Lab 9: Few-Shot Learning with Examples

← [Lesson 9](lesson.md) | [Home](../../README.md) | [Next: Lab 10 →](../10-accuracy-hallucinations/lab.md)

---

## Overview

**Chapter**: 9 - Few-Shot Learning with Examples  
**Level**: Intermediate  
**Estimated Time**: 30 minutes  
**Prerequisites**: Complete Lesson 9

## Learning Objectives

By completing this lab, you will:
- Practice using examples to teach AI patterns
- Learn to select effective examples
- Master few-shot prompting techniques
- Apply pattern learning to business scenarios

## Business Scenario

Your company has specific styles, formats, and tones that need to be maintained across all communications. Instead of writing lengthy descriptions of your style, you can show AI examples of your best work and have it replicate the pattern. This ensures consistency and saves time explaining every detail.

## Materials Needed

- Access to Google Gemini
- Sample examples provided in exercises
- Optional: Your own company examples to practice with

---

## Exercise 1: Email Response Style

**Objective**: Use examples to maintain consistent customer service tone

**Scenario**: Your support team needs to respond to customer inquiries with a friendly, helpful, and professional tone.

### Your Task

Create a few-shot prompt to generate customer responses:

```
Respond to customer inquiries in our support style.

Here are examples of our tone:

Example 1:
Customer: "When will my order ship?"
Response: "Great question! Your order is scheduled to ship tomorrow (March 15th). You'll get a tracking number via email as soon as it's on its way. Anything else I can help with?"

Example 2:
Customer: "Can I change my subscription?"
Response: "Absolutely! You can upgrade or downgrade anytime. Just go to Account > Subscription > Change Plan. Takes about 30 seconds. Let me know if you'd like me to walk you through it!"

Example 3:
Customer: "I got charged twice"
Response: "Oh no, I'm so sorry about that! Let me look into this right away. Can you send me your order number? I'll make sure we get this corrected and refunded within 24 hours."

Now respond to this customer inquiry:
"How do I reset my password? I've tried the forgot password link but didn't get an email."
```

**Expected Output**:
A response that matches the friendly, helpful tone with:
- Empathetic acknowledgment
- Clear solution steps
- Offer of additional help
- Positive, can-do attitude

**Validation Prompt**:
```
I'm practicing few-shot learning for customer support responses:

My prompt with examples: [paste your prompt]

Generated response: [paste Gemini's output]

Please assess:
1. Does the response match the tone of the examples?
2. Is it friendly, helpful, and professional?
3. Does it follow the pattern (acknowledge, solve, offer help)?
4. Would this response satisfy a customer?
5. What could improve the examples or prompt?
```

### Success Criteria
- [ ] Included 3 diverse examples showing the pattern
- [ ] Examples demonstrate key tone characteristics
- [ ] Generated response matches the style
- [ ] Response is helpful and actionable
- [ ] Tone is consistent with examples

**Troubleshooting**:
- **Issue**: Response is too formal or robotic
  **Solution**: Add more personality to your examples, use contractions and friendly language
- **Issue**: Response doesn't follow the pattern
  **Solution**: Add explicit instruction: "Follow the same structure: acknowledge, provide solution, offer additional help"

---

## Exercise 2: Brand Voice for Social Media

**Objective**: Teach AI your brand's social media voice through examples

**Scenario**: Your company has a distinct social media voice that's casual, encouraging, and emoji-friendly.

### Your Task

Create a few-shot prompt for social media posts:

```
Write social media posts in our brand voice.

Here are examples of our style:

Example 1 (Product Feature):
"🎉 New feature alert! Now you can schedule posts across all platforms in one click. Because your time is precious. Try it free for 14 days → [link] #ProductivityHack"

Example 2 (Tip):
"💡 Pro tip: The best time to post? When your audience is actually online. Check your analytics → find your peak hours → schedule accordingly. Simple but effective. 📊"

Example 3 (Customer Story):
"❤️ 'This tool saved me 10 hours a week' - Sarah, Marketing Manager. Stories like this fuel our team. What's your favorite feature? Drop a comment below! 👇"

Example 4 (Behind the Scenes):
"☕ Monday morning at HQ: Our dev team just shipped 3 new features. Our design team is perfecting the mobile app. Our support team is crushing it with 98% satisfaction. We're building something special. 🚀"

Now write a post announcing: We just hit 50,000 users milestone
```

**Expected Output**:
A social media post that:
- Uses emojis appropriately
- Has an encouraging, celebratory tone
- Includes a call-to-action or engagement prompt
- Matches the casual but professional style
- Uses short, punchy sentences

**Validation Prompt**:
```
I'm using few-shot learning for social media posts:

My prompt with examples: [paste your prompt]

Generated post: [paste Gemini's output]

Please assess:
1. Does the post match the brand voice from examples?
2. Is the emoji usage appropriate and similar?
3. Does it have the same energy and tone?
4. Would this fit naturally in the feed with the examples?
5. Is there a clear call-to-action or engagement element?
```

### Success Criteria
- [ ] Included 3-4 diverse examples (different post types)
- [ ] Examples show consistent voice across scenarios
- [ ] Generated post matches tone and style
- [ ] Emoji usage is appropriate
- [ ] Post encourages engagement

**Troubleshooting**:
- **Issue**: Too many or too few emojis
  **Solution**: Count emojis in your examples and note the pattern (typically 2-4 per post)
- **Issue**: Tone is off (too corporate or too casual)
  **Solution**: Review your examples - they set the standard. Adjust them to your ideal tone

---

## Exercise 3: Report Formatting Consistency

**Objective**: Use examples to maintain consistent report structure

**Scenario**: Your team creates weekly project status reports that need to follow a specific format.

### Your Task

Create a few-shot prompt for status reports:

```
Create a project status report following our standard format.

Here are examples:

Example 1:
**Project:** Website Redesign
**Status:** 🟢 On Track
**Progress:** 65% complete
**This Week:** 
- Completed homepage mockups
- Started mobile designs
- Conducted user testing session
**Next Week:** 
- Finalize mobile designs
- Begin development phase
- Set up staging environment
**Blockers:** None
**Budget:** $45K spent of $60K (75%)
**Notes:** User testing feedback was very positive. On schedule for May 15 launch.

Example 2:
**Project:** CRM Migration
**Status:** 🟡 At Risk
**Progress:** 40% complete
**This Week:**
- Completed data mapping
- Started testing phase
- Identified data quality issues
**Next Week:**
- Address data quality issues
- Continue testing
- Train support team
**Blockers:** Waiting on IT approval for server access (requested March 10)
**Budget:** $30K spent of $50K (60%)
**Notes:** Data quality issues may delay timeline by 1 week. Working with IT to expedite server access.

Now create a status report for:
Project: Mobile App Launch
Status: On track
Progress: 80% complete
This week: Completed beta testing, fixed 23 bugs, submitted to app stores
Next week: Monitor app store review, prepare launch marketing, train customer support
No blockers
Budget: $72K of $80K spent
Note: App store review typically takes 2-3 days, launch planned for April 1
```

**Expected Output**:
A status report that:
- Follows the exact format structure
- Uses appropriate status emoji
- Includes all required sections
- Maintains professional tone
- Provides actionable information

**Validation Prompt**:
```
I'm using few-shot learning for status reports:

My prompt with examples: [paste your prompt]

Generated report: [paste Gemini's output]

Please assess:
1. Does the report follow the exact format from examples?
2. Are all sections present and properly formatted?
3. Is the status indicator appropriate?
4. Is the information clear and actionable?
5. Would this report be useful for stakeholders?
```

### Success Criteria
- [ ] Examples show consistent format structure
- [ ] Generated report matches format exactly
- [ ] All required sections are present
- [ ] Information is clear and organized
- [ ] Professional tone maintained

**Troubleshooting**:
- **Issue**: Format is inconsistent
  **Solution**: Make sure all examples use identical section headers and structure
- **Issue**: Missing sections
  **Solution**: Add instruction: "Include all sections shown in examples, even if some are 'None' or 'N/A'"

---

## Exercise 4: Tone Transformation

**Objective**: Use examples to show how to adapt content for different audiences

**Scenario**: You need to communicate the same information to different audiences with appropriate tone for each.

### Your Task

Create a few-shot prompt showing tone adaptation:

```
Adapt this message for different audiences, following these examples:

Example 1 - Quarterly Results:

For Executives:
"Q1 revenue increased 15% YoY to $2.3M, driven by enterprise sales growth of 28%. Customer acquisition cost decreased 12% while retention improved to 94%. Recommend increasing sales team headcount by 3 to capitalize on enterprise momentum."

For Team:
"Amazing quarter, team! We hit $2.3M in revenue - that's 15% growth from last year. Our enterprise sales were the star performers, and we're keeping customers happy with 94% retention. Leadership is considering expanding our team based on these results. Great work everyone!"

For Customers:
"We're growing! Thanks to customers like you, we're serving more businesses than ever and investing in new features. This quarter we expanded our team and improved our platform. You'll see faster support responses and exciting new capabilities coming soon."

Example 2 - System Maintenance:

For Executives:
"Scheduled maintenance Sunday 2-4 AM EST. Zero customer impact expected. Upgrading database infrastructure for 40% performance improvement and enhanced security compliance."

For Team:
"Heads up: We're doing system maintenance Sunday 2-4 AM EST. Customers won't notice anything, but we'll have someone on call just in case. This upgrade will make everything faster and more secure. Check Slack for the maintenance channel if you're around."

For Customers:
"Quick heads up: We're making improvements to our system Sunday night (2-4 AM EST). You won't experience any downtime, but you might notice things running even faster afterward! We're always working to give you the best experience."

Now adapt this message for all three audiences:
"We're launching a new mobile app next month with offline mode, dark theme, and faster sync. Beta testing showed 95% satisfaction. The app will be free for all current users."
```

**Expected Output**:
Three versions of the message:
- Executive version: Data-focused, strategic, concise
- Team version: Celebratory, inclusive, motivating
- Customer version: Benefit-focused, friendly, exciting

**Validation Prompt**:
```
I'm using few-shot learning to adapt tone for audiences:

My prompt with examples: [paste your prompt]

Generated versions: [paste all three outputs]

Please assess:
1. Does each version match the tone of its example category?
2. Is the executive version data-driven and strategic?
3. Is the team version motivating and inclusive?
4. Is the customer version benefit-focused and friendly?
5. Do all versions convey the same core information?
```

### Success Criteria
- [ ] Provided 2 complete example sets (6 total examples)
- [ ] Examples clearly show tone differences
- [ ] Generated versions match respective tones
- [ ] Core information preserved across versions
- [ ] Each version appropriate for its audience

**Troubleshooting**:
- **Issue**: Tones are too similar
  **Solution**: Make your examples more distinct - exaggerate the differences slightly
- **Issue**: Missing key information in some versions
  **Solution**: Add instruction: "Ensure all versions include the core facts, adapted for audience"

---

## Exercise 5: Email Signature Pattern

**Objective**: Use examples to replicate exact formatting patterns

**Scenario**: Your company has a specific email signature format that needs to be consistent across all employees.

### Your Task

Create a few-shot prompt for email signatures:

```
Create an email signature following our company format.

Here are examples:

Example 1:
John Smith | Senior Marketing Manager
Acme Corp | john.smith@acme.com | (555) 123-4567
LinkedIn: linkedin.com/in/johnsmith | Schedule a meeting: calendly.com/johnsmith

Example 2:
Sarah Johnson | Product Designer
Acme Corp | sarah.j@acme.com | (555) 234-5678
Portfolio: sarahjohnson.design | LinkedIn: linkedin.com/in/sarahjohnson

Example 3:
Michael Chen | VP of Sales
Acme Corp | m.chen@acme.com | (555) 345-6789
LinkedIn: linkedin.com/in/michaelchen | Mobile: (555) 999-8888

Example 4:
Jennifer Martinez | Customer Success Lead
Acme Corp | jennifer.martinez@acme.com | (555) 456-7890
LinkedIn: linkedin.com/in/jennifermartinez | Support: help.acmecorp.com

Now create signatures for:

1. David Park | Data Analyst
   Email: david.park@acme.com | Phone: (555) 567-8901
   LinkedIn: linkedin.com/in/davidpark | GitHub: github.com/davidpark

2. Lisa Thompson | HR Director
   Email: l.thompson@acme.com | Phone: (555) 678-9012
   LinkedIn: linkedin.com/in/lisathompson | Schedule: calendly.com/lisathompson
```

**Expected Output**:
Two email signatures that:
- Follow the exact format pattern
- Use consistent separators (|)
- Include company name
- Have appropriate optional links
- Match the professional style

**Validation Prompt**:
```
I'm using few-shot learning for email signatures:

My prompt with examples: [paste your prompt]

Generated signatures: [paste both outputs]

Please assess:
1. Do the signatures follow the exact format from examples?
2. Are separators and spacing consistent?
3. Are optional elements (LinkedIn, etc.) formatted correctly?
4. Would these signatures look professional in emails?
5. Is the pattern clear and replicable?
```

### Success Criteria
- [ ] Provided 3-4 diverse examples
- [ ] Examples show consistent formatting
- [ ] Generated signatures match format exactly
- [ ] Spacing and separators are consistent
- [ ] Optional elements handled appropriately

**Troubleshooting**:
- **Issue**: Formatting is inconsistent
  **Solution**: Check your examples for exact spacing and separator usage - AI will copy it precisely
- **Issue**: Optional elements in wrong format
  **Solution**: Show variety in examples - some with calendly, some with portfolio, etc.

---

## Reflection Questions

1. **How did examples improve AI's understanding?** Compare outputs with and without examples.

2. **What makes a good example?** Think about quality, relevance, and clarity.

3. **How many examples do you typically need?** Reflect on when 2 examples were enough vs. when you needed 4-5.

4. **How will you collect examples for your work?** Consider building a library of your best work.

---

## Key Takeaways

- **Examples teach patterns better than descriptions** - Show, don't just tell
- **Quality matters more than quantity** - 3 great examples beat 10 mediocre ones
- **Consistency in examples ensures consistency in output** - AI replicates what it sees
- **Diverse examples show range** - Include variations within your pattern
- **Few-shot learning saves time** - No need to explain every detail

---

## Next Steps

Excellent work! You now know how to use examples to teach AI your specific patterns and styles.

**To continue improving:**

1. **Build an example library** - Collect your best work for future prompts
2. **Apply to your work** - Use few-shot learning for any task requiring consistency
3. **Move to Chapter 10** - Learn about reducing hallucinations and improving accuracy
4. **Experiment** - Try different numbers of examples to find your sweet spot

**Ready for more?** → [Chapter 10: Reducing Hallucinations and Improving Accuracy](../10-accuracy-hallucinations/lesson.md)

---

## Additional Practice (Optional)

Try creating few-shot prompts for these scenarios:

1. **Product descriptions**: Show 3 examples of your product copy style
2. **Meeting notes**: Demonstrate your preferred note-taking format
3. **Code comments**: Show how you want code documented
4. **Presentation titles**: Examples of engaging slide titles
5. **Blog post intros**: Show your blog's opening paragraph style

---

## Navigation

- **Previous**: [Lesson 9: Few-Shot Learning with Examples](lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 10: Reducing Hallucinations and Improving Accuracy](../10-accuracy-hallucinations/lesson.md)
- **Resources**: [Quick Reference](../../QUICK_REFERENCE.md) | [Templates](../../templates/)

---

**Lab 9 Complete!** 🎉 You've mastered few-shot learning!
