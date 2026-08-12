---
name: uk-government-ai-playbook
description: "Knowledge base from \"Artificial Intelligence Playbook for the UK Government\" by the Government Digital Service (GDS). Use when applying the 10 principles for safe/responsible AI in government, assessing AI use cases, ethics, data protection, procurement, AI security, governance, or referencing the playbook's concepts and case studies."
---

<!-- argument-hint: [topic, framework name, or chapter number] -->

# Artificial Intelligence Playbook for the UK Government

**Author**: Government Digital Service (GDS), Cabinet Office | **Pages**: ~118 | **Chapters**: 10 | **Generated**: 2026-08-08

## How to Use This Skill

- **Without arguments** — load core frameworks for reference
- **With a topic** — ask about `procurement`, `data protection`, `prompt injection`, `DPIA`, or another indexed topic; I find and read the relevant chapter
- **With chapter** — ask for `ch05`; I load that specific chapter
- **Browse** — ask "what chapters do you have?" to see the full index

When you ask about a topic not covered in Core Frameworks below, I will read
the relevant chapter file before answering.

---

## Core Frameworks & Mental Models

**The 10 Principles for AI in government** — the master acceptance criteria. Apply all ten to any AI project; a failure on any is a fix-or-stop signal. Know limits (P1) · lawful/ethical/responsible (P2) · secure (P3) · meaningful human control (P4) · full life cycle (P5) · right tool for the job (P6) · open & collaborative (P7) · commercial colleagues from the start (P8) · skills & expertise (P9) · org policies + assurance (P10).

**Right tool for the job** — when choosing a technology, be as open to "AI is not the answer" as to AI itself. Use AI when traditional tools can't handle the volume, complexity or real-time demands, or when you need pattern detection/personalisation. Avoid fully automated decision making on significant decisions and high-risk/high-impact solo-AI applications.

**Meaningful human control at the right stage** — for slow, high-impact decisions put a human in the loop (validating outputs). For instant-response apps (chatbots), move human control into pre-deployment testing, live monitoring, and user "report → human review" redress. Where risks are too high, reconsider whether AI should be used at all.

**The 6 ethics themes** — review every AI system against safety/security/robustness, transparency & explainability, fairness/bias/discrimination, accountability & responsibility, contestability & redress, and societal wellbeing & public good. Themes overlap and can trade off (e.g. fairness data collection vs privacy) — decide explicitly whether benefits outweigh risks.

**5 types of transparency** — technical (code/data), process (decisions/practices), outcome-based (how decisions are made), internal (records), public (ATRS, labelling). Disclose at the level each audience needs; comply with the Algorithmic Transparency Recording Standard (ATRS) where in scope; label automated responses to the public.

**Accountability triad** — answerability (chain of human responsibility incl. supply chain), auditability (document every stage accessibly), liability (all parties lawful; vendor responsibilities contractual). Nominate a Senior Responsible Owner (SRO).

**DPIA (10 steps)** — the mandatory data-protection risk process for AI: purpose, necessity/proportionality, data inventory, lawful basis, roles, impact stages, views of individuals, human-involvement stages, bias/detriment, safeguards + residual risk. Mandatory for profiling with significant effects, large-scale special-category data, large-scale public-area monitoring, and innovative technologies.

**10 data protection principles for AI** — accountability · lawfulness · purpose limitation · transparency & individual rights · fairness · data minimisation · storage limitation · human oversight · accuracy · security. Treat AI outputs as "statistically informed guesses, not facts". Article 22 UK GDPR prohibits solely-automated decisions with legal/significant effects.

**Security-by-deployment-mode** — match controls to how AI runs: public apps (educate users; never enter unpublished official data), embedded AI (vendor mitigations; no unverified plugins), APIs (PETs, content filters, logging), self-hosted (own security/updates), organisational data (leakage controls + access review). Open vs closed source: neither inherently more secure.

**Generative AI hard rules** — never train/fine-tune on data with differing access permissions · never let generative AI take destructive/irreversible actions without human review · treat LLM-generated code as inherently insecure until reviewed · avoid public LLM chatbots unless prompt-injection risk is acceptable · generative AI cannot be trusted for facts.

