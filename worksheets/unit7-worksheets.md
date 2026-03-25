# Unit 7: The Smart Analyst — Worksheets

> **Printable Handout** | Participant Name: _______________________________ | Date: _______________

---

## Worksheet 7-A: Data Cleaning Checklist

**Objective:** Prepare your dataset for AI-assisted analysis by completing all pre-analysis steps.

**Instructions:** Before uploading any data to an AI tool, work through every item below. Check each box only after confirming the step is complete.

### Pre-Analysis Preparation Steps

| Step | Task | Done? | Notes |
|------|------|:-----:|-------|
| 1 | **Review the raw data** — Open the file and scan for obvious issues | [ ] | |
| 2 | **Check file format** — Confirm CSV, XLSX, or compatible format | [ ] | |
| 3 | **Verify column headers** — Ensure all columns have clear, descriptive names | [ ] | |
| 4 | **Remove empty rows/columns** — Delete any fully blank rows or columns | [ ] | |
| 5 | **Handle missing values** — Identify cells with blanks, N/A, or nulls; decide: delete, fill, or flag | [ ] | |
| 6 | **Standardize date formats** — Ensure all dates use one consistent format (e.g., YYYY-MM-DD) | [ ] | |
| 7 | **Standardize number formats** — Remove currency symbols, extra spaces, inconsistent decimals | [ ] | |
| 8 | **Check for duplicates** — Identify and remove or flag duplicate rows | [ ] | |
| 9 | **Validate categorical values** — Look for typos or inconsistent categories (e.g., "Riyadh" vs "riyadh" vs "RUH") | [ ] | |
| 10 | **Check units of measurement** — Confirm all values in a column use the same unit | [ ] | |
| 11 | **Remove personal/sensitive data** — Strip names, IDs, emails, phone numbers before uploading | [ ] | |
| 12 | **Create a backup** — Save a copy of the original file before making changes | [ ] | |

**Dataset name:** ________________________________ **Rows:** _________ **Columns:** _________

**Issues found and fixed:**

_________________________________________________________________________________

_________________________________________________________________________________

_________________________________________________________________________________

> **Key Takeaway:** Garbage in, garbage out. The quality of AI analysis is only as good as the data you feed it. Spending 10 minutes on data cleaning can save hours of misleading results.

---

## Worksheet 7-B: Exercise 28 — HSE Data Analysis

**Objective:** Use AI to analyze Health, Safety, and Environment (HSE) incident data, interpret heatmaps, and uncover hidden causes.

### Part 1: Heatmap Interpretation Questions

After generating a heatmap of incidents (by time, location, type, or severity), answer the following questions.

| # | Question | Your Answer |
|---|---|---|
| 1 | Which area/location has the highest concentration of incidents? | |
| 2 | What time of day or shift shows the most incidents? | |
| 3 | Is there a seasonal or monthly pattern? Describe it. | |
| 4 | Are high-severity incidents clustered in a specific zone? Where? | |
| 5 | Which combination of factors (e.g., night shift + Zone B) appears most dangerous? | |
| 6 | Does the heatmap reveal anything that tabular data alone would not? | |

### Part 2: Hidden Cause Documentation Table

Use the AI analysis to look beyond surface-level incident categories. Document underlying causes that are not immediately obvious.

| # | Incident Pattern Observed | Surface-Level Cause (Obvious) | Hidden/Root Cause (AI-Discovered) | Supporting Evidence | Recommended Action |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Reflection Questions:**

1. Did the AI identify any cause you had not previously considered?

   _________________________________________________________________________________

   _________________________________________________________________________________

2. How would you validate the AI's root cause suggestions before presenting them to management?

   _________________________________________________________________________________

   _________________________________________________________________________________

3. What additional data would strengthen this analysis?

   _________________________________________________________________________________

   _________________________________________________________________________________

> **Key Takeaway:** AI can detect patterns across thousands of records that human reviewers would miss. But correlation is not causation — always validate AI-suggested root causes with domain experts before acting.

---

## Worksheet 7-C: Exercise 29 — Inventory Intelligence

