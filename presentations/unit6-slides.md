---
marp: true
theme: default
paginate: true
header: "Unit 6: Specialized AI Tools & Knowledge Engines | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# Unit 6: Specialized AI Tools & Knowledge Engines

**APC AI Excellence Program**

---

# Learning Objectives

By the end of this unit, you will be able to:

- **Leverage** NotebookLM to build searchable knowledge bases from internal documents
- **Conduct** deep research using ChatGPT, Gemini, and Perplexity tools
- **Use** scientific AI tools (Consensus, Elicit) for evidence-based decisions
- **Design** a knowledge ecosystem workflow for your department
- **Select** the right AI tool for a given research or knowledge task

---

# NotebookLM: Your AI Research Assistant

**What is NotebookLM?** A Google AI tool that grounds responses in *your* uploaded documents.

### Core Features

- **Source-grounded answers** - AI only references your uploaded materials, reducing hallucination
- **Multi-source synthesis** - Upload PDFs, Google Docs, websites, YouTube links
- **Audio overviews** - Auto-generates podcast-style summaries of your sources
- **Inline citations** - Every answer links back to the specific source passage
- **Notebook guides** - FAQ, study guide, table of contents auto-generated

> **Why it matters for APC:** Answers come from *your* documents, not the open internet. This keeps proprietary knowledge secure.

---

# NotebookLM: Industrial Use Cases at APC

| Use Case | Sources to Upload | Value |
|----------|------------------|-------|
| **Equipment troubleshooting** | OEM manuals, maintenance logs, SOPs | Instant answers from 1000s of pages |
| **Regulatory compliance** | JMRE regulations, ISO standards, audit reports | Quick cross-reference during inspections |
| **Onboarding new engineers** | Training manuals, safety procedures, P&IDs | Self-service knowledge for new hires |
| **Incident investigation** | Past incident reports, root cause analyses | Pattern recognition across historical data |
| **Vendor evaluation** | Vendor proposals, spec sheets, performance data | Side-by-side comparison with citations |

> **Example prompt:** "Based on the uploaded maintenance logs, what are the top 3 recurring failure modes for the crystallizer pumps in the last 2 years?"

---

# Building a Maintenance Knowledge Base in NotebookLM

### Step-by-Step Setup

1. **Create a notebook** for each major equipment system (e.g., "Crystallizer System")
2. **Upload sources:**
   - OEM maintenance manuals (PDF)
   - Historical work orders (exported from CMMS)
   - Past root cause analysis reports
   - Relevant engineering standards
3. **Test with queries:**
   - "What is the recommended bearing replacement interval?"
   - "Summarize all crystallizer pump failures from 2024-2025"
   - "Compare the troubleshooting steps for high vibration vs. cavitation"

### Best Practices
- Keep each notebook focused on **one system or topic**
- Update sources quarterly with new maintenance data
- Share notebooks with team members for collaborative use

---

# Deep Research Tools: Overview

> **Deep Research** = AI agents that autonomously search, read, and synthesize information from many sources over extended periods.

| Tool | Provider | Strengths | Best For |
|------|----------|-----------|----------|
| **ChatGPT Deep Research** | OpenAI | Thorough multi-step research, report generation | Comprehensive technical reports |
| **Gemini Deep Research** | Google | Google Search integration, real-time data | Current market/technology trends |
| **Perplexity Pro** | Perplexity | Source transparency, academic focus | Quick answers with citations |

### How They Work
1. You submit a research question
2. AI creates a research plan
3. Agent browses dozens of sources autonomously
4. Synthesizes findings into a structured report
5. Provides citations for every claim

---

# Deep Research: Practical Examples for APC

### Example 1: Technology Scouting
> "Research the latest advances in potash crystallization technology published in the last 2 years. Compare energy efficiency of mechanical vapor recompression vs. multi-effect evaporation. Include vendor options and estimated costs."

### Example 2: Regulatory Intelligence
> "What changes to Jordanian environmental regulations affecting potash mining have been proposed or enacted since January 2025? Summarize compliance requirements and deadlines."

### Example 3: Failure Analysis Support
> "Research documented cases of stress corrosion cracking in 316L stainless steel exposed to potash brine solutions above 80C. What mitigation strategies have been effective in similar industries?"

**Tip:** The more specific your research prompt, the more actionable the output.

---

# Scientific AI Tools: Consensus & Elicit

## Consensus
- Searches **peer-reviewed research papers** only
- Provides a "consensus meter" showing scientific agreement
- Ideal for evidence-based technical decisions

