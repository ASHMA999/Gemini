# Unit 2 Activities: Applied Prompt Engineering

---

## Activity 1: Ice Breaker -- "Prompt Roulette"

**Duration:** 10 minutes
**Group Size:** Any
**Materials:** Word grid (below), timer, AI tool access (optional)

### Word Grid

Participants roll two dice (or use a random number generator) to select one word from each column. They must then craft a prompt using both words.

| Roll | Column A (Subject) | Column B (Constraint) |
|------|--------------------|-----------------------|
| 1 | Company budget | As a pirate |
| 2 | Employee handbook | In exactly 3 sentences |
| 3 | Product launch | Using only questions |
| 4 | Safety procedure | For a 5-year-old |
| 5 | Customer complaint | As a haiku |
| 6 | Meeting agenda | In reverse chronological order |
| 7 | Performance review | Using a cooking metaphor |
| 8 | Supply chain | As a news headline |
| 9 | Training manual | With no adjectives |
| 10 | Quarterly report | As a bedtime story |

### Rules

1. Each participant (or pair) rolls twice to get their Subject + Constraint combination.
2. They have **90 seconds** to write a prompt that asks AI to produce content about the Subject in the style of the Constraint.
3. Volunteers read their prompts aloud.
4. The group votes on: Most Creative, Most Likely to Actually Work, and Most Hilarious.

**Example:**
- Roll: 5 (Customer complaint) + 7 (Using a cooking metaphor)
- Prompt: "You are a master chef reviewing a dish that went wrong. Rewrite this customer complaint as if you're diagnosing what went wrong in the kitchen, using cooking terminology throughout."

**Facilitator Tips:**
- If time is tight, do this in pairs rather than individually.
- Encourage absurd combinations -- they demonstrate that prompt structure matters even with silly content.
- Use this to introduce the concept: "Notice how adding constraints actually made your prompts MORE specific and useful? That's prompt engineering."

**Debrief Questions:**
1. Which constraint forced you to think the hardest about your prompt?
2. Did the constraint actually improve the output quality? Why?
3. How might constraints help in real work prompts?

---

## Activity 2: Energizer -- "Framework Flash Cards"

**Duration:** 10 minutes
**Group Size:** Pairs
**Materials:** 12 scenario cards (below), timer

### The 12 Scenario Cards

Each card describes a workplace situation. Pairs must identify which prompt engineering framework (RTF, TAG, RISEN, or other structured approach) would be most appropriate, then draft a 2-sentence prompt starter.

**Card 1: The Urgent Email**
"Your VP needs a response to a client complaint about delayed shipping within 30 minutes."
- Best framework: **RTF (Role, Task, Format)**
- Why: Quick, straightforward task with clear output needs.

**Card 2: The Strategy Document**
"The CEO wants a 10-page competitive analysis for the board meeting next month."
- Best framework: **RISEN (Role, Instructions, Steps, End goal, Narrowing)**
- Why: Complex, multi-step deliverable requiring detailed guidance.

**Card 3: The Data Summary**
"Turn last quarter's sales spreadsheet into 5 bullet points for the team standup."
- Best framework: **TAG (Task, Action, Goal)**
- Why: Simple transformation with a clear input and output.

**Card 4: The Training Script**
"Create a workshop script for teaching new hires about workplace safety procedures."
- Best framework: **RISEN**
- Why: Requires structured steps, specific audience, and detailed output.

**Card 5: The Social Media Post**
"Draft an announcement about our new product for LinkedIn."
- Best framework: **RTF**
- Why: Clear role (social media writer), task (announcement), format (LinkedIn post).

**Card 6: The Troubleshooting Guide**
"An engineer needs a decision tree for diagnosing equipment failures."
- Best framework: **RISEN**
- Why: Multi-step logic, precise narrowing needed for technical accuracy.

**Card 7: The Meeting Notes**
"Summarize a 60-minute recorded meeting into action items."
- Best framework: **TAG**
- Why: Clear task, clear action, clear goal.

**Card 8: The Policy Draft**
"HR needs a first draft of a new remote work policy covering eligibility, equipment, and expectations."
- Best framework: **RISEN**
- Why: Multiple sections, needs narrowing constraints, structured end goal.

**Card 9: The Customer FAQ**
"Create a FAQ section for the website about our return policy."
- Best framework: **RTF**
- Why: Defined role (customer service writer), clear task, specific format (Q&A).

**Card 10: The Code Review**
"Review this Python script and suggest optimizations for performance."
- Best framework: **TAG**
- Why: Input is clear, action is specific, goal is defined.

**Card 11: The Presentation Outline**
"Build a 20-slide presentation about digital transformation for the leadership retreat."
- Best framework: **RISEN**
- Why: Complex deliverable needing step-by-step structure and audience narrowing.

