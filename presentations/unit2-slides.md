---
marp: true
theme: default
paginate: true
header: "Unit 2: Applied Prompt Engineering | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# Unit 2: Applied Prompt Engineering

### From Basic Prompts to Professional Frameworks

**APC AI Excellence Program**

---

# Learning Objectives

By the end of this unit, you will be able to:

1. Apply the **CO-STAR** framework to structure any professional prompt
2. Compare and select from **RACE, RTF, and PARA** frameworks
3. Use **Few-Shot Learning** to guide AI output through examples
4. Employ **Chain-of-Thought** reasoning for complex, multi-step problems
5. Design **Multi-Role** prompts that simulate expert panels
6. Apply **Constraint Engineering** to control output precisely
7. Adapt prompt formatting between **GPT and Claude**

---

# The CO-STAR Framework

> **The gold standard for structured prompting**

| Component     | Description                          | Example (APC Context)                          |
|---------------|--------------------------------------|-------------------------------------------------|
| **C** Context    | Background information               | "APC produces potash via solar evaporation..."  |
| **O** Objective  | What you want the AI to do           | "Write a safety briefing for new hires"         |
| **S** Style      | Writing style or persona             | "Professional, formal, HSE-compliant"           |
| **T** Tone       | Emotional quality of the response    | "Authoritative yet approachable"                |
| **A** Audience   | Who will read the output             | "New plant operators with basic English"         |
| **R** Response   | Desired output format                | "Numbered checklist, max 1 page"                |

---

# CO-STAR in Action

**Prompt Example:**

> **Context:** APC's Dead Sea operations require daily safety inspections across evaporation ponds.
> **Objective:** Create a daily safety inspection checklist.
> **Style:** ISO 45001-aligned, concise and action-oriented.
> **Tone:** Firm and safety-critical.
> **Audience:** Field supervisors with 2+ years of experience.
> **Response:** A table with checkpoint, method, pass/fail criteria, and escalation action.

**Why it works:** Each component removes ambiguity. The AI knows *what* to write, *how* to write it, *for whom*, and in *what format*.

---

# Alternative Frameworks: RACE, RTF & PARA

| Framework | Components | Best Used When |
|-----------|-----------|----------------|
| **RACE** | **R**ole, **A**ction, **C**ontext, **E**xpectation | You need the AI to adopt a specific persona |
| **RTF** | **R**ole, **T**ask, **F**ormat | Quick, simple tasks with clear format needs |
| **PARA** | **P**roblem, **A**ction, **R**esult, **A**djustment | Iterative refinement workflows |

### When to choose which?

- **CO-STAR** -- Comprehensive, high-stakes documents
- **RACE** -- Role-heavy tasks (e.g., "Act as an HSE auditor...")
- **RTF** -- Fast, everyday prompts (emails, summaries)
- **PARA** -- When you plan to iterate and improve output

---

# Few-Shot Learning

> Teach the AI by **showing, not just telling**

**Zero-Shot** (no examples):
```
Classify this maintenance request as Urgent, Routine, or Deferred.
```

**Few-Shot** (with examples):
```
Classify maintenance requests:

Request: "Conveyor belt tearing, production stopped" -> Urgent
Request: "Office AC filter replacement due next month" -> Deferred
Request: "Pump vibration slightly above normal" -> Routine

Request: "Crystallizer agitator bearing overheating" -> ?
```

**Key principle:** 2-5 examples are usually enough. Use examples that cover edge cases and represent the variety of expected inputs.

---

# Chain-of-Thought (CoT) Prompting

> Force the AI to **show its reasoning** step by step

**Without CoT:**
```
What is the optimal harvest time for Pond 7?
```

**With CoT:**
```
Determine the optimal harvest time for Pond 7.
Think step by step:
1. Consider current brine density readings
2. Factor in weather forecast for evaporation rates
3. Check equipment availability on the schedule
4. Account for transport logistics to the plant
5. Recommend a harvest window with justification
```

**When to use CoT:**
- Math or calculation tasks
- Multi-factor decisions
- Troubleshooting and root-cause analysis
- Any task where reasoning quality matters more than speed

---

# Multi-Role Prompting

> Simulate a **panel of experts** in a single prompt

```
I need you to analyze APC's Q3 production shortfall
from three perspectives:

ROLE 1 - Production Engineer:
Analyze equipment utilization and downtime factors.

ROLE 2 - Financial Analyst:
Quantify the revenue impact and cost per ton changes.

ROLE 3 - HR Manager:
Assess workforce availability and overtime patterns.

After all three analyses, provide a unified summary
with the top 3 root causes and recommended actions.
```

