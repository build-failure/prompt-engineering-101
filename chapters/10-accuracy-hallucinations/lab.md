# Lab 10: Reducing Hallucinations and Improving Accuracy

← [Lesson 10](lesson.md) | [Home](../../README.md) | [Next: Lab 11 →](../11-multi-step-workflows/lab.md)

---

## Overview

**Chapter**: 10 - Reducing Hallucinations and Improving Accuracy  
**Level**: Advanced  
**Estimated Time**: 35 minutes  
**Prerequisites**: Complete Lesson 10

## Learning Objectives

By completing this lab, you will:
- Identify hallucinations in AI-generated content
- Apply techniques to improve factual accuracy
- Practice verification and validation strategies
- Build reliable prompts for critical business tasks

## Business Scenario

You're responsible for creating accurate business reports and communications where factual errors could have serious consequences. You need to ensure that AI-generated content is reliable, verifiable, and free from fabricated information. In this lab, you'll practice techniques to prevent hallucinations and verify accuracy in real business contexts.

## Materials Needed

- Access to Google Gemini
- Sample data provided in exercises
- 35 minutes of focused time

---

## Exercise 1: Spot the Hallucinations

**Objective**: Learn to identify fabricated information in AI outputs

**Scenario**: You asked AI to summarize quarterly sales performance, but you only provided partial data.

### Your Task

Review these AI outputs and identify the hallucinations:

**Your Original Prompt:**
```
Summarize our Q2 sales performance.

Data provided:
- Total revenue: $3.2M
- New customers: 45
```

**AI Output 1:**
```
Q2 Sales Performance Summary:

Our Q2 revenue reached $3.2M, representing a 23% increase over Q1. We acquired
45 new customers, bringing our total customer base to 487. The average deal
size was $71,111, up from $65,000 in Q1. Our top-performing region was the
Northeast, contributing 42% of total revenue. Customer satisfaction scores
improved to 4.7/5.0, and our Net Promoter Score reached 68.
```

**AI Output 2:**
```
Q2 Sales Performance Summary:

Revenue: $3.2M
New customers: 45

Note: Additional metrics (growth rate, total customers, deal size, regional
performance, satisfaction scores) were not provided in the source data.
```

### Identify the Hallucinations

In Output 1, mark which claims are hallucinations:

- [ ] "23% increase over Q1" - Not provided
- [ ] "Total customer base to 487" - Not provided
- [ ] "Average deal size was $71,111" - Not provided
- [ ] "Northeast contributed 42%" - Not provided
- [ ] "Customer satisfaction 4.7/5.0" - Not provided
- [ ] "Net Promoter Score reached 68" - Not provided

**Which output is better and why?**

<details>
<summary>Click to reveal analysis</summary>

**Output 2 is correct.** It only reports the data provided and explicitly notes what's missing.

**Output 1 contains multiple hallucinations:**
- All the checked items above are fabricated
- The numbers sound plausible but are invented
- Percentages and metrics appear authoritative but are false

**Key lesson:** AI will confidently fill gaps with plausible-sounding data when information is missing.

</details>

### Success Criteria
- [ ] Identified all hallucinated claims in Output 1
- [ ] Understood why Output 2 is more reliable
- [ ] Recognized how AI fills information gaps

**Troubleshooting**:
- **Issue**: Hard to tell what's real vs. fabricated
  **Solution**: Compare every claim in the output against the original data provided. If it's not in the source, it's likely a hallucination.

---

## Exercise 2: Write an Accuracy-Focused Prompt

**Objective**: Create prompts that prevent hallucinations

**Scenario**: You need to analyze customer feedback data accurately.

### Your Task

Improve this prompt to prevent hallucinations:

**Original Prompt (Prone to Hallucinations):**
```
Analyze this customer feedback and tell me what customers think about our product.

Feedback:
- "Love the new interface!" - Sarah M.
- "Shipping took too long" - John D.
- "Great customer service" - Maria L.
- "Price is too high" - Robert K.
- "Easy to use" - Jennifer T.
```

**Your Improved Prompt:**

Write a version that:
- Constrains AI to only use provided information
- Prevents invented statistics
- Requires evidence for claims
- Handles missing data appropriately

```
[Write your improved prompt here]
```

### Example Solution

<details>
<summary>Click to see example</summary>

```
Analyze this customer feedback using ONLY the information provided below.

RULES:
- Do not invent statistics, percentages, or counts beyond what's given
- Do not add feedback that wasn't provided
- If you identify a theme, cite specific feedback as evidence
- If data is insufficient for a conclusion, state "Insufficient data"
- Do not make assumptions about overall customer sentiment

Customer feedback (5 responses total):
- "Love the new interface!" - Sarah M.
- "Shipping took too long" - John D.
- "Great customer service" - Jennifer T.
- "Price is too high" - Robert K.
- "Easy to use" - Jennifer T.

Format your analysis as:
Theme: [name]
Frequency: [X out of 5 responses]
Evidence: [exact quotes]
Confidence: [High/Medium/Low based on sample size]
```

</details>

### Test Your Prompt

1. Run your improved prompt in Gemini
2. Check if the output stays within the provided data
3. Verify no invented statistics appear

**Validation Prompt**:
```
I'm learning to write accuracy-focused prompts. Here's my improved version:

[Paste your prompt]

Output I received:
[Paste Gemini's output]

Please assess:
1. Does my prompt explicitly constrain AI to provided information?
2. Does the output contain any hallucinations or invented data?
3. What else could I add to improve accuracy?
```

### Success Criteria
- [ ] Prompt includes "use only provided information" constraint
- [ ] Prompt prevents statistical invention
- [ ] Prompt requires evidence/citations
- [ ] Output contains no hallucinations
- [ ] Missing data is handled appropriately

**Troubleshooting**:
- **Issue**: AI still adds extra information
  **Solution**: Add stronger language: "CRITICAL: Do not invent any statistics, percentages, or data points not explicitly provided."

---

## Exercise 3: Financial Data Accuracy

**Objective**: Ensure accuracy in critical financial reporting

**Scenario**: You need to create a financial summary for your manager where accuracy is critical.

### Your Task

Write a prompt that ensures exact accuracy with financial data:

**Context:**
- You have Q3 financial data
- Your manager needs a summary for the board meeting
- Any errors could affect major decisions
- Numbers must be exact (no rounding or estimates)

**Financial Data:**
```
Q3 Financial Results:
Revenue: $4,247,893
Expenses: $3,156,721
