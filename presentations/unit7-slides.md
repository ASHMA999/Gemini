---
marp: true
theme: default
paginate: true
header: "Unit 7: The Smart Analyst - Mining Insights from Data | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# Unit 7: The Smart Analyst
## Mining Insights from Data

**APC AI Excellence Program**

---

# Learning Objectives

By the end of this unit, you will be able to:

- **Explain** how AI chatbots analyze data using Python sandboxes
- **Generate** safety heatmaps from incident data
- **Perform** text analysis on maintenance logs to uncover hidden failure causes
- **Identify** inventory dead stock using AI-driven analysis
- **Build** demand forecasting models with AI assistance
- **Create** KPI dashboards using AI tools
- **Handle** Arabic-language data in AI analysis workflows
- **Apply** best practices for data verification and validation

---

# How AI Analyzes Your Data

### The Python Sandbox Model

When you upload data (CSV, Excel) to ChatGPT, Gemini, or Claude:

1. **Upload** - You provide the data file
2. **Code Generation** - AI writes Python code (pandas, matplotlib, scikit-learn)
3. **Execution** - Code runs in a sandboxed environment
4. **Results** - Charts, tables, and insights returned to you

> **You don't need to know Python.** The AI writes and executes code on your behalf. But you *do* need to understand your data and verify results.

### What You Can Analyze
- Spreadsheets (CSV, XLSX) up to millions of rows
- Time series data (sensor readings, production logs)
- Text data (maintenance notes, incident reports)
- Mixed data (numbers + text + dates)

---

# Safety Heatmaps from Incident Data

**Goal:** Visualize where, when, and why safety incidents occur at APC.

### Sample Prompt
> "I'm uploading our safety incident log for 2024-2025. Create a heatmap showing incident frequency by: (1) location/plant area on one axis, and (2) month on the other. Color-code by severity. Also create a separate heatmap by incident type vs. shift."

### What AI Delivers
- **Location x Time heatmap** - Spot seasonal/area patterns
- **Type x Shift heatmap** - Identify shift-specific risks
- **Statistical summary** - Top 5 locations, trend direction, anomalies
- **Recommendations** - Data-driven safety focus areas

### APC Application
- Identify **high-risk zones** for targeted safety campaigns
- Detect **seasonal patterns** (summer heat-related incidents)
- Compare **shift performance** for training needs assessment

---

# Text Analysis for Hidden Causes

**Problem:** Maintenance logs contain valuable insights buried in free-text descriptions that no one has time to read.

### AI Text Mining Techniques

| Technique | What It Finds | Example |
|-----------|--------------|---------|
| **Keyword extraction** | Most common terms/phrases | "bearing failure", "seal leak" |
| **Sentiment/urgency analysis** | Escalation patterns | Repeated "temporary fix" warnings |
| **Clustering** | Groups of similar issues | Related failures across equipment |
| **Pattern detection** | Recurring sequences | "Vibration high" always precedes "bearing failure" |
| **Root cause mapping** | Cause-effect relationships | 70% of pump failures follow filter bypass events |

### Sample Prompt
> "Analyze the attached maintenance work orders. Extract the top 20 recurring failure descriptions, group them by root cause category, and identify any sequential patterns (failure A often follows event B)."

---

# Inventory Dead Stock Analysis

**Problem:** Warehouses accumulate parts that haven't moved in years, tying up capital.

### AI-Driven Analysis Steps

1. **Upload** inventory data (part number, description, last movement date, quantity, unit cost)
2. **Classify** items by movement:
   - **Active:** Moved in last 6 months
   - **Slow-moving:** Moved 6-18 months ago
   - **Dead stock:** No movement in 18+ months
3. **Calculate** financial impact:
   - Total value tied up in dead stock
   - Carrying cost per year (typically 20-30% of value)
4. **Recommend** actions:
   - Dispose, transfer, return to vendor, reclassify

### Sample Prompt
> "Analyze this inventory export. Classify all items by movement status. Calculate total dead stock value. Identify the top 50 items by value with no movement in 2+ years. Suggest disposition for each based on the item description."

---

# Demand Forecasting with AI

**Goal:** Predict future consumption of spare parts and materials.

### What AI Can Do
- Analyze **historical consumption patterns** (seasonality, trends)
- Factor in **maintenance schedules** (planned shutdowns increase demand)
- Identify **correlated items** (if Part A is ordered, Part B usually follows)
- Generate **reorder point recommendations**

### Sample Prompt
> "Using the attached 3-year consumption history, forecast monthly demand for the next 12 months for each item. Flag items with seasonal patterns. Calculate recommended safety stock levels using a 95% service level target."

### Methods AI May Use
- **Moving averages** - Simple trend following
- **Exponential smoothing** - Weighted recent history
- **ARIMA/SARIMA** - Statistical time series models
- **Prophet** - Facebook's forecasting library (handles seasonality well)

