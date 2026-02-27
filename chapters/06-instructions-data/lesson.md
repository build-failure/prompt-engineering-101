# Chapter 6: Separating Instructions from Data

← [Previous: Chapter 5 - Context and Examples](../05-context-examples/lesson.md) | [Home](../../README.md) | [Next: Chapter 7 - Output Formatting →](../07-output-formatting/lesson.md)

---

## Overview

**Level:** Intermediate  
**Duration:** 30 minutes  
**Prerequisites:** Chapters 1-5

## Learning Objectives

- Understand why instruction-data separation improves clarity
- Learn formatting techniques for data inclusion
- Practice structuring prompts with embedded data
- Handle different data types effectively

---

## The Separation Principle

When your prompt includes both instructions AND data to process, separating them makes everything clearer.

### Why Separate?

**Mixed together (confusing):**
```
Analyze the sales data from January which was $50K, February $45K, March $60K
and identify trends and also the customer feedback saying "great product" and
"slow shipping" and "love the features" and tell me what actions to take.
```

**Separated (clear):**
```
Analyze this sales and feedback data to identify trends and recommend actions.

Sa