# Chapter 7: Output Formatting and Structure

← [Previous: Chapter 6 - Separating Instructions from Data](../06-instructions-data/lesson.md) | [Home](../../README.md) | [Next: Chapter 8 - Step-by-Step Reasoning →](../08-step-by-step/lesson.md)

---

## Overview

**Level:** Intermediate  
**Duration:** 30 minutes  
**Prerequisites:** Chapters 1-6

## Learning Objectives

- Learn to specify desired output formats
- Understand structured vs. unstructured outputs
- Master format specifications for different use cases
- Ensure consistency in AI-generated content

---

## Why Format Matters

The same information can be presented in many ways. Format affects:
- **Readability** - How easy it is to scan and understand
- **Usability** - Whether you can use it directly
- **Professionalism** - How polished it appears
- **Effectiveness** - Whether it achieves your goal

### Format Changes Everything

**Same content, different formats:**

**Paragraph format:**
```
Our Q1 sales increased by 15% compared to Q4, driven primarily by strong performance in the Northeast region which grew 22%, while the Southwest region declined by 8% due to increased competition. Product A remained our top seller with 45% of revenue, followed by Product B at 30% and Product C at 25%.
```

**Bullet format:**
```
Q1 Sales Summary:
- Overall growth: +15% vs Q4
- Northeast region: +22% (strong performance)
- Southwest region: -8% (increased competition)
- Product A: 45% of revenue (top seller)
- Product B: 30% of revenue
- Product C: 25% of revenue
```

**Table format:**
```
| Metric | Q4 | Q1 | Change |
|--------|----|----|--------|
| Total Sales | $1.0M | $1.15M | +15% |
| Northeast | $400K | $488K | +22% |
| Southwest | $300K | $276K | -8% |
| Product A | $450K | $517K | +15% |
| Product B | $300K | $345K | +15% |
| Product C | $250K | $288K | +15% |
```

Each format serves different purposes!

---

## Common Output Formats

### 1. Bullet Points

**Best for:**
- Lists of items
- Key points
- Action items
- Quick scanning

**How to request:**
```
Format as bullet points:
- [Specification]
- Maximum [X] bullets
- Each bullet [length/style]
```

**Example:**
```
Summarize the meeting decisions as bullet points:
- Start each with an action verb
- Include owner and deadline
- Maximum 5 bullets
- Keep each under 20 words
```

---

### 2. Numbered Lists

**Best for:**
- Sequential steps
- Prioritized items
- Ranked results
- Procedures

**How to request:**
```
Format as numbered list:
1. [Specification]
2. Order by [priority/sequence/importance]
3. Include [details]
```

**Example:**
```
Create a numbered list of implementation steps:
1. Order by sequence (what to do first, second, etc.)
2. Include estimated time for each step
3. Note any dependencies
4. Maximum 10 steps
```

---

### 3. Tables

**Best for:**
- Comparisons
- Data presentation
- Structured information
- Multiple dimensions

**How to request:**
```
Format as table with columns:
- Column 1: [Name]
- Column 2: [Name]
- Column 3: [Name]
Include [X] rows
```

**Example:**
```
Create a comparison table with these columns:
- Competitor Name
- Pricing
- Key Features (3 max)
- Target Market
- Our Advantage

Include our top 5 competitors.
```

---

### 4. Paragraphs

**Best for:**
- Narrative content
- Explanations
- Detailed descriptions
- Flowing text

**How to request:**
```
Format as [X] paragraphs:
- Each paragraph [length]
- Structure: [opening/body/closing]
- Style: [descriptive/persuasive/informative]
```

**Example:**
```
Write as 3 paragraphs:
- Paragraph 1: Problem statement (3-4 sentences)
- Paragraph 2: Our solution (4-5 sentences)
- Paragraph 3: Benefits and call-to-action (3-4 sentences)
Each paragraph maximum 100 words.
```

---

### 5. Sections with Headers

**Best for:**
- Reports
- Documents
- Comprehensive content
- Organized information

