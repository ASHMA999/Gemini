# Unit 7 Applications: Data Analysis with AI

> **Hands-On Practical Exercises**
> Complete these exercises using AI-powered data analysis tools to transform raw data into actionable insights, visualizations, and dashboards for real-world decision-making.

---

## Guided Exercises

### Exercise 1: Safety Heatmap Analysis

**Objective:** Upload accident log data to ChatGPT and generate heatmap visualizations to identify patterns in workplace incidents.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis)

**Step-by-Step Instructions:**

1. **Prepare Your Data**
   - Use a CSV file with workplace accident/incident records containing at minimum:
     - Date, Day of Week, Shift (Morning/Afternoon/Night), Location, Incident Type, Severity
   - If you do not have real data, create a sample dataset with at least 50 rows.
   - Save as `accident_log.csv`.

2. **Upload and Explore**
   - Open ChatGPT and attach the CSV file.
   - Use this prompt to start:
   ```
   I've uploaded an accident log CSV. Please:
   1. Show me the first 10 rows and summarize the columns
   2. Report total number of incidents
   3. Identify any data quality issues (missing values, inconsistent formats)
   ```

3. **Generate Heatmap 1: Day of Week vs. Shift**
   - Use this prompt:
   ```
   Create a heatmap showing the number of incidents by Day of Week (rows)
   and Shift (columns). Use a red color gradient where darker = more incidents.
   Add the count numbers inside each cell. Title it "Incident Frequency:
   Day of Week vs. Shift"
   ```
   - Save the generated image.

4. **Generate Heatmap 2: Month vs. Location**
   - Use this prompt:
   ```
   Create a heatmap showing incident count by Month (rows) and Location
   (columns). Use the same red gradient. Add count numbers in cells.
   Title it "Incident Frequency: Month vs. Location"
   ```
   - Save the generated image.

5. **Interpret Findings**
   Complete this analysis:

   | Finding | Detail |
   |---------|--------|
   | Highest-risk day + shift combination | |
   | Highest-risk month + location combination | |
   | Are there seasonal patterns? | |
   | Does any shift have consistently more incidents? | |
   | Recommended action based on the data | |

6. **Generate a Summary**
   - Use this prompt:
   ```
   Based on the heatmap analysis, write a 3-paragraph safety briefing
   for management. Include: key findings, risk patterns, and 3 specific
   recommendations with justification from the data.
   ```

### Troubleshooting
- **ChatGPT says it can't read the file**: Ensure the file is CSV (not Excel). If using Excel, save as CSV UTF-8 first.
- **Heatmap looks wrong or has missing cells**: Ask ChatGPT to show you the pivot table it used. Verify the data is being grouped correctly.
- **Color scale is misleading**: Specify the exact color range in your prompt (e.g., "use white for 0 incidents and dark red for the maximum").
- **Date parsing errors**: Ensure dates are in a consistent format (YYYY-MM-DD recommended). Ask ChatGPT to parse and reformat if needed.

---

### Exercise 2: Hidden Cause Discovery

**Objective:** Perform text analysis on incident descriptions to uncover patterns that are not captured in structured fields.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis)

**Step-by-Step Instructions:**

1. **Prepare the Data**
   - You need a column of free-text incident descriptions (e.g., "Worker slipped on oil near Machine 3 during shift change").
   - At least 30 descriptions are recommended for meaningful patterns.

2. **Extract Hidden Factors**
   - Use this prompt:
   ```
   Analyze the incident description text column. Extract and count mentions of:
   1. Environmental factors (weather, lighting, temperature, noise)
   2. Equipment mentioned (specific machines, tools, vehicles)
   3. Time-related factors (rush, overtime, end of shift, break time)
   4. Human factors (fatigue, training, communication, supervision)
   5. Substance/material factors (oil, chemical, water, debris)

   Present results as a ranked table for each category showing factor and
   frequency count.
   ```

3. **Compare Text vs. Official Records**
   - Use this prompt:
   ```
   Compare the factors found in the text descriptions to the official
   categorical fields in the dataset. What factors appear in the text
   descriptions that are NOT captured in any structured column?
   Create a table showing "Hidden Factor", "Frequency in Text",
   and "Captured in Official Records? (Yes/No)"
   ```

4. **Visualize the Hidden Factors**
   - Use this prompt:
   ```
   Create a horizontal bar chart of the top 15 factors mentioned in
   incident descriptions, color-coded by whether they are captured
   in official records (green) or hidden (red). Title: "Hidden vs.
   Recorded Incident Factors"
   ```