**Objective:** Use AI to analyze inventory data, identify dead stock, calculate frozen inventory costs, and compare forecasting approaches.

### Part 1: Dead Stock Findings Table

| # | Item / SKU | Description | Last Movement Date | Days Since Movement | Quantity on Hand | Estimated Value | Recommended Action |
|---|---|---|---|---|---|---|---|
| 1 | | | | | | | |
| 2 | | | | | | | |
| 3 | | | | | | | |
| 4 | | | | | | | |
| 5 | | | | | | | |
| 6 | | | | | | | |
| 7 | | | | | | | |
| 8 | | | | | | | |

**Total dead stock items identified: _________ | Total estimated dead stock value: _________**

### Part 2: Frozen Inventory Percentage

Calculate the percentage of total inventory value that is "frozen" (not moving).

| Metric | Value |
|---|---|
| Total inventory value | _________________ |
| Frozen inventory value (no movement > ___ days) | _________________ |
| **Frozen inventory %** | _________________ % |
| Industry benchmark (if known) | _________________ % |
| Gap vs benchmark | _________________ % |

**Is your frozen inventory % acceptable?** [ ] Yes [ ] No [ ] Need more context

**What is the carrying cost of frozen inventory per month?** _________________________________

### Part 3: Forecast Comparison

Compare AI-generated demand forecast against traditional methods (if available).

| Item / Category | Historical Average (units/month) | AI Forecast (units/month) | Actual (if known) | Most Accurate Method | Variance (%) |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

**Reflection Questions:**

1. What surprised you most about the dead stock analysis?

   _________________________________________________________________________________

2. What operational changes would you recommend based on the frozen inventory findings?

   _________________________________________________________________________________

   _________________________________________________________________________________

3. Would you trust the AI forecast enough to change purchasing decisions? Why or why not?

   _________________________________________________________________________________

   _________________________________________________________________________________

> **Key Takeaway:** Inventory intelligence is not just about knowing what you have — it is about knowing what is costing you money by sitting still. AI can surface these hidden costs in minutes.

---

## Worksheet 7-D: Exercise 30 — Full Analysis Pipeline

**Objective:** Execute a complete data analysis pipeline from raw data to presentation-ready insight, documenting each step.

### Step-by-Step Pipeline

Complete each step in order. Record your observations and paste or sketch screenshots where indicated.

#### Step 1: Define the Question

**What business question are you trying to answer?**

_________________________________________________________________________________

_________________________________________________________________________________

**Who is the audience for the results?** ________________________________________________

---

#### Step 2: Prepare the Data

**Dataset used:** ________________________________ **Cleaned?** [ ] Yes (used Worksheet 7-A)

**Observations after cleaning:**

_________________________________________________________________________________

---

#### Step 3: Upload and Initial Exploration

**Tool used:** ________________________________

**First prompt sent to AI:**

_________________________________________________________________________________

_________________________________________________________________________________

**AI's initial observations about the data:**

_________________________________________________________________________________

_________________________________________________________________________________

_________________________________________________________________________________

**Screenshot / key visual (paste or sketch):**

```
[Space for screenshot or sketch]




```

---

#### Step 4: Deep Analysis

**Follow-up prompts sent:**

1. _________________________________________________________________________________

2. _________________________________________________________________________________

3. _________________________________________________________________________________

**Key findings from AI analysis:**

- Finding 1: _______________________________________________________________________

- Finding 2: _______________________________________________________________________

- Finding 3: _______________________________________________________________________

**Screenshot / key visual (paste or sketch):**

```
[Space for screenshot or sketch]




```

---

#### Step 5: Verify and Challenge

**Did you verify the AI's calculations independently?** [ ] Yes [ ] No

**Any errors or questionable claims found?**

_________________________________________________________________________________

_________________________________________________________________________________

---

#### Step 6: Prepare the Deliverable

**Format chosen:** [ ] Report [ ] Presentation [ ] Dashboard [ ] Executive summary

**Top 3 insights for your audience:**

1. _________________________________________________________________________________

2. _________________________________________________________________________________

3. _________________________________________________________________________________

---

### "Most Surprising Finding" — Presentation Notes

