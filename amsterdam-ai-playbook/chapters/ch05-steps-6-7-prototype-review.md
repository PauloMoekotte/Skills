# Chapter 5: Steps 6–7 — Prototype, Review, Adjust

## Core Idea
Step 6 builds a small-scale prototype or pilot — tested by the people it is meant to serve — and Step 7 stress-tests the results with bug bashing, red teaming, and outcomes assessments before anything scales. Small first, improve, then expand.

## Frameworks Introduced
- **Prototype or Pilot (Step 6)**:
  - When to use: once a technology solution is selected, to test it cheaply before city-wide deployment.
  - How: build a prototype (a model of what the tool will do) or a pilot (the AI tested in one area or for one issue). Procure existing technology, hire an external vendor, or use a low-cost academic research partnership. Test with individuals representing older persons and people with disabilities to gather requirements and insights. Plan monitoring so community stakeholders can review results before scale.
- **Evaluation Toolkit (Step 7)** — three methods for reviewing pilot results:
  - **Bug bashing**: ask people who have never used the technology to try it and record every issue — broken parts, confusing or frustrating actions, design feedback — as "bugs" for the team to fix.
  - **Red teaming**: testers intentionally try to produce errors and harmful outcomes, stress-testing the system for results that would hinder inclusivity and accessibility.
  - **Outcomes assessments**: score results on two measures — **accuracy** (did the AI produce results in line with expectations?) and **fairness** (examining specific demographic populations, geographic populations, or characteristics of users and impacted populations).

## Key Concepts
- **Accessibility safari**: an in-person field validation where teams physically measure real-world conditions (e.g. sidewalk widths) and compare them against the AI-generated dataset.
- **Data labeling**: tagging objects in datasets (e.g. obstacles in point clouds) so the AI can learn to identify them; quality depends on labeling accuracy.
- **Labeling guidelines**: documentation of how to label consistently, created to raise data quality.
- **Academic partnerships**: engaging universities and students as a low-cost route to develop, test, and evaluate new technology while training the next workforce.
- **Employing the community**: community stakeholders should not only give feedback — they should be hired onto technology teams, contributing lived experience and diverse skill sets.

## Mental Models
- **Test with the intended users, not the builders**: prototype evaluation is meaningful only when it involves older persons and people with disabilities who will actually use the tool.
- **Think of bugs as design information, not blame**: bug bashing treats every friction point as a recorded fix, not a failure of the user.
- **Red team for inclusion**: stress-test specifically for outcomes that would exclude or harm — the failure mode that matters most here is an inaccessible result, not just a crash.
- **Validate against reality**: compare AI output to physical ground truth (accessibility safaris) rather than trusting the model's self-reported accuracy.

## Anti-patterns
- **Scaling before testing**: deploying AI city-wide without a small test case; the playbook explicitly warns technical teams to start small and improve first.
- **Consulting the community without employing them**: limiting community roles to feedback when hiring them on the team (like Spectrum Intelligence's 13,000 labels) yields better data and honors inclusion.
- **Measuring accuracy only**: assessing the pilot solely on accuracy scores and skipping fairness — fairness is the harder, essential half.
- **Self-validation**: checking AI results only against the AI's own output; ground-truth checks (Google Maps comparison, in-person measurement) are what expose real error.

## Worked Example
Amsterdam's pilot evaluation (Steps 6–7):

1. **Pilot build**: computer vision AI processed laser-scanner data from a select city area, combined with existing maps into a 3D model, and applied an accessible-sidewalk-width calculation to identify accessible and inaccessible routes.
2. **Found gap**: many obstacles in the map needed labeling and some were hard to identify. A new partner, **Spectrum Intelligence** (which employs people across the autism spectrum), was brought in for precise labeling — adding **13,000 data labels** in a single in-person day, with a labeling guideline planned to keep quality high.
3. **Digital validation**: sidewalk widths in Google Maps images were compared against point-cloud measurements.
4. **Physical validation — the accessibility safari**: 45 Danish Erasmus+ students traveled the city with maps and measuring tapes to manually measure sidewalk widths and annotate the AI dataset. The exercise combined briefing, mapping, and debriefing — and doubled as workforce training. As student Mathilde put it, students "realized that sidewalks are designed for people without disabilities."

Result: the AI's accuracy was checked against reality, the dataset improved through community hiring, and the next generation of urban planners was trained.

## Key Takeaways
1. Pilot in a bounded area first — prototypes and pilots exist to be corrected cheaply.
2. Involve intended users (older persons, people with disabilities) in testing, and consider hiring community members onto the team.
3. Use all three evaluation methods: bug bashing, red teaming, and outcomes assessments covering accuracy and fairness.
4. Validate AI output against physical ground truth, not just the model's own metrics.
5. Enlist academic and student partners to evaluate pilots — cost-effective and capacity-building.

## Connects To
- **Ch 04**: the pilot operationalizes the solution selected through the Step 5 feasibility gate.
- **Ch 06**: lessons from Step 7 decide what is ready to scale (Step 8) and what monitoring to build (Step 10).
- **Ch 07**: the full Amsterdam sidewalk project is the case study this chapter draws on.
