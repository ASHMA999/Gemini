# Unit 4: Industrial Prompt Engineering

## Applied Prompt Engineering for Arab Potash Company

| Detail | Description |
|--------|-------------|
| **Duration** | 4 hours |
| **Delivery** | Department-specific workshops (HR, Production, Maintenance) |
| **Tools Required** | ChatGPT or Claude.ai (live prompting) |
| **Objective** | Apply prompt frameworks to real APC industrial scenarios across all departments |

---

## 4.1 The Golden Formula for Industrial Prompts

### The APC Prompt Formula

**Industrial Role + Specific Task + Operational Context + Required Format + Safety/Budget Constraints**

**Template:**
> 'You are a [engineer/technician/specialist] in [department]. [Task] for [equipment/process]. Context: [operational environment]. Deliver results in [format] while adhering to [constraints].'

---

## 4.2 Department Workshops

### HR Department: Recruitment & Talent

**Challenge Scenario:** Difficulty attracting chemical engineers. The last 3 job postings failed to attract suitable candidates.

**Sample Prompt (PARA + Multi-Role):**

> **(P)** We're struggling to recruit chemical engineers. Last 3 job ads attracted zero qualified applicants.
> **(A)** Analyze root causes of poor recruitment AND write a compelling job advertisement AND suggest alternative recruitment channels.
> **(R)** I need at least 5 qualified applicants within 30 days.
> **(A)** Budget is limited to online channels only. Consider what makes our Dead Sea location attractive.
>
> Analyze from 3 perspectives: as a recruitment specialist, as a chemical engineer evaluating employers, and as a university career counselor.

### Production Department: Efficiency & Quality

**Challenge Scenario:** Production Line #2 has been running at only 85% of target capacity for 3 months.

**Sample Prompt (CO-STAR + CoT):**

> **(C)** Arab Potash Company, Production Line #2, potash crystallization unit.
> **(O)** Analyze root causes of the 15% capacity gap and propose a recovery plan within 2 months.
> **(S)** Write as an industrial efficiency consultant with Six Sigma expertise.
> **(T)** Data-driven and objective.
> **(A)** Plant manager and production supervisors.
> **(R)** Deliver a table: [Root Cause] [Probability] [Impact] [Recommended Action] [Timeline].
>
> Think step by step: seasonal factors, equipment age, process parameters, human factors, supply chain issues.

### Maintenance Department: Preventive Programs

**Challenge Scenario:** Building a preventive maintenance program for 25 heavy trucks (currently reactive only).

**Sample Prompt (RACE + Constraints):**

> **(R)** You are a fleet maintenance engineer with CMMS expertise.
> **(A)** Build a complete preventive maintenance program for 25 heavy-duty trucks.
> **(C)** Current approach is 100% reactive. Trucks operate in extreme heat and dusty conditions. Fleet age: 2-8 years.
> **(E)** Deliver: monthly inspection checklist, annual overhaul schedule, spare parts inventory list, and KPI dashboard.
>
> Constraints: Budget not exceeding 200,000 JOD/year. Use available technicians only. Comply with manufacturer warranty requirements. Target: zero unplanned breakdowns within 6 months.

---

## 4.3 Prompt Command Lab: Weak-to-Strong Transformation

| Department | Weak Prompt | Your Mission: Rewrite It |
|-----------|-------------|--------------------------|
| HR | "Write a job advertisement" | Apply RACE framework with full context |
| Production | "Analyze production data" | Apply CO-STAR with specific KPIs |
| Maintenance | "Write a maintenance report" | Apply RTF with equipment IDs and standards |
| HR | "Evaluate the employee" | Add performance period, metrics, and audience |
| Production | "Give me ideas to improve quality" | Add constraints, timeline, and measurement criteria |
| Maintenance | "Explain how to fix the pump" | Add pump model, symptoms, and safety requirements |

### Hands-On Exercise 20: Team Challenge - Department Sprint (15 minutes)

3 teams (HR, Production, Maintenance). Each team gets the same problem from their department. Scoring: Quality of solution + Speed + Number of AI iterations needed.
- **HR:** Write an exit interview analysis for a resigning employee.
- **Production:** Generate an urgent quality report for a key client.
- **Maintenance:** Diagnose abnormal vibrations in a motor and recommend fixes.

### Hands-On Exercise 21: Fix the Broken Prompt (10 minutes)

The broken prompt: 'Write something about safety in the factory that's understandable for workers and useful for managers and short but covers everything important and in Arabic and English.'

Identify and fix: (1) Conflicting audience (workers vs. managers), (2) Conflicting length (short but comprehensive), (3) Vague topic, (4) No format specified. Split into 2 separate, well-crafted prompts.

---

## 4.4 Ready-Made Templates

### Job Description Template Prompt

> "Act as a recruitment specialist at an industrial company. Write a job description for [Position] including: Job Summary, 5-7 Key Responsibilities, Required Qualifications, Technical Skills, Benefits. Tone: Professional yet attractive to top talent. Context: [Company details, location, work conditions]."

### Daily Production Report Template Prompt

> "Generate a daily production report with: Executive Summary (3 lines), Actual vs. Target comparison table, Gap Analysis, Downtime causes and corrective actions, Recommendations for next shift. Format: Concise and scannable for quick review."

### Fault & Repair Report Template Prompt

> "Create a fault report for CMMS entry with: Event Summary (what, when, where), Observed Symptoms, Diagnostic Steps, Root Cause, Repair Performed, Recommendations to Prevent Recurrence, Estimated Repair Cost."

---

## 4.5 Common Mistakes Checklist

- **Forgetting safety context:** Always add 'while adhering to occupational safety standards'
- **Vague equipment references:** Specify name, ID number, and location (e.g., 'Pump P-301, Building A')
- **Ignoring operating conditions:** Specify temperature, load, environment, shift pattern
- **Missing standards:** Reference ISO, OSHA, or company-specific regulations
- **Forgetting the audience:** Workers vs. supervisors vs. managers vs. external regulators need different language