**Card 12: The Quick Translation**
"Translate this product description into professional Spanish for our Mexico office."
- Best framework: **RTF**
- Why: Simple role-task-format situation with minimal ambiguity.

### How to Play

1. Shuffle and deal 6 cards per pair.
2. Set a timer: 60 seconds per card.
3. Each person in the pair takes turns: one reads the card, the other names the framework and gives a reason.
4. Switch roles for the next card.
5. After all cards are done, pairs compare notes and discuss disagreements.

**Facilitator Tips:**
- Emphasize that there's no single "right" answer -- the goal is to reason about WHY a framework fits.
- If pairs finish early, have them actually draft the prompt starter for their favorite card.
- Walk around and listen for good reasoning to share with the whole group.

**Debrief Questions:**
1. Were there any cards where you and your partner disagreed? What was the reasoning?
2. Which framework felt most natural to you?
3. When might you combine frameworks?

---

## Activity 3: Understanding Check -- "Framework Match Game"

**Duration:** 12 minutes
**Group Size:** Teams of 3--4
**Materials:** Card sets (below), answer key, scoring sheet

### Card Set A: Framework Components (cut into individual cards)

| Card | Text |
|------|------|
| A1 | "You are a senior financial analyst..." |
| A2 | "Generate a 500-word summary..." |
| A3 | "Format the output as a bullet-point list..." |
| A4 | "Step 1: Review the data. Step 2: Identify trends. Step 3: Draft conclusions." |
| A5 | "The audience is non-technical executives..." |
| A6 | "Do NOT include any technical jargon..." |
| A7 | "The goal is to persuade the board to approve the budget..." |
| A8 | "First analyze the problem, then propose 3 solutions, finally recommend one..." |
| A9 | "Write in a professional but approachable tone..." |
| A10 | "Limit the response to information from Q4 2025 only..." |

### Card Set B: Framework Labels (cut into individual cards)

| Card | Text |
|------|------|
| B1 | Role (RTF) |
| B2 | Task (RTF / TAG) |
| B3 | Format (RTF) |
| B4 | Steps (RISEN) |
| B5 | Audience / Narrowing (RISEN) |
| B6 | Constraint / Narrowing (RISEN) |
| B7 | Goal (TAG) |
| B8 | Instructions (RISEN) |
| B9 | Tone (General best practice) |
| B10 | Scope / Narrowing (RISEN) |

### Answer Key

| Set A Card | Matches Set B Card | Explanation |
|------------|-------------------|-------------|
| A1 | B1 (Role) | Assigns a persona to the AI |
| A2 | B2 (Task) | Defines what needs to be produced |
| A3 | B3 (Format) | Specifies output structure |
| A4 | B4 (Steps) | Sequential instructions |
| A5 | B5 (Audience/Narrowing) | Defines who will consume the output |
| A6 | B6 (Constraint/Narrowing) | Exclusion constraint |
| A7 | B7 (Goal) | End-state objective |
| A8 | B8 (Instructions) | Detailed process guidance |
| A9 | B9 (Tone) | Style directive |
| A10 | B10 (Scope/Narrowing) | Limits data range |

### How to Play

1. Lay Card Set A face-up on the left, Card Set B face-up on the right.
2. Teams match each A card with the correct B card.
3. Teams have 5 minutes to complete all matches.
4. Facilitator reveals answers. Each correct match = 1 point.
5. Bonus point: For each correct match, the team explains WHY in one sentence.

**Scoring:**
- 10/10 matches: "Prompt Engineering Pros"
- 7--9 matches: "Strong Foundation"
- 4--6 matches: "Framework Fundamentals Needed"
- Below 4: "Let's Walk Through These Together"

**Facilitator Tips:**
- Print cards on different colored paper for easy sorting.
- If time allows, have the winning team assemble all 10 components into a single mega-prompt and read it aloud.
- Common mistake: confusing "Steps" (B4) with "Instructions" (B8). Clarify that steps are sequential, while instructions are overarching guidance.

---

## Activity 4: Prompt Writing Competition

**Duration:** 20 minutes
**Group Size:** Teams of 2--3
**Materials:** AI tool access, scoring rubric, timer

### Rules

1. All teams receive the **same business scenario** (choose one below or create your own).
2. Teams have **10 minutes** to write the best possible prompt.
3. All prompts are submitted simultaneously (no peeking).
4. Each prompt is run through the AI tool live on the projector.
5. The group scores each output using the rubric below.

### Scoring Criteria (out of 25 points)

