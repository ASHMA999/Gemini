# Unit 3: Microsoft Copilot

## The Hidden Power in the Browser

| Detail | Description |
|--------|-------------|
| **Duration** | 5 hours (including breaks) |
| **Delivery** | Live demos + hands-on exercises across all M365 apps |
| **Tools Required** | Microsoft Edge + Copilot, Microsoft 365 apps (Word, Excel, PowerPoint, Outlook, Teams), Copilot Studio |
| **Objective** | Master Copilot in the browser AND across all M365 applications, understand Agents, and leverage AI-powered features like live translation and Designer |

---

## 3.1 The Paradigm Shift: Browser as AI Operating System

The browser has evolved from a passive HTML viewer to the closest layer to the user in the digital productivity pyramid. Embedding LLMs directly into the browser chrome means AI can 'see' what the user sees and 'understand' real-time context without switching applications or migrating data.

### Context is the New King

Previously, the FILE was the basic unit of work (a Word doc, an Excel sheet). Today, with Copilot in Edge, CONTEXT is the basic unit. When a user opens an intranet page, a PDF, or a training video, Copilot in the sidebar can read, summarize, and interact with that content instantly.

### Enterprise Data Protection (EDP)

When you log in with your Entra ID (work account), Enterprise Data Protection activates automatically:

- **Complete isolation:** Data never leaves the tenant boundary
- **Zero training:** Your conversations are NEVER used to train OpenAI models
- **Geographic compliance:** Adheres to EU Data Boundary and global regulations

---

## 3.2 E3 vs. E5 Licensing Impact

| Feature | Microsoft 365 E3 | Microsoft 365 E5 | Impact on Copilot |
|---------|-------------------|-------------------|-------------------|
| Sensitivity Labels | Manual creation & application | Automatic creation & AI-based application | E5 auto-blocks Copilot from summarizing classified docs |
| DLP Policies | Standard (SharePoint/Exchange) | Comprehensive (Teams + Endpoints) | E5 prevents pasting sensitive Copilot responses |
| Device Management | Basic Intune | Advanced analytics + endpoint privileges | E5 detects non-compliant devices and blocks Copilot |

---

## 3.3 The Sidebar: Command Center

### Essential Keyboard Shortcuts

- **Open Sidebar:** Ctrl + Shift + . (Windows) or Cmd + Shift + . (Mac)
- **Voice interaction:** Windows + C (Windows 11) for hands-free AI assistance
- **Chat with Page:** Must enable 'Allow Copilot to read context clues on the web' in sidebar settings

### The Compose Tab is Dead; Long Live Inline Rewrite

Microsoft removed the dedicated 'Compose' tab. The replacement: select any text in any text field on the web, and a floating Copilot icon appears offering 'Rewrite with Copilot.' This changes tone, length, and format directly in place.

---

## 3.4 File Analysis: Challenges & Solutions

### The File Upload Puzzle

Upload limits have been reduced to 1MB for some file types in early 2025/2026. Users without full Copilot licenses face hidden daily upload limits that trigger 'Daily limit reached' errors.

### Strategic Workarounds

1. **OneDrive Bridge:** Upload files to OneDrive/SharePoint first, then paste the link into Copilot. This bypasses size limits entirely.
2. **For local PDFs:** Go to edge://extensions, find the Copilot extension, and enable 'Allow access to file URLs.'
3. **PDF-to-Excel trick:** Open PDF in Edge, enable context, then prompt: 'Extract the table on this page and format it as a Markdown table.' Copy the Markdown to Excel for perfect formatting.

### Hands-On Exercise 11: Browser Copilot Power User Lab (25 minutes)

Complete these 5 tasks using Edge Copilot: (1) Open a PDF report in Edge and ask Copilot to summarize the key findings. (2) Navigate to a news article and ask 'What are the 3 things this article gets wrong?' (3) Use inline Rewrite to transform a casual paragraph into a formal business tone. (4) Extract a table from a webpage into Markdown format. (5) Use the sidebar to compare two open tabs and summarize the differences.

---

## 3.5 Copilot for Microsoft 365: The Full Suite

### 3.5.1 Copilot in Microsoft Word

Copilot in Word acts as a co-writer that can draft, rewrite, summarize, and transform documents on command.