5. **Document Methodology**
   Record your approach:

   | Step | Method | Tool | Output |
   |------|--------|------|--------|
   | Data preparation | | | |
   | Text extraction | | | |
   | Pattern identification | | | |
   | Visualization | | | |
   | Validation | | | |

### Troubleshooting
- **AI misinterprets descriptions**: Provide 2-3 example descriptions with your expected categorization so the AI understands your domain terminology.
- **Too few patterns found**: Combine similar terms (e.g., "oil", "lubricant", "grease" are all substance-related). Ask the AI to group synonyms.
- **Results seem unreliable**: Cross-check the top 5 findings manually by searching the descriptions yourself. Report the AI's accuracy rate.

---

### Exercise 3: Dead Stock Discovery

**Objective:** Upload inventory data to identify frozen/dead stock items and calculate the financial impact.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis)

**Step-by-Step Instructions:**

1. **Prepare Inventory Data**
   - Your CSV should include: Item Code, Description, Category, Quantity on Hand, Unit Cost, Last Movement Date, Reorder Point.
   - If using sample data, include at least 100 items with varying last movement dates.

2. **Upload and Define Dead Stock**
   - Use this prompt:
   ```
   I've uploaded inventory data. Please:
   1. Calculate "Days Since Last Movement" for each item based on today's date
   2. Classify items as:
      - Active: moved within 90 days
      - Slow: moved 91-180 days ago
      - Dead Stock: moved 181-365 days ago
      - Frozen: no movement for over 365 days
   3. Show a summary table with count and total value for each category
   ```

3. **Deep Dive on Frozen Items**
   - Use this prompt:
   ```
   For all Frozen items (no movement > 365 days):
   1. List them sorted by total value (Quantity x Unit Cost), highest first
   2. Show the top 20 items in a table with: Item Code, Description,
      Category, Quantity, Unit Cost, Total Value, Days Since Movement
   3. Calculate the grand total value of all frozen inventory
   ```

4. **Generate Recommendations**
   - Use this prompt:
   ```
   Based on the dead stock analysis, generate recommendations:
   1. Top 10 items to prioritize for disposal or write-off (highest value frozen items)
   2. Categories with the most dead stock (potential systemic over-ordering)
   3. Suggested actions: liquidate, repurpose, return to supplier, or scrap
   Present as an actionable recommendation table.
   ```

5. **Visualization**
   - Use this prompt:
   ```
   Create two charts:
   1. A pie chart showing inventory value distribution by status
      (Active, Slow, Dead, Frozen)
   2. A bar chart showing the top 10 frozen items by total value
   Make both charts presentation-ready with clear labels and titles.
   ```

6. **Financial Impact Summary**

   | Metric | Value |
   |--------|-------|
   | Total inventory items | |
   | Total inventory value | |
   | Frozen items count | |
   | Frozen items value | |
   | Frozen as % of total value | |
   | Recommended write-off value | |
   | Potential recovery value | |

### Troubleshooting
- **Date formats cause errors**: Standardize all dates to YYYY-MM-DD before uploading. Ask ChatGPT to detect and fix date format inconsistencies.
- **"Last Movement Date" is missing for some items**: Ask ChatGPT to flag these separately. They may be new items or data entry errors.
- **Numbers seem wrong**: Ask ChatGPT to show its calculation for 2-3 specific items so you can verify the logic manually.

---

### Exercise 4: Demand Forecasting

**Objective:** Compare two forecasting methods (Moving Average vs. Exponential Smoothing) and visualize predictions with confidence intervals.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis)

**Step-by-Step Instructions:**

1. **Prepare Time Series Data**
   - You need at least 24 months of demand data: Month, Demand Quantity.
   - Use real consumption data from your department or create a realistic sample.

2. **Generate Forecasts**
   - Use this prompt:
   ```
   I've uploaded monthly demand data. Please:
   1. Calculate a 3-month Simple Moving Average forecast
   2. Calculate an Exponential Smoothing forecast (alpha = 0.3)
   3. For each method, calculate the forecast for the next 6 months
   4. Calculate MAE (Mean Absolute Error) and MAPE (Mean Absolute
      Percentage Error) for each method on the historical data
   5. Show results in a comparison table
   ```

3. **Visualize with Confidence Intervals**
   - Use this prompt:
   ```
   Create a single chart showing:
   - Actual demand (solid black line)
   - Moving Average forecast (blue dashed line)
   - Exponential Smoothing forecast (red dashed line)
   - 95% confidence intervals as shaded bands for each forecast
   - Clear legend and title: "Demand Forecast Comparison"
   Mark the point where historical data ends and forecast begins
   with a vertical dashed line.
   ```

