# Data Analysis Prompt Templates

Templates for analyzing data from Google Sheets and generating insights.

---

## Descriptive Analysis

### Summary Statistics
```
Analyze this data and provide summary statistics.

Data: [DESCRIBE OR PASTE DATA]
Time period: [DATE RANGE]
Context: [WHAT THIS DATA REPRESENTS]

Calculate and report:
- Total/sum
- Average/mean
- Median
- Range (min to max)
- Notable outliers
- Distribution patterns

Format: Clear summary with specific numbers
Highlight: Any surprising or significant findings
```

### Trend Identification
```
Analyze this [TIME SERIES DATA] to identify trends.

Data:
"""
[PASTE DATA]
"""

Time period: [RANGE]
Granularity: [DAILY/WEEKLY/MONTHLY/QUARTERLY]

Identify:
- Overall trend direction (up/down/flat)
- Rate of change
- Inflection points (where trend changes)
- Seasonal patterns (if applicable)
- Anomalies or unusual periods

Provide: Specific percentages and dates
Format: Narrative summary with key data points
```

### Pattern Recognition
```
Analyze this data to identify patterns.

Data type: [SALES/TRAFFIC/USAGE/PERFORMANCE]
Data:
"""
[PASTE DATA]
"""

Look for:
- Recurring patterns (daily/weekly/monthly cycles)
- Correlations between variables
- Clusters or groupings
- Unexpected relationships

Provide:
- Description of each pattern found
- Significance (why it matters)
- Specific examples with numbers

Format: Bullet list of patterns with explanations
```

### Anomaly Detection
```
Analyze this data and flag anomalies.

Normal baseline: [DESCRIBE TYPICAL PATTERNS]
Data:
"""
[PASTE DATA]
"""

Identify:
- Values significantly outside normal range
- Unexpected spikes or drops
- Missing or inconsistent data
- Timing of anomalies

For each anomaly:
- What it is (specific numbers)
- When it occurred
- How much it deviates from normal
- Possible explanations

Format: Table or structured list
Priority: Most significant anomalies first
```

---

## Comparative Analysis

### Period-over-Period Comparison
```
Compare [METRIC] between [PERIOD 1] and [PERIOD 2].

Data:
- [PERIOD 1]: [DATA OR DESCRIPTION]
- [PERIOD 2]: [DATA OR DESCRIPTION]

Analyze:
- Absolute change (difference in numbers)
- Percentage change
- Which specific areas improved/declined
- Factors that might explain changes

Format:
- Summary paragraph
- Comparison table
- Key insights (3-5 bullets)

Highlight: Biggest changes and their implications
```

### Segment Comparison
```
Compare performance across these segments:

Segments: [LIST SEGMENTS - regions/products/teams/etc.]
Metric: [WHAT YOU'RE MEASURING]
Data:
"""
[PASTE DATA]
"""

For each segment, provide:
- Performance ranking
- Key metrics
- Comparison to average
- Standout characteristics

Identify:
- Top performers (and why)
- Underperformers (and why)
- Biggest gaps between segments

Format: Comparison table + narrative insights
```

### Benchmark Comparison
```
Compare our performance against benchmarks.

Our data: [PASTE OR DESCRIBE]
Benchmarks: [INDUSTRY STANDARD/COMPETITOR/TARGET]
Metrics: [WHAT TO COMPARE]

For each metric:
- Our performance
- Benchmark value
- Gap (above/below)
- Percentage difference
- Trend (closing gap or widening)

Provide:
- Areas where we exceed benchmarks
- Areas needing improvement
- Priority recommendations

Format: Scorecard style with clear indicators
```

### Variance Analysis
```
Analyze variances between actual and [BUDGET/FORECAST/TARGET].

Actual results: [DATA]
Expected results: [DATA]
Time period: [RANGE]

For each significant variance:
- Amount of variance (absolute and %)
- Favorable or unfavorable
- Likely causes
- Impact on overall performance
- Recommended actions

Threshold: Flag variances over [PERCENTAGE]%
Format: Variance report with explanations
Priority: Largest or most critical variances first
```

---

## Insight Generation

### Key Findings from Data
```
Analyze this data and extract key findings.

Data context: [WHAT THIS DATA REPRESENTS]
Business question: [WHAT WE'RE TRYING TO UNDERSTAND]
Data:
"""
[PASTE DATA]
"""

Provide:
- Top 3-5 most important findings
- Supporting evidence (specific numbers)
- Why each finding matters
- Implications for [BUSINESS/TEAM/STRATEGY]

Format: Executive summary style
Tone: Insights-focused, not just data reporting
```

### Actionable Recommendations
```
Based on this data analysis, provide actionable recommendations.

Analysis summary: [PASTE FINDINGS OR DESCRIBE]
Business context: [GOALS/CHALLENGES/CONSTRAINTS]
Decision timeframe: [WHEN ACTION NEEDED]

For each recommendation:
- Specific action to take
- Expected impact
- Resources required
- Timeline
- Priority (high/medium/low)
- Risks or considerations

Number of recommendations: [3-5]
Format: Prioritized list with details
Focus: Practical actions, not just observations
```

### Risk Identification
```
Analyze this data to identify risks.

Data: [PASTE OR DESCRIBE]
Context: [BUSINESS SITUATION]
Risk tolerance: [HIGH/MEDIUM/LOW]

Identify:
- Potential risks indicated by the data
- Severity of each risk
- Likelihood of occurrence
- Early warning signs
- Mitigation strategies

Format:
- Risk description
- Impact assessment
- Recommended actions

Priority: Most critical risks first
```