**Example:** "Is ultrasonic testing more effective than radiographic testing for detecting SCC in austenitic stainless steel welds?"

## Elicit
- AI research assistant for **systematic literature review**
- Extracts key data points across papers into structured tables
- Filters by methodology, sample size, publication date

**Example:** "Find studies on membrane filtration for potash brine purification. Extract: membrane type, flux rate, rejection rate, brine concentration."

> **When to use:** Technical debates, material selection justification, process optimization decisions that need scientific backing.

---

# The Knowledge Ecosystem Workflow

```
         Question / Problem
                |
     +----------+----------+
     |          |          |
  Internal   Current    Scientific
  Knowledge  Research   Evidence
     |          |          |
 NotebookLM  Deep       Consensus
             Research    / Elicit
     |          |          |
     +----------+----------+
                |
         Synthesized Answer
                |
         Decision / Action
```

- **Internal Knowledge** - What does APC already know? (NotebookLM)
- **Current Research** - What is the industry doing now? (Deep Research)
- **Scientific Evidence** - What does the science say? (Consensus, Elicit)

---

# Tool Selection Guide

| Scenario | Recommended Tool | Why |
|----------|-----------------|-----|
| "What does our manual say about X?" | **NotebookLM** | Grounded in your documents |
| "What are industry best practices for X?" | **Gemini/ChatGPT Deep Research** | Broad web synthesis |
| "What does the research say about X?" | **Consensus / Elicit** | Peer-reviewed evidence |
| "Quick answer with sources for X?" | **Perplexity** | Fast, cited responses |
| "Compare vendor claims about X?" | **NotebookLM** (upload vendor docs) | Side-by-side from sources |
| "Is technology X proven effective?" | **Consensus** | Scientific consensus view |
| "Summarize this 200-page report" | **NotebookLM** | Source-grounded summary |

> **Rule of Thumb:** Start with internal knowledge (NotebookLM), then expand outward to research tools.

---

# Exercise 24: Build a NotebookLM Knowledge Base

**Task:** Create a NotebookLM notebook for one of your equipment systems.

1. Select a system you work with regularly
2. Upload at least **5 relevant sources** (manuals, logs, reports)
3. Ask the notebook **10 questions** of increasing complexity
4. Rate answer quality for each (Excellent / Good / Incomplete / Wrong)
5. Generate an **Audio Overview** and evaluate its usefulness

**Deliverable:** Table of 10 questions, AI answers, quality ratings, and recommendations for improving the knowledge base.

---

# Exercise 25: Deep Research Comparison

**Task:** Submit the same technical question to three deep research tools.

1. Formulate a research question relevant to your APC role
2. Submit to: **ChatGPT Deep Research**, **Gemini Deep Research**, **Perplexity Pro**
3. Compare results across:

| Criteria | ChatGPT | Gemini | Perplexity |
|----------|---------|--------|------------|
| Depth of analysis | | | |
| Source quality | | | |
| Accuracy (spot-check) | | | |
| Time to complete | | | |
| Actionability | | | |

**Deliverable:** Comparison report with your recommended tool for different scenarios.

---

# Exercise 26: Scientific Evidence Gathering

**Task:** Use Consensus and Elicit to research a technical decision.

1. Identify a technical question at APC where scientific evidence would help
2. Search **Consensus** for the scientific consensus
3. Use **Elicit** to extract structured data from relevant papers
4. Write a one-page **evidence brief** summarizing findings and recommendation

**Deliverable:** Evidence brief with at least 5 cited papers and a clear recommendation.

---

# Exercise 27: Knowledge Ecosystem Design

**Task:** Design a knowledge workflow for your department.

1. Map the **top 10 questions** your team asks repeatedly
2. For each question, identify the **best tool** and **source documents** needed
3. Create a **knowledge access plan:**
   - Which NotebookLM notebooks to build
   - Which deep research templates to create
   - How to keep sources updated
4. Estimate **time savings** vs. current methods

**Deliverable:** Knowledge ecosystem plan document with tool assignments and maintenance schedule.

---

# Unit 6 Recap

| Topic | Key Takeaway |
|-------|-------------|
| NotebookLM | Ground AI answers in your own documents for trusted responses |
| Deep Research | Let AI agents do hours of research in minutes |
| Consensus & Elicit | Scientific evidence for technical decisions |
| Knowledge Ecosystem | Combine internal, current, and scientific sources |
| Tool Selection | Match the tool to the question type |

> **Next Unit:** We dive into data analysis - using AI to mine insights from operational, maintenance, and safety data.
