# Patterns

## 10 Principles Gate
**When to use**: deciding whether to start/proceed with any AI project in government.
**How**: check the project against all 10 principles (know limits, lawful/ethical, secure, human control, life cycle, right tool, open/collaborative, commercial from start, skills, org policies + assurance). Any failure → fix or stop.
**Trade-offs**: thorough, but some checks (e.g. human control) need interpretation per deployment mode.

## Right-Tool-for-the-Job Comparison
**When to use**: choosing whether AI is the answer at all.
**How**: ask "could a non-AI solution or a simpler ML model work just as well?" Compare volume, complexity, real-time and pattern-detection demands.
**Trade-offs**: avoids overengineering; risks rejecting AI when it genuinely adds value.

## Minimum Viable AI Team
**When to use**: staffing an AI project.
**How**: ensure the team can cover user needs/accessibility, stakeholder management, agile build/test/iterate, safe-by-design, ethical data handling, real-user testing, and live support/retirement.
**Trade-offs**: more roles up front; cheaper than retrofitting safety later.

## UR-for-AI Loop
**When to use**: building or evaluating an AI product.
**How**: run user research across the life cycle — right-tool check, metrics definition, data prep, synthesis, output evaluation (e.g. SME ratings), usability, attitudes, accessibility, actual usage, in-service monitoring.
**Trade-offs**: labour-intensive (GOV.UK Chat); yields baselines, bias insights and trust data.

## Use-Case Selection (Led by Need)
**When to use**: identifying AI opportunities.
**How**: start from user pain points; choose AI only where traditional tools can't handle volume/complexity/real-time needs; run cost-benefit; assess feasibility (skills, infrastructure, partners).
**Trade-offs**: disciplined; may slow adoption of low-risk experiments.

## Business Case Routing
**When to use**: preparing to fund an AI project.
**How**: near/above ~£10M → Green Book five-part case; below → agile business case; assure non-BAU spend >£100K (digital) / >£1M (tech).
**Trade-offs**: proportionate rigour vs speed.

## Framework vs DPS Route Selection
**When to use**: choosing a route to market.
**How**: use a framework when you want pre-vetted suppliers and low buyer effort; use a DPS when the market moves fast and new suppliers must be able to join anytime.
**Trade-offs**: frameworks = less buyer work but closed; DPS = flexible but more buyer-side compliance.

## AI Procurement Specification
**When to use**: drafting requirements for AI suppliers.
**How**: problem statement, data strategy, bias mitigation, transparency into supplier's AI approach, anti-lock-in, IPR, dummy data, budget guidance, liabilities/risk appetite, alignment with Data Ethics Framework and PSC.
**Trade-offs**: detailed specs take time; prevents opaque, non-transferable systems.

## Transparency-by-Level
**When to use**: deciding what to disclose about an AI system.
**How**: cover all five levels — technical (code/data), process (decisions), outcome (how decisions are made), internal (records), public (ATRS, labelling).
**Trade-offs**: public transparency builds trust but may expose proprietary detail — keep internal/technical records proportionate.

## Accountability Triad (Answerability–Auditability–Liability)
**When to use**: establishing responsible ownership of an AI system.
**How**: define responsibility chains across the life cycle + supply chain; document every stage accessibly; ensure all parties act lawfully; contract vendor responsibilities; nominate an SRO.
**Trade-offs**: documentation overhead; essential for defensibility.

## DPIA Walkthrough
**When to use**: any AI processing personal data (mandatory in listed scenarios).
**How**: 10 steps — purpose, necessity/proportionality, data inventory, lawful basis, roles, impact stages, views of individuals, human involvement stages, detriment from bias/inaccuracy, safeguards + residual risk.
**Trade-offs**: upfront effort; gates risky processing; consult ICO if high residual risk.

## Security-by-Deployment-Mode
**When to use**: securing an AI system.
**How**: apply controls matching the mode — public apps (educate users, no unpublished data), embedded AI (vendor mitigations, no unverified plugins), APIs (PETs, content filters, logging), self-hosted (own security), organisational data (leakage controls, access review).
**Trade-offs**: self-hosting gives control but heavy ownership; public tools are easy but un-controllable.

## Defend-in-Depth for Generative AI
**When to use**: mitigating prompt injection, leakage and hallucination.
**How**: filter prompts (ML-based detection), filter outputs, restrict in-context data (RAG over permitted data), block dangerous URLs, log and audit prompts, keep a human to review irreversible actions.
**Trade-offs**: multiple layers cost performance and latency; no layer fully stops injection.

## Governance-in-Place
**When to use**: standing up AI programme governance.
**How**: AI governance board (or representation on existing board); optional ethics committee; AI/ML systems inventory; team governance (roles, escalation, risk prioritisation, data reporting); risk management framework; AI quality assurance (validation, monitoring, managed revertible releases).
**Trade-offs**: process cost; necessary for oversight, assurance and audit.

## Accuracy-Gated Phased Rollout
**When to use**: launching a generative AI service.
**How**: phased experiments → measure accuracy (e.g. SME ratings, inter-rater agreement) → improve → launch limited pilot only if threshold met (~80% in GOV.UK Chat); build QA knowledge base for scale.
**Trade-offs**: slower to launch; avoids deploying hallucination-prone systems publicly.

## Assist-Don't-Replace (Human-in-the-Loop)
**When to use**: high-stakes or public-facing decisions (sensitivity review, moderation, findings).
**How**: AI processes volume and surfaces candidates; trained humans review, decide and remain responsible; provide human review/redress routes.
**Trade-offs**: limits automation gains; preserves accountability and trust.

## Start-Simple-Then-Scale Complexity
**When to use**: proving an AI solution works before investing in ML.
**How**: begin with rules/regex/heuristics to establish architecture (NHS.UK Flask app); then add more complex ML models once architecture and integration are proven.
**Trade-offs**: two phases of work; derisks the harder ML investment.