- **Draft with Copilot:** Click the Copilot icon in the toolbar to generate entire documents from a short description
- **Rewrite Selection:** Highlight any paragraph, click Copilot, and ask it to change tone, simplify language, or expand the content
- **Summarize Long Documents:** Open a 50-page report and ask 'Summarize the key decisions and action items from this document'
- **Reference Files:** Use the / command to pull content from other files: 'Draft a memo based on /Q3-Report.docx and /Budget-2026.xlsx'
- **Transform to Table:** Select a paragraph of data and ask Copilot to restructure it as a formatted table

**Pro Tip: Custom Instructions in Word** - Set persistent writing preferences: 'Always use active voice, keep sentences under 20 words, and follow APC's corporate style guide.' Copilot will apply these to every draft it generates in that document.

### Hands-On Exercise 12: Word Copilot Workshop (20 minutes)

Open a blank Word document. (1) Prompt Copilot: 'Draft a Safety Incident Report template for APC including sections for incident description, root cause analysis, corrective actions, and sign-off fields.' (2) Select the Root Cause section and ask Copilot to expand it with a 5-Why methodology framework. (3) Highlight the entire document and ask: 'Rewrite this in formal Arabic while keeping all technical terms in English.' (4) Ask Copilot to generate an executive summary of the document in 3 bullet points.

### 3.5.2 Copilot in Microsoft Excel

Copilot in Excel transforms data analysis from a technical skill to a conversational experience.

- **Natural Language Formulas:** Ask 'What is the average production output per shift?' and Copilot writes the AVERAGEIF formula for you
- **Highlight Insights:** Ask 'What are the key trends in this data?' and Copilot identifies patterns, outliers, and anomalies automatically
- **Chart Generation:** 'Create a bar chart comparing monthly maintenance costs by department, sorted highest to lowest'
- **Python in Excel:** For advanced analysis, Copilot writes Python code executed in a secure Azure sandbox
- **Conditional Formatting:** 'Highlight all cells where downtime exceeds 4 hours in red'
- **What-If Analysis:** 'If we increase production by 10%, what would be the impact on raw material consumption based on current ratios?'

**Important Limitation:** Copilot in Excel requires data to be formatted as a Table (Ctrl+T). Raw data in plain cells will not be recognized.

### Hands-On Exercise 13: Excel Copilot Analytics Lab (25 minutes)

Open the provided sample production dataset in Excel. (1) Convert the data to a Table (Ctrl+T). (2) Ask Copilot: 'Show me the top 5 products by total revenue.' (3) Ask: 'Create a pivot-style summary showing monthly production by line, with a line chart.' (4) Ask: 'Use Python to forecast next quarter production using exponential smoothing and show a chart with confidence intervals.' (5) Ask: 'What anomalies do you see in this data? Highlight any concerning patterns.'

### 3.5.3 Copilot in Microsoft PowerPoint

Copilot in PowerPoint can create entire presentations, design slides, add speaker notes, and organize content.

- **Create from Prompt:** 'Create a 12-slide presentation about our Q1 safety performance with charts and recommendations'
- **Create from File:** 'Create a presentation from /Safety-Report-Q1.docx'
- **Organize Slides:** 'Reorganize this presentation to tell a better story: start with the problem, then data, then solutions'
- **Add Speaker Notes:** 'Generate speaker notes for each slide that include key talking points and transition phrases'
- **Design Enhancement:** 'Make this slide more visually appealing' or 'Convert this bullet list into a SmartArt diagram'
- **Summarize Presentations:** Open a 40-slide deck and ask 'Summarize the key messages from this presentation in 5 bullet points'

### AI-Powered Translation & Live Subtitles in PowerPoint

**Presentation Translator (Real-Time):** During a live presentation (Slideshow mode), PowerPoint can display real-time subtitles in the presenter's language AND simultaneously translate them into up to 60+ languages for the audience.

**How to activate:** Go to Slide Show tab > Always Use Subtitles > Select Spoken Language (e.g., Arabic) > Select Subtitle Language (e.g., English). Audience members can even scan a QR code to see live subtitles on their phones in their own language!

**Use Case at APC:** Present a safety briefing in Arabic while international consultants see live English subtitles on their phones.

- **Slide Translation:** Right-click any text box > Translate > Select target language
- **Speech-to-Text Notes:** During rehearsal mode, PowerPoint transcribes your spoken words into speaker notes automatically
- **Presenter Coach:** AI analyzes your rehearsal and gives feedback on pace, filler words, pitch variety, and inclusive language

