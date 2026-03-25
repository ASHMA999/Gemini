# Unit 2: Applied Prompt Engineering

## The Art and Science of Commanding AI

| Detail | Description |
|--------|-------------|
| **Duration** | 4 hours (including breaks) |
| **Delivery** | Interactive workshop with 12 exercises and 9 challenges |
| **Tools Required** | ChatGPT (chat.openai.com), Claude (claude.ai), Google AI Studio |
| **Objective** | Master writing professional prompts using structured frameworks for consistent, high-quality AI outputs |

---

## 2.1 The CO-STAR Framework: The Gold Standard

Research and practical applications, including Singapore GovTech's famous prompt engineering competition, have proven that prompts following a strict logical structure dramatically outperform open-ended prompts. The CO-STAR framework, developed by competition winner Sheila Teo, is the gold standard for enterprise prompt engineering.

| Element | Full Name | Description | Effect on Model |
|---------|-----------|-------------|-----------------|
| **C** | Context | Complete background: Who are we? What's the situation? | Shrinks the model's probability search space |
| **O** | Objective | Precise, measurable task: Summarize? Analyze? Create? | Aligns model resources to user intent |
| **S** | Style | Writing personality: journalist, consultant, storyteller | Mimics linguistic patterns from training data |
| **T** | Tone | Emotional stance: formal, friendly, empathetic, urgent | Adjusts vocabulary and adjective selection |
| **A** | Audience | Who reads this? Executive vs. engineer vs. student | Adjusts reading level and terminology |
| **R** | Response | Output format: table, JSON, bullet list, paragraphs | Forces structured visual compliance |

### CO-STAR Transformation Example

**BAD Prompt:**

> "Summarize user complaints and tell me what to do." (No context, vague goal, no format, no audience)

**PERFECT Prompt (CO-STAR Applied):**

> **(C)** I'm a Product Manager for a food delivery app facing user backlash after removing the 'Quick Reorder' button. Reviews below are from the app store in the last 48 hours.
> **(O)** Perform sentiment analysis and extract root causes. Classify problems into categories: Technical, Design, UX.
> **(S)** Write as a strategic analyst focused on actionable insights.
> **(T)** Objective, professional, and direct.
> **(A)** The engineering team and UI/UX designers (use precise technical terms).
> **(R)** Deliver a Markdown table with columns: [Problem Category], [Description], [Impact Level], [Proposed Fix]. End with one top-priority strategic recommendation.

### Hands-On Exercise 7: CO-STAR Transformation Workshop (20 minutes)

Each trainee receives a 'bad prompt' card. Transform it into a perfect prompt using all 6 CO-STAR elements. Bad prompts include: 'Write a job ad,' 'Analyze this data,' 'Fix this report,' 'Make a presentation about safety.' Share transformations with the class for feedback.

---

## 2.2 Additional Frameworks for Specific Scenarios

### RACE Framework (Best for Plans & Projects)

- **R = Role:** "You are an industrial maintenance engineer with 15 years of experience in potash plants"
- **A = Action:** "Develop a preventive maintenance plan for brine transfer pumps"
- **C = Context:** "Pumps operate 24/7, high-salinity environment, last failure was 2 months ago"
- **E = Expectation:** "I need a monthly schedule with spare parts list and estimated costs"

### RTF Framework (Best for Quick Tasks)

- **R = Role:** "Act as an occupational safety specialist in a chemical plant"
- **T = Task:** "Review safety procedures for handling concentrated acids"
- **F = Format:** "Deliver as a 10-point checklist"

Best for: translating technical reports, summarizing meeting minutes, converting data formats, reviewing SOPs.

### PARA Framework (Best for Problem-Solving)

- **P = Problem:** "Employee turnover in the production department has risen to 15%"
- **A = Action:** "Analyze root causes and suggest 5 practical solutions"
- **R = Result:** "I want to reduce the rate to 5% within 6 months"
- **A = Adjustment:** "Focus on solutions that don't require significant additional budget"

### Framework Selection Guide