4. **Evaluate and Compare**

   | Metric | Moving Average | Exponential Smoothing | Winner |
   |--------|:--------------:|:---------------------:|:------:|
   | MAE | | | |
   | MAPE | | | |
   | Tracks trend well? | | | |
   | Handles seasonality? | | | |
   | Reacts to recent changes? | | | |
   | Confidence interval width | | | |
   | Best for your data? | | | |

5. **Recommendation**
   - Based on the comparison, which method would you recommend for your department's demand planning? Why?
   - What additional data or methods might improve the forecast?

### Troubleshooting
- **Forecast looks flat or unresponsive**: The Moving Average window may be too wide. Try a shorter window (e.g., 2-month) or increase the Exponential Smoothing alpha.
- **Confidence intervals are extremely wide**: This suggests high variability in your data. Consider whether there are outliers that should be investigated.
- **MAPE is over 50%**: Your data may have irregular demand patterns. Ask ChatGPT to check for outliers and seasonality before forecasting.

---

### Exercise 5: KPI Dashboard Design

**Objective:** Design a management dashboard with 5 KPIs including traffic light status indicators.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis) or Excel/Google Sheets

**Step-by-Step Instructions:**

1. **Select 5 KPIs**
   Choose KPIs relevant to your department. Examples:

   | KPI | Unit | Target | Red Threshold | Yellow Threshold |
   |-----|------|--------|:-------------:|:----------------:|
   | OEE (Overall Equipment Effectiveness) | % | 85% | <70% | 70-84% |
   | MTBF (Mean Time Between Failures) | hours | 500 | <300 | 300-499 |
   | Inventory Turnover | ratio | 6.0 | <3.0 | 3.0-5.9 |
   | Safety Incident Rate | per month | 0 | >3 | 1-3 |
   | On-Time Delivery | % | 95% | <80% | 80-94% |

2. **Populate with Current Data**
   - Use this prompt:
   ```
   Create a KPI dashboard table with these columns:
   KPI Name | Current Value | Target | Trend (last 3 months) | Status (🟢🟡🔴)

   Use these KPIs and values: [insert your 5 KPIs with current values]

   Apply traffic light logic:
   - Green: at or above target
   - Yellow: within warning range
   - Red: below acceptable threshold

   Add a trend arrow: ↑ improving, → stable, ↓ declining
   ```

3. **Generate Visualizations**
   - Use this prompt:
   ```
   For each KPI, create a small gauge chart or bullet chart showing
   current value vs. target. Arrange all 5 in a single dashboard
   layout. Use traffic light colors (red/yellow/green) for the
   background of each gauge.
   ```

4. **Add Commentary**
   - For each KPI in red or yellow status, write:
     - Root cause hypothesis (1 sentence)
     - Recommended action (1 sentence)
     - Expected timeline to green (1 sentence)

5. **Dashboard Template**

   | KPI | Current | Target | Status | Trend | Action Required |
   |-----|:-------:|:------:|:------:|:-----:|-----------------|
   | | | | | | |
   | | | | | | |
   | | | | | | |
   | | | | | | |
   | | | | | | |

### Troubleshooting
- **Traffic light logic seems inverted**: Remember that some KPIs are "higher is better" (OEE) and others are "lower is better" (incident rate). Specify the direction in your prompt.
- **Gauge charts look cluttered**: Simplify by using bullet charts instead. They convey the same information in less space.
- **Trend data is unavailable**: Estimate based on memory or use placeholder data. The goal is to practice the dashboard design pattern.

---

### Exercise 6: 10-Minute Demo Replication

**Objective:** Follow a structured demo script to complete a full data analysis cycle in 10 minutes.

**Tool:** ChatGPT (Plus/Pro with Advanced Data Analysis)

**Step-by-Step Instructions:**

1. **Minute 0-1: Upload**
   - Upload your prepared CSV dataset (any dataset from previous exercises works).
   - Prompt: `"Summarize this dataset: how many rows, columns, data types, and any quality issues."`

2. **Minute 1-3: Explore**
   - Prompt: `"Show descriptive statistics for all numeric columns. Highlight any outliers or unusual values."`
   - Prompt: `"What are the top 3 most interesting patterns you notice in this data?"`

3. **Minute 3-5: Visualize**
   - Prompt: `"Create the single most informative chart for this dataset. Choose the chart type that best reveals the main story in the data."`
   - Prompt: `"Now create a second chart that reveals a pattern not visible in the first chart."`

4. **Minute 5-7: Analyze**
   - Prompt: `"Perform a deeper analysis. Are there correlations, clusters, or trends that management should know about? Show supporting evidence."`