### Opportunity Identification
```
Analyze this data to identify opportunities.

Data: [PASTE OR DESCRIBE]
Business goals: [WHAT WE'RE TRYING TO ACHIEVE]
Resources available: [CONSTRAINTS]

Look for:
- Untapped potential
- Positive trends to amplify
- Gaps in market/performance
- Quick wins
- Strategic opportunities

For each opportunity:
- Description
- Potential value/impact
- Effort required
- Timeline to realize
- Priority

Format: Opportunity matrix or prioritized list
```

---

## Specialized Analysis

### Customer Segmentation Analysis
```
Analyze this customer data to identify segments.

Data:
"""
[PASTE CUSTOMER DATA]
"""

Segment by: [BEHAVIOR/DEMOGRAPHICS/VALUE/USAGE]

For each segment:
- Size (number and % of total)
- Characteristics
- Value to business
- Needs and preferences
- Recommended strategies

Provide: 3-5 distinct segments
Format: Segment profiles with actionable insights
```

### Cohort Analysis
```
Perform a cohort analysis on this data.

Data: [PASTE OR DESCRIBE]
Cohort definition: [HOW TO GROUP - by signup date/first purchase/etc.]
Metric to track: [RETENTION/REVENUE/USAGE/etc.]
Time periods: [MONTHLY/QUARTERLY]

Analyze:
- Performance by cohort
- Trends over time
- Which cohorts perform best/worst
- Patterns in cohort behavior
- Implications for [STRATEGY/PRODUCT/MARKETING]

Format: Cohort table + insights
```

### Funnel Analysis
```
Analyze this funnel data.

Funnel stages:
1. [STAGE 1]: [NUMBER]
2. [STAGE 2]: [NUMBER]
3. [STAGE 3]: [NUMBER]
4. [STAGE 4]: [NUMBER]

Calculate:
- Conversion rate at each stage
- Drop-off points
- Overall conversion rate
- Comparison to [BENCHMARK/PREVIOUS PERIOD]

Identify:
- Biggest bottlenecks
- Stages performing well
- Opportunities for improvement
- Recommended optimizations

Format: Funnel visualization description + insights
```

### Root Cause Analysis
```
Analyze this data to identify root causes of [PROBLEM].

Problem: [DESCRIBE ISSUE]
Data:
"""
[PASTE RELEVANT DATA]
"""

Investigate:
- When did the problem start?
- What changed around that time?
- Which factors correlate with the problem?
- What patterns emerge?

Provide:
- Most likely root causes (ranked)
- Supporting evidence from data
- Additional data needed (if any)
- Recommended next steps

Format: Structured analysis with clear conclusions
```

---

## Reporting Templates

### Dashboard Summary
```
Create a dashboard summary from this data.

Data sources: [LIST SOURCES]
Time period: [RANGE]
Audience: [WHO WILL VIEW THIS]

Key metrics to highlight:
- [METRIC 1]: [VALUE AND TREND]
- [METRIC 2]: [VALUE AND TREND]
- [METRIC 3]: [VALUE AND TREND]

For each metric:
- Current value
- Change from previous period
- Status (on track/at risk/behind)
- Brief insight

Format: Dashboard-style summary
Use: Traffic light indicators (🟢🟡🔴) where appropriate
```

### Data Story
```
Tell the story of what this data reveals.

Data: [PASTE OR DESCRIBE]
Audience: [NON-TECHNICAL/EXECUTIVES/TEAM]
Purpose: [INFORM/PERSUADE/EXPLAIN]

Structure the story:
- Setup: What we were looking at and why
- Discovery: What the data shows
- Insight: What it means
- Action: What we should do

Style: Narrative, not just numbers
Include: Specific data points to support the story
Avoid: Technical jargon or complex statistics
```

### Performance Scorecard
```
Create a performance scorecard from this data.

Metrics: [LIST KEY METRICS]
Data: [PASTE OR DESCRIBE]
Targets: [GOALS FOR EACH METRIC]

For each metric:
- Actual performance
- Target
- Variance
- Status indicator
- Trend (improving/declining/stable)
- Brief comment

Format: Scorecard table
Visual: Use symbols or colors to show status
Overall: Summary assessment
```

---

## Tips for Data Analysis Prompts

1. **Provide context** - Explain what the data represents
2. **Specify time periods** - Be clear about date ranges
3. **Define metrics** - Explain what you're measuring
4. **State the goal** - What decision does this support?
5. **Request specific formats** - Tables, charts, narratives
6. **Include benchmarks** - Give AI comparison points
7. **Ask for insights, not just numbers** - Request interpretation

---

## Validation Prompt

```
Please review this data analysis:

**Analysis Goal**: [WHAT WE WERE TRYING TO LEARN]
**Data Context**: [WHAT THE DATA REPRESENTS]

**Analysis Output**:
[Paste the generated analysis]

**Please assess**:
1. Are the insights accurate and meaningful?
2. Is the analysis appropriate for the data type?
3. Are recommendations actionable?
4. Is anything important missing?
5. Is it presented clearly for the intended audience?
6. What would improve this analysis?
```

---

[← Presentation Templates](presentation-templates.md) | [Home](../README.md) | [Meeting Templates →](meeting-templates.md)