| Framework | Best For | Examples |
|-----------|----------|----------|
| CO-STAR | Complex reports & strategy | Board reports, government correspondence, strategic analysis |
| RACE | Plans & projects | Maintenance plans, training programs, project proposals |
| RTF | Quick tasks | Translations, summaries, format conversions, SOP reviews |
| PARA | Problem-solving | Fault analysis, safety incidents, performance gaps |

### Hands-On Exercise 8: Framework Selection Challenge (25 minutes)

You receive 8 real-world scenarios. For each, select the best framework AND write the complete prompt. Scenarios: (1) Writing a job ad for a chemical engineer, (2) Analyzing production line downtime, (3) Translating a technical manual, (4) Preparing a quarterly board report, (5) Investigating a safety incident, (6) Creating an emergency response plan, (7) Summarizing meeting minutes, (8) Evaluating a new equipment purchase.

---

## 2.3 Advanced Prompting Techniques

### Few-Shot Learning (Teaching by Example)

Instead of giving abstract instructions, provide the model with examples from your actual company records. Examples act as 'micro training data' that guide the model to replicate patterns with precision.

**Strong Prompt with Examples:**

> Write a fault report in the same format as these examples:
> Example 1: Equipment: Conveyor Belt B-201, Fault: Belt slippage, Cause: Worn tensioner...
> Example 2: Equipment: Electric Motor M-105, Fault: Overheating, Cause: Bearing failure...
> New fault: Pump P-301 is producing abnormal noise.

### Chain-of-Thought (CoT) Reasoning

Adding 'Think step by step' to your prompt dramatically improves accuracy for complex analytical tasks. Google research proved this single phrase can increase mathematical reasoning accuracy by 40%+.

**CoT Example for Industrial Analysis:**

> Analyze why crusher downtime has increased by 8%. Think step by step:
> 1. What are the observed symptoms?
> 2. Which subsystems are likely affected?
> 3. What inspections are needed?
> 4. Rank causes from most to least probable.
> 5. What is the proposed repair plan and estimated cost?

### Multi-Role Perspective

Get multiple expert viewpoints on the same decision by asking the AI to analyze from different roles simultaneously.

- **As CFO:** What's the ROI on this new crusher purchase?
- **As Production Manager:** Does it solve our capacity bottleneck?
- **As Maintenance Manager:** What are lifecycle costs and spare parts availability?
- **As Safety Officer:** What are the risks and compliance requirements?

### Constraint Engineering

Constraints ensure outputs comply with company standards and industry regulations. Types include:

- **Standards constraints:** "Per ISO 45001" or "OSHA-compliant"
- **Operational constraints:** "Without stopping production"
- **Budget constraints:** "Not exceeding 50,000 JOD"
- **HR constraints:** "Using available staff only"
- **Safety constraints:** "Zero-incident target"

### Hands-On Exercise 9: The Debugging Lab (20 minutes)

You receive 3 'catastrophically bad' prompts. Diagnose what's wrong and fix each one. (1) 'Send an email to clients about the new product.' (No product, no audience, no tone) (2) 'Summarize the article and give me quotes the author never said.' (Forces hallucination) (3) 'Explain quantum mechanics in PhD-level academic depth but simple enough for a 5-year-old.' (Conflicting audience) Present your fixes to the class.

---

## 2.4 GPT-5.4 vs. Claude Opus 4.6: Formatting Preferences

| Criterion | GPT-5.4 Thinking (OpenAI) | Claude Opus 4.6 (Anthropic) |
|-----------|--------------------------|----------------------------|
| Preferred Format | Markdown (# Headlines, bullet lists) | XML Tags (`<instruction>`, `<context>`, `<example>`) |
| Thinking Style | Thinking traces expose step-by-step reasoning for complex tasks | Natural narration, 1M-token context, superior long-document analysis |
| Long Context | Excellent agentic multi-step workflows | Industry-leading long-context retrieval with no detail loss |
| Pro Hack | Use 'Thinking' mode for complex reasoning chains | Pre-fill the response start to force format compliance |

### Hands-On Exercise 10: Prompt Battle (15 minutes)

Teams compete! The trainer shows an AI-generated image. Each team has 2 minutes to write a prompt that recreates the image as closely as possible. Prompts are run live. The audience votes on the closest match. Lesson: precise language creates precise results.
