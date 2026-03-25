# Unit 1: The Physics of AI — Worksheets

> **Instructions:** Print this handout and bring it to the training session. Complete each exercise during the corresponding activity. Write directly in the spaces provided.

---

## Exercise 1: Token Explorer

**Objective:** Understand how tokenization works across languages and calculate the "linguistic tax" for non-English text.

### Step-by-Step Instructions

1. Open the tokenizer tool provided by your instructor (e.g., OpenAI Tokenizer or tiktoken).
2. Enter the **English sentence** provided below and record the token count.
3. Enter the **Arabic translation** of the same sentence and record the token count.
4. Calculate the linguistic tax using the formula provided.
5. Repeat for all three sentence pairs.

### Workspace

#### Sentence Pair 1

| | Text | Token Count |
|---|------|-------------|
| English | "Artificial intelligence is transforming how we work." | __________ |
| Arabic | (provided by instructor) | __________ |

**Linguistic Tax Calculation:**

```
Linguistic Tax = (Arabic Tokens - English Tokens) / English Tokens x 100

Linguistic Tax = ( ______ - ______ ) / ______ x 100 = ________ %
```

#### Sentence Pair 2

| | Text | Token Count |
|---|------|-------------|
| English | "Please summarize this quarterly financial report and highlight key risks." | __________ |
| Arabic | (provided by instructor) | __________ |

**Linguistic Tax Calculation:**

```
Linguistic Tax = ( ______ - ______ ) / ______ x 100 = ________ %
```

#### Sentence Pair 3

| | Text | Token Count |
|---|------|-------------|
| English | "Generate a professional email declining a vendor proposal politely." | __________ |
| Arabic | (provided by instructor) | __________ |

**Linguistic Tax Calculation:**

```
Linguistic Tax = ( ______ - ______ ) / ______ x 100 = ________ %
```

#### Summary Table

| Sentence Pair | English Tokens | Arabic Tokens | Linguistic Tax (%) |
|---------------|---------------|---------------|-------------------|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| **Average** | | | **____%** |

### Reflection Questions

1. Which sentence pair had the highest linguistic tax? Why do you think that is?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. What are the practical implications of the linguistic tax for Arabic-speaking users?

   _____________________________________________________________________________

   _____________________________________________________________________________

3. How might you adjust your prompting strategy to compensate for this tax?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> Non-Latin scripts consume more tokens for the same meaning, which means shorter effective context windows, higher API costs, and potential quality differences. Always account for this when designing prompts in multilingual environments.

---

## Exercise 2: Context Window Stress Test

**Objective:** Observe how AI accuracy degrades as information moves further from the model's attention focus within a long context.

### Step-by-Step Instructions

1. Paste the **long document** provided by your instructor into the AI model.
2. Ask the model a question about information found on **Page 1** (beginning). Record the accuracy.
3. Ask a question about information found on **Page 2** (middle). Record the accuracy.
4. Ask a question about information found on **Page 3** (end). Record the accuracy.
5. Rate accuracy on a scale of 1-5 (1 = completely wrong, 5 = perfectly accurate).

### Workspace

#### Question & Accuracy Log

| Location | Question Asked | Model's Answer (summary) | Accuracy (1-5) | Correct Answer |
|----------|---------------|--------------------------|-----------------|----------------|
| Page 1 (Beginning) | | | /5 | |
| Page 2 (Middle) | | | /5 | |
| Page 3 (End) | | | /5 | |

#### Comparison Table: Context Position vs. Accuracy

| Factor | Beginning | Middle | End |
|--------|-----------|--------|-----|
| Accuracy Score | /5 | /5 | /5 |
| Detail Level (High/Med/Low) | | | |
| Hallucinations Detected? (Y/N) | | | |
| Response Confidence Tone | | | |

### Reflection Questions

1. Where did the model perform best — beginning, middle, or end? Does this match the "Lost in the Middle" research?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. If you had a 50-page document, how would you structure your prompt to ensure the model focuses on the right section?

   _____________________________________________________________________________

   _____________________________________________________________________________

