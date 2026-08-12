# Chapter 4: Steps 4–5 — Anticipate Risk, Select the Solution

## Core Idea
Before any technology is committed to, Step 4 surfaces and mitigates risks through transparency, accessibility reviews, and pre-mortems; Step 5 then selects the right tool with a hard feasibility check — because AI is not the right answer to every problem.

## Frameworks Introduced
- **Risk Toolkit for Inclusive AI (Step 4)** — three complementary practices:
  - **Proactive Transparency**: explain to the public how AI works in clear, non-technical language — especially when AI makes decisions or affects access to services. Amsterdam's **AI Register** (2020) lists every AI tool used by the city, describing what it does, the data it uses or creates, how people oversee it, and how risks are handled. Pairs with "open by default": share documents and code publicly unless there is a compelling reason not to (e.g. privacy).
  - **Accessibility Reviews**: every technology product, including AI systems, should undergo an accessibility review. Define accessibility goals during procurement so outside vendors are contractually expected to meet them.
  - **Pre-mortem**: a facilitator asks reviewers to imagine the project has already failed and identify the reasons for that failure, drawing on their personal experiences and technical knowledge. This surfaces weaknesses fixable before execution. Engage experts with lived experience early — they know why similar projects have failed.
- **Feasibility Gate for AI Selection (Step 5)**: before choosing an AI solution, verify the fundamentals.
  - When to use: at every candidate technology decision.
  - How: balance costs, the team's skills, and the tool's actual capabilities; work with technology experts to estimate implementation effort; confirm the right data, skills, and budget exist to support a small test project; and check risks to privacy, civil rights, and civil liberties. If AI is not viable, improve existing technology or choose no technology at all.

## Key Concepts
- **Pre-mortem**: anticipating failure in advance by having reviewers enumerate why the project could fail.
- **AI Register**: a public inventory of AI systems in use, maintained in plain language — a transparency mechanism cities can adopt.
- **Open by default**: sharing technical resources (documents, code) with the public unless privacy gives a compelling reason not to.
- **Procurement as an accessibility lever**: defining accessibility goals during procurement forces vendors to meet them.
- **3D point cloud technology**: laser-scanner data capturing the position of every point in a street scene, used to record sidewalk widths and obstacles (trees, benches, bicycles, terraces).
- **Public-private partnership**: the procurement route Amsterdam used (with CycloMedia) to mount a 3D scanner on a car and collect street-level visual data.

## Mental Models
- **Assume failure, then prevent it**: the pre-mortem reframes risk work from "will this work?" to "how will this fail, and what can we fix now?"
- **Think of the AI Register as infrastructure, not paperwork**: it is what makes the transparency principle operationally real and inspectable by citizens.
- **AI is a candidate, not a default**: treat AI as one option among many; the feasibility gate decides whether it earns the job.
- **Match the data to the question**: Amsterdam could not measure obstacles with 2D topographic maps; the question (obstacles that block sidewalks) demanded 3D data. Let the problem dictate the data dimensionality, not the other way around.

## Anti-patterns
- **Deploying without a transparency plan**: rolling out AI that makes decisions without a public plain-language record of how it works and who oversees it.
- **Buying without accessibility requirements**: procuring vendor AI without contractually defined accessibility goals, then discovering compliance too late.
- **Skipping the pre-mortem**: committing resources before an experienced, diverse group — including people with lived experience — has imagined how the project could fail.
- **Choosing AI because it is exciting**: selecting AI when existing technology could be improved, or when data, skills, or budget cannot support even a small test.

## Worked Example
Amsterdam's solution-selection decision (Step 5):

1. **Problem re-scoped**: users reported sidewalk obstacles (benches, trees, bicycles, terraces) as the decisive barrier; 2D topographic maps could not capture them.
2. **Feasibility check**: computing sidewalk widths at city scale required three-dimensional data; the in-house team lacked the capture capability.
3. **Selection**: a public-private partnership with CycloMedia mounted a laser scanner to a car to collect street-level 3D point clouds; computer vision mapped sidewalks, recording width and every obstacle.
4. **De-risking before scale**: the output was a comprehensive 3D map that let planners understand city-wide accessibility and prioritize improvement areas — with validation deferred to the prototype phase (Step 6–7).

The decision satisfied the feasibility gate: right data (3D point clouds), right skills (partner + computer vision), right budget (partnership), and risks to privacy/civil liberties assessed up front.

## Key Takeaways
1. Run transparency, accessibility reviews, and pre-mortems before committing to any technology — they are cheap relative to failure.
2. Publish an AI Register or equivalent so citizens can see which AI the city runs and how it is overseen.
3. Encode accessibility into procurement contracts so vendors are bound to it.
4. Gate every AI choice on data, skills, budget, and rights-risk — if any fail, the tool is not ready.
5. Let the accessibility problem dictate the data you need (e.g. 3D over 2D for obstacles).

## Connects To
- **Ch 03**: risk and selection build directly on the barrier and data inventory of Steps 2–3.
- **Ch 05**: the feasibility gate hands off to prototyping and testing (Steps 6–7).
- **Ch 08**: the risk toolkit extends into the ethics policies in Appendix C (transparency, bias mitigation, civil rights).
