# Unit 1 Applications: The Physics of AI

> **Hands-On Practical Exercises**
> Complete these exercises using real AI tools to build foundational understanding of how AI models work, their capabilities, and their limitations.

---

## Guided Exercises

### Exercise 1: Token Exploration Lab

**Objective:** Understand how tokenization works across languages and technical domains.

**Tool:** [OpenAI Tokenizer](https://platform.openai.com/tokenizer) (select GPT-4 model)

**Step-by-Step Instructions:**

1. Open the OpenAI Tokenizer in your browser.
2. Select the **GPT-4** model from the dropdown menu.
3. Enter each of the following texts one at a time and record the token count:

| # | Text to Enter | Expected Tokens (approx.) | Your Count |
|---|--------------|--------------------------|------------|
| 1 | `Hello, how are you today?` | 6 | ___ |
| 2 | `مرحباً، كيف حالك اليوم؟` | 12-15 | ___ |
| 3 | `The polyethylene terephthalate extrusion line operates at 280°C` | 11-13 | ___ |
| 4 | `خط بثق البولي إيثيلين تيريفثاليت يعمل عند 280 درجة مئوية` | 35-45 | ___ |
| 5 | `Q3 2025 KPI dashboard: OEE=87.2%, MTBF=342hrs, yield=94.6%` | 25-30 | ___ |

4. Now enter a full paragraph from one of your work documents (approximately 100 words in English). Record the token count: ___
5. Translate that same paragraph to Arabic and enter it. Record the token count: ___

**Key Observations to Document:**
- What is the ratio of Arabic tokens to English tokens for equivalent text?
- Why do technical abbreviations (OEE, MTBF, KPI) tokenize differently from full words?
- What does this mean for the cost of processing Arabic content versus English content?

**Record your findings here:**
```
English paragraph word count:    ___
English paragraph token count:   ___
Arabic paragraph word count:     ___
Arabic paragraph token count:    ___
Token ratio (Arabic/English):    ___
```

---

### Exercise 2: Context Window Test

**Objective:** Test how well AI retrieves information from different positions within a long document.

**Tool:** Google AI Studio (gemini.google.com) or ChatGPT

**Step-by-Step Instructions:**

1. Prepare a multi-page document (5-10 pages). Use an existing work report or create one by combining several shorter documents.
2. Insert three unique "marker phrases" that do not naturally belong in the document:
   - **Page 1 (Beginning):** Insert the phrase: `"The secret code for the beginning is ALPHA-7742."`
   - **Middle of the document:** Insert the phrase: `"The hidden reference number is BRAVO-3391."`
   - **Last page (End):** Insert the phrase: `"The final verification code is CHARLIE-5568."`
3. Upload the document to Google AI Studio.
4. Ask the following questions one at a time and record the results:

| Question | Expected Answer | AI's Answer | Correct? |
|----------|----------------|-------------|----------|
| "What is the secret code for the beginning?" | ALPHA-7742 | ___ | Y / N |
| "What is the hidden reference number?" | BRAVO-3391 | ___ | Y / N |
| "What is the final verification code?" | CHARLIE-5568 | ___ | Y / N |
| "List all three codes mentioned in the document." | All three | ___ | Y / N |

5. Now ask a question about a specific detail from the **middle** of the document that was part of the original content (not your inserted codes).

**Key Observations:**
- Did the AI retrieve information from all three positions equally well?
- Was information from the middle of the document harder to retrieve? (This is the "Lost in the Middle" phenomenon.)
- How did the AI perform when asked to synthesize information from multiple positions?

---

### Exercise 3: Temperature Experiment

**Objective:** Observe how the temperature parameter affects AI output variability and creativity.

**Tool:** Google AI Studio (with adjustable temperature setting) or OpenAI Playground

**Step-by-Step Instructions:**

1. Open Google AI Studio and locate the temperature slider in the settings panel (right side).
2. Use this exact prompt for all three runs:

```
Write a one-paragraph product description for a new industrial adhesive
designed for high-temperature plastic bonding in manufacturing environments.
```

3. **Run 1 - Temperature 0.0:**
   - Set temperature to 0.0
   - Generate the response
   - Copy and paste the output below:

```
Temperature 0.0 Output:
[Paste here]
```

4. **Run 2 - Temperature 0.5:**
   - Set temperature to 0.5
   - Generate the response three times (click generate three separate times)
   - Copy all three outputs:

```
Temperature 0.5 Output (Run A):
[Paste here]

Temperature 0.5 Output (Run B):
[Paste here]

Temperature 0.5 Output (Run C):
[Paste here]
```

5. **Run 3 - Temperature 1.0:**
   - Set temperature to 1.0
   - Generate the response three times
   - Copy all three outputs:

```
Temperature 1.0 Output (Run A):
[Paste here]

Temperature 1.0 Output (Run B):
[Paste here]

Temperature 1.0 Output (Run C):
[Paste here]
```

**Analysis Table:**

| Criteria | Temp 0.0 | Temp 0.5 | Temp 1.0 |
|----------|----------|----------|----------|
| Are repeat runs identical? | ___ | ___ | ___ |
| Vocabulary variety (low/med/high) | ___ | ___ | ___ |
| Factual accuracy (high/med/low) | ___ | ___ | ___ |
| Creativity level (low/med/high) | ___ | ___ | ___ |
| Suitable for: (list use cases) | ___ | ___ | ___ |

**Key Takeaway:** When should you use each temperature setting in your work?
- Temperature 0.0 is best for: ___
- Temperature 0.5 is best for: ___
- Temperature 1.0 is best for: ___

---

### Exercise 4: Hallucination Hunt

**Objective:** Identify and document AI hallucinations to understand the limits of AI reliability.

**Tool:** ChatGPT, Claude, or Gemini (pick one)

**Step-by-Step Instructions:**

1. Ask the AI the following five questions, one at a time.
2. Record the AI's answer.
3. Verify each answer using a reliable source (Google Scholar, official website, encyclopedia).
4. Mark whether the answer is correct, partially correct, or a hallucination.

| # | Question | AI's Answer | Verified Answer | Source Used | Verdict |
|---|----------|-------------|-----------------|-------------|---------|
| 1 | "Who is the current CEO of Saudi Aramco and when did they start?" | ___ | ___ | ___ | Correct / Partial / Hallucination |
| 2 | "What is the exact melting point of HDPE (high-density polyethylene) in Celsius?" | ___ | ___ | ___ | Correct / Partial / Hallucination |
| 3 | "List the three most recent winners of the King Abdulaziz Quality Award in the industrial category." | ___ | ___ | ___ | Correct / Partial / Hallucination |
| 4 | "What Saudi labor law article covers end-of-service benefits calculation?" | ___ | ___ | ___ | Correct / Partial / Hallucination |
| 5 | "What is the annual plastic production capacity of Saudi Arabia as of 2024?" | ___ | ___ | ___ | Correct / Partial / Hallucination |

**Hallucination Patterns to Watch For:**
- Confident but fabricated statistics
- Invented names or dates
- Mixing up similar but distinct facts
- Outdated information presented as current
- Plausible-sounding but nonexistent references or article numbers

**Summary:** Out of 5 questions, how many had fully accurate answers? ___/5

---

### Exercise 5: Model Shootout

**Objective:** Compare the strengths and weaknesses of different AI models on the same task.

**Tools:** ChatGPT (chat.openai.com), Claude (claude.ai), Gemini (gemini.google.com)

**Step-by-Step Instructions:**

1. Use this exact prompt in all three models:

```
You are an industrial engineering consultant. A plastic packaging factory
in Saudi Arabia is experiencing a 12% increase in defect rates on their
blow molding line over the past quarter. The main defects are uneven wall
thickness and base cracking.

Provide a structured root cause analysis with:
1. Top 5 most likely causes ranked by probability
2. Recommended diagnostic tests for each cause
3. Estimated timeline and cost category (low/medium/high) for each fix
4. A prioritized action plan for the next 30 days
```

2. Record responses from all three models.
3. Complete the comparison table:

| Criteria | ChatGPT | Claude | Gemini |
|----------|---------|--------|--------|
| Response length (words) | ___ | ___ | ___ |
| Technical accuracy (1-5) | ___ | ___ | ___ |
| Practical usefulness (1-5) | ___ | ___ | ___ |
| Structure and clarity (1-5) | ___ | ___ | ___ |
| Saudi/regional awareness (1-5) | ___ | ___ | ___ |
| Actionability (1-5) | ___ | ___ | ___ |
| **Total Score** | ___ | ___ | ___ |

**Key Observations:**
- Which model provided the most technically detailed response?
- Which model was most practical and actionable?
- Did any model reference Saudi-specific regulations or standards?
- Which model would you trust most for this type of analysis? Why?

---

## Independent Practice

### Practice 1: Token Cost Calculation

**Task:** Calculate the token cost of translating a 10-page English technical report into Arabic.

**Instructions:**
1. Take a 10-page report (or estimate at approximately 3,000 English words / ~4,000 tokens).
2. Using the token ratios you discovered in Exercise 1, estimate the Arabic token count.
3. Look up current API pricing for GPT-4 and calculate total cost:
   - Input tokens: English original = ___
   - Output tokens: Arabic translation = ___
   - GPT-4 input price per 1K tokens: $___
   - GPT-4 output price per 1K tokens: $___
   - **Total estimated cost: $___**
4. Compare this cost to a professional human translation service quote.

### Practice 2: "Lost in the Middle" Deep Dive

**Task:** Design and run your own experiment to test the "Lost in the Middle" phenomenon.

**Instructions:**
1. Create a document with 20 distinct facts numbered and placed at known positions.
2. Upload to an AI tool and ask about facts from positions 1, 5, 10, 15, and 20.
3. Create a retrieval accuracy chart showing performance by position.
4. Write a one-paragraph summary of your findings and what this means for how you provide information to AI tools.

---

## Real-World Challenge

### AI Usage Audit

**Task:** Audit your department's current AI usage and classify each use case by risk level.

**Instructions:**

1. Survey your team (or reflect on your own usage) and list every way AI is currently being used or could be used.
2. Classify each use case using this risk matrix:

| Use Case | AI Tool Used | Data Sensitivity (H/M/L) | Decision Impact (H/M/L) | Verification Needed? | Risk Level |
|----------|-------------|--------------------------|-------------------------|---------------------|------------|
| ___ | ___ | ___ | ___ | ___ | ___ |
| ___ | ___ | ___ | ___ | ___ | ___ |
| ___ | ___ | ___ | ___ | ___ | ___ |

**Risk Level Classification:**
- **Low Risk:** General knowledge queries, brainstorming, drafting non-sensitive content
- **Medium Risk:** Analyzing business data, drafting client communications, summarizing reports
- **High Risk:** Legal/compliance content, financial decisions, safety-critical analysis, personal data processing

3. For each High Risk use case, write a one-sentence mitigation strategy.
4. Present your findings in a one-page summary.

---

## Extension Task

### Secure AI Deployment Design for APC

**Task:** Research and design a secure AI deployment architecture for APC (Advanced Petrochemical Company).

**Deliverable:** A 2-3 page proposal covering:

1. **Current Landscape:** What AI tools are available for enterprise deployment (Azure OpenAI, Google Vertex AI, AWS Bedrock)?
2. **Data Classification:** Which APC data categories (public, internal, confidential, restricted) can be used with which AI tools?
3. **Architecture Recommendation:** Diagram showing where AI processes data - cloud, hybrid, or on-premise for each use case.
4. **Policy Framework:** Draft 5 key AI usage policies specific to APC's industrial context.
5. **Implementation Roadmap:** Phased approach (3-month, 6-month, 12-month milestones).

**Research Sources to Consult:**
- Microsoft Azure OpenAI Service documentation
- Saudi NDMO (National Data Management Office) data classification standards
- SDAIA (Saudi Data and AI Authority) AI ethics guidelines
- Industry-specific AI governance frameworks (ISO/IEC 42001)

---

## Troubleshooting Tips

| Problem | Cause | Solution |
|---------|-------|----------|
| OpenAI Tokenizer shows different counts than expected | Model version mismatch | Ensure you select the GPT-4 tokenizer, not GPT-3.5 |
| Cannot upload document to Google AI Studio | File too large or unsupported format | Convert to PDF or plain text; keep under 20 pages |
| Temperature slider not visible | Tool does not expose this setting | Use Google AI Studio or OpenAI Playground instead of the chat interfaces |
| AI refuses to answer a question | Content policy trigger | Rephrase the question to be more specific and professional |
| Responses vary wildly between runs at Temperature 0.0 | Caching or system prompt changes | Clear conversation history and start a new chat for each run |
| Model Shootout results are too similar | Prompt is too simple | Use a more domain-specific, detailed prompt that differentiates model capabilities |
| Token counts for Arabic seem inconsistent | Mixed scripts (Arabic + numbers/English) | Test pure Arabic text separately from mixed-language text |
| Google AI Studio is unavailable in your region | Regional restrictions | Use a VPN or switch to an alternative tool such as ChatGPT or Claude |