5. **Minute 7-9: Recommend**
   - Prompt: `"Based on this analysis, write 3 specific, actionable recommendations for management. Include the data evidence supporting each recommendation."`

6. **Minute 9-10: Export**
   - Prompt: `"Create a 3-slide executive summary: Slide 1 = Key Findings, Slide 2 = Visualizations, Slide 3 = Recommendations. Format as a clean report I can copy into PowerPoint."`

**Timing Tracker:**

| Stage | Target Time | Actual Time | Prompts Used | Quality (1-5) |
|-------|:-----------:|:-----------:|:------------:|:--------------:|
| Upload | 1 min | | | |
| Explore | 2 min | | | |
| Visualize | 2 min | | | |
| Analyze | 2 min | | | |
| Recommend | 2 min | | | |
| Export | 1 min | | | |

### Troubleshooting
- **AI takes too long on a step**: Skip detailed formatting requests during the timed demo. You can polish outputs afterward.
- **Chart type is wrong for the data**: Specify the chart type explicitly (e.g., "Create a bar chart" instead of "Create a chart").
- **Recommendations are too generic**: Add context to your prompt: "Recommendations should be specific to [your department/industry] and include numeric thresholds."

---

## Independent Practice

### Practice 1: Analyze Your Own Department Data

1. Obtain a dataset from your department (anonymize if necessary by removing names and sensitive identifiers).
2. Upload to ChatGPT and run a complete analysis:
   - Data quality assessment
   - Descriptive statistics
   - At least 3 visualizations
   - Pattern discovery
   - Actionable recommendations
3. Document what you found that was NOT previously known or suspected.

### Practice 2: Create a Presentation-Ready Chart

1. Choose the single most impactful finding from Practice 1.
2. Create a chart that tells the story clearly:
   - Clear title that states the insight (not just "Sales by Month" but "Sales Dropped 23% After Policy Change")
   - Properly labeled axes
   - Annotation highlighting the key finding
   - Color used purposefully (not decoratively)
3. Write a 2-sentence caption that a manager could read and immediately understand the implication.

---

## Real-World Challenge

### Full Data Analysis Pipeline

**Goal:** Complete the entire pipeline from raw data to executive presentation.

**Pipeline Steps:**

| Step | Task | Output | Status |
|------|------|--------|:------:|
| 1. Upload | Load raw data into ChatGPT | Data summary | |
| 2. Explore | Descriptive stats, quality check | Clean dataset profile | |
| 3. Visualize | 3-5 charts revealing key patterns | Saved chart images | |
| 4. Analyze | Statistical analysis, pattern discovery | Written analysis (1 page) | |
| 5. Export | Format for PowerPoint | Slide-ready content | |

**Deliverables:**
- 3-5 presentation-ready visualizations
- 1-page written analysis with findings
- 3 actionable recommendations with supporting data
- PowerPoint-ready export (or actual PowerPoint if time permits)

**Success Criteria:**
- Analysis reveals at least 1 finding that was not previously known
- Visualizations are clear enough for a non-technical audience
- Recommendations are specific and actionable (not generic)

---

## Extension Task

### Automated Weekly Analysis Prompt

**Goal:** Create a reusable prompt template that could be run weekly on refreshed data to produce a consistent analysis report.

**Deliverable:** A documented prompt (or prompt chain) that:

1. **Accepts any weekly data refresh** -- specify the expected CSV format:
   ```
   Expected columns: [list them]
   Expected date range: Most recent 7 days
   Expected row count: Approximately [N]
   ```

2. **Runs a standardized analysis** -- the prompt should:
   - Check data quality and flag anomalies
   - Compare this week to last week and to the same week last year
   - Generate 3 standard charts (specify which)
   - Highlight anything that exceeds defined thresholds
   - Generate a traffic-light summary

3. **Produces a consistent output format**:
   ```
   Weekly Report: [Date Range]

   Executive Summary: [2-3 sentences]

   Key Metrics This Week:
   - Metric 1: [value] (vs. last week: [value], trend: [up/down/stable])
   - Metric 2: ...
   - Metric 3: ...

   Alerts:
   - [Any thresholds exceeded]

   Charts:
   - [Chart 1: description]
   - [Chart 2: description]
   - [Chart 3: description]

   Recommendations:
   - [Based on this week's data]
   ```

4. **Include the full prompt text** that someone else could copy and use:
   - Prompt 1: Data validation and cleaning
   - Prompt 2: Weekly comparison analysis
   - Prompt 3: Visualization generation
   - Prompt 4: Report compilation

**Test your prompt chain** by running it on your dataset and verifying the output matches the expected format.
