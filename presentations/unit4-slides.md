---
marp: true
theme: default
paginate: true
header: "Unit 4: Industrial Prompt Engineering for APC | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# Unit 4: Industrial Prompt Engineering for APC

### From Generic Prompts to APC-Specific Excellence

**APC AI Excellence Program**

---

# Learning Objectives

By the end of this unit, you will be able to:

1. Apply the **Golden Formula** for crafting APC-specific prompts
2. Participate in department-level workshops for **HR, Production, and Maintenance**
3. Transform **weak prompts into strong prompts** using systematic techniques
4. Use **ready-made templates** for common APC tasks
5. Identify and avoid **common prompt engineering mistakes**

---

# The Golden Formula

> **Role + Context + Task + Format + Constraints = Excellent Output**

```
[ROLE]        You are a senior [department] specialist at APC.
[CONTEXT]     APC operates potash and bromine extraction facilities
              at the Dead Sea, Jordan, with [relevant details].
[TASK]        [Specific action verb] + [precise deliverable].
[FORMAT]      Present the output as [table / checklist / report / etc.].
[CONSTRAINTS] [Length / language / compliance / scope limits].
```

**Why "Golden"?**
- Combines the best elements of CO-STAR, RACE, and RTF
- Optimized for **industrial and corporate** APC contexts
- Every component directly reduces ambiguity and improves output quality

---

# Golden Formula: Applied Example

> **Before (Weak):** "Write something about safety at APC."

> **After (Golden Formula):**

| Component | Content |
|-----------|---------|
| **Role** | You are APC's Chief HSE Officer with 20 years of Dead Sea mining experience |
| **Context** | APC has 3 active production sites, 2,800 employees, and processes concentrated brine in high-temperature environments. The company follows ISO 45001 and Jordanian MOENV regulations |
| **Task** | Create a quarterly HSE performance report covering lost-time incidents, near-miss trends, and top 3 corrective actions implemented |
| **Format** | Executive summary (150 words), KPI dashboard table, incident trend chart description, and recommendations as numbered list |
| **Constraints** | Use formal English, no abbreviations without first defining them, align with GRI sustainability reporting standards, maximum 2 pages |

---

# HR Department Workshop

> **Transforming HR operations with targeted prompts**

**Common HR use cases at APC:**

| HR Task | Golden Formula Prompt Approach |
|---------|-------------------------------|
| Job descriptions | Role: HR specialist. Task: Write a JD for [position] aligned with APC grade structure |
| Interview questions | Role: Hiring manager. Task: Generate behavioral questions testing [competencies] |
| Policy drafting | Role: HR policy analyst. Context: Jordanian labor law + APC employee handbook. Task: Draft policy on [topic] |
| Training needs analysis | Role: L&D specialist. Task: Identify skill gaps for [department] based on [performance data description] |
| Onboarding plans | Role: HR coordinator. Task: Create a 90-day onboarding schedule for [role] including mentorship milestones |

> **Key HR constraint:** Always include "Comply with Jordanian Labour Law and APC internal policies" in HR prompts.

---

# Production Department Workshop

> **AI-assisted production planning, reporting, and troubleshooting**

**Production prompt patterns:**

1. **Shift Handover Reports**
   - Role: Shift supervisor. Task: Generate a handover report template covering production volumes, equipment status, safety incidents, and pending tasks.

2. **Production Variance Analysis**
   - Role: Production analyst. Context: Target output is X tons/day. Task: Analyze the following production data and identify top 3 variance drivers.

3. **Process Optimization**
   - Role: Process engineer. Context: Crystallizer operating parameters [details]. Task: Recommend adjustments to improve crystal size distribution.

4. **Quality Control**
   - Role: QC chemist. Task: Create an inspection checklist for final product sampling per APC quality standards.

> **Key production constraint:** Always specify units (metric tons, mg/L, degrees Celsius) and reference relevant APC SOPs.

---

# Maintenance Department Workshop

> **Predictive, preventive, and corrective maintenance enhanced by AI**

