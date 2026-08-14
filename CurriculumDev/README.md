# ai-curriculum-dev

Apply AI models to accelerate curriculum development and online course creation.
Use when designing curricula, mapping learning outcomes, aligning CLOs/PLOs,
classifying Bloom's Taxonomy levels, building knowledge graphs/ontologies,
sequencing courses, generating assessments or instructional content, or
personalizing learning paths.

> **Core principle:** AI augments, never replaces, human curriculum judgment.
> Always review AI output for accuracy, bias, and pedagogical fit before adoption.

## Which approach fits the task?

| Your task | Approach | Reference |
|-----------|----------|----------|
| Tag outcomes by Bloom's level; detect missing/over-represented levels | NLP classification | Prompt A |
| Align course outcomes (CLO) to program outcomes (PLO); detect gaps | NLP semantic alignment | Prompt B |
| Map curriculum to standards/competency frameworks; spot overlap/gaps | Ontology / Knowledge Graph | Prompt C, D |
| Recommend course order; personalize learning paths; find prereq issues | Recommender / Graph | Prompt E |
| Draft lecture notes, quiz items, case studies; simplify/adapt content | Generative AI | Prompt F |

## Workflows

1. **Outcome classification & alignment (NLP)** — Classify outcomes by Bloom's
   level, cross-check CLO→PLO alignment, surface mismatches, human review.
2. **Competency / standards mapping (Ontology + KG)** — Build a lightweight
   knowledge graph linking outcomes to frameworks (e.g. SFIA, national
   qualifications); run gap/overlap queries; align old↔new frameworks.
3. **Course sequencing & learning paths (Recommender + Graph)** — Encode the
   prerequisite graph, recommend next courses, validate against hard rules,
   mine successful real-world pathways.
4. **Content generation & adaptive design (Generative AI)** — Generate first
   drafts (notes, MCQs, case studies), adapt tone/level per cohort, produce
   explanation variants; human review every item.

## Guardrails (apply to all workflows)

- **Hallucination risk** — LLMs invent plausible-but-wrong mappings. Combine
  with curated knowledge bases + human-in-the-loop.
- **Trust** — require explainability; AI must show reasoning, not just a verdict.
- **Equity/quality** — vet AI content like peer-reviewed OER; involve subject
  experts, designers, and student feedback.
- **Accountability stays human** — AI drafts, educator owns the final curriculum.

## Files

- `SKILL.md` — decision guide and workflows (this skill's entry point).
- `REFERENCE.md` — copy-paste prompts (A–F) and the supporting evidence base
  from Ratiarson (2025).

## Reference

Ratiarson (2025), *"AI Models for Accelerating Curriculum Development and
Online Course Creation"* (literature review).
