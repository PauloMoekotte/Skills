# Cheatsheet — AI Playbook for Inclusive and Accessible Cities

## Ten Step Checklist (run in order, loop back to stakeholders at 2, 4, 7)
1. Engage stakeholders & define values → 2. Identify barriers → 3. Tech & data inventory → 4. Anticipate & mitigate risks → 5. Select solution (feasibility gate) → 6. Prototype/pilot → 7. Review & adjust → 8. Scale → 9. Communicate & train → 10. Monitor & evaluate.

## Should this be AI at all? (Step 5 gate)
| Check | Pass | Fail → do this |
|---|---|---|
| Data exists (diverse, representative) | Proceed | Collect or reuse before AI |
| Skills in team/partners | Proceed | Partner or train first |
| Budget for small test | Proceed | Scope down or delay |
| Privacy / civil-liberties risk acceptable | Proceed | Redesign or drop AI |
| AI better than improving existing tech | Proceed | Improve existing tech |

## AI category → risk & inclusion lever (Ch 1)
| Category | What it does | Example | Watch for |
|---|---|---|---|
| Anticipatory | Predicts from historical data | Sidewalk failure prediction | Training data bias |
| Generative | Creates new content | Accessibility chatbot | Copyright, hallucination, immaturity |
| Decisive | Automates recommendations | Infrastructure prioritization | Fairness of the decisions |

## Barrier → data implication (Ch 3)
| Barrier | Data gap it implies |
|---|---|
| Historic infrastructure | Street-level imagery, point clouds |
| Planning shortcomings | Geo-referenced sidewalk/ramp/signal data |
| Info & communication barriers | Multilingual, audio/visual content data |
| Transportation gaps | Transit facility & route accessibility data |
| Emergency preparedness | Evacuation & alert accessibility data |
| Unequal resource distribution | Geospatial service-coverage data |

## Decision rules
- **Nothing about us without us** — if the affected community was not genuinely in the room (and compensated), stop and fix that first.
- **Stakeholders before technology** — no solution talk until Steps 1–2 are done.
- **Start small** — always prototype/pilot before scale; never deploy city-wide untested.
- **Validate against reality** — compare AI output to physical ground truth (accessibility safaris), not just the model's own metrics.
- **Compensate participation** — budget for paying lived-experience experts; "representation in return for free labor" is a smell.
- **Open by default** — share documents and code unless privacy forbids; maintain an AI Register.
- **Generative AI = higher caution** — integrate prudently, keep rollback ready, avoid copyrighted training data; not yet critical infrastructure.
- **High-risk domains need explicit civil-rights rules** — no unregulated AI in law enforcement, courts, or public assistance.
- **Transparency when AI replaces humans** — plain-language explanations are mandatory when AI affects access to services.

## Procurement & standards (Ch 8)
- Define **accessibility goals in procurement contracts** so vendors are bound to them.
- Standards ladder: **WCAG 2.0** (web) → **ISO 21542/ISO 71** (built environment) → **ETSI EN 301549** (ICT) → **CRPD** (human rights) → **EU AI Act** (regulation, risk-tiered).

## Tells & smells
- **Smell**: unpaid community input → compensation is missing from the budget.
- **Smell**: AI chosen before an inventory was done → AI is being prescribed, not selected.
- **Smell**: accuracy-only evaluation → fairness assessment is missing.
- **Smell**: no public record of what the AI does → transparency/AI Register absent.
- **Smell**: one-shot consultation → the engagement loop has broken; monitoring must be lifecycle-long.
- **Tell**: "garbage in, garbage out" → if data isn't diverse, expect reproduced bias.

## Defaults the playbook commits to
- KPIs measure **fairness, accuracy, and quality of service** — not just speed/cost.
- Every evaluation checks **both accuracy and fairness**.
- Monitoring: **weekly (core team)** + **quarterly/annual (community)**.
- Compensation: **always budget for lived-experience experts and user testers**.
- Scale only **after** pilot validation; reuse validated data in adjacent pilots.