---

# KPI Dashboards with AI

**From raw data to executive dashboards in minutes.**

### Process
1. Upload your KPI data (production, maintenance, safety, quality metrics)
2. Describe the dashboard you need
3. AI generates visualizations and summary statistics

### Sample Prompt
> "Create a monthly KPI dashboard from this data showing:
> - Production output vs. target (bar chart)
> - Equipment availability trend (line chart)
> - MTBF and MTTR by equipment class (table)
> - Safety incident rate (gauge chart)
> - Top 5 maintenance cost drivers (pie chart)
> Use a professional color scheme. Add red/yellow/green indicators for metrics vs. targets."

### Output Formats
- **Static charts** - PNG/SVG images for reports
- **Interactive HTML** - Plotly-based dashboards
- **PowerPoint ready** - Charts sized for presentation slides

---

# Handling Arabic Data

**Challenge:** APC data often contains Arabic text (maintenance descriptions, employee names, location labels).

### Common Issues & Solutions

| Issue | Solution |
|-------|----------|
| **Encoding errors** | Specify UTF-8 encoding when uploading: "This file uses UTF-8 encoding with Arabic text" |
| **RTL display problems** | Ask AI to handle right-to-left text rendering in charts |
| **Mixed Arabic/English** | Tell AI: "Column A is in Arabic, Column B is in English" |
| **Arabic date formats** | Specify format: "Dates are in DD/MM/YYYY format" |
| **Transliteration needs** | Ask AI to create bilingual labels on charts |

### Sample Prompt
> "This maintenance log has Arabic descriptions in column D. Analyze the Arabic text to extract the top failure modes. Create a bilingual chart (Arabic and English labels) showing failure frequency by type."

---

# Best Practices & Verification

### The VERIFY Framework for AI Data Analysis

- **V**alidate row counts - Does AI see all your data?
- **E**xamine outliers - Are extreme values real or errors?
- **R**echeck calculations - Spot-check totals and averages manually
- **I**nspect chart axes - Are scales appropriate and not misleading?
- **F**lag assumptions - What did AI assume about missing data?
- **Y**ield to domain knowledge - Does the result make operational sense?

> **Golden Rule:** If an AI insight surprises you, verify it before acting on it. If it confirms what you expected, still spot-check the numbers.

### Data Security Reminders
- **Never upload** classified or restricted data to public AI tools
- **Remove PII** (employee names, ID numbers) before uploading
- **Use approved tools** per APC IT security policy
- **Check data retention** policies of each AI platform

---

# Exercise 28: Safety Data Heatmap

**Task:** Create a safety heatmap from incident data.

1. Export safety incident data for the past 2 years (or use provided sample)
2. Upload to ChatGPT or Gemini with this prompt structure:
   - Request heatmap by location x month
   - Request heatmap by incident type x shift
   - Ask for top 5 findings and recommendations
3. **Verify** results against your known safety experience
4. **Document** any insights the AI found that you did not expect

**Deliverable:** Heatmap visualizations, AI findings, your verification notes, and actionable recommendations.

---

# Exercise 29: Maintenance Text Mining

**Task:** Uncover hidden patterns in maintenance work order descriptions.

1. Export 6-12 months of work order descriptions from CMMS
2. Upload to AI with instructions to:
   - Extract top 20 recurring issues
   - Group by root cause category
   - Identify sequential failure patterns
   - Flag "repeat offender" equipment
3. **Cross-reference** AI findings with your reliability team's known issues

**Deliverable:** Root cause analysis report comparing AI findings to known issues, highlighting any new discoveries.

---

# Exercise 30: Inventory Optimization Analysis

**Task:** Identify dead stock and forecast spare parts demand.

1. Export inventory data with movement history
2. Perform **dead stock analysis:**
   - Classify all items by movement status
   - Calculate financial impact
   - Recommend disposition for top 50 items
3. Perform **demand forecast** for top 20 high-value items:
   - 12-month forecast with confidence intervals
   - Recommended reorder points and safety stock

**Deliverable:** Dead stock report with financial impact and demand forecast with reorder recommendations.

---

# Unit 7 Recap

| Topic | Key Takeaway |
|-------|-------------|
| Python Sandbox | AI writes and runs code on your data - you guide and verify |
| Safety Heatmaps | Visualize incident patterns to drive targeted interventions |
| Text Analysis | Mine free-text maintenance logs for hidden failure patterns |
| Dead Stock | Identify tied-up capital and recommend dispositions |
| Demand Forecasting | Predict spare parts needs using historical consumption |
| KPI Dashboards | From raw data to executive visuals in minutes |
| Arabic Data | Specify encoding, handle RTL, use bilingual labels |
| Verification | Always VERIFY - never trust AI output without checking |

> **Next Unit:** Capstone Project - put everything together in a real-world regulatory inspection preparation scenario.