3. What strategies could you use to work around context window limitations?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> Models tend to pay more attention to information at the beginning and end of the context window, while "losing" information in the middle. Place critical information strategically and use chunking for long documents.

---

## Exercise 3: Temperature Lab

**Objective:** Observe how the temperature parameter affects output variability and creativity.

### Step-by-Step Instructions

1. Choose the prompt provided by your instructor (or use: *"Write a one-paragraph company description for a tech startup."*).
2. Set temperature to **0.0** and run the prompt **3 times**. Record each output.
3. Set temperature to **1.0** and run the prompt **3 times**. Record each output.
4. Compare the results in the observation table.

### Workspace

#### Temperature = 0.0 (Deterministic)

**Run 1:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

**Run 2:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

**Run 3:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

#### Temperature = 1.0 (Creative)

**Run 1:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

**Run 2:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

**Run 3:**

_____________________________________________________________________________

_____________________________________________________________________________

_____________________________________________________________________________

#### Observation Table

| Criterion | Temp = 0.0 | Temp = 1.0 |
|-----------|-----------|-----------|
| Are the 3 outputs identical or different? | | |
| Vocabulary variety (Low/Med/High) | | |
| Creativity level (Low/Med/High) | | |
| Factual consistency (Low/Med/High) | | |
| Risk of nonsense or errors (Low/Med/High) | | |
| Best use case for this setting | | |

### Reflection Questions

1. Were the outputs at temperature 0.0 truly identical? If not, what small differences did you notice?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. At temperature 1.0, did any output contain errors or nonsensical phrases? Give an example.

   _____________________________________________________________________________

   _____________________________________________________________________________

3. For your daily work tasks, what temperature setting would you recommend and why?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> Temperature controls randomness. Use low temperature (0.0-0.3) for factual, consistent tasks like reports and data extraction. Use higher temperature (0.7-1.0) for creative tasks like brainstorming and marketing copy. Match the setting to the task.

---

## Exercise 4: Hallucination Detection

**Objective:** Practice identifying AI-generated false information by verifying citations and claims.

### Step-by-Step Instructions

1. Ask the AI model to generate a short literature review or list of references on the topic provided by your instructor.
2. Select **3 citations** from the AI's response.
3. Attempt to verify each citation using Google Scholar, library databases, or other reliable sources.
4. Record your findings in the table below.

### Workspace

**Prompt used:** _______________________________________________________________

**Topic:** ____________________________________________________________________

#### Citation Verification Table

| # | Title (as given by AI) | Authors (as given by AI) | Year | Real? (Y/N) | Verification Source Used | Notes |
|---|------------------------|--------------------------|------|-------------|--------------------------|-------|
| 1 | | | | | | |
| 2 | | | | | | |
| 3 | | | | | | |

#### Hallucination Analysis

For each citation marked "N" (Not Real), describe what the AI got wrong:

**Citation #____:**

_____________________________________________________________________________

_____________________________________________________________________________

**Citation #____:**

_____________________________________________________________________________

_____________________________________________________________________________

**Citation #____:**

_____________________________________________________________________________

_____________________________________________________________________________

### Reflection Questions

1. How many of the 3 citations were real? Does this match your expectations?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. Were the hallucinated citations plausible? What made them convincing (or not)?

   _____________________________________________________________________________

   _____________________________________________________________________________

3. What verification workflow would you recommend to colleagues who use AI for research?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> AI models can generate convincing but entirely fabricated citations, names, and statistics. Never trust AI-generated references without independent verification. Build a verification step into every research workflow.

---

## Exercise 5: Model Comparison Lab

**Objective:** Compare different AI models on the same task to understand their relative strengths and weaknesses.

### Step-by-Step Instructions

1. Use the **same prompt** across all models assigned by your instructor (e.g., GPT-4, Gemini, Claude, Copilot).
2. Evaluate each model's output on the four criteria below using a 1-10 scale.
3. Record your scores and determine which model is best suited for which task type.

**Prompt used:** _______________________________________________________________

### Workspace

#### Model Comparison Table

