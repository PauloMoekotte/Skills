# Chapter 3: Steps 1–3 — Engage, Identify, Inventory

## Core Idea
Steps 1–3 build the foundation: align on values with stakeholders, surface concrete accessibility barriers through their lived experience, and take stock of the technology and data the city already holds — before any solution is discussed.

## Frameworks Introduced
- **Asset Inventory for Inclusion (Step 1)**: catalog what already exists before creating anything new.
  - When to use: at project outset, to avoid duplicating existing work and to ground the project in city commitments.
  - How: survey existing policies/public commitments; roadmaps, strategic plans, and accessibility reviews; government grants and their metrics; governing bodies such as resident councils and community engagement groups; employee positions dedicated to advocacy for underrepresented groups. Then gather targeted feedback via interviews, focus groups, workshops, and innovation work groups.
- **Barrier Categorization (Step 2)**: classify the accessibility challenges a city faces into six recurring types, so the needs assessment is systematic.
  - When to use: during stakeholder needs assessment; use as a checklist to ensure no barrier class is missed.
  - How: check each category — **Historic infrastructure** (buildings, roads, sidewalks, transit not compliant with newer regulations, costly to retrofit); **Shortcomings in planning** (demographics overlooked → uneven sidewalks, missing ramps, non-audible traffic signals); **Information and communication barriers** (inaccessible public information, hurting non-native speakers and people with visual/auditory impairments); **Transportation gaps** (transit not serving all areas, lacking facilities); **Emergency preparedness** (emergency systems not catering to people with disabilities); **Inefficient resource distribution** (water, electricity, green space not fairly distributed).
- **Data Inventory (Step 3)**: audit datasets before selecting a tool.
  - When to use: once barriers are known, before committing to AI.
  - How: ask — what technology is in place for these issues, how does it perform against city values, can technology from another department be repurposed or expanded, and what internal teams/vendors already operate here? Then map available dataset types: automated data (IoT, water/waste, building systems), surveillance data (traffic cams, dashcams), user-generated data (issue-reporting apps, public comments), crowdsourced data (citizen science campaigns), administrative data (human services databases, grant reporting), survey data, social media data (geotagged posts), and documents data (ordinances, policies).

## Key Concepts
- **Lived experience**: the direct expertise people with disabilities and older persons hold about the barriers they face; the core input for needs assessment.
- **Compensation for participation**: paying community stakeholders and user testers for their time — too often marginalized people are asked to work for free "in return for representation."
- **Garbage in, garbage out**: if training data is not diverse and representative, AI reproduces stereotypes and bias.
- **KPI for inclusion**: project metrics should measure fairness, accuracy, and quality of service delivery.
- **Data sharing agreement**: the mechanism for using data from a different city department or partner.
- **3D vs 2D data**: two-dimensional maps cannot capture obstacles (trees, benches, terraces) that block sidewalks; three-dimensional data is often required.

## Mental Models
- **Think of the city as already half-built**: most of what an AI project needs — strategies, grants, relationships, datasets — exists somewhere in city departments; Step 1 and Step 3 are audits, not inventions.
- **Use barriers to frame the data gap**: each barrier category implies a data need; e.g. "historic infrastructure can't be audited manually" → street-level imagery and point clouds.
- **Compensation is inclusion infrastructure**: if you cannot pay lived-experience experts, your stakeholder process is not genuinely participatory.

## Anti-patterns
- **Instituting one-off consultation**: asking community for input once and never looping back — the framework demands ongoing engagement.
- **Unpaid lived experience**: treating disability community participation as volunteer labor; funding plans must budget for payment.
- **Assuming AI before inventorying**: prescribing an AI solution before Step 3 reveals the data and technology already on hand (or missing).
- **Collecting data no one owns**: building a new dataset when an existing city system already generates it — or when a data sharing agreement could unlock it.

## Worked Example
Amsterdam's barrier identification flow (Step 2):

1. **Round one — focus groups** with disability organizations and older residents surfaced the six barrier categories, with three priority areas: readability of city signs and communication materials, venue accessibility, and sidewalk accessibility.
2. **Key user insight**: mobility means knowing not only that a venue is accessible, but that the route to it is accessible too. Users were frustrated finding non-passable routes that increased travel time.
3. **Round two — multi-stakeholder engagement**: interviews, surveys, and facilitated workshops gathered resident perspectives on possible improvements. Amsterdam held eight meetings across 2021–2023 to set priorities and co-create the project plan, compensating participants throughout.

Result: the three priority areas became the project's scoping statement, and the data gap ("sidewalks can't be measured at scale from 2D maps") drove the Step 3 inventory toward street imagery and point clouds.

## Key Takeaways
1. Start with an asset inventory (Step 1) — policies, grants, relationships, and staff already exist and anchor the project.
2. Assess barriers against all six categories so no class of exclusion is overlooked.
3. Budget to compensate community stakeholders and user testers for their expertise.
4. Inventory data and technology before any solution talk — AI builds on what already exists, and "garbage in, garbage out" makes data quality the deciding factor.
5. Let the barriers define the data gap: the accessibility problem determines what data the AI tool needs.

## Connects To
- **Ch 02**: Steps 1–3 are the first half of the Ten Step Framework and rest on its five principles.
- **Ch 04**: the barrier and data picture from Steps 2–3 feeds directly into risk anticipation (Step 4) and solution selection (Step 5).
- **Ch 07**: Amsterdam's sidewalk project is the concrete execution of these first three steps.
