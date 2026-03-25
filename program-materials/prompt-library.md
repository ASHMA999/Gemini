# Prompt Library

## Cumulative Collection of All Prompts - Ready to Use

### Arab Potash Company | AI Excellence Program | 2026

---

## How to Use This Library

1. Find the category that matches your task
2. Copy the prompt template
3. Replace [bracketed text] with your specific details
4. Paste into your preferred AI tool
5. Iterate and refine based on the output

---

## Category 1: General Analysis & Reports

### CO-STAR Template (Universal)

```
(C) Context: I am a [your role] at [company/department]. [Describe the situation].

(O) Objective: [Specific task - analyze/summarize/create/compare].

(S) Style: Write as a [professional role or writing style].

(T) Tone: [Formal/professional/empathetic/urgent/objective].

(A) Audience: [Who will read this - executives/engineers/workers/clients].

(R) Response: Deliver as [table/bullet list/report/JSON/numbered steps].
```

### RACE Template (Plans & Projects)

```
(R) Role: You are a [specific professional role with X years experience in Y industry].

(A) Action: [Precise task to perform].

(C) Context: [Operational details - environment, constraints, timeline, history].

(E) Expectation: [Specific deliverables with format requirements].
```

### RTF Template (Quick Tasks)

```
(R) Role: Act as a [specific specialist].

(T) Task: [One clear, specific task].

(F) Format: Deliver as [checklist/table/summary/numbered list/email].
```

### PARA Template (Problem-Solving)

```
(P) Problem: [Describe the problem with data/metrics].

(A) Action: [What analysis or solutions you need].

(R) Result: [Target outcome with timeline].

(A) Adjustment: [Constraints - budget, resources, time, scope].
```

---

## Category 2: HR Department

### Job Description Generator

```
Act as a recruitment specialist at an industrial company located in [location].
Write a job description for [Position Title] including:
- Job Summary (3-4 sentences)
- 5-7 Key Responsibilities
- Required Qualifications (education + experience)
- Technical Skills (list specific tools/certifications)
- Benefits & Perks (emphasize unique location advantages)

Tone: Professional yet attractive to top talent.
Context: [Company name], [industry], [work conditions], [team size].
The role reports to [position] and collaborates with [departments].
```

### Exit Interview Analysis

```
You are an HR analyst specializing in employee retention.

Analyze the following exit interview responses and:
1. Identify the top 3 root causes of resignation
2. Classify causes as: Compensation, Management, Growth, Culture, or Work-Life Balance
3. Compare patterns to industry benchmarks for [industry]
4. Provide 5 actionable recommendations with estimated implementation cost (Low/Med/High)
5. Suggest 3 KPIs to track retention improvement

Format: Executive summary (3 lines) + detailed analysis table + recommendations.
```

### Performance Review Helper

```
Act as an HR consultant. Help me write a performance review for a [job title] covering the period [dates].

Performance data:
- [Key metric 1]: [value]
- [Key metric 2]: [value]
- [Notable achievement or concern]

Include:
1. Strengths (3 bullet points with evidence)
2. Areas for improvement (2 bullet points with specific, actionable suggestions)
3. Goals for next period (3 SMART goals)
4. Overall rating recommendation with justification

Tone: Constructive, fair, and development-focused.
```

### Training Needs Assessment

```
You are an L&D specialist for [industry].

Based on the following department performance data and skills gaps:
[Paste data or describe gaps]

Create a training needs assessment that includes:
1. Skills gap analysis table: [Skill] [Current Level] [Required Level] [Gap] [Priority]
2. Recommended training programs (internal and external)
3. Estimated costs and timeline
4. Expected ROI of addressing each gap
5. Suggested delivery methods (classroom, e-learning, OJT, mentoring)

Constraint: Total annual training budget is [amount].
```

---

## Category 3: Production Department

### Daily Production Report

```
Generate a daily production report for [date] using the following data:
[Paste or describe production data]

Include:
1. Executive Summary (3 lines highlighting key numbers)
2. Actual vs. Target comparison table by product line
3. Gap Analysis with root cause for any variance > 5%
4. Downtime log: [Equipment] [Duration] [Cause] [Corrective Action]
5. Recommendations for next shift
6. Running weekly/monthly cumulative performance

Format: Concise, scannable. Use traffic light colors (Green/Yellow/Red) for KPI status.
```

### Root Cause Analysis (5-Why + Fishbone)

```
You are a Six Sigma Black Belt in [industry].

Perform a root cause analysis for the following problem:
Problem: [Describe the problem with data]
When: [Date/time/shift]
Where: [Location/equipment/line]
Impact: [Production loss/safety incident/quality defect]

Conduct the analysis using:
1. 5-Why Analysis (trace from symptom to root cause)
2. Fishbone Diagram categories: Man, Machine, Method, Material, Measurement, Environment
3. Rank causes by probability (High/Medium/Low) and impact
4. Corrective actions table: [Cause] [Action] [Owner] [Deadline] [Status]
5. Preventive measures to avoid recurrence

Think step by step through each possible cause.
```

