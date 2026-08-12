# Chapter 8: Policy, Ethics & Standards

## Core Idea
The appendices turn the framework's principles into compliance: six responsible-AI policies cities should adopt, and the international legislation, standards, and guidelines (CRPD, EU AI Act, WCAG, ISO, UNESCO) that anchor inclusive AI work — giving teams a checklist for lawful, ethical deployment.

## Frameworks Introduced
- **Responsible AI Policy Suite (Appendix C)** — six policies a city should have in place:
  1. **Data Privacy and Consent Policy**: be transparent about what data is collected, how it is used, and who has access; use anonymization, privacy-enhancing technologies (PETs), and synthetic data; provide opt-out mechanisms and clear avenues for data-misuse complaints. Models to copy: Seattle's Privacy Statement and Surveillance Ordinance.
  2. **Bias Mitigation Policy**: ensure training data is diverse and representative; regularly assess algorithms for fairness using fairness metrics; run demographic impact assessments; involve independent experts; share evaluations with civil society, industry, and academia.
  3. **Transparency and Accountability Policy**: communicate how algorithms make decisions in understandable formats; give individuals mechanisms to understand and challenge algorithmic decisions; publish documentation publicly (Helsinki's AI Register is the model).
  4. **Accessibility and Inclusivity Policy**: require accessibility features across all public technology including AI; test and validate for accessibility compliance; train procurement officers buying from external vendors.
  5. **Copyright Policy**: avoid training public-sector AI on copyrighted material where possible; be prudent with generative AI integrations and prepared to roll back — these technologies are not yet mature enough to serve as critical public infrastructure.
  6. **Civil Rights Protection Policy**: set clear guidelines before deploying AI in profiling, surveillance, or predictive policing; stipulate where AI must not be used (law enforcement, court systems, public assistance); align with EU AI Act risk levels; engage civil rights organizations; consider a regulatory body overseeing AI in city planning.
- **International Standards Landscape (Appendix B)** — the instruments that anchor the work:
  - **Human rights base**: World Programme of Action (1982), Standard Rules (1994), **UN CRPD (2006)** — Article 9 (equal access to physical environment, transportation, information, and communications) and Article 20 (personal mobility); 2030 Agenda / SDG10 (reduced inequalities).
  - **AI governance**: Universal Guidelines for AI (2018), OECD AI Principles (2019), UNESCO Recommendations on AI Ethics (2021, including do-no-harm, fairness, human oversight, transparency, accountability), G7 Hiroshima Process Principles (2023), **EU AI Act (2023)** — risk-tiered regulation (minimal, limited, high-risk, unacceptable).
  - **Technical standards**: ISO 21542:2011 (building accessibility), ISO 71:2014 (accessibility guide), **WCAG 2.0** (web content), ETSI EN 301549 (ICT accessibility), U.S. Sections 504/508 (universally applicable principles), Washington Group Short Set (disability data collection).

## Key Concepts
- **EU AI Act risk levels**: minimal, limited, high-risk, and unacceptable — high-risk systems (e.g. critical infrastructure, elections) face strict regulation; transparency is required even at minimal risk.
- **Privacy-enhancing technologies (PETs)**: techniques that protect individuals' identity while still enabling valuable AI applications.
- **Fairness metrics**: quantitative checks that an algorithm's outcomes are equitable across demographic or geographic groups.
- **AI Register**: a public inventory describing each AI system, its data, oversight, and risk handling — Amsterdam (2020) and Helsinki both maintain one.
- **Synthetic data**: generated data used as a privacy-preserving alternative to real personal data.

## Mental Models
- **Think of the policy suite as the framework's enforcement layer**: the Ten Step Framework says what to do; these six policies make it a legal and organizational requirement.
- **Use the standards as a sourcing ladder**: when unsure what "good" looks like, climb from WCAG (web) to ISO (built environment) to CRPD (human rights) to EU AI Act (regulation).
- **Generative AI = higher caution**: treat generative tools as not-yet-mature for critical public infrastructure — prudent integration, rollback-ready.
- **Transparency is the through-line**: AI Register, public documentation, and challenge mechanisms all serve the same goal — accountable, explainable city AI.

## Anti-patterns
- **Collecting indiscriminately**: gathering large datasets without privacy safeguards in pursuit of "more data"; the playbook warns this harms the people the AI is meant to help.
- **Publishing without the right to publish**: training public AI on copyrighted material, or integrating generative AI without rollback plans.
- **Deploying in high-risk domains unregulated**: using AI in law enforcement, courts, or public assistance without explicit civil rights guidelines.
- **Checking bias only in theory**: claiming fairness without fairness metrics, demographic impact assessments, or independent review.
- **Treating standards as optional**: skipping WCAG/ISO/CRPD alignment because "the tool is AI, not a website" — accessibility requirements cover all public technology.

## Worked Example
Policy walk-through for a city deploying a sidewalk-accessibility AI (the Amsterdam model):

1. **Privacy**: street-level point-cloud data may capture people and vehicles — apply anonymization/PETs, publish what is collected and who can access it (Seattle-style), and enable opt-out where feasible.
2. **Bias**: the model must perform fairly across all neighborhoods — run demographic impact assessments and fairness metrics before any funding decision uses its output.
3. **Transparency**: register the tool in a public AI Register (what it does, its data, how humans oversee it) and document decisions so residents can challenge outcomes.
4. **Accessibility**: the resulting mapping service must meet WCAG 2.0 and ETSI EN 301549, and procurement contracts must encode those requirements.
5. **Civil rights**: scope the tool strictly to infrastructure assessment — no predictive-policing or surveillance spillover, consistent with EU AI Act risk tiers.

Each policy maps to a concrete, checkable action — which is exactly how the suite is meant to be used.

## Key Takeaways
1. Adopt the six responsible-AI policies before deploying public AI — privacy, bias, transparency, accessibility, copyright, and civil rights.
2. Publish an AI Register and public documentation; give residents a way to challenge algorithmic decisions.
3. Anchor project claims in the international landscape: CRPD for rights, EU AI Act for regulation, WCAG/ISO/ETSI for technical compliance.
4. Apply stricter caution to generative AI — integrate prudently, keep rollback options, avoid copyrighted training data.
5. Treat fairness metrics and demographic impact assessments as mandatory, not optional, deliverables.

## Connects To
- **Ch 02**: the five ethical principles are the philosophical base these policies operationalize.
- **Ch 04**: the Step 4 risk toolkit (transparency, accessibility reviews, pre-mortem) expands into these formal policies.
- **Ch 07**: the Amsterdam project demonstrates the practices — AI Register, open code, bias-mitigated labeling — this chapter codifies.