### Hands-On Exercise 14: PowerPoint AI Features Lab (25 minutes)

Part A - Copilot: (1) Create a new presentation using Copilot: 'Create a 6-slide presentation about preventive maintenance best practices for industrial pumps.' (2) Ask Copilot to add speaker notes to all slides. (3) Ask: 'Add a comparison slide between reactive and preventive maintenance with a visual table.'

Part B - Live Translation: (4) Enter Slideshow mode and activate live subtitles (Spoken: Arabic, Subtitle: English). (5) Present 2 slides speaking in Arabic and observe the English subtitles. (6) Use Presenter Coach in rehearsal mode and review your feedback report.

### 3.5.4 Copilot in Microsoft Outlook

- **Draft with Copilot:** Describe what you need: 'Write a follow-up email to the maintenance team about last week's pump failure, requesting a root cause report by Thursday'
- **Coaching Tone:** 'Make this more diplomatic' or 'Make this more urgent'
- **Summarize Email Threads:** Open a long chain and ask 'Summarize this thread and list all action items with owners'
- **Smart Reply Suggestions:** Context-aware replies based on the email content
- **Schedule Optimization:** 'Find a 1-hour slot this week when all maintenance managers are free'
- **Custom Coaching (Persistent):** 'Always keep my emails under 150 words, use bullet points for action items'

### Hands-On Exercise 15: Outlook Copilot Mastery (15 minutes)

(1) Use 'Draft with Copilot' to write a message requesting all department heads submit their monthly safety statistics by Friday. (2) Ask Copilot: 'Make this more assertive with a clear deadline.' (3) Ask: 'Translate this email to Arabic while keeping department names in English.' (4) Open a sample email thread (15+ messages). Ask: 'What are the key decisions made in this thread and who is responsible for each?'

### 3.5.5 Copilot in Microsoft Teams

- **Meeting Summarization:** Auto-generated summary with key topics, decisions, and action items
- **Real-Time During Meetings:** 'What has been discussed so far?' or 'What did [person] say about the budget?'
- **Meeting Recap for Latecomers:** 'Catch me up on what I missed'
- **Meeting Notes to Tasks:** 'Convert the action items into Planner tasks with due dates and assignees'
- **Chat Summarization:** 'Summarize the last 7 days of discussion in this channel'
- **Intelligent Recap:** 'What did I miss in Teams while I was away?'
- **Live Translation in Meetings:** Real-time captioning and translation in 30+ languages

### Hands-On Exercise 16: Teams AI Features (20 minutes)

(1) Watch a provided 10-minute recorded Teams meeting. (2) Ask: 'Summarize this meeting in 5 bullet points.' (3) Ask: 'What action items were assigned and to whom?' (4) Ask: 'What questions were raised but not answered?' (5) Ask: 'Draft a follow-up email based on this meeting.'

---

## 3.6 AI-Powered Features Built into Microsoft 365 Apps

| App | AI Feature | What It Does | License Required |
|-----|-----------|--------------|-----------------|
| PowerPoint | Designer (Design Ideas) | Auto-suggests professional slide layouts | M365 Basic |
| PowerPoint | Live Captions & Subtitles | Real-time speech-to-text in 60+ languages | M365 Basic |
| PowerPoint | Presenter Coach | AI feedback on pace, filler words, pitch | M365 Basic |
| PowerPoint | Cameo | Live camera feed embedded in slides | M365 Basic |
| Word | Editor (AI Writing Assistant) | Grammar, clarity, conciseness suggestions | M365 Basic |
| Word | Dictation + Transcription | Voice-to-text in 30+ languages | M365 Basic |
| Excel | Ideas (Analyze Data) | One-click insight suggestions | M365 Basic |
| Excel | XLOOKUP / Dynamic Arrays | AI-assisted formula suggestions | M365 Basic |
| Outlook | Scheduling Assistant | AI-powered meeting time suggestions | M365 Basic |
| Outlook | Text Predictions | Ghost text suggestions while typing | M365 Basic |
| Teams | Intelligent Recap | Auto meeting summaries and topics | Teams Premium |
| Teams | Live Translation (Captions) | Real-time caption translation (30+ lang) | Teams Premium |
| Teams | Speaker Attribution | Identifies who said what | Teams Premium |
| OneNote | Copilot Summary | Summarizes notebooks/sections | M365 Copilot |
| Forms | Copilot Form Builder | Natural language to survey | M365 Copilot |
| Whiteboard | Copilot Brainstorm | Generate & organize ideas | M365 Copilot |

