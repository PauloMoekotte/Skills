---
name: amsterdam-ai-playbook
description: "Knowledge base from \"AI Playbook for Inclusive and Accessible Cities\" by the City of Amsterdam CTO Office & World Enabled. Use when applying the Ten Step Framework for inclusive AI, planning accessible city technology, mitigating AI bias and risk, engaging disability stakeholders, or referencing inclusive urban AI concepts and policy."
---

<!-- argument-hint: [topic, framework name, or chapter number] -->

# AI Playbook for Inclusive and Accessible Cities
**Author**: City of Amsterdam (CTO Office) & World Enabled | **Pages**: ~49 | **Chapters**: 8 | **Generated**: 2026-08-08

## How to Use This Skill

- **Without arguments** — load core frameworks for reference
- **With a topic** — ask about `stakeholder engagement`, `bias`, `procurement`, `monitoring`, or another indexed topic; I find and read the relevant chapter
- **With chapter** — ask for `ch05`; I load that specific chapter
- **Browse** — ask "what chapters do you have?" to see the full index

When you ask about a topic not covered in Core Frameworks below, I will read
the relevant chapter file before answering.

---

## Core Frameworks & Mental Models

### Ten Step Framework for developing inclusive AI
The master process for any AI-for-inclusion project. Run steps in order, but loop back to stakeholders at Steps 2, 4, and 7.
1. **Engage Stakeholders and Define Values** — engage advocacy groups and community organizations; agree on values; ask proactively about privacy, human rights, and civil liberties risks.
2. **Identify Barriers to Inclusion** — with stakeholders, identify specific accessibility challenges for older persons and people with disabilities.
3. **Conduct a Technology and Data Inventory** — review existing technology and datasets for tool development and performance monitoring.
4. **Anticipate and Mitigate Risks** — identify ethical risks (accessibility, fairness, bias, data privacy, misuse) before committing to new technology.
5. **Select a Technology Solution** — engage experts; estimate feasibility; define scope.
6. **Develop a Prototype or Pilot** — test small before scaling.
7. **Review Initial Results and Adjust** — gather feedback; identify strengths and improvements.
8. **Scale** — expand to larger areas and services; build a monitoring framework.
9. **Support Through Communication and Training** — raise awareness and train users.
10. **Monitor and Evaluate** — evaluate impact; build in ongoing community feedback; share findings responsibly.

**Nothing about us without us** is the standing test: was the affected community genuinely in the room?

### Three Categories of AI Applications
Classify any municipal AI before assessing it — the category sets the risk profile and inclusion levers.
- **Anticipatory** (predicts from historical data) — traffic, energy, healthcare staffing; bake inclusion goals into predictions.
- **Generative** (creates content) — chatbots, legislative text, urban renderings; use with proactive guidance for inclusive conversations.
- **Decisive** (automates recommendations) — resource allocation, infrastructure decisions; audit for equitable, inclusive outcomes.

### Seven AI Capabilities for Inclusion
Use to brainstorm and scope use cases: **Detection & Classification** (asset inventories, sign-language interpretation), **Forecasting & Prediction** (asset failure, disaster alerting), **Clustering** (economies of scale), **Optimization** (prioritize infrastructure by cost/inclusivity/equity), **Anomaly Detection** (wheelchair-accessible transit updates, fall detection), **Decision-making** (assistive navigation, adaptive traffic signals), **Generation** (service chatbots).

### Five Ethical Principles
Validate every decision against: **Accessibility** (usable by everyone; train users), **Transparency and Accountability** (explain in non-technical terms, especially when AI replaces humans), **User-Centered Design** (engage users in design/testing), **Diversity and Representation** (diverse training data; test/correct bias), **Scalability and Sustainability** (funding longevity; weigh energy/water use).

### Risk Toolkit (Step 4)
- **Proactive Transparency** — plain-language explanations; maintain an **AI Register** listing every tool, its data, oversight, and risk handling; open by default unless privacy.
- **Accessibility Reviews** — every product undergoes one; encode goals into procurement so vendors are bound.
- **Pre-mortem** — reviewers imagine the project already failed and enumerate why; include lived-experience experts.

### Evaluation Toolkit (Step 7)
- **Bug bashing** — first-time users record every issue as a bug.
- **Red teaming** — testers intentionally try to produce errors and harmful outcomes.
- **Outcomes assessments** — score **accuracy** AND **fairness** (demographic/geographic/user characteristics); fairness is the harder, essential half.
- **Accessibility safari** — validate AI output against physical ground truth, e.g. students measuring sidewalk widths.

