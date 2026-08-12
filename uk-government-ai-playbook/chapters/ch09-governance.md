# Chapter 9: Governance

## Core Idea
Strong governance is essential for any AI programme because of risks around lawfulness, security, bias and data. It provides oversight, accountability and strategic direction via a governance board, optional ethics committee, an AI systems inventory, clear team structures, risk management and AI quality assurance.

## Frameworks Introduced
- **Governance structure options**: an AI governance board or AI expert representation on an existing board provides oversight, accountability and strategic guidance (risk management, compliance, assurance, resource allocation, stakeholder engagement, alignment with objectives). An **ethics committee** is more specialised — assesses ethical implications (fairness, transparency, privacy), includes legal experts, other relevant organisations, community members and stakeholders. Use an ethics committee only where context warrants it; a board can advise whether you need one.
- **AI/ML systems inventory**: a live inventory of all deployed AI systems, in addition to ATRS records. Keep up to date with purpose/usage/risks, data elements, ownership, dates, and use protocols. Use for oversight of risks (data quality, accuracy, bias, security, compliance) and audit.
- **Risk management approach**: risk assessment determines whether benefits outweigh risks (base on objective assessment, define acceptable risk levels, identify risks early). Build a risk management framework with defined roles, responsibilities and escalation routes. Consider autonomy: more autonomy (e.g. SAE driving-automation scale 0–5) correlates with higher operational risk.
- **AI quality assurance**: ensures the service meets requirements and is fit for purpose — trustworthy, accountable, transparent, robust, safe, privacy-respecting, bias-mitigated, fair, secure and resilient. Uses tools like risk assessment, impact assessment, bias audit, compliance audit, conformity assessment and formal verification.

## Key Concepts
- **Validation**: "confirmation, through the provision of objective evidence, that the requirements for a specific intended use or application have been fulfilled" (ISO 9000:2015); part of change control with quantitative testing.
- **Model drift**: system/environment evolution diverges from training period → retrain or replace; catch via close monitoring.
- **Managed release process**: updates go through a controlled release; the release must be withdrawable and reverted if needed.
- **Risk prioritisation plan**: specific project controls throughout delivery and post-delivery (e.g. how data sets are evaluated for bias).
- **Escalation pathways**: clear routes and points of contact for AI-related issues.

## Mental Models
- Use **"governance = continuous improvement + stakeholders + sustainability"**: focus governance on new knowledge/methods, broad stakeholder engagement (incl. Civil Society Organisations), and long-term sustainability.
- Use **"autonomy scales risk"**: higher AI autonomy → higher operational risk → more human intervention required; decisions in social care/healthcare need controlled environments with human oversight to avoid reintroducing bias.
- Use **"guardrails not just reviews"**: programme and technical guardrails guide design, implementation and operation; evaluate across the whole life cycle.

## Anti-patterns
- **Creating an ethics committee when it's overkill**: a small department or low-risk programme may only need a governance board or an AI expert on the programme board.
- **No continuity plan for AI knowledge**: without knowledge-transfer and training plans, the model can't be sustainably managed.
- **Releasing updates without managed release or revert capability**: risks uncontrolled impact.
- **Ignoring model drift**: systems diverge from training; without monitoring you keep an unfit model in service.

## Worked Example
**Setting up governance for a department's first AI project.**
- Board: senior leaders + experts approve the use case against AI principles; AI representative on the existing programme board.
- Inventory: register the system — purpose, data elements, owner, risks, dates; share with the AI community of practice.
- Team structure: maintenance plan, knowledge transfer and training, clear roles (who may modify code), diversity, escalation pathways, risk prioritisation plan, data reporting mechanism.
- Risk: risk assessment on benefits vs harms; autonomy level kept low with human-in-the-loop; OWASP-style risk rating for security.
- Quality assurance: DSIT's Introduction to AI assurance techniques; quantitative validation as part of change control; operational monitoring with managed release and revert.
Result: oversight, accountability and evidence that the service stays fit for purpose.

## Key Takeaways
1. Put AI governance on a board — dedicated or as representation on an existing one; add an ethics committee only when context warrants.
2. Maintain a live AI/ML systems inventory and share it with the community of practice.
3. Give teams clear governance: maintenance, knowledge transfer, roles, diversity, escalation, risk prioritisation and data reporting.
4. Use risk assessment + risk management framework; treat autonomy as a risk multiplier.
5. Apply AI quality assurance across the life cycle, with quantitative validation, operational monitoring and managed (revertible) releases.

## Connects To
- **Ch 1**: operationalises Principles 7 and 10
- **Ch 3**: the AI support structure includes the governance board
- **Ch 5**: ethics committee draws on the six ethics themes
- **Ch 6**: legal compliance embedded in governance
- **Ch 7**: data protection accountability sits in governance
- **Ch 8**: risk rating and security controls feed the risk framework
- **Ch 10**: case studies show real assurance processes (e.g. NHS reviews sign-off)