**Buying AI** — business case by scale (~£10M+ → Green Book five-part case; below → agile case; assure >£100K digital / >£1M tech spend) · framework vs DPS route by market speed · specification must cover data quality, bias mitigation, transparency, anti-lock-in, IPR, dummy data, liabilities, and align with the Data Ethics Framework and PSC.

**Governance** — AI governance board (or representation on an existing board) + optional ethics committee · live AI/ML systems inventory (beyond ATRS) · team governance (roles, escalation, risk prioritisation, data reporting) · risk management treating autonomy as a risk multiplier · AI quality assurance with quantitative validation, operational monitoring, and managed revertible releases.

---

## Chapter Index

| # | Title | Key Frameworks |
|---|-------|----------------|
| [ch01](chapters/ch01-principles.md) | The 10 Principles | 10 Principles, human control at the right stage |
| [ch02](chapters/ch02-understanding-ai.md) | Understanding AI | OECD definition, fields hierarchy, limitations |
| [ch03](chapters/ch03-building-ai-solutions.md) | Building AI Solutions | Minimum viable team, 5 learner groups, UR-for-AI, use cases to avoid |
| [ch04](chapters/ch04-buying-ai.md) | Buying AI | Business case routing, framework vs DPS, AI spec |
| [ch05](chapters/ch05-ethics.md) | Using AI Safely & Responsibly (Ethics) | 6 ethics themes, 5 transparency types, accountability triad |
| [ch06](chapters/ch06-legal-considerations.md) | Legal Considerations | Legal early, public law, delegation test |
| [ch07](chapters/ch07-data-protection.md) | Data Protection & Privacy | 10 DP principles, DPIA 10 steps, PETs, Article 22 |
| [ch08](chapters/ch08-security.md) | Security | Deployment-mode matrix, AI risk taxonomy, prompt injection |
| [ch09](chapters/ch09-governance.md) | Governance | Governance board, inventory, risk mgmt, QA |
| [ch10](chapters/ch10-case-studies.md) | Case Studies (Appendix) | RAG pattern, UR-for-AI, assist-don't-replace |

## Topic Index

- **Accountability** → ch05, ch09
- **Agentic AI** → ch02
- **ATRS** → ch01, ch05, ch09
- **Bias** → ch02, ch05, ch07
- **Business case** → ch04
- **Chatbot safety** → ch08, ch10
- **Data leakage** → ch08
- **Data minimisation** → ch07
- **Data protection / GDPR** → ch06, ch07
- **DPIA** → ch07
- **Ethics** → ch05
- **Fairness** → ch05, ch07
- **Generative AI** → ch02, ch08, ch10
- **Governance** → ch09
- **Hallucination** → ch02, ch08
- **Human oversight / control** → ch01, ch07
- **Intellectual property** → ch04, ch06
- **Legal** → ch06
- **Life cycle management** → ch01, ch09
- **Procurement / Buying AI** → ch04
- **Prompt injection** → ch08
- **Right tool for the job** → ch01, ch02, ch03
- **Security** → ch08
- **Skills & talent** → ch03
- **Transparency / explainability** → ch05, ch07
- **Use cases** → ch03, ch10
- **User research for AI** → ch03, ch10

## Supporting Files

- [glossary.md](glossary.md) — all key terms with definitions
- [patterns.md](patterns.md) — all techniques and design patterns
- [cheatsheet.md](cheatsheet.md) — quick reference tables and decision guides
- [gaps-education-context.md](gaps-education-context.md) — Dutch gap analysis for education contexts, cross-referencing uk + amsterdam + vlaanderen playbook skills, with actionable checklist
- [intro-bestuurders-directeuren.md](intro-bestuurders-directeuren.md) — Dutch one-pager for governors/directors: key decisions and first steps
- [intro-docenten-onderwijsmanagers.md](intro-docenten-onderwijsmanagers.md) — Dutch one-pager for teachers/education managers: classroom do's & don'ts

---

## Scope & Limits

This skill covers the playbook content only (Feb 2025, GDS/Cabinet Office). It is a decision aid, not legal advice — consult your organisation's lawyers, DPO, commercial and security teams for specific situations. For hands-on implementation in your codebase, combine with project-specific tools. For topics beyond this book, check related skills or ask the agent directly.