**Benefits:**
- Surfaces blind spots a single-role prompt would miss
- Produces more balanced, cross-functional analysis
- Excellent for decision memos and executive briefings

---

# Constraint Engineering

> **Boundaries produce better outputs**

| Constraint Type | Example |
|----------------|---------|
| **Length** | "Respond in exactly 5 bullet points" |
| **Format** | "Use a markdown table with 4 columns" |
| **Vocabulary** | "Use only terms a non-engineer would understand" |
| **Scope** | "Only discuss potash operations, not bromine" |
| **Exclusion** | "Do not include financial figures or projections" |
| **Compliance** | "Align with ISO 14001 terminology" |
| **Language** | "Write in formal Modern Standard Arabic" |

> **Pro tip:** Stack multiple constraints. The more precise your boundaries, the less you need to edit the output.

---

# GPT vs Claude: Formatting Differences

| Aspect | GPT (OpenAI) | Claude (Anthropic) |
|--------|-------------|-------------------|
| **System prompt** | `system` role message | `system` parameter or `\n\nHuman:` prefix |
| **XML tags** | Supported but not preferred | Highly effective: `<context>`, `<instructions>` |
| **Markdown** | Native and strong | Native and strong |
| **Long context** | Up to 128K tokens | Up to 200K tokens |
| **Best for roles** | "You are a..." in system prompt | Role in system + XML-tagged sections |
| **Chain-of-Thought** | "Let's think step by step" | `<thinking>` tags or explicit step requests |
| **Output control** | JSON mode, function calling | Prefill technique, XML output tags |

> **Key takeaway:** Claude responds exceptionally well to XML-structured prompts. GPT excels with function calling and JSON mode.

---

# Exercise 7: CO-STAR Framework Practice

> **Task:** Write a complete CO-STAR prompt for the following scenario:

**Scenario:** APC needs a monthly potash production report summary for the board of directors. The report should highlight KPIs, compare targets vs. actuals, and flag any deviations above 5%.

- Define each CO-STAR component explicitly
- Submit the prompt to an AI and evaluate the output
- Refine at least one component and resubmit

---

# Exercise 8: Few-Shot Classification

> **Task:** Build a Few-Shot prompt to classify APC internal emails.

**Categories:** Action Required, For Information, Escalation Needed

1. Write 3 example email snippets with correct classifications
2. Include one ambiguous example to test the boundary
3. Submit 5 unclassified test emails and evaluate accuracy
4. Adjust your examples if accuracy is below 80%

> **Bonus:** Add a confidence score (High/Medium/Low) to each classification.

---

# Exercise 9: Chain-of-Thought Problem Solving

> **Task:** Use CoT prompting to troubleshoot the following:

**Problem:** Potash crystal size from Crystallizer Unit 3 has decreased by 15% over the past two weeks, affecting product grade.

- Prompt the AI to reason through possible causes step by step
- Require it to consider: feed brine quality, temperature control, agitator speed, residence time, and seeding rate
- Ask for a ranked list of most likely root causes with recommended diagnostic tests

---

# Exercise 10: Multi-Role Analysis

> **Task:** Use Multi-Role prompting for a workforce planning decision.

**Scenario:** APC is considering shifting from 8-hour to 12-hour shifts at the main processing plant.

Create a prompt with these roles:
1. **Operations Manager** -- productivity and coverage analysis
2. **HSE Officer** -- fatigue risk and safety implications
3. **Employee Representative** -- morale and work-life balance
4. **Finance Controller** -- cost impact (overtime, benefits, transport)

Require a final unified recommendation with pros, cons, and a suggested pilot plan.

---

# Unit 2 Recap

| Topic | Key Takeaway |
|-------|-------------|
| **CO-STAR** | Six components that eliminate prompt ambiguity |
| **RACE / RTF / PARA** | Choose frameworks based on task complexity |
| **Few-Shot Learning** | Examples teach better than instructions alone |
| **Chain-of-Thought** | Step-by-step reasoning improves complex outputs |
| **Multi-Role** | Multiple perspectives produce balanced analysis |
| **Constraint Engineering** | Precise boundaries yield precise results |
| **GPT vs Claude** | Adapt format to the model -- XML for Claude, JSON/functions for GPT |

> **Next up:** Unit 3 -- Microsoft Copilot 365 in the APC Workplace
