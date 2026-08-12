# Chapter 6: Legal Considerations

## Core Idea
Most AI legal issues are not new — they build on existing law (data protection, contracts, IP, equality, public law, human rights). Engage legal advisers from the outset; many ethical issues your team identifies are legal issues too.

## Frameworks Introduced
- **Engage legal early (before contracts)**: when contacting your legal team, explain your aims, what the solution will do, and known risks. This reveals whether you need legislation, and minimises risk of court challenge, unintended/unethical consequences, and negative impact on intended beneficiaries.
- **Example legal issues checklist** (illustrative, not advice): data protection; contractual issues; IP/copyright; equality; public law principles; human rights; legislation.

## Key Concepts
- **Data protection**: a legal issue with serious consequences if government gets it wrong; work with your DPO and legal team (→ Ch 7).
- **Contractual issues**: IP handling, transparency levels needed for buyers to understand the system, transfer to successor suppliers, defence against legal challenge, procedures for system errors/outages.
- **IP and copyright**: decide up front who owns which parts of generated IP, who has ongoing use rights (and on what basis), and how risk/liability is balanced between parties for third-party infringement claims.
- **Equality Act 2010 / Public Sector Equality Duty**: obligations that AI must not undermine; an equality impact assessment is one way to guard against bias.
- **Public law principles**: public bodies must act rationally, fairly, lawfully and compatibly with human rights. Procedural fairness = how a decision is arrived at (transparency/explainability is key to demonstrating it). Rationality = relevant when testing the choice of AI system, features, outcomes and metrics.
- **Human rights (ECHR)**: public authorities must act compatibly; AI using personal data may affect rights — especially Article 8 (private/family life) and Article 10 (freedom of expression).

## Mental Models
- Use **"procedural fairness"**: for decisions, the how matters as much as the what — an opaque AI tool can't demonstrate a fair procedure.
- Use **"delegation test"**: public law helps decide whether a decision should be delegated to a decision-maker rather than automated; in regulated settings, automated decisions risk challenge unless fairness, lack of bias and rationality are evidenced.
- Use **"legislation check"**: confirm whether your use is within the current legal framework or needs new legislation (e.g. the framework may not allow the process to be delegated to a machine).

## Anti-patterns
- **Treating AI legal issues as novel**: most are established areas of law — go to your lawyers, who already have the frameworks.
- **Bringing legal in after contracts are signed**: equality impact and other assessments are most effective early.
- **Automating regulated decisions without evidence**: without demonstrated procedural fairness, lack of bias and rationality, automated decisions in procurement-like environments are challengeable.

## Worked Example
**Legal intake for an AI decision-support tool.** A team plans an AI that recommends which benefit claimants need review.
- Legal brief: aims (prioritise reviews), capability (ranking via ML), risks (bias, opacity).
- Data protection: DPIA required (→ Ch 7); DPO consulted.
- Public law: procedural fairness demands explainability of the ranking; a human must make the final decision — AI only supports (meaningful human control).
- Equality: impact assessment against protected characteristics before sign-off.
- Legislation: confirm no new legislation needed; automated *decisions* would be restricted.
Result: proceed with human-in-the-loop design, documented explainability, and DPIA.

## Key Takeaways
1. Engage legal at the outset; brief them on aims, capabilities and known risks.
2. Decide IP ownership, use rights and liability distribution early — contracts drive route-to-market choices.
3. Demonstrate procedural fairness through transparency and explainability.
4. Use the delegation test: keep significant decisions with human decision-makers.
5. Check whether your use fits existing legislation or needs new legislation.

## Connects To
- **Ch 1**: Principle 2 (lawful, ethical, responsible)
- **Ch 4**: contracts and procurement legalities
- **Ch 5**: ethics issues overlap legal issues
- **Ch 7**: data protection as the main legal issue for personal data
- **Ch 9**: governance and risk management embed legal compliance