### Evaluation & Monitoring Essentials
- KPIs measure **fairness, accuracy, and quality of service** — not just speed/cost.
- **Multi-tiered monitoring**: weekly core-team KPI check-ins + quarterly/annual community assessments; resource a dedicated project manager or participatory work collapses.
- **Compensate participation** — budget for paying lived-experience experts; unpaid "representation" is a smell.

### Feasibility Gate (Step 5)
AI is not always the answer. Gate every choice on: right **data** (diverse, representative), right **skills**, right **budget** for a small test, acceptable **privacy/civil-liberty risk**, and AI genuinely better than improving existing technology. Let the accessibility problem dictate the data (Amsterdam needed 3D point clouds because 2D maps can't show obstacles).

### Anti-patterns
- Prescribing AI before any inventory is done.
- Scaling before the pilot is validated; one-shot consultation instead of lifecycle engagement.
- Measuring accuracy only; collecting data no one owns; deploying generative AI as critical infrastructure.

---

## Chapter Index

| # | Title | Key Frameworks |
|---|-------|----------------|
| [ch01](chapters/ch01-foundations-ai-inclusive-cities.md) | Foundations — AI for Inclusive Cities | Three AI categories, seven capabilities, AI risks |
| [ch02](chapters/ch02-ten-step-framework-principles.md) | The Ten Step Framework & Core Principles | Ten Step Framework, five ethical principles, Tada Manifesto |
| [ch03](chapters/ch03-steps-1-3-engage-identify-inventory.md) | Steps 1–3 — Engage, Identify, Inventory | Asset inventory, barrier categorization, data inventory |
| [ch04](chapters/ch04-steps-4-5-risk-solution-selection.md) | Steps 4–5 — Anticipate Risk, Select the Solution | Risk toolkit, pre-mortem, AI Register, feasibility gate |
| [ch05](chapters/ch05-steps-6-7-prototype-review.md) | Steps 6–7 — Prototype, Review, Adjust | Prototype/pilot, bug bashing, red teaming, outcomes assessments |
| [ch06](chapters/ch06-steps-8-10-scale-train-monitor.md) | Steps 8–10 — Scale, Communicate, Monitor | Scale with guardrails, communication & training, multi-tiered monitoring |
| [ch07](chapters/ch07-case-study-amsterdam-for-all.md) | Case Study — Amsterdam for All | Framework in action, 3D sidewalk mapping, accessibility safari |
| [ch08](chapters/ch08-policy-ethics-standards.md) | Policy, Ethics & Standards | Responsible AI policy suite, CRPD, EU AI Act, WCAG/ISO |

## Topic Index

- **Accessibility** → ch01, ch02, ch08
- **AI Register / transparency** → ch04, ch08
- **AI is not always the answer (feasibility gate)** → ch04
- **Anticipatory / generative / decisive AI** → ch01
- **Barriers to inclusion** → ch03
- **Bias / algorithmic bias** → ch01, ch03, ch08
- **Bug bashing** → ch05
- **Case study (Amsterdam for All)** → ch07
- **Communication & training** → ch06
- **Compensation for participation** → ch03
- **Data inventory / datasets** → ch03
- **Digital redlining** → ch01
- **Ethical Leaflet / Tada Manifesto** → ch02
- **EU AI Act** → ch08
- **Evaluation / outcomes assessments** → ch05, ch06
- **Feasibility / solution selection** → ch04
- **Generative AI caution** → ch01, ch08
- **Lived experience / nothing about us without us** → ch02, ch03, ch07
- **Monitoring & evaluation** → ch06
- **Pre-mortem** → ch04
- **Privacy / data consent** → ch08
- **Procurement / accessibility reviews** → ch04, ch08
- **Prototype / pilot** → ch05
- **Red teaming** → ch05
- **Risk mitigation** → ch04
- **Scale / scaling** → ch06
- **Stakeholder engagement** → ch02, ch03
- **Standards (WCAG, ISO, CRPD)** → ch08
- **Ten Step Framework** → ch02
- **Universal Design** → ch01
- **Validation (accessibility safari)** → ch05, ch07

## Supporting Files

- [glossary.md](glossary.md) — all key terms with definitions
- [patterns.md](patterns.md) — all techniques and design patterns
- [cheatsheet.md](cheatsheet.md) — quick reference tables and decision guides

---

## Scope & Limits

This skill covers the book content only: the Ten Step Framework, inclusive-AI principles, the Amsterdam case study, and the policy/ethics appendix material. For hands-on implementation in your codebase, combine with project-specific tools. For topics beyond this book, check related skills or ask the agent directly.
