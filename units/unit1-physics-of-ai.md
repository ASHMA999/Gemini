# Unit 1: The Physics of AI

## Infrastructure, Core Concepts & Enterprise Risks of Generative AI

| Detail | Description |
|--------|-------------|
| **Duration** | 4 hours (including breaks) |
| **Delivery** | Lecture + Live Demos + Group Exercises |
| **Tools Required** | Google AI Studio (aistudio.google.com), OpenAI Tokenizer (platform.openai.com/tokenizer) |
| **Objective** | Understand how LLMs work under the hood, and why using free accounts for work is a strategic and legal disaster |

---

## 1.1 Tokens: The Currency of the New Digital Economy

A Token is NOT a word. It is the smallest semantic unit that a model can process. It could be a full word (like "Apple"), a sub-word (like "ing" in "Playing"), or even a space character. Understanding tokens is critical because they determine cost, capacity, and performance.

### The Golden Rule

1,000 tokens = approximately 750 English words. Arabic text consumes roughly 2x more tokens for the same meaning because tokenizers are primarily trained on Latin-based languages. This is the 'Linguistic Tax' that organizations must budget for.

### Why Tokens Are the Currency

- **Cost:** AI providers charge per million tokens (both input and output)
- **Capacity:** Model memory is limited by a fixed number of tokens
- **Performance:** More tokens = longer processing time (higher latency)

### Hands-On Exercise 1: Token Explorer (15 minutes)

Open platform.openai.com/tokenizer. Type the sentence 'Arab Potash Company produces potassium chloride' and observe the token count. Now type the same sentence in Arabic and compare. Calculate the 'linguistic tax' percentage. Then open Google AI Studio and test how the same prompt produces different results when you change the model.

---

## 1.2 Context Window: The Working Memory

The Context Window is the maximum amount of information (text, files, code) that a model can 'see' and process at any given moment before it starts forgetting the beginning of the conversation. Think of it as RAM for AI.

| Window Size | Analogy | Best For |
|-------------|---------|----------|
| Small (8K-32K) | A sticky note | Quick chats, simple Q&A, single-task prompts |
| Medium (32K-128K) | A notebook | Document analysis, multi-step reasoning |
| Large (128K-1M+) | An entire library | Analyzing entire codebases, books, or years of records |

### Lost in the Middle Phenomenon

Large context windows suffer from reduced accuracy when retrieving information located in the MIDDLE of a long text, compared to the beginning and end. Always place your most critical instructions at the TOP and BOTTOM of your prompt.

### Hands-On Exercise 2: Context Window Stress Test (20 minutes)

In Google AI Studio, select Gemini 3.1 Pro. Paste a 3-page document and ask a question about content on page 1, page 2, and page 3 separately. Observe which answers are most accurate. Then try the same with a shorter-context model and compare quality degradation.

---

## 1.3 Temperature: The Precision-Creativity Dial

Temperature is a mathematical parameter (added to the Softmax equation) that controls the 'randomness' of the next word selection. It is the single most impactful setting you can adjust.

| Temperature | Behavior | Ideal Use Cases |
|-------------|----------|-----------------|
| Low (0.0 - 0.2) | Deterministic, precise, conservative | Coding, data extraction, financial analysis, legal contracts |
| Medium (0.5) | Balanced | Customer replies, email drafting, meeting summaries |
| High (0.8 - 1.0) | Random, creative, diverse | Brainstorming, ad copy, storytelling, ideation |

### Hands-On Exercise 3: Temperature Lab (15 minutes)

In Google AI Studio, write this prompt: 'Suggest 5 names for a new potash-based fertilizer product.' Run it 3 times at Temperature 0.0, then 3 times at Temperature 1.0. Document the differences in creativity and consistency. Which setting would you use for a board report vs. a marketing brainstorm?

---

## 1.4 Hallucinations: When the Model Dreams

A hallucination is when the model generates a response that sounds linguistically logical and extremely confident, but is entirely fabricated with no basis in reality. This is NOT the same as an error. An error might come from outdated information. A hallucination is pure invention.

### Why It Happens

LLMs are probabilistic systems, NOT knowledge bases. They are designed to predict 'the most probable next word,' not 'the truthful next word.' The model doesn't 'lie' with intent to deceive; it performs 'Pattern Completion' and fills gaps with plausible-sounding fiction.

