# Cheatsheet

## Is AI the right tool? (decision rules)
- Traditional tools can't handle the **volume, complexity, real-time** nature of the task, or you need **advanced pattern detection / personalisation** → consider AI.
- **Fully automated decision making** on significant decisions (health, safety) → avoid (Ch 3).
- **High-risk/high-impact** applications used alone → avoid (Ch 3).
- Could a simpler ML model or non-AI solution work? → **if yes, use that** (P6).

## Governance gates (before deploy)
| Check | Gate |
|---|---|
| 10 principles | all pass, else fix/stop |
| Legal | legal engaged from outset; IPR/liability defined |
| Data protection | DPIA done; lawful basis; minimisation; human oversight |
| Security | secure-by-design; risk-rated (OWASP-style) |
| Assurance | validation + managed release; AI systems inventory |
| Transparency | ATRS recorded (if in scope); AI responses labelled |

## Procurement thresholds
- **~£10M+** investment → Green Book five-part business case (mandatory).
- **<£10M** → CDDO agile business case.
- **Non-BAU spend** → assure >£100K (digital), >£1M (technology).

## Framework vs DPS
- **Framework**: pre-vetted at launch, closed; thorough CCS compliance; direct award possible → use for stable requirements, low buyer effort.
- **DPS**: open registration anytime; further competition only; buyer does more compliance → use in fast-moving markets / when new suppliers matter.

## DPIA mandatory triggers (Art. 35(3)(a) UK GDPR)
- Systematic + extensive evaluation with profiling → decisions with legal/similar significant effects.
- Large-scale processing of special-category data.
- Large-scale systematic monitoring of public areas.
- ICO: innovative technologies processing personal data.

## The 10 data protection principles (AI mapping)
accountability · lawfulness · purpose limitation · transparency & individual rights · fairness · data minimisation · storage limitation · human oversight · accuracy · security

## AI security risks → mitigations
| Risk | Mitigation |
|---|---|
| Data/model poisoning | test outputs vs known-good; bias tests; evaluate fine-tuned third-party models |
| Data leakage | RAG over permitted data; content filters; access-control review; exclude unread/attachments |
| Insecure tool chain | approve tools with cyber team; auth + least privilege; no default configs |
| Perturbation attack | adversarial training with noisy inputs |
| Prompt injection (direct/indirect) | filter prompts & outputs; log/audit prompts; meta-prompts; human review of actions |
| Hallucination | never trust for facts; verify; keep human oversight |
| Exacerbated existing risks | review enterprise access controls before and during deployment |

## Generative AI hard rules
- **Never** enter unpublished official info into public AI apps/APIs.
- **Never** train/fine-tune on data with differing user access permissions.
- **Never** let generative AI cause destructive/irreversible actions automatically → human review.
- **Treat LLM-generated code as inherently insecure** → code review + dependency scanning before production.
- **Avoid public LLM chatbots** unless prompt-injection risk is acceptable for the use case.
- Filter external links in responses; block dangerous URLs.

## Autonomy → risk
Higher autonomy = higher operational risk. Keep human intervention for autonomous decisions (e.g. social care/healthcare); control environment to avoid reintroducing bias.

## Tell-tale signs (tells & smells)
- "The model is accurate, why don't users follow it?" → model metrics vs service metrics mismatch; check trust/usability (Ch 3).
- Offline hit metrics look bad for a discovery recommender → expected; you recommend what users haven't touched (Ch 10).
- AI search suddenly surfaces sensitive data → over-privileged access / data leakage; review access controls (Ch 8).
- LLM recommends a package/lib that shouldn't exist → hallucination + possible typosquatting; verify dependencies (Ch 8).
- Same report summarised twice, different results → LLM output variability; design for human review (Ch 10).

## Decision tree: public LLM chatbot?
1. Is instant public access essential? → if not, use limited/controlled deployment.
2. Can we prevent direct prompt injection? → not fully; filters/meta-prompts reduce but don't eliminate.
3. Is a wrong/false answer acceptable? → if no, do not rely on it for facts; verify and gate on accuracy.
4. Human review possible for actions? → yes → proceed with safeguards; no → avoid autonomous actions.
