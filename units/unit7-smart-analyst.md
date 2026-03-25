# Unit 7: The Smart Analyst

## Mining Insights from Big Data with AI

| Detail | Description |
|--------|-------------|
| **Duration** | 4 hours |
| **Delivery** | Live demos with real data files + hands-on analysis |
| **Tools Required** | ChatGPT (Code Interpreter / Advanced Data Analysis), Claude Artifacts, Google Sheets + Gemini |
| **Objective** | Extract hidden patterns from Excel/CSV files using AI, generate charts, dashboards, and strategic insights in minutes |

---

## 7.1 The Technical Unlock: How AI Analyzes Your Data

### The Secret That Changes Everything

AI models are NOT calculators. When you upload a file, the model writes Python code, executes it in a secure sandbox, and returns precise results with charts. It's a programmer working for you in real-time.

| Traditional Way | With AI | Time Savings |
|----------------|---------|--------------|
| Learn advanced Excel for weeks | Describe what you want in plain language | Weeks to minutes |
| Build complex Pivot Tables | Code is built automatically | Hours to seconds |
| Search for chart formulas | Say 'Draw me a...' and it's done | Trial-and-error eliminated |
| Manual pattern hunting | Automatic anomaly detection | Days to instant |

### Trust but Verify

You can ALWAYS ask: 'Show me the code you used.' This lets you verify accuracy and run the same code in your own environment.

---

## 7.2 Scenario 1: Safety & HSE Data Analysis

**Problem:** A 5-year accident log with columns: Date, Injury Type, Location, Shift, Root Cause, Incident Description.

### Application 1: Danger Heatmap

> Act as an occupational safety expert and data analyst. Analyze the attached accident file and create:
> 1. A Heatmap: X-axis = Days of the week, Y-axis = Shifts (Morning/Evening/Night), Color intensity = Number of incidents
> 2. A second Heatmap: X-axis = Months, Y-axis = Locations
> I need to know: WHEN and WHERE do most accidents happen?

### Application 2: Hidden Cause Discovery (Text Analysis)

> You are an expert accident investigator. Analyze the 'Incident Description' column using Text Analysis:
> 1. Extract the most frequently occurring words and common phrases
> 2. Identify the top 3 'hidden' root causes that repeat in descriptions but were NOT officially recorded in the 'Root Cause' column
> 3. For each hidden cause: count, examples from text, preventive recommendation

### Application 3: Auto-Generate Safety Briefing

> Based on last month's incidents, write a Safety Briefing:
> 1. Attention-grabbing headline
> 2. One shocking statistic from the actual data
> 3. Top 3 risks to watch for this month
> 4. Short 'Do / Don't' checklist
> 5. Motivational closing line
> Style: Simple, direct, short sentences. Fit on one A4 page.

### Hands-On Exercise 28: HSE Data Analysis (25 minutes)

Upload sample accident log. Execute all 3 prompts. Compare heatmaps. Identify hidden causes.

---

## 7.3 Scenario 2: Inventory & Supply Chain Analysis

### Dead Stock Discovery

> Act as a supply chain analyst. Discover 'Dead Stock':
> 1. Items with zero movement for 6+ months
> 2. Total value of frozen inventory
> 3. Rank by frozen value (descending)
> For each: suggest discount %, bundle, return to supplier, or dispose.

### Demand Forecasting

> You are a Demand Planner. Using 12 months of data:
> 1. Trend Analysis: rising, falling, seasonal?
> 2. Forecast next 3 months: Moving Average AND Exponential Smoothing
> 3. Plot actual + forecast + error margin
> 4. Optimal order quantity and timing

### KPI Dashboard Design

> Design a warehouse KPI Dashboard with 5 daily indicators. For each:
> 1. Name and definition
> 2. Calculation formula
> 3. Current value from data
> 4. Target benchmark
> 5. Status: GREEN / YELLOW / RED
> Add trend arrows vs. last month.

### Hands-On Exercise 29: Inventory Intelligence (25 minutes)

Upload sample inventory file. Run Dead Stock discovery. Calculate frozen inventory percentage. Run demand forecast. Compare methods.

---

## 7.4 Best Practices for AI Analytics

### Data Cleaning: Why It Matters

- Remove headers, logos, and merged cells
- Row 1 = Column names
- Standardize date formats
- Replace empty cells with 0 or N/A
- Delete duplicate rows
- Numbers formatted as numbers, not text

### Data Privacy: Never Upload These

- Real customer names with financial data
- National ID or passport numbers
- Employee medical records
- Trade secrets and patents
- Passwords or API keys
- Confidential supplier contracts

**Solutions:** Anonymization, Enterprise versions, dummy data with same structure.

### Verification: The Golden Rule

- "Explain step by step how you reached this conclusion"
- "Show me the code you used"
- "What assumptions did you make?"
- "Are there limitations I should know about?"
- "Recalculate using a different method to confirm"

**Red flags:** Results that seem 'too perfect,' numbers contradicting intuition, illogical charts, disappearing data.

---

## 7.5 Working with Arabic Data

| Aspect | Status | Notes |
|--------|--------|-------|
| Arabic column names | Fully supported | Works fine |
| Arabic text data | Fully supported | Product names, regions in Arabic |
| Arabic numerals (Eastern) | Convert recommended | Use 123 instead |
| Hijri dates | Needs clarification | Add Gregorian column |

**Arabic Data Prompt Tip:**
> 'The attached file contains data in Arabic. Column names are: [list them]. Analyze while preserving Arabic names in results and visualizations.'

---

## 7.6 The 10-Minute Live Demo Script

1. **Minutes 0-2:** Upload CSV. Show raw file.
2. **Minutes 2-4:** 'Examine this file. Quick summary, top 3 surprising findings, one suggested question.'
3. **Minutes 4-6:** 'Bar Chart comparing total sales by branch, sorted. Average line. Below-average in red.'
4. **Minutes 6-8:** 'Best and worst day of the week? Product-region correlation? One decision for tomorrow?'
5. **Minutes 8-10:** 'Convert to PowerPoint: 3 slides - Summary, Chart + Analysis, Recommendations.'

### Hands-On Exercise 30: Full Analysis Pipeline (30 minutes)

Replicate the demo with the provided dataset. Upload, explore, visualize, analyze, export to PowerPoint. Present your most surprising finding.