**How to request:**
```
Format with these sections:
## Section 1: [Name]
[Content specification]

## Section 2: [Name]
[Content specification]
```

**Example:**
```
Format as a report with these sections:

## Executive Summary
Brief overview in 2-3 sentences

## Key Findings
5-7 bullet points with data

## Recommendations
Numbered list of 3-5 actions

## Next Steps
Timeline with owners
```

---

### 6. Email Format

**Best for:**
- Email communications
- Professional correspondence
- Structured messages

**How to request:**
```
Format as email:
- Subject line: [specification]
- Greeting: [style]
- Body: [structure]
- Closing: [style]
```

**Example:**
```
Format as professional email:
- Subject line: Clear and specific
- Greeting: Professional but warm
- Body: 3 paragraphs (context, main message, next steps)
- Closing: Professional sign-off
- Include: Clear call-to-action
```

---

### 7. Q&A Format

**Best for:**
- FAQs
- Documentation
- Training materials
- Explanations

**How to request:**
```
Format as Q&A:
- [X] questions and answers
- Questions: [style]
- Answers: [length and detail]
```

**Example:**
```
Format as FAQ with 5 Q&A pairs:
- Questions: Start with common question words (What, How, Why)
- Answers: 2-3 sentences each, clear and direct
- Order: Most common questions first
```

---

## Format Specifications

### Length Specifications

Be precise about length:
- "Exactly 5 bullet points"
- "Maximum 200 words"
- "3-4 paragraphs"
- "Between 150-200 words"
- "No more than 10 items"

### Style Specifications

Define the style:
- "Each bullet starts with action verb"
- "Use complete sentences"
- "Short phrases only (no full sentences)"
- "Include specific numbers and dates"
- "Use professional business language"

### Organization Specifications

Specify order and structure:
- "Order by priority (most important first)"
- "Organize chronologically"
- "Group by category"
- "Rank by impact"
- "Sequence by implementation order"

---

## Business Use Cases

### Meeting Agendas

**Format specification:**
```
Create meeting agenda in this format:

**Meeting Details**
- Date, time, location, attendees

**Objectives** (2-3 bullet points)

**Agenda Items** (table format)
| Time | Topic | Owner | Duration |

**Pre-Meeting Preparation**
- Bullet list of what to review

**Expected Outcomes**
- Bullet list of decisions/deliverables
```

---

### Executive Summaries

**Format specification:**
```
Format as executive summary:

**Overview** (1 paragraph, 50 words max)

**Key Findings**
- 5-7 bullet points
- Each with specific data/metrics
- Start with most important

**Recommendations**
1. [Action 1] - Priority: High/Medium/Low
2. [Action 2] - Priority: High/Medium/Low
3. [Action 3] - Priority: High/Medium/Low

**Next Steps** (bullet list with owners and dates)
```

---

### Comparison Documents

**Format specification:**
```
Create comparison in table format:

| Feature/Aspect | Option A | Option B | Option C |
|----------------|----------|----------|----------|
| [Criterion 1] | [Details] | [Details] | [Details] |
| [Criterion 2] | [Details] | [Details] | [Details] |
| [Criterion 3] | [Details] | [Details] | [Details] |

**Summary** (paragraph explaining recommendation)

**Decision Criteria** (ranked list of what matters most)
```

---

### Status Reports

**Format specification:**
```
Format as status report:

**Project:** [Name]
**Period:** [Dates]
**Status:** 🟢 On Track / 🟡 At Risk / 🔴 Behind

**Progress This Period**
- Completed: [bullet list]
- In Progress: [bullet list with % complete]
- Planned: [bullet list]

**Blockers/Issues**
- [Issue 1]: Impact and mitigation
- [Issue 2]: Impact and mitigation

**Metrics**
| Metric | Target | Actual | Status |

**Next Period Focus**
[3-5 bullet points]
```

---

## Ensuring Consistency

### Use Format Templates

Create reusable format specifications:

