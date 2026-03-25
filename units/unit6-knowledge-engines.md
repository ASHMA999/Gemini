# Unit 6: Specialized AI Tools & Knowledge Engines

## NotebookLM, Deep Research, Scientific Research AI & Industrial Knowledge Bases

| Detail | Description |
|--------|-------------|
| **Duration** | 4 hours (including breaks) |
| **Delivery** | Live demos + hands-on with real documents and research queries |
| **Tools Required** | NotebookLM (notebooklm.google.com), Perplexity (perplexity.ai), Consensus (consensus.app), Elicit (elicit.com), ChatGPT Deep Research, Google Gemini Deep Research |
| **Objective** | Master AI-powered knowledge management, scientific research, and build always-available expert systems from your own documents |

---

## 6.1 Google NotebookLM: Your Personal AI Research Assistant

NotebookLM is fundamentally different from ChatGPT or Copilot. Instead of drawing from the entire internet, it ONLY answers from sources YOU upload.

| Feature | ChatGPT / Claude / Gemini | NotebookLM |
|---------|--------------------------|------------|
| Knowledge Source | Entire internet (training data) | ONLY your uploaded documents |
| Hallucination Risk | Medium to High | Very Low (grounded in your sources) |
| Citation | Sometimes vague or fabricated | Always cites exact source and page number |
| Max Sources | Limited by context window | Up to 50 sources, 500K words each |
| Audio Overview | Not available | Generates AI podcast from your documents |
| Sharing | Cannot share grounded knowledge | Share notebook link with team members |
| Cost | Varies by subscription | Free (with Google account) |

### What Can You Upload to NotebookLM?

- PDF documents (manuals, reports, research papers, policies)
- Google Docs and Google Slides
- Web URLs (articles, documentation pages)
- Copied text (paste directly)
- YouTube videos (extracts transcript automatically)
- Audio files (transcribes and indexes them)

### Core Capabilities

- **Ask Questions:** Chat with your documents with exact source citations
- **Auto-Summary:** Generates document guide, FAQ, study guide, or briefing document
- **Audio Overview (AI Podcast):** Converts documents into a 10-15 minute podcast discussion
- **Cross-Source Analysis:** 'What are the contradictions between these documents?'
- **Interactive Notes:** Save key insights, organize them, ask follow-up questions

---

## 6.2 Industrial Use Case: Equipment Maintenance Knowledge Base

### The Vision: Always-Available Maintenance Expert

Instead of a technician searching through a 300-page pump manual, they open NotebookLM on their phone and ask: 'What is the torque spec for the main bearing bolts on the P-301 pump?' - instant answer with exact page reference.

### Step-by-Step: Building an Equipment Knowledge Base

1. **Collect Manuals:** Gather PDF manuals for critical equipment (start with 10 most frequently serviced)
2. **Upload to NotebookLM:** Create a notebook called 'APC Maintenance Library'
3. **Test Questions:** Ask common technician questions
4. **Generate Quick Reference Guides:** 'Create a 1-page quick reference card for the daily inspection checklist of pump P-301'
5. **Generate Audio Briefing:** Create a podcast-style briefing on 'Top 10 maintenance mistakes to avoid'
6. **Share with Team:** Share the notebook link with all maintenance technicians

### Practical Prompts for the Maintenance Knowledge Base

**Troubleshooting Assistant:**
> 'The pump P-301 is showing high vibration readings (above 7mm/s). Based on the uploaded manual, what are the possible causes, diagnostic steps, and corrective actions? List in order of probability.'

**Spare Parts Finder:**
> 'I need to replace the mechanical seal on pump P-301. From the manual, what is the exact part number, compatible alternatives, and installation procedure? Include special tools required.'

**Training Content Generator:**
> 'Based on all uploaded manuals, create a training quiz with 15 multiple-choice questions about safety procedures for new maintenance technicians.'

**Cross-Manual Comparison:**
> 'Compare the lubrication schedules across all uploaded equipment manuals. Create a master lubrication calendar. Highlight any conflicts or inconsistencies.'

### Beyond Maintenance: Other Applications

| Department | What to Upload | What to Ask |
|-----------|---------------|-------------|
| Safety/HSE | Safety procedures, incident reports, OSHA standards | 'What PPE is required for working with concentrated acid in Building C?' |
| HR | Employee handbook, policies, labor law documents | 'What is our policy on overtime during Ramadan? Cite the exact clause.' |
| Production | SOPs, process flow diagrams, quality standards | 'What are the acceptable ranges for pH levels in the crystallization process?' |
| Legal | Regulatory documents, permits, environmental standards | 'What are our reporting obligations under the Energy & Minerals Regulatory Commission?' |
| Training | Training manuals, course materials, assessment guides | Generate a podcast overview of the safety induction program |

### Hands-On Exercise 24: NotebookLM Knowledge Base Builder (35 minutes)

**Part A - Build (15 min):** (1) Create a new notebook. (2) Upload 2-3 PDF documents. (3) Read the auto-generated summary. (4) Ask 5 different questions and verify citations.

**Part B - Audio (10 min):** (5) Generate Audio Overview. (6) Evaluate accuracy and training usefulness.

**Part C - Industrial (10 min):** (7) Create a 1-page quick reference checklist. (8) Find the 5 most critical safety warnings. (9) Share the notebook link.

