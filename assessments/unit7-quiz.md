# Unit 7 Quiz: The Smart Analyst

**Time Limit:** 15 minutes
**Total Points:** 50
**Passing Score:** 35/50 (70%)

---

**Instructions:**
- Answer all 10 questions.
- Multiple choice: Select the single best answer.
- Short answer: Write 2-4 sentences unless otherwise specified.
- Practical: Follow the specific instructions provided. Show your reasoning.
- No AI tools may be used during this assessment.

---

## Section A: Multiple Choice (2 points each | 10 points total)

**1. How does ChatGPT/Claude typically perform data analysis when you upload a spreadsheet?**

- A) It reads the data visually like a human
- B) It executes Python code in a sandboxed environment to process, calculate, and visualize the data programmatically
- C) It sends the data to a team of human analysts
- D) It can only summarize the column headers

**2. Which of the following is a critical data cleaning step BEFORE uploading data to AI for analysis?**

- A) Adding color formatting to cells
- B) Removing blank rows, standardizing headers, fixing inconsistent date formats, and ensuring a single data type per column
- C) Converting the file to PDF
- D) Adding a company logo to the spreadsheet

**3. Which of the following should you NEVER upload to a public AI tool for analysis?**

- A) Publicly available commodity price data
- B) Employee personal data, salary information, medical records, or customer PII (Personally Identifiable Information)
- C) Historical weather data
- D) Publicly published industry benchmark statistics

**4. What special challenge does Arabic data present when using AI for analysis?**

- A) AI cannot read Arabic at all
- B) Right-to-left text, mixed Arabic/English columns, Arabic-Indic numerals, and Hijri date formats can cause parsing errors if not handled properly
- C) Arabic data files are always too large for AI
- D) Arabic data must be translated to English before any analysis

**5. Why is verification of AI-generated analysis essential?**

- A) AI analysis is always wrong
- B) AI can produce plausible-looking but incorrect calculations, misinterpret data structures, or make silent errors -- human verification catches these issues
- C) Verification is only necessary for financial data
- D) AI tools always display a warning when their analysis is incorrect

---

## Section B: Short Answer (5 points each | 15 points total)

**6. Trust but Verify**

Explain the "Trust but Verify" principle in the context of AI data analysis. What does it mean in practice? Provide two specific methods a user can employ to verify that an AI's analysis is correct.

**7. Red Flags in AI Analysis**

Describe three specific "red flags" that should make you suspicious of an AI-generated data analysis. For each red flag, explain what it might indicate about the quality of the analysis.

**8. Data Cleaning Steps**

List and briefly describe at least four data cleaning steps you should perform on a spreadsheet before uploading it to AI for analysis. Explain why each step matters for getting accurate results.

---

## Section C: Practical Application (12-13 points each | 25 points total)

**9. Analytical Prompt Writing (12 points)**

**Scenario:** You have a dataset called "Maintenance_Log_2025.xlsx" with the following columns:
- Work Order ID
- Equipment Tag (e.g., P-101A, C-205B)
- Failure Type (Mechanical, Electrical, Instrumentation, Other)
- Date Reported
- Date Completed
- Total Cost (SAR)
- Downtime Hours
- Technician Name

Write a complete prompt you would use with ChatGPT or Claude to analyze this dataset. Your prompt must: **(4 points each)**
- Ask at least two specific analytical questions (not just "analyze this data")
- Request specific output formats (e.g., tables, charts, summary statistics)
- Include at least one instruction for data validation or quality checking

**10. KPI Dashboard Design (13 points)**

**Scenario:** You are a production manager at a food processing plant. Management wants a monthly KPI dashboard that tracks operational performance. You plan to use AI to help create it from monthly production data.

Design the dashboard by answering the following:
- **Part A:** List at least five KPIs you would include on the dashboard, with a brief description of each. **(5 points)**
- **Part B:** Write the AI prompt you would use to generate the dashboard from a monthly data export. Include specific instructions for layout, visualizations, and calculations. **(5 points)**
- **Part C:** Describe two verification steps you would perform on the AI-generated dashboard before presenting it to management. **(3 points)**

---

**End of Quiz**