**Template: Product Description**
```
Format each product description:

**[Product Name]**
*Tagline:* [One compelling sentence]

**Key Features:**
- Feature 1 with benefit
- Feature 2 with benefit
- Feature 3 with benefit

**Best For:** [Target user description]

**Price:** [Pricing info]

**Learn More:** [CTA]
```

### Specify Formatting Rules

Be explicit about formatting:
```
Formatting rules:
- Use title case for all headers
- Bold all section titles
- Italicize product names
- Use bullet points (•) not dashes (-)
- End each bullet with period
- Use consistent date format (MM/DD/YYYY)
- Numbers: Use commas for thousands (1,000 not 1000)
```

### Request Consistency Checks

Ask AI to maintain consistency:
```
Ensure consistent formatting throughout:
- All bullets follow same structure
- All sections have same level of detail
- All examples use same style
- Tone remains consistent
- Terminology is used consistently
```

---

## Format for Different Platforms

### Google Docs

```
Format for Google Docs:
- Use heading styles (Heading 1, Heading 2)
- Include table of contents markers
- Use standard fonts (Arial, Calibri)
- Include page breaks between major sections
- Format for printing (margins, spacing)
```

### Google Sheets

```
Format for Google Sheets import:
- Use tab or comma delimiters
- First row as headers
- One data point per cell
- Numbers without formatting (no $ or %)
- Dates in YYYY-MM-DD format
```

### Google Slides

```
Format for presentation slides:
- Slide title (clear and concise)
- 3-5 bullet points maximum per slide
- Each bullet: 1-2 lines maximum
- Include visual suggestions
- Note where to add charts/images
```

### Email

```
Format for email:
- Subject line (specific and clear)
- Greeting (appropriate for relationship)
- Short paragraphs (2-4 sentences)
- White space between paragraphs
- Clear call-to-action
- Professional signature
```

---

## Common Formatting Mistakes

### 1. No Format Specified

❌ "Summarize this report"
✅ "Summarize this report as 5 bullet points, each highlighting one key finding with supporting data"

### 2. Vague Format Request

❌ "Make it look professional"
✅ "Format as business memo with: header (To/From/Date/Re), 3 sections with bold headers, bullet points for key items"

### 3. Conflicting Format Requirements

❌ "Keep it brief but include lots of detail in paragraph form with bullets"
✅ "Brief overview paragraph (50 words) followed by 5 detailed bullet points (20-30 words each)"

### 4. Platform Mismatch

❌ Requesting complex tables for email
✅ "For email: simple bullet list. For document: detailed comparison table"

---

## Format Checklist

Before submitting, verify:

- [ ] Have I specified the format type? (bullets, table, paragraphs, etc.)
- [ ] Have I defined length/quantity? (how many items, words, etc.)
- [ ] Have I specified organization? (order, grouping, structure)
- [ ] Have I defined style? (complete sentences, phrases, etc.)
- [ ] Is the format appropriate for the platform?
- [ ] Have I requested consistency?
- [ ] Are formatting rules clear?

---

## Key Takeaways

1. **Format affects usability** - Choose format for your purpose
2. **Be specific** - Define exact structure and style
3. **Match format to platform** - Different tools need different formats
4. **Request consistency** - Ensure uniform formatting throughout
5. **Use templates** - Create reusable format specifications

---

## What's Next

You now know how to control output formatting for any business need!

**Next Steps:**
1. Complete [Lab 7](lab.md) to practice format specifications
2. Create format templates for your common tasks
3. Experiment with different formats for the same content

In **Chapter 8**, we'll learn step-by-step reasoning techniques to help AI show its work and improve accuracy.

---

## Navigation

- **Previous**: [Chapter 6: Separating Instructions from Data](../06-instructions-data/lesson.md)
- **Home**: [Course Overview](../../README.md)
- **Next**: [Chapter 8: Step-by-Step Reasoning](../08-step-by-step/lesson.md)
- **Lab**: [Lab 7: Output Formatting Exercises](lab.md)

---

**Chapter 7 Complete!** Ready to practice? → [Start Lab 7](lab.md)
