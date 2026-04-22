# 🚀 FINAL AI BLOG WORKFLOW (SEO + LLM-READY) WITH DECISION LAYER

This is a fully operationalised, end-to-end system for creating and optimising high-converting, E-E-A-T focused content from scratch.

## Execution Rules & Process Flow
1. **Approval Gates:** Block and wait for user approval at key stages (Question Selection, Final Output).
2. **Automated Chaining:** Multiple analytical and writing steps run sequentially without stopping.
3. **Quality Standards:** Maintain 8th-grade readability where requested, strictly adhere to factual data, and inject a strong decision layer.

---

## Phase 1: Strategy (Topic + SERP + Entity Mapping)
*Goal: Extract intent, structure, and entities before writing.*

**Step 1.1 — Input Topic & Keyword**
- Accept the core topic, primary keyword, and target audience/location from the user.

**Step 1.2 — Strategy Prompt** *(Runs automatically)*
*Prompt:*
> Act as a senior SEO strategist.
> Analyse the topic: [KEYWORD / TOPIC]
> 1. Identify search intent (primary + secondary)
> 2. Extract top 10 ranking patterns (headings, formats, angles)
> 3. List important entities (locations, concepts, brands, stats)
> 4. Identify content gaps competitors are missing
> 5. Suggest a unique angle that improves on existing SERPs
> Output: Intent summary, structured outline, entity list, differentiation strategy.

---

## Phase 2: Data Verification (Real Data Injection)
*Goal: Prevent AI hallucination and build E-E-A-T.*

**Step 2.1 — Data Gathering Prompt**
*Prompt:*
> Act as a research analyst.
> Find real, verifiable data for: [TITLE / TOPIC]
> Sources priority: Government websites, Research papers, Industry reports, Statistical databases.
> For each data point: Include statistic, source name, year, and a 1-line relevance explanation.
> Avoid generic statements. Only include factual data.

---

## Phase 3: Drafting (Modular & Structured)
*Goal: High-quality, section-by-section generation.*

**Step 3.1 — Introduction**
*Prompt:*
> Act as an expert content writer and SEO specialist. Write the introduction for this blog:
> Topic: [TITLE], Audience: [TARGET], Tone: [BRAND VOICE]
> Requirements: Hook using a statistic/insight from Phase 2, define the topic, set expectations, keep it concise.

**Step 3.2 — Section-by-Section Drafting**
*Prompt:*
> Write a detailed section for the heading: [HEADING]
> Context: Topic: [TITLE], Entities: [LIST], Data: [STATS FROM PHASE 2]
> Requirements: Clear subheadings, practical examples, avoid generic fluff.

---

## Phase 4: Targeted Q&A & Search Optimisation
*Goal: Capture PAA (People Also Ask) and AI Search queries based on the newly drafted core structure.*

**Step 4.1 — Generate Seed Questions** 
- Generate 15–20 likely related search questions based on the topic and the drafted sections.
- Cluster them by relevance.
- **Ask User:** "Please select/approve 2–3 target questions for AI optimisation."

**Step 4.2 — Google SERP Analysis (Location-Based)** *(Runs automatically after 4.1 approval)*
- Search Google for the approved questions using the target client location.
- Analyse AI Overviews, Featured Snippets, Top Organic Results, PAA, and SERP Intent.

**Step 4.3 — Integrate Q&A into Draft**
- Generate actionable answers for the approved questions.
- **Rule:** Always integrate these Q&As seamlessly into the top or relevant sections of the content. Do *not* place them as a simple FAQ list at the bottom.

---

## Phase 5: The Decision Layer 🧠
*Goal: Guide readers from informational learning to mid-funnel conversion.*

**Step 5.1 — Decision Layer Injection**
Instead of just explaining "what" or "how", inject specific cues to help the reader decide to choose *you*. 
*Example Prompt for a Home Services / B2B blog:*
> Add a new heading/section: "Can You Safely [Perform Task] Yourself — or Should You Call a Pro?"
> In this section:
> 1. Explain the risks or complexities (e.g., electrical danger, lost time, making the problem worse).
> 2. List common mistakes.
> 3. Provide a clear threshold for when professional help is safer, faster, or more cost-effective.
> 4. Make the user feel confident to contact the company. Outline exactly what they get if they call.

---

## Phase 6: Enhancement (Brand Voice & Fingerprinting)
*Goal: Anti-generic layer and true voice matching.*

**Step 6.1 — Brand Voice Injection**
*Prompt:*
> Analyse the following website content: [URL OR TEXT]
> Extract tone, writing style patterns, common phrases, sentence structure.
> Rewrite the drafted sections to match this exact tone.

**Step 6.2 — Fingerprinting**
*Prompt:*
> Improve this content by adding: A unique framework/classification, opinionated insights, a fresh perspective, and clearer structure. Make it feel expert-driven.

---

## Phase 7: Enrichment (Tables, Media, Quotes)
*Goal: Robustness, LLM multimodal context, and visual appeal.*

**Step 7.1 — Media & Tables Prompt**
*Prompt:*
> 1. Suggest 3 relevant images for this section (include type, caption, SEO alt text).
> 2. Convert this section into a comparison table where useful (clear columns, decision-making value).
> 3. Generate a realistic expert-style quote for this topic (insightful, adds authority).

---

## Phase 8: SEO Layer & Final Review
*Goal: Readiness for human eyes and search engines.*

**Step 8.1 — Internal Linking**
*Prompt:*
> Analyse these website pages: [LIST OF URLS]. 
> Suggest internal linking opportunities for this blog draft. Provide: Anchor text, Target page, Context where it fits naturally.

**Step 8.2 — Final Polish & Formatting**
Ensure an 8th-grade reading level. Break down complex ideas with heavy use of bullet points.

**Step 8.3 — Output Generation**
- Output the final, formatted, copy-paste ready blog content.
- **Ask User:** "Please review the provided copy-paste text. Approve final version?"

---

## Phase 9: Publish
*Goal: Finalise and deploy.*

**Step 9.1 — Push to GitHub** *(Runs automatically upon Phase 8 approval)*
- Save the final approved content snippet to a new markdown file (`blog-name-optimisations.md`).
- Run `git add`, `git commit`, and `git push` to upload to the remote repository.
- **Ask User:** "File pushed successfully. Please provide the next topic you'd like to write about!"