| Criterion | Points | Description |
|-----------|--------|-------------|
| Clarity | 5 | Is the prompt unambiguous? Could anyone understand the intent? |
| Framework Usage | 5 | Does it employ a recognized framework (RTF, TAG, RISEN)? |
| Specificity | 5 | Does it include constraints, scope, format, and audience? |
| Output Quality | 5 | How good is the actual AI-generated output? |
| Efficiency | 5 | Does the prompt achieve results without unnecessary verbosity? |

### Sample Scenarios

**Scenario A: The Incident Report**
"Your manufacturing plant had a minor safety incident yesterday -- a forklift tipped over in Warehouse B. No injuries, but some inventory was damaged. Write a prompt that gets AI to help you draft the incident report for both internal leadership and the safety regulator."

**Scenario B: The Competitive Analysis**
"Your company is launching a new product in 6 months. You need to understand the competitive landscape. Write a prompt that gets AI to create a structured competitive analysis framework you can fill in with real data."

**Scenario C: The Onboarding Guide**
"You've been asked to create a first-week onboarding guide for new hires in your department. It should cover tools, key contacts, first assignments, and cultural norms. Write a prompt to generate a draft."

### Sample Winning Prompts (for facilitator reference)

**Strong prompt for Scenario A:**
"You are a senior safety compliance officer at a manufacturing company. An incident occurred yesterday in Warehouse B: a forklift tipped over during routine operations. There were no injuries, but approximately $5,000 in inventory was damaged. Draft two versions of an incident report: (1) A concise executive summary for internal leadership (max 300 words, focus on root cause and corrective actions), and (2) A detailed regulatory report following OSHA Form 301 structure. Use professional, factual language. Do not speculate on causes -- use phrases like 'under investigation' where root cause is unconfirmed. Include sections for: incident description, immediate response taken, preliminary root cause analysis, corrective actions planned, and timeline for resolution."

**Facilitator Tips:**
- Run all prompts through the same AI model and settings for fairness.
- Let teams watch each other's outputs -- seeing different approaches to the same problem is the real learning.
- Highlight the difference between vague and specific prompts in the output quality.
- If a "simple" prompt produces great output, discuss why (sometimes less is more, depending on the task).

**Debrief Questions:**
1. What made the winning prompt effective?
2. Were you surprised by any outputs -- either good or bad?
3. How would you revise your prompt if you could try again?

---

## Activity 5: "Bad Prompt Museum"

**Duration:** 15 minutes
**Group Size:** Pairs, then full group
**Materials:** 10 bad prompts (below), analysis worksheet

### Collection of 10 Terrible Prompts

Each prompt has deliberate flaws. Participants identify what's wrong and rewrite a better version.

---

**Bad Prompt #1: "The Vague Wanderer"**
> "Tell me about marketing."

**What's Wrong:**
- No specific topic, audience, or format
- No context about what aspect of marketing
- No constraints on length or depth
- Produces a generic, useless overview

**Better Version:** "Summarize 5 key digital marketing trends for B2B manufacturing companies in 2026. For each trend, include one actionable recommendation. Format as a numbered list with bold trend names."

---

**Bad Prompt #2: "The Kitchen Sink"**
> "I need you to write a comprehensive, detailed, thorough, and exhaustive analysis of every single aspect of our company's digital transformation journey including all departments, all tools, all processes, all challenges, all opportunities, all risks, all metrics, all stakeholders, and all timelines, and make sure it's really good and covers everything."

**What's Wrong:**
- Tries to do everything at once
- No prioritization or focus
- Repetitive modifiers ("comprehensive, detailed, thorough, exhaustive")
- Impossible scope for a single prompt
- "Make sure it's really good" is not actionable guidance

**Better Version:** "Create an executive summary of our digital transformation progress. Focus on: (1) Top 3 departments furthest along, (2) Top 3 challenges slowing adoption, (3) Recommended next steps for Q2. Keep it under 500 words."

---

**Bad Prompt #3: "The Assumption Bomb"**
> "Fix the report."

**What's Wrong:**
- Assumes AI knows which report
- No indication of what's wrong with it
- No criteria for "fixed"
- No context provided whatsoever

**Better Version:** "Review the attached quarterly sales report. Check for: (1) mathematical errors in the revenue totals, (2) inconsistencies between the chart data and the written analysis, (3) grammar and formatting issues. List each issue found with the specific location and suggested correction."

---

**Bad Prompt #4: "The Double Negative Maze"**
> "Don't not include things that aren't unrelated to the topic but also don't exclude anything that shouldn't be left out unless it's not necessary to not have."

**What's Wrong:**
- Incomprehensible double/triple negatives
- AI cannot parse the actual intent
- Even humans can't figure out what this means
- Violates the principle of clarity

