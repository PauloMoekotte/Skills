# Chapter 3: Building AI Solutions

## Core Idea
Building an AI solution is a multidisciplinary, user-led process: form the right team, acquire the right skills, define the goal from user needs, do AI-specific user research, choose use cases AI can actually win, and put an organisational support structure in place. Technology is only part of it.

## Frameworks Introduced
- **Minimum viable AI team**: a team that can (1) identify user needs and accessibility requirements, (2) manage stakeholders and collaborate with field experts, (3) design/build/test/iterate using agile, (4) ensure lawful, ethical, secure and safe-by-design development, (5) handle data ethically/ safely/ securely, (6) test with real users and measure performance, (7) support live running, iterate and retire the service. Use it as a checklist when staffing a project.
- **5 learner groups for AI skills** (CDDO cross-government user research): Beginners, Technical roles outside digital & data, Data & analytics professionals, Digital professionals, Leaders. Use to target learning by audience — each group has a distinct learning focus (awareness → safe tool use → analytics → building → strategy/culture).
- **User research for AI (9 applications)**: right-tool check, defining performance metrics, preparing data, synthesising data, evaluating model output, measuring usability, understanding attitudes, accessibility, identifying actual usage, and in-service monitoring. Use UR throughout the life cycle, not just upfront.

## Key Concepts
- **Model metrics vs service metrics**: model metrics measure how well the technology performs; service metrics measure whether user needs and business goals are met. They can diverge — a high-accuracy model can be ignored by users through lack of trust.
- **RLHF (reinforcement learning from human feedback)**: humans rank outputs to train models — useful for tasks hard to specify but easy to judge (e.g. bias-free, non-toxic text).
- **Use cases to avoid**: fully automated decision making on significant decisions (health, safety) and high-risk/high-impact applications used on their own.
- **AI support structure**: AI strategy & adoption plan, AI principles, AI governance board, AI communication strategy, AI sourcing & partnership strategy, AI training — plus optional change management team, use cases register, monitoring systems, review/change processes, fallback processes.

## Mental Models
- Use **"led by need, not by technology"**: identify use cases from business/user pain points; choose AI only where traditional solutions can't handle volume, complexity, real-time demands, or pattern detection.
- Use **"AI is a means to an end"**: define goals and user needs before touching technology.
- Use **"first project shapes the structure"**: support structures need not be mature before the first project — the first experience shapes them, but sufficient control and a safe environment are required from the start.

## Anti-patterns
- **Building in a silo**: without cross-government collaboration (e.g. AI community of practice), you duplicate work and miss reusable code/infrastructure.
- **Single-discipline teams**: no diversity of groups and viewpoints = higher risk of bias and discrimination going unnoticed.
- **Selecting use cases for the technology's sake**: starts from what AI can do rather than user needs.
- **Skipping UR for AI**: without it you cannot establish a baseline of metrics or understand bias in the existing human process.

## Worked Example
**Scoping a use case with the right-tool check.** A team wants to answer citizen questions about a complex policy area.
- UR observes users: many can't navigate to the right GOV.UK page; queries are complex and multi-department.
- Right-tool check: traditional search can't resolve complex natural-language questions; a retrieval-augmented-generation (RAG) chatbot can pull relevant pages. Feasibility: skills and infra exist; an LLM API + vector store is viable.
- Baseline metrics established via UR before building.
- Decision: proceed with a phased experiment (limited pilot, accuracy threshold), the pattern used by GOV.UK Chat — not a full public launch on day one.

## Key Takeaways
1. Form a multidisciplinary minimum viable AI team before writing code; include data, engineering, UR, legal, commercial, security, ethics and privacy expertise.
2. Target AI learning by learner group; give data/digital professionals safe sandboxes to experiment.
3. Do AI-specific user research across the life cycle — it keeps the human in the loop and defines metrics.
4. Pick use cases led by user needs; avoid fully automated decision making and high-risk, high-impact solo-AI applications.
5. Stand up the AI support structure (strategy, principles, governance board, comms, sourcing, training) and capture use cases in a register.

## Connects To
- **Ch 1**: operationalises Principles 1, 4, 5, 6, 9, 10
- **Ch 2**: use-case selection grounded in AI capabilities/limitations
- **Ch 4**: team includes commercial colleagues; skills for procurement
- **Ch 5–8**: safe/responsible-by-design is built into the team's remit
- **Ch 9**: governance board, assurance and risk management
- **Ch 10**: GOV.UK Chat case study shows UR-for-AI in practice