Use this section to prepare a 2-minute verbal summary of your most surprising finding.

**The finding:** ____________________________________________________________________

_________________________________________________________________________________

**Why it is surprising:** _____________________________________________________________

_________________________________________________________________________________

**The evidence (data point or visual):** _________________________________________________

_________________________________________________________________________________

**What action should be taken:** _____________________________________________________

_________________________________________________________________________________

**Practice your delivery — aim for 2 minutes. Time yourself:** Actual time: _________ minutes

> **Key Takeaway:** A structured analysis pipeline ensures you move from raw data to actionable insight without skipping critical steps. The "Most Surprising Finding" exercise forces you to distill complexity into clarity.

---

## Worksheet 7-E: Data Privacy Checklist — Never Upload These Items

**Instructions:** Before uploading ANY data to an AI tool, review this list. If your dataset contains any of the items below, you MUST remove or anonymize them first.

### Prohibited Data — Do NOT Upload to External AI Tools

| Category | Examples | In My Data? (Y/N) | Action Taken |
|---|---|:---:|---|
| **Employee personal data** | Names, national IDs, phone numbers, home addresses, salaries | | |
| **Customer personal data** | Names, account numbers, contact info, purchase history with PII | | |
| **Medical / health records** | Patient data, injury details with names, medical test results | | |
| **Financial account data** | Bank account numbers, credit card numbers, financial statements with names | | |
| **Authentication credentials** | Passwords, API keys, access tokens, security certificates | | |
| **Proprietary trade secrets** | Formulas, patented processes, confidential R&D data | | |
| **Legal / contractual data** | Active legal cases, contract terms under NDA, settlement details | | |
| **Government classified data** | Any data with a government classification marking | | |
| **Location tracking data** | GPS logs tied to individuals, badge-in/out records with names | | |
| **Communications content** | Private emails, chat logs, recorded meeting transcripts with names | | |

### My Anonymization Steps

Before uploading, I will:

- [ ] Replace all names with generic identifiers (Employee A, Customer 001, etc.)
- [ ] Remove or mask national ID numbers, phone numbers, and email addresses
- [ ] Aggregate individual records into group summaries where possible
- [ ] Remove any column that is not directly needed for the analysis
- [ ] Confirm with my supervisor if uncertain about any data element

**Supervisor approval obtained?** [ ] Yes [ ] No [ ] Not required

> **Key Takeaway:** When in doubt, leave it out. Uploading personal or confidential data to external AI tools may violate privacy laws, company policy, and professional ethics. Anonymize first, analyze second.

---

## Worksheet 7-F: Verification Checklist — 5 Questions to Ask AI

**Instructions:** After receiving ANY analytical result from AI, ask yourself these 5 verification questions before trusting or sharing the output.

| # | Verification Question | Your Answer | Verified? (Y/N) |
|---|---|---|:---:|
| 1 | **Does the math check out?** Pick 2-3 numbers from the AI's output and recalculate them manually or in a spreadsheet. Do they match? | | |
| 2 | **Does this match my domain knowledge?** Based on your experience, does the result make sense? If the AI says incidents dropped 90% in one month, is that plausible? | | |
| 3 | **Did the AI use the right data?** Confirm the AI analyzed the correct columns, date ranges, and categories. Did it accidentally include or exclude data? | | |
| 4 | **Are the conclusions supported by the data?** Does the AI's recommendation logically follow from the numbers, or is it making an unsupported leap? | | |
| 5 | **What would change if the data were slightly different?** Consider: if 10% of the data were wrong or missing, would the conclusion still hold? Is the finding robust? | | |

### My Verification Results

**Analysis being verified:** _________________________________________________________

**Errors found:** _________________________________________________________________

_________________________________________________________________________________

**Confidence in AI output after verification:** [ ] High [ ] Medium [ ] Low

**Changes made before sharing:** ____________________________________________________

_________________________________________________________________________________

> **Key Takeaway:** Trust but verify. AI is a powerful analyst, but it cannot replace your judgment. These 5 questions take less than 5 minutes and can prevent costly mistakes from reaching decision-makers.

---

*End of Unit 7 Worksheets*