| Criterion | Model 1: _________ | Model 2: _________ | Model 3: _________ | Model 4: _________ |
|-----------|-------------------|-------------------|-------------------|-------------------|
| Structure Score (1-10) | /10 | /10 | /10 | /10 |
| Creativity Score (1-10) | /10 | /10 | /10 | /10 |
| Limitations Cited? (Y/N + count) | | | | |
| Accuracy (1-10) | /10 | /10 | /10 | /10 |
| Response Length (words) | | | | |
| Tone Appropriateness (1-10) | /10 | /10 | /10 | /10 |
| **Total Score** | **/40** | **/40** | **/40** | **/40** |
| **Best For** (task type) | | | | |

#### Detailed Observations

**Model 1 (____________):** Strengths & Weaknesses

_____________________________________________________________________________

_____________________________________________________________________________

**Model 2 (____________):** Strengths & Weaknesses

_____________________________________________________________________________

_____________________________________________________________________________

**Model 3 (____________):** Strengths & Weaknesses

_____________________________________________________________________________

_____________________________________________________________________________

**Model 4 (____________):** Strengths & Weaknesses

_____________________________________________________________________________

_____________________________________________________________________________

### Reflection Questions

1. Which model scored highest overall? Was the winner the same across all criteria?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. Did any model refuse or hedge on part of the task? What does that tell you about its safety settings?

   _____________________________________________________________________________

   _____________________________________________________________________________

3. Based on this lab, which model would you choose for (a) drafting reports, (b) creative brainstorming, (c) data analysis? Why?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> No single model is best at everything. Develop a "model portfolio" approach — choose the right model for the right task. Regularly re-evaluate as models are updated frequently.

---

## Exercise 6: Security Audit Simulation

**Objective:** Practice classifying AI use cases by risk level using a traffic-light framework for organizational data governance.

### Step-by-Step Instructions

1. Read each AI use case scenario below.
2. Classify it as **GREEN** (safe to proceed), **YELLOW** (proceed with caution/approval needed), or **RED** (do not use AI for this).
3. Write a brief justification for your classification.
4. Compare your answers with your team after completing individually.

### Workspace

#### Classification Key

- **GREEN:** Public or non-sensitive data; low risk; standard AI tools acceptable.
- **YELLOW:** Internal data with some sensitivity; requires manager approval or anonymization; use approved tools only.
- **RED:** Confidential, personal, or regulated data; significant legal/compliance risk; do not use external AI tools.

#### Use Case Classification Table

| # | Use Case | Classification (G/Y/R) | Justification |
|---|----------|----------------------|---------------|
| 1 | Drafting a public press release about a new product launch | | |
| 2 | Summarizing internal employee performance reviews | | |
| 3 | Generating marketing slogans for a social media campaign | | |
| 4 | Analyzing patient medical records to identify treatment patterns | | |
| 5 | Creating a training presentation about company policies using the employee handbook | | |
| 6 | Uploading a confidential merger agreement to AI for clause extraction | | |
| 7 | Using AI to translate a public-facing FAQ into multiple languages | | |
| 8 | Asking AI to debug a snippet of proprietary source code | | |
| 9 | Generating interview questions for a hiring panel | | |
| 10 | Feeding customer complaint emails (with names and account numbers) into AI for sentiment analysis | | |

#### Team Comparison

After comparing with your team, note any cases where you disagreed:

| Use Case # | Your Classification | Team Consensus | Resolution/Reasoning |
|-----------|-------------------|----------------|---------------------|
| | | | |
| | | | |
| | | | |

### Reflection Questions

1. Which use case was hardest to classify? Why?

   _____________________________________________________________________________

   _____________________________________________________________________________

2. Does your organization currently have an AI usage policy? If so, how does it align with your classifications above?

   _____________________________________________________________________________

   _____________________________________________________________________________

3. What additional information would you need to make a more confident classification for the YELLOW cases?

   _____________________________________________________________________________

   _____________________________________________________________________________

> **Key Takeaway**
>
> Not all AI use cases carry the same risk. Organizations must establish clear data classification policies and AI usage guidelines. When in doubt, escalate — it is far easier to get approval than to recover from a data breach.

---

*End of Unit 1 Worksheets*
