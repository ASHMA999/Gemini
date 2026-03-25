# Unit 6 Applications: Knowledge Engines & Research

> **Hands-On Practical Exercises**
> Complete these exercises using real AI-powered knowledge and research tools to build, query, and share knowledge bases that transform how your team accesses information.

---

## Guided Exercises

### Exercise 1: NotebookLM Knowledge Base

**Objective:** Build a complete knowledge base from multiple documents, test it with targeted questions, generate an Audio Overview, and share it with a partner.

**Tool:** [Google NotebookLM](https://notebooklm.google.com)

**Step-by-Step Instructions:**

1. **Prepare Your Sources**
   - Gather at least 3 documents related to a single topic (e.g., a procedure manual, a policy document, and a report).
   - Accepted formats: PDF, Google Docs, Google Slides, website URLs, copied text, YouTube videos.
   - Aim for a mix of document types to test NotebookLM's versatility.

2. **Create a New Notebook**
   - Go to [notebooklm.google.com](https://notebooklm.google.com) and sign in with your Google account.
   - Click **New Notebook**.
   - Give it a descriptive name (e.g., "Safety Procedures Knowledge Base").

3. **Upload Your Sources**
   - Click **Add Source** (the "+" icon).
   - Upload each of your 3+ documents one at a time.
   - After each upload, wait for the processing indicator to complete.
   - Verify each source appears in the Sources panel on the left.

4. **Test with 10 Questions**
   - Ask the following types of questions in the chat panel. Record NotebookLM's answer and whether it cites the correct source:

   | # | Question Type | Your Question | Answer Quality (1-5) | Correct Source Cited? |
   |---|--------------|---------------|:--------------------:|:---------------------:|
   | 1 | Factual lookup | | | |
   | 2 | Factual lookup | | | |
   | 3 | Cross-document synthesis | | | |
   | 4 | Cross-document synthesis | | | |
   | 5 | Comparison between documents | | | |
   | 6 | Procedure / how-to | | | |
   | 7 | Specific data point or number | | | |
   | 8 | "What if" scenario based on content | | | |
   | 9 | Question NOT covered in sources | | | |
   | 10 | Open-ended analysis | | | |

5. **Generate an Audio Overview**
   - In the Notebook Guide panel, click **Generate** under Audio Overview.
   - Wait for generation to complete (typically 2-5 minutes).
   - Listen to the full audio overview.
   - Rate the audio:
     - Accuracy of content: ___/5
     - Natural conversational flow: ___/5
     - Coverage of key topics: ___/5
     - Would you share this with a colleague? (Yes/No): ___

6. **Share with a Partner**
   - Click the **Share** button in the top right.
   - Add your partner's email address as a **Viewer** (or **Editor** if you want them to add sources).
   - Ask your partner to open the notebook and ask 3 questions of their own.
   - Compare: Did they find the knowledge base useful?

**Key Observations to Document:**
- Which question types did NotebookLM handle best?
- Did it ever "hallucinate" information not in the sources?
- How does the Audio Overview compare to reading the source documents directly?

### Troubleshooting
- **Source upload fails**: Check that your file is under 500,000 words per source. Split large documents if needed.
- **Answers seem vague or generic**: Your question may be too broad. Rephrase with specific terms that appear in your sources.
- **Audio Overview sounds incomplete**: It prioritizes the most prominent themes. Add a note or briefing document as a source to steer the focus.
- **Sharing doesn't work**: Ensure you are using a Google Workspace or personal Gmail account. Organizational restrictions may block external sharing.

---

### Exercise 2: Deep Research Comparison

**Objective:** Run the same research question through three different deep research tools and evaluate the quality, depth, and sourcing of each result.

**Tools:** ChatGPT Deep Research, Gemini Deep Research, Perplexity

**Step-by-Step Instructions:**

1. **Define Your Research Question**
   - Choose a question relevant to your work that requires multi-source synthesis. Examples:
     - "What are the best practices for predictive maintenance in heavy vehicle fleets?"
     - "How are military organizations implementing AI for logistics optimization?"
     - "What safety protocols should be followed when integrating cobots into manufacturing?"
   - Write your chosen question here: _______________________________________________

2. **Run on ChatGPT Deep Research**
   - Open [chatgpt.com](https://chatgpt.com) and select the Deep Research mode.
   - Paste your research question exactly as written above.
   - Wait for the full report to generate (may take 5-15 minutes).
   - Save or copy the complete response.

3. **Run on Gemini Deep Research**
   - Open [gemini.google.com](https://gemini.google.com) and select Deep Research.
   - Paste the identical question.
   - Approve the research plan when prompted (or modify if needed).
   - Wait for the full report and save it.

4. **Run on Perplexity**
   - Open [perplexity.ai](https://perplexity.ai).
   - Paste the identical question.
   - Select **Pro Search** if available.
   - Save the complete response with sources.

5. **Comparison Matrix**

   | Criterion | ChatGPT Deep Research | Gemini Deep Research | Perplexity |
   |-----------|:---------------------:|:--------------------:|:----------:|
   | Report length (approx. words) | | | |
   | Number of sources cited | | | |
   | Source quality (academic, gov, industry) | | | |
   | Depth of analysis | /5 | /5 | /5 |
   | Actionable recommendations | /5 | /5 | /5 |
   | Recency of sources | | | |
   | Factual accuracy (spot-check 3 claims) | /5 | /5 | /5 |
   | Organization and readability | /5 | /5 | /5 |
   | Time to generate | | | |
   | Overall usefulness | /5 | /5 | /5 |

6. **Verification Step**
   - Pick 3 specific claims from across the three reports.
   - Trace each claim back to its cited source. Is the source real? Does it actually say what the report claims?
   - Record findings:

   | Claim | Tool | Source Cited | Source Exists? | Claim Accurate? |
   |-------|------|-------------|:--------------:|:---------------:|
   | 1 | | | | |
   | 2 | | | | |
   | 3 | | | | |

### Troubleshooting
- **ChatGPT Deep Research is not available**: This feature requires ChatGPT Plus/Pro. Use standard ChatGPT with web browsing enabled as a fallback.
- **Gemini Deep Research plan seems off-track**: You can edit the research plan before it runs. Add specific sub-questions to guide it.
- **Perplexity results are too shallow**: Switch to Pro Search mode and add context to your question (e.g., "I need a detailed technical analysis suitable for an engineering team").
- **Sources are behind paywalls**: Note this as a limitation. Use Google Scholar or your institution's library access to verify paywalled sources.

---

### Exercise 3: Scientific Evidence Gathering

**Objective:** Use specialized research tools to gather evidence on a topic, then combine findings into an executive summary.

**Tools:** Consensus, Elicit, Perplexity

**Step-by-Step Instructions:**

1. **Choose a Research Topic**
   - Select a topic where published evidence matters. Examples:
     - "Does predictive maintenance reduce unplanned downtime?"
     - "What is the failure rate improvement from AI-based quality inspection?"
     - "How effective is VR training compared to traditional training for maintenance tasks?"
   - Your topic: _______________________________________________

2. **Consensus: Find Scientific Consensus**
   - Go to [consensus.app](https://consensus.app).
   - Enter your topic as a yes/no question (e.g., "Does predictive maintenance reduce downtime?").
   - Review the Consensus Meter (what percentage of studies agree).
   - Record the top 5 relevant papers:

   | # | Paper Title | Year | Key Finding | Agree/Disagree |
   |---|------------|------|-------------|:--------------:|
   | 1 | | | | |
   | 2 | | | | |
   | 3 | | | | |
   | 4 | | | | |
   | 5 | | | | |

3. **Elicit: Extract Structured Data**
   - Go to [elicit.com](https://elicit.com).
   - Enter the same topic.
   - Use the table view to extract: sample size, methodology, key metric, result.
   - Export or copy the structured data.

4. **Perplexity: Find Case Studies and Real-World Examples**
   - Go to [perplexity.ai](https://perplexity.ai).
   - Search: "[Your topic] real-world case studies industry examples"
   - Record 3 case studies with company name, implementation details, and results.

5. **Combine into Executive Summary**
   Write a 1-page executive summary using this structure:
   - **Question**: What we investigated
   - **Scientific Evidence**: Key findings from Consensus (X% of Y studies agree that...)
   - **Data Points**: Specific metrics from Elicit (average improvement of X%, based on N studies)
   - **Real-World Examples**: 2-3 case studies from Perplexity
   - **Recommendation**: Based on the evidence, we recommend...

### Troubleshooting
- **Consensus shows few results**: Your question may be too specific or too niche. Broaden the search terms or try synonyms.
- **Elicit returns irrelevant papers**: Use the filter options to narrow by year, methodology, or relevance score.
- **Case studies are hard to find**: Try adding industry-specific terms or company names you know are leaders in the field.

---

### Exercise 4: End-to-End Knowledge Workflow

**Objective:** Complete the full knowledge pipeline from discovery through sharing.

**Tools:** Perplexity, Google Drive, NotebookLM

**Step-by-Step Instructions:**

1. **Stage 1 -- Discover**
   - Use Perplexity to research a topic relevant to your department.
   - Save or export the 5 best sources (articles, papers, reports).

2. **Stage 2 -- Collect**
   - Download PDFs or save URLs for each source.
   - Organize them in a Google Drive folder with clear naming: `[Topic]_Source01_[ShortTitle].pdf`

3. **Stage 3 -- Build**
   - Create a new NotebookLM notebook.
   - Upload all 5 sources.
   - Write 3 "guide notes" in the notebook that summarize what the team should focus on.

4. **Stage 4 -- Query**
   - Test the notebook with 5 questions your team would actually ask.
   - Refine: If answers are weak, consider what additional sources would strengthen the knowledge base.

5. **Stage 5 -- Audio**
   - Generate an Audio Overview.
   - Listen and evaluate: Would this be useful as a briefing for someone joining the team?

6. **Stage 6 -- Share**
   - Share the notebook with at least one colleague.
   - Collect their feedback: What was useful? What was missing?

**Pipeline Tracker:**

| Stage | Status | Time Spent | Notes |
|-------|:------:|:----------:|-------|
| Discover | | | |
| Collect | | | |
| Build | | | |
| Query | | | |
| Audio | | | |
| Share | | | |

### Troubleshooting
- **Pipeline feels slow at the Collect stage**: Batch your downloads. Use Perplexity's "Copy" feature to quickly grab source URLs.
- **NotebookLM answers don't match expectations**: The quality of answers is directly proportional to the quality of sources. Replace weak sources with better ones.
- **Audio Overview misses key points**: Add a summary document as a source that explicitly states the most important points you want covered.

---

### Exercise 5: Department Knowledge Base Design

**Objective:** Plan (not just build) a comprehensive NotebookLM knowledge base tailored to your department's needs.

**Step-by-Step Instructions:**

1. **Identify the Knowledge Gap**
   - What questions do new team members ask repeatedly?
   - What information is currently scattered across emails, shared drives, and people's heads?
   - List the top 10 questions your department knowledge base should answer:

   | # | Question | Where is the answer currently? | Difficulty to find (1-5) |
   |---|----------|-------------------------------|:------------------------:|
   | 1 | | | |
   | 2 | | | |
   | 3 | | | |
   | 4 | | | |
   | 5 | | | |
   | 6 | | | |
   | 7 | | | |
   | 8 | | | |
   | 9 | | | |
   | 10 | | | |

2. **Source Inventory**
   - List all documents you would upload:

   | Document Name | Type | Pages/Size | Priority (Must/Should/Could) |
   |--------------|------|:----------:|:----------------------------:|
   | | | | |
   | | | | |
   | | | | |
   | | | | |
   | | | | |

3. **Access Plan**
   - Who should have access? (Names or roles)
   - What permission level? (Viewer vs. Editor)
   - Are there any documents with restricted classification that should NOT be uploaded?

4. **Maintenance Plan**
   - How often will sources be updated?
   - Who is responsible for adding new documents?
   - How will you know if the knowledge base is being used and is useful?

### Troubleshooting
- **Too many potential documents**: Prioritize by frequency of use. Start with the 5 most-referenced documents and expand later.
- **Sensitive documents**: Never upload classified or restricted documents to cloud-based tools. Create a separate plan for handling sensitive information.
- **Team resistance**: Start with one high-value use case that saves obvious time. Success breeds adoption.

---

## Independent Practice

### Practice 1: Build a Department NotebookLM Notebook

1. Using your design from Exercise 5, create an actual NotebookLM notebook with your department documents (use only documents cleared for cloud upload).
2. Upload at least 3 real department documents.
3. Test with 10 questions that reflect real daily needs.
4. Record results:

   | Question | Answer Quality (1-5) | Source Cited Correctly? | Would You Trust This Answer? |
   |----------|:--------------------:|:----------------------:|:----------------------------:|
   | | | | |
   | | | | |
   | | | | |
   | | | | |
   | | | | |

5. Generate the Audio Overview and evaluate whether it could replace a verbal briefing.

### Practice 2: Deep Research on a Work-Relevant Topic

1. Choose a topic directly relevant to your current work or an upcoming project.
2. Run the query on the deep research tool of your choice (based on Exercise 2 findings).
3. Produce a 1-page summary with:
   - 3 key findings
   - 2 actionable recommendations
   - 1 area that needs further investigation
4. Share with your supervisor and record their feedback.

---

## Real-World Challenge

### Create a Sharable Team Knowledge Base

**Goal:** Create a knowledge base that your team can start using tomorrow.

**Requirements:**
- Minimum 5 relevant source documents
- Tested with at least 15 realistic questions
- Audio Overview generated and reviewed
- Shared with at least 2 team members
- Feedback collected from each team member

**Deliverables:**

1. **The Notebook** (shared link)
2. **Test Report** documenting the 15 questions, answers, and quality ratings
3. **Feedback Summary** from team members:
   - What worked well?
   - What was missing or incorrect?
   - Would they use this regularly?
4. **Improvement Plan** -- 3 specific changes you would make based on feedback

**Success Criteria:**
- At least 80% of questions answered satisfactorily (4 or 5 out of 5)
- At least 1 team member says they would use it regularly
- Audio Overview is rated 3/5 or higher by reviewers

---

## Extension Task

### Design a Department Knowledge Ecosystem

**Using the 6-stage framework (Discover, Collect, Build, Query, Audio, Share), design a complete knowledge ecosystem for your department.**

**Deliverable:** A 2-page proposal or a presentation (5-8 slides) covering:

1. **Current State Assessment**
   - How does knowledge currently flow in your department?
   - What are the biggest bottlenecks? (Person-dependent knowledge, outdated documents, scattered storage)

2. **Proposed Ecosystem Architecture**
   - Map out which tools handle which stages:
     - Discover: Which research tools? How often?
     - Collect: Where are sources stored? What format?
     - Build: How many NotebookLM notebooks? Organized by what?
     - Query: Who has access? What types of questions?
     - Audio: Which topics get Audio Overviews? For whom?
     - Share: Distribution channels, access controls, update schedules

3. **Implementation Roadmap**
   - Phase 1 (Week 1-2): Quick wins -- what can you set up immediately?
   - Phase 2 (Month 1): Core notebooks covering top 3 knowledge areas.
   - Phase 3 (Month 2-3): Full ecosystem with maintenance processes.

4. **Success Metrics**
   - How will you measure adoption?
   - How will you measure time saved?
   - How will you measure answer quality over time?

5. **Risk Mitigation**
   - Data security considerations
   - What happens if a tool becomes unavailable?
   - How to handle knowledge that cannot be uploaded to cloud tools
