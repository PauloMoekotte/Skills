# Chapter 10: Case Studies (Appendix)

## Core Idea
Real AI projects from spring 2024 show the playbook's principles in practice: phased experimentation, UR-for-AI, RAG over fine-tuning for fresh content, human-in-the-loop assurance, and the ethical/legal/security work each team had to do. Use them as worked templates — not formal advice.

## Frameworks Introduced
- **GOV.UK Chat pattern — RAG over fine-tuning**: for content that changes regularly (GOV.UK's 700K+ pages), a retrieval augmented generation (RAG) approach beats fine-tuning an LLM, because retrieved content stays current. Run phased experiments (couple of weeks each), evaluate accuracy with SMEs, and gate public launch on an accuracy threshold (~80%).
- **GOV.UK Chat UR-for-AI pattern**: evaluate LLM answers against human answers via SME Likert ratings; measure inter-rater agreement (consistency = reliable data); then scale testing (1,000 users via research banner) combining accuracy ratings, question types, usefulness feedback and response times.
- **CCS recommendation system pattern — two-tower NN**: TensorFlow Recommenders two-tower architecture learns embeddings for transaction context and candidate products; recommend agreements new to each customer (discovery), validated against a control group by increased unique agreements used.
- **FCDO Digital Sensitivity Review pattern — assist, don't replace**: AI augments trained sensitivity reviewers (10% of review effort, risk of release well below baseline); uses ephemeral/duplicate identification and clustering to reduce digital volume; built with off-the-shelf modular software and academic collaboration (Team Cicero, ISO 44001).
- **NHS user research finder pattern — LLM via API with human review**: users upload research; a commercial LLM summarises; the user reviews/edits before submission; natural-language search over the database. Watch for output variability and vaguely-related results on long/complex queries.
- **NHS.UK reviews moderator pattern — graduated complexity**: start with regex/NER/part-of-speech tagging on a Flask app to establish architecture, then add more complex ML models; test with confusion matrices, clerical review of false positives/negatives, and non-functional testing (latency, throughput).

## Key Concepts
- **Red teaming**: GOV.UK Chat collaborated with CDDO, Number 10DS and i.AI on red teaming to find vulnerabilities.
- **Synthetic data for training**: NHS.UK augmented scarce training data (safeguarding rejection cases) using NLP-generated synthetic data validated by expert moderators.
- **Discovery metric problem**: offline "hit" metrics misjudge discovery systems — the whole point is recommending what a customer has NOT interacted with yet.
- **Statistical constraint on ML**: FCDO's redaction rate (<1% of reviewed docs) limits training data volume; differing departmental policies further fragment it.
- **Inter-rater agreement**: high SME agreement on ratings → reliable evaluation data; LLM rated on par with human answers.

## Mental Models
- Use **"accuracy threshold gates launch"**: pilot → measure → improve → launch only if the threshold is met (GOV.UK Chat 80%).
- Use **"assist not replace"**: FCDO reviewers remain responsible; the AI augments volume but does not remove reviewer responsibility or human decision.
- Use **"human in the loop for public-facing content"**: NHS finder requires user review/edit of AI summaries before publication; NHS.UK offers human review of automated moderation.
- Use **"start simple, then scale complexity"**: NHS.UK began with regex/rules to prove architecture before ML; GOV.UK Chat began with whole-page retrieval before chunking/re-ranking/few-shot improvements.

## Anti-patterns
- **Fine-tuning on fast-changing content**: GOV.UK's content updates constantly — fine-tuning goes stale; RAG stays current.
- **Evaluating discovery systems with offline hit metrics**: penalises exactly the "new to customer" recommendations the system is designed to make.
- **Assuming LLM summarisation is consistent**: the same report summarised repeatedly gives varied results; design for human review.
- **Skipping non-functional testing**: NHS.UK tested latency/throughput under likely and extreme scenarios to assure the product owner the solution was fit for use.

## Worked Example
**Phased rollout decision (GOV.UK Chat).**
1. Focus area chosen for complexity: "business" (multi-department policy).
2. First experiment: whole-page retrieval → errors when long niche pages exceeded LLM token limits; answer accuracy ~80%.
3. Improvements: chunking, alternative embeddings, re-ranking, improved few-shot examples.
4. Evaluation: content designers + cross-gov SMEs assessed answers; ~70% of users found responses useful, ~65% satisfied; SME ratings consistent (high agreement) and LLM rated on par with human answers.
5. Decision: pursue limited public pilot only if accuracy thresholds met; build a knowledge base of quality-assessed questions for semi-automated QA at scale.
Takeaway: measure, gate, then scale.

## Key Takeaways
1. Prefer RAG over fine-tuning when source content changes frequently.
2. Gate public deployment on measured accuracy thresholds.
3. Use UR-for-AI (SME rating, agreement metrics) to evaluate generative outputs safely.
4. Keep humans responsible: assist-with-AI over replace-with-AI, with human review/redress paths.
5. Plan for data scarcity (synthetic data), metric pitfalls (discovery), and non-functional requirements.

## Connects To
- **Ch 3**: UR-for-AI and use-case selection in practice
- **Ch 4**: procurement and vendor management (CCS, NHS finder third-party API)
- **Ch 5**: ethics and safeguards in real projects
- **Ch 7**: data protection and privacy in real projects
- **Ch 8**: red teaming and security in real projects
- **Ch 9**: sign-off and assurance processes (NHS compartmentalised sign-off)