---

## 6.3 Deep Research Tools

| Tool | Provider | How It Works | Best For | Access |
|------|---------|-------------|---------|--------|
| Deep Research | ChatGPT (OpenAI) | Browses web 5-30 min, reads dozens of pages | Market research, competitive analysis | ChatGPT Plus/Pro |
| Deep Research | Google Gemini | Google Search at scale, multi-section reports | Academic research, regulatory compliance | Gemini Advanced |
| Perplexity Pro Search | Perplexity AI | Real-time web search with AI synthesis | Quick fact-finding, technical docs | Free / Pro |

### When to Use Deep Research vs. Regular Chat

| Scenario | Regular AI Chat | Deep Research |
|---------|----------------|---------------|
| Quick concept question | Perfect fit | Overkill |
| Latest ISO standard for potash quality | May hallucinate | Finds actual standard with sources |
| Compare 5 CMMS vendors | Generic list | Current pricing, reviews, features |
| New mining regulations in Jordan 2026 | Doesn't know | Searches government sites |
| Literature review on predictive maintenance | Superficial | Reads 20+ papers, structured review |

### Practical Deep Research Prompts for APC

**Vendor Evaluation (ChatGPT):**
> 'Research the top 5 CMMS platforms in 2026. For each: pricing tiers, mining features, Arabic support, mobile app, user reviews. Comparison table with recommendation for potash mining with 500+ assets.'

**Regulatory Research (Gemini):**
> 'Research all environmental and safety regulations issued by Jordan's Energy and Minerals Regulatory Commission in the last 2 years affecting potash mining. Include: name, date, requirements, deadlines, penalties.'

**Technology Scout (Perplexity):**
> 'Latest IoT sensor technologies for predictive maintenance in mining (2026). Focus on vibration monitoring, thermal imaging, oil analysis. Include product names, manufacturers, costs.'

### Hands-On Exercise 25: Deep Research Showdown (30 minutes)

Pick a research question for your department. Run the SAME question on all 3 platforms. Compare: comprehensiveness, citations, speed, trustworthiness.

---

## 6.4 Scientific Research AI Tools

### Consensus (consensus.app)

AI-powered academic search engine using real peer-reviewed papers with a 'consensus meter.'

### Elicit (elicit.com)

Research assistant that finds papers, extracts specific data points, and builds evidence tables.

### Scholar AI (ChatGPT Plugin)

Searches academic databases (Semantic Scholar, arXiv, PubMed) with proper citations.

| Tool | Best For | Citation Quality | Full Paper Access | Cost |
|------|---------|-----------------|------------------|------|
| Consensus | Evidence-based answers | Excellent (real papers) | Abstracts + links | Free / Premium |
| Elicit | Data extraction | Excellent (real papers) | Abstracts + extraction | Free / Plus |
| Scholar AI | Quick literature search | Good (real databases) | Can read uploaded PDFs | ChatGPT Plus |
| Perplexity | Web + academic hybrid | Good (live sources) | Links to sources | Free / Pro |

### Hands-On Exercise 26: Scientific Research Challenge (30 minutes)

Build a business case for predictive maintenance IoT sensors: (1) Consensus: search for cost evidence. (2) Elicit: extract ROI data from 5 papers. (3) Perplexity: find real-world case studies. (4) Combine into a 1-page executive summary for APC's CFO.

---

## 6.5 Building an AI-Powered Knowledge Ecosystem

| Stage | Task | Best Tool | Output |
|-------|------|-----------|--------|
| 1. Discover | Find latest research | Perplexity + Consensus | Curated source list |
| 2. Analyze | Read, compare, extract | Elicit + NotebookLM | Evidence tables |
| 3. Synthesize | Generate reports | ChatGPT / Claude + NotebookLM | Executive summaries |
| 4. Distribute | Share with teams | NotebookLM (shared + audio) | Knowledge bases, podcasts |
| 5. Apply | Answer daily questions | NotebookLM (grounded Q&A) | Instant cited answers |
| 6. Maintain | Keep updated | NotebookLM + scheduled Deep Research | Living knowledge base |

### Hands-On Exercise 27: End-to-End Knowledge Workflow (30 minutes)

(1) DISCOVER with Perplexity. (2) COLLECT PDFs/URLs. (3) BUILD NotebookLM notebook. (4) QUERY with specific questions. (5) Generate AUDIO overview. (6) SHARE with a partner.

---

## 6.6 Quick Reference: Tool Selection Guide

| I Need To... | Use This Tool | Why |
|-------------|---------------|-----|
| Answer questions from MY documents only | NotebookLM | Zero hallucination, grounded |
| Find peer-reviewed academic evidence | Consensus | Real papers with consensus meter |
| Extract data from multiple papers | Elicit | Automated extraction tables |
| Get a comprehensive research report | ChatGPT / Gemini Deep Research | Autonomous multi-source research |
| Quick fact-check with real-time sources | Perplexity | Fastest search-and-synthesize |
| Create a shareable team knowledge base | NotebookLM (shared) | Upload, share, team chats |
| Turn documents into audio | NotebookLM Audio Overview | AI podcast from any documents |
| Research latest regulations or market data | Perplexity + Deep Research | Live web access |