**Maintenance prompt patterns:**

| Maintenance Type | Prompt Structure |
|-----------------|-----------------|
| **Preventive** | Role: Maintenance planner. Task: Generate a PM schedule for [equipment] based on OEM recommendations and APC operating hours |
| **Corrective** | Role: Reliability engineer. Context: [Equipment] failed with [symptoms]. Task: Provide a root-cause analysis framework and probable causes ranked by likelihood |
| **Predictive** | Role: Condition monitoring analyst. Context: Vibration data shows [readings]. Task: Interpret the data and recommend action |
| **Spare parts** | Role: Inventory analyst. Task: Determine reorder points for [critical spares] based on lead time and consumption rate |

**Constraint stack for maintenance prompts:**
- Reference equipment tag numbers and P&ID references
- Specify safety isolation requirements (LOTO)
- Align with APC's CMMS (Computerized Maintenance Management System)

---

# Weak-to-Strong Transformations

> **See the difference systematic prompting makes**

### Example 1: HR

| | Prompt |
|---|--------|
| **Weak** | "Write a warning letter" |
| **Strong** | "Role: HR manager at APC. Task: Draft a first written warning letter for repeated tardiness (5 instances in 30 days). Format: Formal letter with date, employee details, violation description, previous verbal warning reference, improvement expectations, consequences of recurrence, and signature block. Constraint: Comply with APC disciplinary policy Section 7.3 and Jordanian Labour Law Article 28." |

### Example 2: Production

| | Prompt |
|---|--------|
| **Weak** | "Help me with the production report" |
| **Strong** | "Role: Production shift supervisor at APC Plant 2. Context: Today's KCl production was 1,850 MT against a target of 2,100 MT. Downtime: 3.5 hrs on Crystallizer C-201 due to bearing failure. Task: Write a shift production report. Format: Summary paragraph, production table (target vs actual), downtime log, and next-shift recommendations. Constraint: Use APC report template structure, metric units only." |

---

# Weak-to-Strong Transformations (Continued)

### Example 3: Maintenance

| | Prompt |
|---|--------|
| **Weak** | "What's wrong with the pump?" |
| **Strong** | "Role: Rotating equipment specialist at APC. Context: Centrifugal pump P-301A (KSB Omega 150-340) serving brine transfer shows: discharge pressure dropped from 8.5 to 6.2 bar, motor current increased by 12%, audible cavitation noise at suction. Installed: 2022, last overhaul: 18 months ago, operating hours: 11,400. Task: Provide a differential diagnosis with the 5 most probable causes ranked by likelihood. For each cause, specify the diagnostic test to confirm and the corrective action. Format: Numbered list with sub-bullets. Constraint: Reference APC maintenance standards and KSB technical manual recommendations." |

> **Pattern:** Every weak prompt fails because it lacks **role, context, specificity, format, or constraints**.

---

# Ready-Made Templates

> **Copy, customize, and use -- APC prompt templates for everyday tasks**

### Template 1: Meeting Minutes Generator
```
Role: Executive assistant at APC.
Context: Meeting held on [date] regarding [topic] with
         attendees: [names and roles].
Task: Generate structured meeting minutes.
Format: Header (date, attendees, location), agenda items
        with discussion summary, decisions made (table),
        action items (table: item, owner, deadline), next
        meeting date.
Constraint: Formal tone, max 2 pages, English.
```

### Template 2: Email Response Drafter
```
Role: [Your department] professional at APC.
Context: Received email about [topic]. Key points: [summary].
Task: Draft a professional response that [accepts/declines/
      requests clarification on] the proposal.
Format: Standard business email with greeting, body (3
        paragraphs max), and sign-off.
Constraint: Diplomatic tone, reference APC policy if
            applicable, under 200 words.
```

---

# Ready-Made Templates (Continued)

