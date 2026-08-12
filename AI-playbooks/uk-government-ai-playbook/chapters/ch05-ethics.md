# Chapter 5: Using AI Safely and Responsibly (Ethics)

## Core Idea
Ethical AI use rests on six themes: safety/security/robustness, transparency & explainability, fairness/bias/discrimination, accountability & responsibility, contestability & redress, and societal wellbeing & public good. They overlap and sometimes trade off against each other — decide explicitly whether benefits outweigh risks and whether any risks are unacceptable.

## Frameworks Introduced
- **The 6 ethics themes**: the playbook's organising framework for responsible AI. Use each as a review lens over the full life cycle.
  1. Safety, security and robustness
  2. Transparency and explainability
  3. Fairness, bias and discrimination
  4. Accountability and responsibility
  5. Contestability and redress
  6. Societal wellbeing and public good
- **5 types of transparency**: technical (code, training data), process (design/development/deployment decisions), outcome-based (how the solution works and what factors drive decisions), internal (up-to-date internal records), public (communication to the public in open format). Use to decide what to document and disclose at each level.
- **Answerability–auditability–liability (accountability)**: answerability = a chain of human responsibility across the life cycle incl. supply chain; auditability = documenting every stage so stakeholders can understand it; liability = all parties act lawfully and understand obligations.

## Key Concepts
- **Representational bias**: people under/over/misrepresented in training data → harmful stereotypes, abusive content, performance disparities across groups.
- **Contestability and redress**: mechanisms to challenge AI systems/outputs (public awareness, appeal mechanisms, change processes) — designed before deployment, maintained for the life cycle.
- **Justified trust**: public trust earned by competent, responsible, ethical development — essential for adoption.
- **Trade-offs**: promoting one value can hurt another (e.g. collecting demographic data for fairness vs privacy); assess early and explicitly.
- **ATRS**: recording standard for algorithmic tools in decision-making; mandatory for central departments and in-scope arm's length bodies.

## Mental Models
- Use **"transparency has levels"**: choose what to disclose at technical vs process vs outcome vs internal vs public level — each serves different audiences.
- Use **"bias is life-cycle-wide"**: bias enters through data, prompts, and deployment interactions; evaluate continuously, including intersectional groups.
- Use **"net positive impact"**: ensure AI generates net positive benefit to stakeholders and society; if negative consequences are too high, terminate the project.

## Anti-patterns
- **Relying on redress alone**: contestability/redress mitigate harm but don't prevent it — harms may not be apparent to all impacted; prevent via the other themes.
- **Ignoring bias until after testing**: fairness issues can appear in implementation even when tests passed — users may ignore or selectively follow recommendations.
- **Using AI for misinformation-prone outputs unchecked**: generative AI spreads plausible false content; verify outputs and assess misinformation risk.
- **Not weighing environmental impact**: training your own model when a suitable pre-trained one exists; ignoring provider energy credentials.

## Worked Example
**Applying the ethics review to a generative AI chatbot.**
- Safety/security/robustness: red-team the model; log behaviour in anomalous scenarios; content filters in place.
- Transparency: publish ATRS record; label responses "written by an automated AI chatbot"; keep model/data cards internally.
- Fairness/bias: test outputs across protected characteristics and intersectional groups; review prompts for bias; monitor post-deployment.
- Accountability: nominate an SRO; contractually define vendor responsibilities; human-in-the-loop for high-impact outputs.
- Contestability/redress: public signposting of reporting routes; contingency plan if the system must be stopped.
- Societal wellbeing: weigh benefits vs harms (e.g. misinformation risk); verify outputs; assess environmental cost.
All six pass → deploy. Otherwise fix or stop.

## Key Takeaways
1. Run the six ethics themes as review lenses across design, deployment and operation.
2. Disclose at the transparency level the audience needs; comply with ATRS where required.
3. Evaluate fairness across the full life cycle, including intersectional groups and post-deployment behaviour.
4. Establish accountability (answerability, auditability, liability), nominate an SRO, and keep human oversight for high-impact outputs.
5. Design contestability and redress mechanisms before deployment, and ensure net positive societal impact.

## Connects To
- **Ch 1**: deepens Principles 2, 4, 7
- **Ch 3**: safe/responsible-by-design is a team requirement
- **Ch 4**: ethics → procurement requirements
- **Ch 6**: many ethics issues are also legal issues
- **Ch 7**: fairness, transparency and human oversight map to data protection principles
- **Ch 8**: safety and security themes ground the security chapter
- **Ch 9**: governance and assurance operationalise accountability
