---
marp: true
theme: default
paginate: true
header: "Unit 1: The Physics of AI | APC AI Excellence Program"
footer: "Arab Potash Company | 2026"
---

# The Physics of AI
## Infrastructure, Core Concepts & Enterprise Risks

**Applied AI Training Program**
Arab Potash Company | AI Excellence Program

---

# Learning Objectives

By the end of this unit, you will be able to:

1. Explain how tokens, context windows, and temperature work
2. Identify and prevent AI hallucinations
3. Compare major AI models and their strengths
4. Classify enterprise AI security risks
5. Understand why free AI accounts are dangerous for work

---

# 1.1 Tokens: The Currency of AI

## A Token is NOT a Word

| Input | Tokens |
|-------|--------|
| "Apple" | 1 token |
| "Playing" | "Play" + "ing" = 2 tokens |
| A space character | 1 token |

## The Golden Rule

**1,000 tokens = ~750 English words**

Arabic text = ~2x more tokens for the same meaning ("Linguistic Tax")

---

# Why Tokens Matter

| Factor | Impact |
|--------|--------|
| **Cost** | Providers charge per million tokens (input + output) |
| **Capacity** | Model memory is limited by token count |
| **Performance** | More tokens = longer processing time |

### Exercise 1: Token Explorer (15 min)
Open **platform.openai.com/tokenizer**
- Type: "Arab Potash Company produces potassium chloride"
- Type the same in Arabic
- Calculate the linguistic tax percentage

---

# 1.2 Context Window: The Working Memory

Think of it as **RAM for AI**

| Size | Analogy | Best For |
|------|---------|----------|
| Small (8K-32K) | Sticky note | Quick chats, simple Q&A |
| Medium (32K-128K) | Notebook | Document analysis |
| Large (128K-1M+) | Entire library | Codebases, books, years of records |

---

# Lost in the Middle

AI has **reduced accuracy** for information in the **MIDDLE** of long text

### The Fix:
Place critical instructions at the **TOP** and **BOTTOM** of your prompt

### Exercise 2: Context Window Stress Test (20 min)
Paste a 3-page document into Google AI Studio. Ask questions about page 1, 2, and 3. Which answers are most accurate?

---

# 1.3 Temperature: The Precision-Creativity Dial

| Temperature | Behavior | Use For |
|------------|----------|---------|
| **0.0 - 0.2** | Precise, deterministic | Coding, data extraction, legal |
| **0.5** | Balanced | Emails, summaries |
| **0.8 - 1.0** | Creative, diverse | Brainstorming, ad copy |

### Exercise 3: Temperature Lab (15 min)
Prompt: "Suggest 5 names for a new potash fertilizer product"
- Run 3 times at Temperature 0.0
- Run 3 times at Temperature 1.0
- Document the differences

---

# 1.4 Hallucinations: When AI Dreams

> A hallucination = AI generates confident, logical-sounding information that is **completely fabricated**

## Why It Happens

LLMs predict the **most probable next word**, NOT the **truthful next word**

They perform **Pattern Completion**, not **Fact Retrieval**

---

# Three Hallucination Disasters

| Case | What Happened | Lesson |
|------|--------------|--------|
| **Samsung (2023)** | Engineers pasted secret code into ChatGPT. Data leaked. | Never paste secrets into free AI |
| **Mata v. Avianca (2023)** | Lawyer cited fake cases from ChatGPT in court. Fined. | Always verify. Human in the Loop. |
| **Air Canada (2024)** | Chatbot gave false refund policy. Company liable. | You ARE responsible for AI outputs |

### Exercise 4: Hallucination Detection (20 min)
Ask ChatGPT for "top 3 papers on potash mining safety in 2024." Verify on Google Scholar. How many are real?

---

# 1.5 The AI Landscape 2026

| Provider | Specialization | Key Strength |
|---------|---------------|-------------|
| **OpenAI (GPT-5.4)** | Deep reasoning | Thinking traces, agentic workflows |
| **Anthropic (Claude 4.6)** | Coding & safety | 1M-token context window |
| **Google (Gemini 3.1)** | Multimodal | Text + image + video reasoning |
| **DeepSeek (V3)** | Cost efficiency | Best cost-to-performance ratio |
| **xAI (Grok)** | Real-time data | Live X/Twitter integration |

### Exercise 5: Model Comparison (25 min)
Same prompt to 3 models. Compare structure, creativity, and limitations cited.

---

# 1.6 Data Privacy & Enterprise Security

| | Free Account | Enterprise Account |
|---|-------------|-------------------|
| **Training** | Your data trains the model | Contractually prohibited |
| **Retention** | 30+ day logs | Zero retention |
| **Ownership** | Ambiguous | Full company ownership |
| **Security** | Standard | SOC2, HIPAA, GDPR |

---

# The Critical Message

> **Using free AI accounts for work = Voluntarily leaking trade secrets**

**Shadow AI** = Employees using unauthorized AI tools
= **#1 emerging enterprise risk in 2026**

### The Solution: RAG
Retrieval-Augmented Generation = AI engine connected securely to YOUR data. No training. No export.

### Exercise 6: Security Audit Simulation (20 min)
Classify 10 AI use cases as GREEN / YELLOW / RED

---

# Unit 1 Recap

1. **Tokens** = AI currency. Arabic costs 2x more.
2. **Context Window** = AI's RAM. Put important info at top/bottom.
3. **Temperature** = Creativity dial. Low for precision, high for ideas.
4. **Hallucinations** = AI invents facts confidently. Always verify.
5. **2026 Landscape** = Each model has strengths. Choose wisely.
6. **Security** = Free accounts are dangerous. Use enterprise solutions.

### Key Takeaway:
> **AI is a powerful tool, not a trustworthy source. Human judgment is non-negotiable.**