### Template 3: Incident Report
```
Role: HSE officer at APC [location].
Context: Incident occurred on [date] at [location].
         Type: [near miss / first aid / medical treatment /
         lost time]. Description: [brief facts].
Task: Write a formal incident report.
Format: Incident details table, sequence of events
        (timeline), root cause analysis (5-Why), corrective
        actions table (action, responsible, deadline, status),
        lessons learned.
Constraint: Align with APC HSE reporting standards and
            ISO 45001 Clause 10.2. Factual tone, no
            speculation, no blame language.
```

### Template 4: Training Material Outline
```
Role: L&D specialist at APC.
Context: Target audience is [role/department] with
         [experience level]. Topic: [subject].
Task: Create a training session outline for a [duration]
      workshop.
Format: Learning objectives, agenda with time blocks,
        key content bullets per section, 2 hands-on
        activities, assessment method.
Constraint: Practical and APC-specific, not generic.
            Include safety briefing if operational topic.
```

---

# Common Prompt Engineering Mistakes

> **Avoid these pitfalls to get reliable AI outputs**

| Mistake | Problem | Fix |
|---------|---------|-----|
| **Too vague** | "Help me with a report" | Specify report type, audience, format, and data scope |
| **No role** | AI defaults to generic assistant | Always assign a relevant professional role |
| **No format** | Output comes as unstructured wall of text | Explicitly request tables, lists, sections, or templates |
| **Overloading** | One prompt asks for 10 different things | Break into focused, sequential prompts |
| **No constraints** | Output is too long, wrong tone, or off-scope | Add length, tone, scope, and compliance constraints |
| **Ignoring iteration** | Accepting first output as final | Always review, refine the prompt, and regenerate |
| **Copy-paste syndrome** | Using the same prompt for different contexts | Customize role and context for each situation |
| **Assuming AI knows APC** | AI invents plausible but wrong APC details | Always provide APC-specific context in the prompt |

---

# Exercise 20: Weak-to-Strong Transformation Challenge

> **Task:** Transform these weak prompts using the Golden Formula.

**Weak Prompt 1 (HR):**
"Write an email to employees about the new vacation policy."

**Weak Prompt 2 (Production):**
"Summarize last month's production."

**Weak Prompt 3 (Maintenance):**
"Create a maintenance plan for the conveyor."

**For each prompt:**
1. Identify what is missing (role, context, task clarity, format, constraints)
2. Rewrite using the full Golden Formula
3. Submit both versions to an AI and compare outputs side by side
4. Document the quality difference in a brief paragraph

> **Deliverable:** A comparison document showing all 3 weak/strong pairs with AI outputs and your quality assessment.

---

# Exercise 21: Department Prompt Portfolio

> **Task:** Build a personal prompt library for your department.

**Requirements:**
1. Create **5 Golden Formula prompts** for tasks you perform regularly
2. Each prompt must include all 5 components (Role, Context, Task, Format, Constraints)
3. At least one prompt must involve **data analysis** (Excel/reporting)
4. At least one prompt must involve **communication** (email/memo/presentation)
5. Test each prompt with an AI tool and **refine until output quality is 8/10 or higher**

**Submission format:**

| # | Task Description | Golden Formula Prompt | Output Quality (1-10) | Refinement Notes |
|---|-----------------|----------------------|----------------------|-----------------|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |

> **This portfolio becomes your personal AI productivity toolkit at APC.**

---

# Unit 4 Recap

| Topic | Key Takeaway |
|-------|-------------|
| **Golden Formula** | Role + Context + Task + Format + Constraints = reliable output |
| **HR Workshop** | Tailor prompts to Jordanian labor law and APC HR policies |
| **Production Workshop** | Always specify units, SOP references, and operating parameters |
| **Maintenance Workshop** | Include equipment tags, failure data, and safety isolation context |
| **Weak-to-Strong** | Every weak prompt fails due to missing formula components |
| **Ready-Made Templates** | Customize proven templates rather than starting from scratch |
| **Common Mistakes** | Vagueness, overloading, and ignoring iteration are the top failures |

> **Key message:** The difference between amateur and professional AI use is **prompt structure**. Master the Golden Formula and you will consistently produce high-quality outputs tailored to APC's needs.