**Key Takeaway:** Many AI Features Are Already Free - Designer, Editor, Transcription, Live Captions, and Data Insights are available with standard M365 licenses.

### Hands-On Exercise 17: Discovering Hidden AI Features (20 minutes)

(1) PowerPoint: Insert a text-heavy slide, click 'Designer.' (2) PowerPoint: Start Slideshow with Live Subtitles in a different language. (3) Word: Use Dictation to add a paragraph by speaking. (4) Excel: Select data and click 'Analyze Data.' (5) Outlook: Notice Text Predictions while typing.

---

## 3.7 Copilot Agents: The Future of Autonomous AI at Work

### What Are Copilot Agents?

| Aspect | Copilot Chat (Today) | Copilot Agent (Future) |
|--------|---------------------|----------------------|
| Interaction | You ask, it answers one question | You give a goal, it executes multiple steps |
| Scope | Single app or single context | Cross-app: reads email, checks calendar, updates SharePoint |
| Autonomy | Requires manual prompting each time | Runs in background, reports when done |
| Memory | Forgets between conversations | Maintains context across sessions |
| Example | 'Summarize this document' | 'Monitor daily production reports, flag anomalies, and email me a weekly summary every Sunday' |

### Copilot Studio: Building Custom Agents

- **No-Code Builder:** Drag-and-drop interface for creating agent workflows
- **Knowledge Grounding:** Connect agents to SharePoint sites, company databases
- **Multi-Channel Deployment:** Deploy in Teams, website, Edge sidebar, or M365 chat
- **Action Plugins:** Create tickets in ServiceNow, update SAP records, send emails
- **Guardrails:** Set boundaries on what the agent can and cannot do

### Real-World Agent Scenarios for APC

| Agent Name | Department | What It Does | Tools Connected |
|------------|-----------|--------------|-----------------|
| Safety Watchdog | HSE | Monitors incident reports daily, alerts on patterns | SharePoint + Outlook + Power BI |
| Maintenance Scheduler | Maintenance | Reads sensor data, auto-generates work orders | CMMS + SharePoint + Teams |
| Recruitment Assistant | HR | Screens CVs, ranks candidates, sends shortlists | Outlook + SharePoint + Forms |
| Production Reporter | Production | Collects daily data, generates formatted reports by 8 AM | SharePoint + Excel + Teams |
| Policy Q&A Bot | All | Answers employee questions from approved document library | SharePoint + Teams + Edge |

### Hands-On Exercise 18: Agent Design Workshop (30 minutes)

Form teams of 3-4 people. Design a Copilot Agent for your department. Deliverables: (1) Agent Name and Purpose (2) Trigger (3) Data Sources (4) Actions (3-5 steps) (5) Guardrails (6) Output format. Present to class. Best design wins!

---

## 3.8 Admin Security Policies & Governance

| Policy Name | Function | Recommendation |
|------------|----------|----------------|
| HubsSidebarEnabled | Controls sidebar visibility | Enable |
| CopilotPageContext | Allows reading active page | Enable with training |
| ComposeInlineEnabled | Controls inline rewrite | Enable unless regulatory restrictions |
| M365 Copilot License Assignment | Controls who gets Copilot | Start with power users, expand |
| Copilot Studio - DLP Policies | Controls agent connectors | Block personal email & social media |
| Agent Publishing Approval | Requires admin review | Enable - all agents reviewed before live |

### Oversharing Prevention: The #1 Risk

- Use SharePoint Advanced Management (SAM) to audit overshared files
- Enable Restricted Search mode to limit Copilot's searchable sites
- Run a permissions audit BEFORE rolling out Copilot
- Train users: 'Copilot can only see what YOU can see'

### Hands-On Exercise 19: Copilot 365 Full Workflow Challenge (30 minutes)

Complete this end-to-end workflow: (1) Word: Draft a 'Monthly Maintenance Summary Report' template. (2) Excel: Analyze maintenance costs and create a chart. (3) PowerPoint: Create a 5-slide presentation from the Word report. (4) PowerPoint: Activate live subtitles and present in Arabic with English subtitles. (5) Outlook: Draft an email to the Plant Manager with key findings. (6) Teams: Post the report and ask Copilot to summarize for absent members. Time yourself!
