# AI Blog Optimisation Workflow (Step-by-Step Review Process)

## Goal
Enhance existing blog content for AI Search / LLM / AI Overview visibility by analysing user intent, extracting related questions, modelling AI-generated answers, and improving content relevance.

---

## STEP 1 — Input Blog URL & Scrape Content

### AI Task
1. Accept blog URL from user.
2. Crawl/scrape the full blog content.
3. Extract: Title, Meta Title, Meta Description, H1, All H2/H3 headings, Main body content, FAQ section (if any)

### Output for Review
```text
BLOG SCRAPE COMPLETE

URL:
Title:
Primary Topic:
...
```

### Ask User
"Please review the extracted blog summary. Approve to proceed?"

---

## STEP 2 — Understand Core Topic & Search Intent
*(Runs automatically after Step 1 approval)*

### AI Task
Analyse scraped content and determine Primary Topic, Search Intent, Audience Persona, Pain Points, and Likely Search Motivations.

### Output
Outputs the Topic Analysis and immediately proceeds to Step 3 without asking for approval.

---

## STEP 3 — Generate Seed Questions

### AI Task
1. Generate 15–20 likely related search questions.
2. Cluster by relevance.

### Output for Review
```text
QUESTION RESEARCH COMPLETE

Highly Relevant Questions:
1.
2.
3.

Secondary Questions:
4.
5.
6.
```

### Ask User
"Please select/approve 2–3 target questions for AI optimisation."

---

## STEP 4 — Google SERP Analysis (Location-Based)
*(Runs automatically after Step 3 approval)*

### AI Task
For each approved question:
1. Search Google using target client location.
2. Analyse AI Overview, Featured Snippets, Top Organic Results, PAA, SERP Intent.
---

## STEP 5 — LLM / AI Search Analysis
*(Runs automatically)*

### AI Task
Analyse responses from standard LLMs. Proceeds to Step 6 automatically.

---

## STEP 6 — Review Referenced / Ranking Sources
*(Runs automatically)*

### AI Task
Analyse competitor structural patterns and recommended additions. Proceeds to Step 7 automatically.

---

## STEP 7 — Create AI Optimisation Recommendations
*(Runs automatically)*

### AI Task
Generate actionable recommendations for content structure. (Note: Always place Q&A at the top, no bottom FAQs). Proceeds to Step 8 automatically.

---

## STEP 8 — Output Blog Recommendations (Copy-Paste Format)
*(Runs automatically)*

### AI Task
Generate the exact text for the new recommendations so the user can manually copy-paste it into their live blog. Only output the new content blocks.

**Strict Content Writing Rules:**
1. Write content at an 8th-grade English comprehension level.
2. Use simple, clear language; avoid jargon and long sentences.
3. Break down complex ideas and use bullet points heavily.

### Output for Review
```markdown
[INSERT THE FORMATTED NEW 8TH-GRADE CONTENT BLOCKS HERE]
```
```text
UPDATED BLOG DRAFT READY
```

### Ask User
"Please review the provided copy-paste text. Approve final version?"

---

## STEP 9 — Push Final Content to GitHub

### AI Task
Once the user approves Step 8, automatically save the generated output snippet to a new markdown file named closely after the blog post (e.g., `blog-name-optimisations.md`) in the local workspace. Run `git add`, `git commit`, and `git push` to upload to the remote GitHub repository.

### Output
```text
GITHUB PUSH COMPLETE

The final optimisations have been committed and pushed safely to your repository. 
```

### Ask User
"File pushed successfully. Please provide the URL for the next blog you'd like to optimize!"

---

## Execution Rules
1. ONLY block and wait for user approval after **Step 1**, **Step 3**, and **Step 8**.
2. Steps 2, 4, 5, 6, 7, and 8 must be executed sequentially in a single turn without stopping.
3. Once Step 8 is approved, execute Step 9 immediately.
4. Adhere strictly to the 8th-grade readability and formatting rules during output generation in Step 8.
