# Chapter 1: The 10 Principles

## Core Idea
The UK government's 10 principles define the minimum bar for using AI safely, responsibly and effectively across government and public sector organisations. They build on the 5 sector-agnostic principles from the white paper *A pro-innovation approach to AI regulation* and apply them to government AI use.

## Frameworks Introduced
- **The 10 Principles for AI use in government**: the playbook's master framework. Use them as the acceptance criteria for any AI project — a project that fails any principle needs rework or a stop decision.
  1. You know what AI is and what its limitations are
  2. You use AI lawfully, ethically and responsibly
  3. You know how to use AI securely
  4. You have meaningful human control at the right stages
  5. You understand how to manage the full AI life cycle
  6. You use the right tool for the job
  7. You are open and collaborative
  8. You work with commercial colleagues from the start
  9. You have the skills and expertise needed to implement and use AI
  10. You use these principles alongside your organisation's policies and have the right assurance in place
- **How**: treat Principles 1–6 as technical/operational gates, 7–8 as collaboration gates, and 9–10 as capability and governance gates. Apply them all together, not selectively.
- **Right-tool principle (6)**: be as open to "AI is not the answer" as to AI itself. A problem may be more easily solved with established technologies — reaching that conclusion is a valid outcome.

## Key Concepts
- **Meaningful human control**: monitoring AI behaviour and having intervention plans; humans validate high-risk decisions influenced by AI. For instant-response apps (e.g. chatbots), control shifts to other life-cycle stages: full pre-deployment testing, assurance, live checks and user feedback loops.
- **AI life cycle**: choose the right tool, set it up, maintain it day-to-day, update it, and securely close it down at end of useful life.
- **ATRS (Algorithmic Transparency Recording Standard)**: mandatory for central departments and in-scope arm's length bodies — document algorithmic tools used in decision-making and make it publicly accessible.
- **Secure by Design / Cyber Security Standard**: the required security baseline for government services (developed by CDDO).
- **Senior Responsible Owner (SRO)**: the named individual accountable for AI use in a project.

## Mental Models
- Think of the principles as **acceptance criteria**, not aspirations — each is a yes/no gate before a project proceeds.
- Use **"meaningful human control" at the right stage** — for slow decisions put a human in the loop; for instant decisions (chatbots) put human control into testing, monitoring and redress instead.
- Use **right tool for the job** as a forced comparison — ask "what would the non-AI or simpler-ML option look like?" before committing.
- Use **organisation policies as the floor** — the playbook sets a consistent baseline; organisational policies (especially security and data handling) can be stricter.

## Anti-patterns
- **Treating AI as an objective in itself**: using AI is a means to an end; goals and user needs come first.
- **Skipping assurance until late**: connect with assurance teams early; have documented review and escalation processes and a review board from the start.
- **Assuming AI systems are accurate**: they are not guaranteed to be accurate; plan testing and accuracy-improving techniques.
- **Entering official information into public AI tools**: only enter published or clearance-approved information (Principle 3's practical outworking).

## Worked Example
**Deciding whether an AI project passes the principles gate.** A department proposes a chatbot to answer citizen questions about a public service.
- P1 — Team can state what the LLM can/cannot do and its hallucination risk ✓
- P2 — Legal/data protection advice engaged; personal data handling reviewed ✓
- P3 — Content filtering, validation checks and data-leak prevention in place ✓
- P4 — Instant responses mean no real-time human review; so: full pre-deployment testing, live monitoring, and user "report issue → human review" mechanism must be in place ✓
- P5 — Maintenance, drift/hallucination monitoring, and shutdown path defined ✓
- P6 — Compared against simpler alternatives; chatbot chosen because query handling can't be met otherwise ✓
- P7 — ATRS record published; chatbot responses labelled "written by an automated AI chatbot" ✓
- P8 — Commercial colleagues involved in procurement from the start ✓
- P9 — Team has or is acquiring the required skills; leaders trained on AI risks ✓
- P10 — Fits department policies; assurance team engaged; review board exists ✓
All ten pass → proceed. Any failure → fix or stop.

## Key Takeaways
1. Apply all 10 principles together — they are the acceptance criteria for any AI project.
2. Human control does not mean "always a human in real time"; for instant apps, control moves to testing, monitoring and redress.
3. Be genuinely open to the conclusion that AI is the wrong tool.
4. Comply with ATRS transparency recording for in-scope bodies; label automated responses to the public.
5. Engage commercial, legal, data protection and assurance colleagues from the start, not after the fact.

## Connects To
- **Ch 2**: P1's grounding — what AI is and its limitations
- **Ch 3**: P6/P9's outworking — use-case selection and team skills
- **Ch 4**: P8's outworking — commercial and procurement process
- **Ch 5**: P2/P4 — ethics themes and safety
- **Ch 7**: P2 — data protection principles
- **Ch 8**: P3 — secure deployment
- **Ch 9**: P10 — governance, assurance and risk
