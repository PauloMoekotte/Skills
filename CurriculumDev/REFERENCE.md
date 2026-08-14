---
name: ai-curriculum-dev-reference
description: Detailed prompts and evidence for the ai-curriculum-dev skill. See [SKILL.md](SKILL.md).
---

# Reference — Prompts & Evidence (Ratiarson 2025)

Each prompt is copy-paste ready for an LLM (GPT-4-class). Replace the bracketed
placeholders. Always keep a human in the loop.

## Prompt A — Bloom's Taxonomy classification

```
You are a curriculum analyst. For each learning outcome below, classify its highest
cognitive level per Bloom's Taxonomy (Remember, Understand, Apply, Analyze,
Evaluate, Create). Return a table: Outcome | Level | One-line rationale.

Also report the distribution of levels and flag if lower-order (Remember/Understand)
or higher-order (Analyze/Evaluate/Create) levels are missing or over-represented.

Outcomes:
"""
[PASTE CUs / PUs]
"""
```
Evidence: Li et al. (2022) classified 21,000+ objectives; BERT reached Cohen's
kappa 0.93, F1 up to 0.95; even SVM/Random Forest were competitive.

## Prompt B — CU → PU alignment

```
You are an outcomes-based-education specialist. Map each Course Learning Outcome
(CLO) to the most relevant Program Learning Outcome (PLO). For each CLO give:
PLO id | Confidence (High/Med/Low) | Reasoning. Flag CUs that map to no PLO
(gap) and PUs with no supporting CU (coverage gap).

CUs:
"""
[PASTE CIs]
"""
PUs:
"""
[PASTE PUs]
"""
```
Evidence: Zaki et al. (2022) CU-to-PU NLP mapping achieved 83–88% precision
vs human experts.

## Prompt C — Build a curriculum knowledge graph

```
Extract a machine-readable knowledge graph from the curriculum below.
Entities: Course, LearningOutcome, Skill, Competency, Resource, Prerequisite.
Relations: teaches, alignsTo, hasPrerequisite, assessedBy, partOf.

Output as triples: (subject, relation, object), one per line. Then list 3 SPARQL-like
queries a faculty member could run to find (1) uncovered skills, (2) courses with
high overlap, (3) prerequisites before topic X.

Curriculum:
"""
[PASTE syllabus / course catalog]
"""
```
Evidence: Christou et al. (2025) CurrKG OWL ontology; Aliyu et al. (2020) KG for
course management improved resource alignment; Li & Guo (2025) KG-based
personalized piano learning paths.

## Prompt D — Align old framework → new framework

```
Two competency frameworks are below. For each item in Framework A, suggest the
closest item in Framework B (or "new — no equivalent"). Note semantic drift where
terms differ but meaning is similar (e.g. "team collaboration" ≈ "teamwork skills").

Framework A:
"""
[PASTE old framework]
"""
Framework B:
"""
[PASTE new standard]
"""
```
Evidence: LLM-assisted ontology alignment recommended framework equivalences from
description semantics.

## Prompt E — Course sequencing / next-course recommendation

```
Act as an academic advisor agent. Given the prerequisite graph and a student's
completed courses, recommend the next 1–3 courses. Enforce hard rules: every
recommendation must have its prerequisites met and count toward degree requirements.
Explain each choice in natural language. Flag any recommended sequence that would
violate a prerequisite.

Completed courses: [LIST]
Prerequisite graph: [LIST or attach]
Degree requirements: [LIST]
```
Evidence: Wang & Zaïane (2018) dependency-graph recommenders beat unguided
selection; Chen et al. (2025) CNN+graph hybrid reached ~0.83 precision; Zhong et al.
(2023) LLM advisor layer for explanation + constraint checking.

## Prompt F — Generate & adapt instructional content

```
You are a subject-matter co-designer. Produce a first DRAFT only (human will review).
Task: [lecture notes | 5 MCQs | clinical vignette | case study] on:
"""
[TOPIC + learning outcome it supports]
"""
Constraints: align items to outcome "[OUTCOME]"; target audience [e.g. 9th graders,
lower reading level]; provide one simpler and one visual/analogy variant. Mark any
claim that needs factual verification with [VERIFY].
```
Evidence: Coskun & Kiyak (2024) used ChatGPT for clinical vignettes/MCQs (RCT);
Farag (2024) AI content reformatting; Karata et al. (2024) teachers use ChatGPT to
adapt/omit/add content; Almatrafi & Johri (2025) LLM clustering outcomes into
course modules.

## Summary table (from the paper, Table 1)

| Curriculum task | AI approach | Representative work |
|-----------------|------------|---------------------|
| Mapping & outcome alignment | NLP classifiers (BERT for Bloom); semantic similarity; LLM draft mapping | Li et al. (2022); Zaki et al. (2022); Almatrafi & Johri (2025) |
| Competency & standards alignment | Ontologies + knowledge graphs; LLM ontology mapping | Christou et al. (2025); Aliyu et al. (2020) |
| Course sequencing & learning paths | Recommenders (CF, sequence mining); graph algorithms; CNN/RNN | Wang & Zaïane (2018); Chen et al. (2025); Li & Guo (2025) |
| Content generation & adaptive design | LLMs for text; image gen; summarization; RL tutoring; adaptive platforms | Coskun & Kiyak (2024); Farag (2024); Karata et al. (2024); Zhong et al. (2023) |

## Research gaps to watch

- Most tools are research prototypes, not in production curriculum software.
- Adoption + UX + faculty training remain the biggest barrier.
- Trust needs explainability (knowledge graphs, explainable NLP).
- Surface-level text alignment ≠ cognitive-demand alignment; close loop with
  student-performance/learning-analytics data.
- Governance: define review process for partially AI-developed curricula.
