---
name: ai-curriculum-dev
description: Apply AI models to accelerate curriculum development and online course creation. Use when designing curricula, mapping learning outcomes, aligning CLOs/PLOs, classifying Bloom's Taxonomy levels, building knowledge graphs/ontologies, sequencing courses, generating assessments or instructional content, or personalizing learning paths.
---

# AI Curriculum Development Accelerator

Apply the four AI approaches from Ratiarson (2025) to speed up curriculum design while
keeping educators in control. Pick the workflow that matches the task, then use the
ready-to-use prompts in [REFERENCE.md](REFERENCE.md).

Core principle: **AI augments, never replaces, human curriculum judgment.** Always
review AI output for accuracy, bias, and pedagogical fit before adoption.

## Decision guide — which approach fits the task?

| Your task | Approach | Section |
|-----------|----------|---------|
| Tag outcomes by Bloom's level; detect missing/over-represented levels | NLP classification | 2 |
| Align course outcomes (CLO) to program outcomes (PLO); detect gaps | NLP semantic alignment | 2 |
| Map curriculum to standards/competency frameworks; spot overlap/gaps | Ontology / Knowledge Graph | 3 |
| Recommend course order; personalize learning paths; find prereq issues | Recommender / Graph | 4 |
| Draft lecture notes, quiz items, case studies, simplify/adapt content | Generative AI | 5 |

## Workflow 1 — Outcome classification & alignment (NLP)

1. Collect learning outcome statements (CLOs, PLOs, module outcomes).
2. Classify each by Bloom's Taxonomy cognitive level (prompt A in REFERENCE).
3. Cross-check CLO→PLO alignment via semantic similarity (prompt B).
4. Surface mismatches: outcomes with no mapping, or programs missing a level.
5. Human review + rewording; do not auto-publish.

## Workflow 2 — Competency / standards mapping (Ontology + KG)

1. Define entities: Course, Outcome, Skill, Competency, Resource, Prerequisite.
2. Build a lightweight knowledge graph (prompt C) linking outcomes to frameworks
   (e.g. SFIA, national qualifications).
3. Run gap/overlap queries ("which skills are taught by no course?").
4. Use LLM to align old↔new frameworks when standards change (prompt D).

## Workflow 3 — Course sequencing & learning paths (Recommender + Graph)

1. Encode prerequisite graph of courses/modules.
2. Recommend next-item / next-course using dependency graph + history (prompt E).
3. Validate every recommendation against hard rules (prereqs, degree reqs).
4. Mine real enrollment patterns for unintended but successful pathways.

## Workflow 4 — Content generation & adaptive design (Generative AI)

1. Generate first drafts: notes, examples, MCQs, case studies (prompt F).
2. Adapt tone/level for cohort (e.g. 9th graders, lower reading level).
3. Produce multiple explanation variants per concept for inclusivity.
4. Human review every item for factual/clinical/cultural accuracy.

## Guardrails (apply to all workflows)

- **Hallucination risk**: LLMs invent plausible-but-wrong mappings. Combine with
  curated knowledge bases + human-in-the-loop.
- **Trust**: require explainability — AI must show reasoning, not just a verdict.
- **Equity/quality**: vet AI content like peer-reviewed OER; involve subject
  experts, designers, and student feedback.
- **Accountability stays human**: AI drafts, educator owns the final curriculum.

## Where to go next

- Copy-paste prompts + examples: [REFERENCE.md](REFERENCE.md)
- Cite: Ratiarson (2025), "AI Models for Accelerating Curriculum Development and
  Online Course Creation" (literature review).