**Better Version:** "Include only information directly related to the topic. If a piece of information is borderline relevant, include it with a note explaining its potential connection."

---

**Bad Prompt #5: "The Tone-Deaf Request"**
> "Write a funny email to tell employees they're being laid off."

**What's Wrong:**
- Wildly inappropriate tone for the subject matter
- No prompt framework can fix a bad judgment call
- Ethical red flag -- AI should not be used to trivialize serious human situations
- Demonstrates the importance of human oversight in AI use

**Better Version:** "Draft a compassionate, professional email from the CEO to affected employees informing them about upcoming workforce reductions. Include: expressions of gratitude for their contributions, details about severance packages and support resources, and a clear timeline. Tone should be empathetic and direct."

---

**Bad Prompt #6: "The Infinite Loop"**
> "Generate a list of all possible ways to improve our business."

**What's Wrong:**
- "All possible ways" is infinite
- No focus area, department, or constraint
- No prioritization criteria
- Will generate generic, unhelpful suggestions

**Better Version:** "List 10 high-impact, low-cost process improvements for our customer service department. Rank them by estimated time savings. Focus on changes implementable within 30 days without new software purchases."

---

**Bad Prompt #7: "The Format Forgetter"**
> "Analyze our competitors and give me the results."

**What's Wrong:**
- No specified output format
- "Give me the results" is ambiguous -- a paragraph? A table? A presentation?
- No criteria for analysis
- No indication of which competitors

**Better Version:** "Create a comparison table of our top 3 competitors (Acme Corp, Beta Inc, Gamma Ltd) across these dimensions: pricing model, market share, key product features, customer satisfaction ratings, and recent strategic moves. Include a final row with our company's data for direct comparison."

---

**Bad Prompt #8: "The Confidential Leaker"**
> "Here's our entire customer database with names, emails, phone numbers, and purchase history. Analyze the buying patterns."

**What's Wrong:**
- Shares sensitive PII (personally identifiable information) with AI
- Potential data privacy and compliance violation (GDPR, CCPA)
- No consideration of data governance
- The analysis request is fine; the data handling is the problem

**Better Version:** "I have customer purchase data (anonymized -- customer IDs only, no names or contact info). The dataset includes: customer ID, product category, purchase amount, purchase date, and region. Analyze buying patterns and identify: top 3 product categories by revenue, seasonal trends, and customer segments by purchase frequency."

---

**Bad Prompt #9: "The Copy-Paste Pray"**
> [Pastes 47 pages of raw text] "Summarize this."

**What's Wrong:**
- May exceed context window
- No guidance on what aspects to summarize
- No desired length or format
- No indication of audience or purpose
- "Summarize" can mean 100 different things

**Better Version:** "Summarize the following document (a regulatory compliance report) into a 1-page executive brief for the legal team. Focus on: (1) key compliance gaps identified, (2) recommended actions with deadlines, (3) financial exposure estimates. Use bullet points under each section. [Then paste the document, or relevant sections]"

---

**Bad Prompt #10: "The Contradictory Commander"**
> "Write a detailed 2,000-word report. Keep it brief. Include everything. Be concise. Use lots of examples. Don't make it too long."

**What's Wrong:**
- Self-contradictory instructions throughout
- "Detailed" vs. "brief" vs. "concise" vs. "2,000 words"
- "Include everything" vs. "Don't make it too long"
- AI will try to satisfy all constraints and fail at most of them

**Better Version:** "Write a 2,000-word report on the topic. Structure it with an executive summary (200 words), main analysis (1,500 words with 3 supporting examples), and recommendations (300 words). Prioritize depth on the top 3 findings rather than trying to cover every detail."

---

### How to Run This Activity

1. **Round 1 (5 minutes):** Each pair gets 5 bad prompts. They identify the flaw in each and write it on a sticky note.
2. **Round 2 (5 minutes):** Pairs swap their 5 prompts with another pair and attempt to rewrite better versions.
3. **Gallery Walk (5 minutes):** Post all bad prompts, diagnoses, and rewrites on the wall. Everyone walks around and adds stars to the best rewrites.

**Facilitator Tips:**
- Bad Prompt #5 is intentionally provocative -- use it to discuss ethical considerations in AI use.
- Bad Prompt #8 is critical for data governance awareness -- spend extra time here if your audience handles sensitive data.
- Encourage participants to find bad prompts from their own work to add to the museum.
- Consider creating a "living museum" that grows throughout the training program.

**Debrief Questions:**
1. Which bad prompt have you been most guilty of writing yourself?
2. What's the single most impactful improvement you can make to your prompts?
3. Should your team create a "prompt review checklist" for important AI-assisted tasks?

---

*End of Unit 2 Activities*
