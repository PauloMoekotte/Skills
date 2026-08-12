# Chapter 7: Case Study — Amsterdam for All

## Core Idea
Amsterdam for All is the playbook's proof-of-concept: an end-to-end execution of the Ten Step Framework in which the city combined existing 2D maps and 3D point-cloud data with community engagement to measure sidewalk accessibility at city scale — and turned the result into an asset-management benchmark for cities worldwide.

## Framework in Action
The project followed the Ten Step Framework from stakeholder values to monitoring:

- **Step 1 — Values**: Amsterdam reviewed existing commitments (Tada Manifesto, Ethical Leaflet), developed five ethical principles with stakeholders, and set aside funds to compensate experts with lived experience.
- **Step 2 — Barriers**: focus groups identified six barrier classes; three priority areas emerged — readability of city signs and communication materials, venue accessibility, and **sidewalk accessibility**. Users stressed that the route to a venue must be accessible, not just the venue itself.
- **Step 3 — Inventory**: the city combined existing two-dimensional topographic maps with newly collected street imagery — a data asset that could be fed to AI.
- **Step 4 — Risks**: a global-expert pre-mortem predicted possible issues and gave technical guidance before resources were committed.
- **Step 5 — Solution**: a public-private partnership with **CycloMedia** mounted a laser scanner to a car; computer vision on 3D point clouds mapped sidewalk widths and obstacles (benches, trees, bicycles, terraces).
- **Step 6 — Pilot**: the tool was tested in a select area; obstacles proved hard to label, so **Spectrum Intelligence** — a company employing people across the autism spectrum — added **13,000 data labels** in one day, with a labeling guideline planned for quality.
- **Step 7 — Review**: results were validated digitally (Google Maps images vs point-cloud measurements) and physically via **accessibility safaris** with 45 Danish Erasmus+ students manually measuring sidewalks — training the next generation of urban planners while checking accuracy.
- **Step 8 — Scale**: 3D maps were shared with planning and maintenance colleagues to pinpoint problem areas; the sidewalk-width data was earmarked for an accessible route-planning pilot for wheelchair users, re-running the full framework.
- **Step 9 — Communication**: Amsterdam Intelligence published 9 blog posts, 3 academic papers, interviews, and workshop findings, and released open-source code.
- **Step 10 — Monitoring**: a dedicated Project Manager ran weekly KPI meetings with the core team and quarterly/annual assessments with the disability community and academic partners.

## Key Components
- **Community Involvement**: stakeholders participated throughout, were financially compensated for lived experience, and students were brought into data collection for learning opportunities.
- **AI-Driven Accessibility Assessment**: AI measured sidewalk accessibility, predicted potential obstructions, and identified the presence and location of curb ramps and crosswalks — producing route accessibility rankings and problem-area maps.
- **Partnerships for Broader Impact**: World Enabled, Project Sidewalk, and Amsterdam Intelligence combined global expertise to ensure success and international visibility.
- **Reuse and Adjacent Pilots**: the data-rich 3D map became a platform for future AI applications, including accessible route planning.

## Key Concepts
- **Amsterdam for All**: the initiative promoting inclusivity and accessibility in the City of Amsterdam, launched in 2020 by the CTO office with World Enabled.
- **Data for Development**: a core Global Compact principle — collect and manage data to advance inclusion; the playbook is an instrument for accelerating partnerships under it.
- **Accessibility safari**: ground-truth validation where teams physically measure conditions and compare with AI output.
- **Lived-experience hiring**: employing people with disabilities in data labeling and other technical roles — both inclusive and higher quality.
- **Benchmark project**: Amsterdam's initiative is positioned as a model for using AI in sustainable, efficient, inclusive asset management.

## Mental Models
- **Think of the project as a flywheel of data and reuse**: each step's output (3D map) feeds the next application (route planning), multiplying the original investment.
- **Compensation is the price of genuine participation**: paying lived-experience experts made community involvement real rather than symbolic.
- **Localize before replicating**: other cities should adapt the framework to their geography, demographics, and political priorities — not copy Amsterdam wholesale.

## Anti-patterns
- **Treating the case study as a template to copy**: the playbook insists on local customization; blind replication ignores context.
- **Collecting data without a reuse plan**: Amsterdam's impact came from turning the map into an asset-management platform — data alone was not the outcome.
- **Engaging without compensating**: participation without payment undercuts the equity the project claims.

## Worked Example
Sidewalk accessibility end-to-end:

1. **Problem**: users reported sidewalks cluttered with benches, signs, trees, bicycles, and terraces that block mobility; 2D maps could not measure this.
2. **Data**: combined topographic maps with 3D point clouds from laser scanners, describing each sidewalk's width and obstacles.
3. **Model**: computer vision classified obstacles and computed accessible sidewalk widths; validation combined Google Maps comparison with student-run accessibility safaris.
4. **Output**: a comprehensive 3D map showing widths and available walking space, letting planners identify problem areas and prioritize improvements.
5. **Impact**: a data foundation for wheelchair route planning and city-wide asset management, plus raised awareness among 45 students who "realized that sidewalks are designed for people without disabilities."

## Key Takeaways
1. The Ten Step Framework works end-to-end when followed faithfully — Amsterdam is the reference execution.
2. Combine existing city data (2D maps) with new capture (3D point clouds) rather than starting from scratch.
3. Hire and compensate the community — labeling by Spectrum Intelligence and paid lived experience were quality and equity wins.
4. Validate AI against physical ground truth before trusting it at scale.
5. Design data for reuse: one map became route planning, asset management, and a benchmark for other cities.

## Connects To
- **Ch 02**: the case study is the Ten Step Framework applied; return here when you need the principles made concrete.
- **Ch 03–06**: each framework step is detailed in the corresponding chapter.
- **Ch 08**: the project's transparency and ethics practices connect to the policy standards in the appendices.