### Three Real-World Hallucination Disasters

#### Case Study 1: Samsung Leak (2023)

Engineers in Samsung's semiconductor division pasted top-secret source code into ChatGPT to debug it. The code became part of OpenAI's training data. Samsung banned all generative AI tools and began building an internal solution.

**Lesson:** Never put anything in a free chatbox that you wouldn't want published in a newspaper.

#### Case Study 2: Mata v. Avianca (2023)

A lawyer used ChatGPT to write a legal brief and asked it for case precedents. The model hallucinated entire cases with fake names, dates, and citations that looked completely real. The lawyer submitted the brief to court, was caught, fined, and professionally humiliated.

**Lesson:** An LLM is a generation engine, NOT a search engine. Always verify. Human in the Loop is non-negotiable.

#### Case Study 3: Air Canada Chatbot (2024)

Air Canada's AI chatbot gave a passenger false information about the refund policy, contradicting the written policy on the website. The airline argued the chatbot was a 'separate entity.' The court ruled the company IS responsible for its AI's outputs and ordered compensation.

**Lesson:** Hallucinations have direct financial and legal costs for the company.

### Hands-On Exercise 4: Hallucination Detection Challenge (20 minutes)

Ask ChatGPT: 'What are the top 3 academic papers published about potash mining safety in 2024? Provide full citations.' Then try to verify each citation using Google Scholar. How many are real? Now ask the same question to Claude and compare. Discuss strategies to prevent hallucination-based decisions.

---

## 1.5 The AI Landscape 2026: Comparing the Giants

| Provider / Model | Specialization | Key Strengths | Enterprise Notes |
|------------------|---------------|---------------|------------------|
| OpenAI (GPT-5.4 Thinking) | Deep reasoning & agentic workflows | Thinking traces for complex multi-step tasks | Released March 2026, premium pricing |
| Anthropic (Claude Opus 4.6) | Coding, safety & long-context | 1M-token context window, massive long-context retrieval gains | Released Feb 2026, preferred for deep analysis |
| Google (Gemini 3.1 Pro) | Native multimodal & agentic search | High-efficiency reasoning across text, image, video | Released Feb 2026, deep Google Workspace integration |
| DeepSeek (V3) | Cost efficiency | Stunning cost-to-performance ratio | Data sovereignty concerns (host locally) |
| xAI (Grok) | Real-time data | Integration with X/Twitter live feeds | Good for trend analysis |

### Hands-On Exercise 5: Model Comparison Lab (25 minutes)

Give the EXACT same prompt to ChatGPT, Claude, and Gemini: 'You are a safety engineer. Analyze why conveyor belt failures increase during summer months in mining operations. Provide a root cause analysis in table format.' Compare: Which model gave the most structured answer? Which was most creative? Which cited limitations?

---

## 1.6 Data Privacy & Enterprise Security

This is the most legally dangerous section for companies. Misunderstanding here has cost organizations millions of dollars.

| Comparison Point | Free / Personal Account | Enterprise / Team / API |
|-----------------|------------------------|------------------------|
| Model Training | ENABLED by default. Your inputs train the model. | Contractually PROHIBITED (Zero-Training Policy) |
| Data Retention | Logs retained for 30+ days | Zero-Retention. Can be set to never save. |
| Data Ownership | Ambiguous (broad usage license) | Full and exclusive ownership by the organization |
| Security | Standard protection | SOC2, HIPAA, GDPR compliance certificates |

### Critical Message for Enterprises

Using free AI accounts for work purposes is the equivalent of voluntarily leaking your company's trade secrets. Shadow AI (employees using unauthorized AI tools) is the #1 emerging risk for enterprise data security in 2026.

### The Enterprise Solution: RAG (Retrieval-Augmented Generation)

Large companies don't use ChatGPT via the web. They build RAG systems: an AI engine (like GPT-5.4) connected securely to the company's internal database. The model acts only as a 'language processor' that reads company files to answer employees, without training on the data or exporting it externally.

### Hands-On Exercise 6: Security Audit Simulation (20 minutes)

Form groups. Each group receives a list of 10 employee AI use cases (e.g., 'pasting customer complaint into ChatGPT,' 'uploading salary spreadsheet to Gemini'). Classify each as GREEN (safe), YELLOW (needs caution), or RED (prohibited). Present your classification to the class with justification.