### Quality Deviation Report

```
Act as a quality assurance manager for [product type].

A quality deviation has been detected:
- Product: [name/batch]
- Specification: [parameter] should be [range]
- Actual reading: [value]
- Detection point: [where in process]

Generate a quality deviation report including:
1. Incident description and timeline
2. Immediate containment actions taken
3. Root cause investigation findings
4. Corrective and preventive actions (CAPA)
5. Impact assessment (affected batches, customer notifications needed)
6. Sign-off section for QA Manager and Production Manager

Format: Formal report suitable for regulatory inspection files.
```

---

## Category 4: Maintenance Department

### Preventive Maintenance Plan

```
(R) You are a maintenance planning engineer with CMMS expertise in [industry].

(A) Build a complete preventive maintenance program for [equipment type/fleet].

(C) Current approach: [reactive/partially preventive]. Equipment operates [hours/conditions].
Fleet details: [count, age range, brand/model]. Environment: [temperature, dust, humidity, corrosion].
Last major failure: [description and date].

(E) Deliver:
1. Monthly inspection checklist (daily/weekly/monthly tasks)
2. Annual overhaul schedule with shutdown windows
3. Spare parts inventory list with minimum stock levels
4. KPI dashboard: MTBF, MTTR, PM Compliance %, Cost per unit
5. Estimated annual budget breakdown

Constraints: Budget not exceeding [amount]. Use available technicians only.
Comply with [manufacturer/ISO/OSHA] requirements. Target: [specific goal].
```

### Fault Diagnosis Assistant

```
You are an experienced [equipment type] technician with 20 years of field experience.

Equipment: [Name, Model, ID, Location]
Symptoms observed:
- [Symptom 1]
- [Symptom 2]
- [Symptom 3]

Operating conditions: [temperature, load, hours since last service]

Diagnose the fault:
1. List all possible causes ranked by probability (Most likely first)
2. For each cause: required inspection/test to confirm
3. Recommended repair procedure (step-by-step)
4. Safety precautions during repair
5. Estimated repair time and parts needed
6. Preventive actions to avoid recurrence

Format: Numbered steps, clear enough for a junior technician to follow.
```

### CMMS Fault Report

```
Create a fault report for CMMS entry:

Equipment: [Name] [ID] [Location]
Reported by: [Name] [Date] [Time]
Priority: [Emergency/Urgent/Normal/Low]

Structure:
1. Event Summary: What happened, when, where (2-3 sentences)
2. Observed Symptoms: Bullet list of what was seen/heard/measured
3. Diagnostic Steps Performed: What was checked and results
4. Root Cause Determination: The confirmed or suspected cause
5. Repair Performed: Actions taken, parts replaced, time spent
6. Post-Repair Testing: Verification results
7. Recommendations: Prevent recurrence, schedule follow-up
8. Estimated Cost: Parts [amount] + Labor [hours x rate]
```

---

## Category 5: Safety & HSE

### Safety Briefing Generator

```
Based on the following incident data for [month/period]:
[Paste or describe recent incidents]

Write a Safety Briefing for [audience - workers/supervisors/all employees]:
1. Attention-grabbing headline
2. One shocking statistic from the actual data
3. Top 3 risks to watch for this period
4. Short 'Do / Don't' checklist (5 items each)
5. Recognition: Name a team/individual with zero incidents
6. Motivational closing line

Style: Simple, direct, short sentences. Maximum one A4 page.
Language: [Arabic/English/Bilingual]
```

### Incident Investigation Report

```
You are an HSE investigator certified in [OSHA/NEBOSH/ISO 45001].

Investigate the following incident:
- Date/Time: [when]
- Location: [where]
- Involved personnel: [who - anonymized]
- Description: [what happened]
- Injury/Damage: [outcome]

Provide:
1. Incident timeline (minute-by-minute reconstruction)
2. Contributing factors analysis (Immediate, Underlying, Root)
3. Barrier analysis (what safety barriers failed?)
4. 5-Why analysis
5. Corrective actions: [Action] [Owner] [Deadline] [Priority]
6. Lessons learned (3 key takeaways)
7. Recommendations for systemic improvement

Comply with [applicable regulations/standards].
```

### Job Safety Analysis (JSA)

```
Create a Job Safety Analysis for the following task:

Task: [Description]
Location: [Where]
Equipment/Materials: [What's used]
Personnel: [How many, what roles]
Duration: [Estimated time]

For each step of the task, provide:
| Step # | Task Step | Potential Hazards | Risk Level (H/M/L) | Control Measures | Responsible Person |

Include:
- Required PPE for each step
- Emergency procedures
- Permit requirements (hot work, confined space, etc.)
- Environmental considerations

Format: Table suitable for printing and posting at the worksite.
```

---

## Category 6: Data Analysis

### Data Exploration Starter

```
Act as an expert data analyst. Examine the attached file carefully.

First, provide:
1. Quick summary: number of records, time period, columns and data types
2. Data quality assessment: missing values, duplicates, anomalies
3. Top 3 surprising or unexpected findings
4. One question you suggest I ask this data for maximum business value

Then create:
5. A summary statistics table for all numerical columns
6. Distribution analysis for key categorical columns
```

### Heatmap & Pattern Analysis

```
Act as an occupational safety expert and data analyst.

Analyze the attached [type] data and create:
1. Heatmap: X-axis = [dimension 1], Y-axis = [dimension 2], Color = [metric]
2. Second Heatmap: X-axis = [dimension 3], Y-axis = [dimension 4], Color = [metric]
3. Identify: WHEN and WHERE do most [events] happen?
4. Statistical significance: Are these patterns real or random?
5. Top 3 actionable recommendations based on the patterns
```

### Demand Forecasting

```
You are a Demand Planner. Using the attached [timeframe] of [data type]:

1. Trend Analysis: Is demand rising, falling, or stable? Is there seasonality?
2. Forecast: Predict next [period] using:
   - Moving Average (specify window)
   - Exponential Smoothing
   - Compare both methods
3. Visualization: Plot actual + forecast + confidence interval
4. Accuracy metrics: MAE, MAPE for each method
5. Recommendations: Optimal order quantity and timing
6. Risk factors that could invalidate this forecast
```

---

## Category 7: Communication & Email

### Professional Email Drafter

```
Draft a [type: follow-up/request/announcement/escalation] email.

From: [Your role]
To: [Recipient role/name]
Subject context: [What is this about]
Key message: [What you need to communicate]
Action required: [What you need them to do]
Deadline: [When]

Tone: [Formal/diplomatic/urgent/friendly]
Length: Maximum [X] words
Include: [Bullet points for action items / Arabic signature / attachments reference]
```

### Meeting Minutes Summary

```
Summarize the following meeting transcript/notes:
[Paste transcript or notes]

Provide:
1. Meeting details: Date, attendees, duration
2. Executive summary (3 sentences)
3. Key decisions made (numbered list with decision owner)
4. Action items table: [Item] [Owner] [Deadline] [Priority]
5. Open issues / parking lot items
6. Next meeting date and agenda preview

Format: Professional, suitable for email distribution to all attendees.
```

---

## Category 8: Research & Knowledge

### NotebookLM Query Templates

```
Based on the uploaded documents:

Troubleshooting: "The [equipment] is showing [symptom]. Based on the uploaded
manual, what are the possible causes, diagnostic steps, and corrective actions?
List in order of probability."

Quick Reference: "Create a 1-page quick reference card for [task/procedure]
based on the manufacturer manual. Include safety warnings."

Training Quiz: "Create [X] multiple-choice questions about [topic] for
[audience]. Include correct answers and source page references."

Cross-Document: "Compare [aspect] across all uploaded documents. Create a
master [schedule/checklist/comparison table]. Highlight any conflicts."
```

### Deep Research Prompt

```
Research [topic] comprehensively. I need:

1. Current state of the art (2025-2026)
2. Top [X] [solutions/vendors/methods] with comparison table
3. For each: [specific data points you need]
4. Real-world case studies from [industry]
5. Cost-benefit analysis where available
6. Regulatory considerations for [region]
7. Expert opinions and industry consensus
8. Limitations and risks

Present as a structured report with clear headings, data tables, and source citations.
Target audience: [who will read this].
```

---

## Quick Reference: Which Tool for Which Prompt

| Task Type | Best Tool | Best Framework |
|-----------|-----------|---------------|
| Complex reports & strategy | ChatGPT or Claude | CO-STAR |
| Plans & project proposals | ChatGPT or Claude | RACE |
| Quick translations & summaries | Any AI | RTF |
| Problem-solving & diagnostics | ChatGPT or Claude | PARA |
| Data analysis & charts | ChatGPT Code Interpreter | Analysis prompts |
| Document Q&A (no hallucination) | NotebookLM | NotebookLM templates |
| Academic research | Consensus + Elicit | Research prompts |
| Comprehensive web research | Deep Research | Deep Research prompt |
| Email & document drafting | Copilot in M365 | Communication prompts |
| Presentations | Copilot in PowerPoint | Direct instruction |

---

*This library grows with you. Add your best prompts as you discover them!*

**Arab Potash Company | AI Excellence Program | 2026**
