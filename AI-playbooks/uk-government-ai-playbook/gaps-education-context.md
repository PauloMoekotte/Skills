# Gap-analyse: AI-governance voor onderwijs

**Doel**: welke aspecten van AI-governance relevant voor een **onderwijscontext** worden
door de drie playbook-skills gedekt, waar zitten de gaten, en wat doe je er concreet aan.

**Drie skills die samenwerken:**
- **uk-government-ai-playbook** — UK *AI Playbook for the UK Government* (GDS, feb 2025): proces en principes (verantwoord bouwen, inkopen, DPIA, security, governance).
- **amsterdam-ai-playbook** — Amsterdam *AI Playbook for Inclusive and Accessible Cities*: inclusie, toegankelijkheid, stakeholderbetrokkenheid ("nothing about us without us").
- **vlaanderen-ai-playbook** — *AI Playbook kernactiviteiten* (Digitaal Vlaanderen): strategie, use cases, betrouwbare AI (EU AI Act), mens & organisatie, architectuur, agentische AI.

**Hoe gebruiken**: per lacune staat eerst *waarom het relevant is* (begrip), daarna wat elke
skill dekt, en telkens een **Actie**-blok (handelingsgericht). Hoofdstukverwijzingen zoals
`ch04` verwijzen naar de `chapters/`-map van de betreffende skill.

> Status: beslissingshulp, geen juridisch advies. Toets altijd bij je eigen jurist, DPO,
> examenreglementen en — in de EU — de EU AI Act-verplichtingen voor onderwijsaanbieders.

---

## 1. Kinderen & kwetsbare gebruikers

**Waarom relevant**: AI in onderwijs raakt minderjarigen; hun toestemming, privacy en rechten
vragen een eigen kader (age-appropriate design, ouderlijke toestemming, beste belang van het kind).

- **UK dekt**: ch07 (generieke UK GDPR, DPIA) — kind-specifieke bril ontbreekt.
- **Amsterdam vult aan**: Ten Step stap 1–2 "engage stakeholders & identify barriers" (ch03); de toets "nothing about us without us".
- **Vlaanderen vult aan**: ch03 betrouwbare AI — AVG-behandeling en GenAI-risico's (bias, hallucinaties, copyright); ch04 stakeholder mapping (impact × invloed) om kinderen/ouders als groep te positioneren.

**Actie**:
1. Voeg aan elke DPIA een kind-rechtenparagraaf toe (UK Children's Code / UNCRC) — bouw voort op de 10-stappen-DPIA uit UK ch07.
2. Veranker ouderlijke toestemming en opt-out van de leerling in het inkoopbestek (zie §7).
3. Breng "kinderen en ouders" als stakeholdergroep in met de Vlaanderen stakeholder mapping (ch04).

## 2. Toetsing & academische integriteit

**Waarom relevant**: AI in toetsing, AI-detectie (met valse positieven voor leerlingen) en
algoritmische beoordeling (denk aan het UK 2020 A-level-debat) raken rechtstreeks de kern van het onderwijsproces.

- **UK dekt**: ch01 (fairness, contestability), ch05 (ethiek) — principes, geen toetsingsspecifiek kader.
- **Amsterdam vult aan**: outcomes assessment "accuraatheid **en** eerlijkheid meten" (ch04–05); pre-mortem (ch04).
- **Vlaanderen vult aan**: ch03 GenAI-risicotypologie (bias, hallucinaties) vertalen naar toetsingsrichtlijnen; ch02 AI-model canvas om de use case (bv. detectietool) volledig te definiëren.

**Actie**:
1. Stel een toetsingsbeleid op: waar AI is toegestaan, waar niet, en hoe je dat communiceert (ch03 Vlaanderen: richtlijnen + procedures).
2. Vereis bij elke detectie-/beoordelings-AI een fairness-meting naast de accuraatheid (Amsterdam ch05) en een bezwaarroute (UK ch01 contestability).
3. Run de Amsterdam pre-mortem met docenten en examencommissie vóór uitrol.

## 3. Pedagogische effectiviteit & leerresultaten

**Waarom relevant**: of AI het leren écht verbetert, wordt door geen van de playbooks getoetst — en dat is de kernvraag in onderwijs.

- **UK dekt**: ch03 (use case selectie, minimaal levensvatbaar team) — toetst noodzaak/haalbaarheid, niet leeruitkomsten.
- **Amsterdam vult aan**: Feasibility Gate stap 5 "AI is not always the answer" (ch04).
- **Vlaanderen vult aan**: ch02 haalbaarheid op 5 dimensies (business, technisch, praktisch, juridisch, ethisch) + impact/inspanning-matrix; ch01 OKR-raamwerk om leerdoelen meetbaar te maken.

**Actie**:
1. Formuleer vóór elk AI-initiatief een meetbaar leerdoel (KPI/SMART via Vlaanderen ch01 OKR's).
2. Draai de 5-dimensies-haalbaarheidscheck (Vlaanderen ch02) + Amsterdam Feasibility Gate vóór je start.
3. Voeg een pedagogisch/eindtermen-oordeel toe (door de school zelf) — geen van de skills dekt dit.

## 4. Professionele autonomie van de leraar & accountability

**Waarom relevant**: wie is verantwoordelijk als AI adviseert over leerlingresultaten? De leraar is de eindverantwoordelijke professional; consultatie en werkdruk tellen mee.

- **UK dekt**: ch01/ch05 meaningful human control + answerability–auditability-triade.
- **Amsterdam vult aan**: transparantie & accountability-principe, proactieve transparantie (ch08).
- **Vlaanderen vult aan**: ch04 verandermanagement — case for change, WIIFM per stakeholdergroep, overlegorganen (strategisch/tactisch/operationeel) voor personeelsbetrokkenheid.

**Actie**:
1. Leg vast dat de leraar eindverantwoordelijk blijft: AI = beslissingsondersteuning (Vlaanderen ch05 categorisering), nooit autonome beoordeling.
2. Doorloop de case for change (WAT, WAAROM, WAAROM NU, HOE) met het lerarenteam vóór uitrol (Vlaanderen ch04).
3. Richt een overlegorgaan (bv. bestaand personeelsoverleg) in dat AI-initiatieven toetst.

## 5. Welzijn, surveillance & proctoring

**Waarom relevant**: proctoring, gedragsmonitoring en welzijnschatbots raken evenredigheid,
toestemming en dataminimalisatie in een machtspositie (school ⇄ leerling).

- **UK dekt**: ch07 (PET's, DPIA, Art. 22) + ch08 security — sterke algemene basis.
- **Amsterdam vult aan**: stap 4 risico-anticipatie incl. privacy/civil-liberty (ch04).
- **Vlaanderen vult aan**: ch03 EU AI Act-risicoclassificatie (beperkte/hoog-risico transparantie-verplichtingen); ch05 architectuur — toegangscontrole en dataminimalisatie.

**Actie**:
1. Loop de UK DPIA (ch07) met kind-bril (§1) vóór elke monitoringtool.
2. Stel proportionaliteitstoets: is minder invasief mogelijk (bv. steekproef i.p.v. continue proctoring)?
3. Check de EU AI Act-classificatie (Vlaanderen ch03) — emissie- en welzijnstools kunnen hoog-risico of verboden praktijk zijn.

## 6. Toegankelijkheid, inclusie & digitale kloof

**Waarom relevant**: apparaat-/internetarmoede en leerstoornissen bepalen of AI bevoordeelt of uitsluit.

- **UK dekt**: ch01 fairness-principe alleen.
- **Amsterdam vult aan**: **dit is de kernsterkte** — Ten Step Framework, accessibility reviews, accessibility safari, Seven AI Capabilities (ch02–07, incl. case "Amsterdam for All").
- **Vlaanderen vult aan**: ch03 bias-behandeling en duurzaamheidsprincipe; ch04 opleiding & begeleiding om geen doelgroep achter te laten.

**Actie**:
1. Laat elke AI-tool een accessibility review doorlopen (Amsterdam) en leg dat in het bestek vast (§7).
2. Inventariseer de digitale kloof binnen je schoolpopulatie (Amsterdam stap 2) vóór een BYOD- of AI-initiatief.
3. Voer een accessibility safari uit met (SEN-)leerlingen (Amsterdam ch05).

## 7. EdTech-leveranciers & inkoop

**Waarom relevant**: edtech is vaak VS-gehost met lock-in en datadoorvoer; schoolbesturen kopen anders in dan departementen.

- **UK dekt**: ch04 (framework vs DPS, AI-spec-checklist, drempelwaarden) — algemeen overheidsinkoop.
- **Amsterdam vult aan**: toegankelijkheid in bestek verankeren, leverancier binden (ch04).
- **Vlaanderen vult aan**: ch05 architectuur — leveranciersonafhankelijkheid, exitstrategie, cloudsoevereiniteit, datalicenties; ch02 AI-model canvas om rollen/data/activiteiten in de opdracht te vatten.

**Actie**:
1. Gebruik de UK AI-spec-checklist (ch04) als ruggengraat van het bestek.
2. Voeg verplichte clausules toe: dataminimalisatie, EU/AVG-doorgifte, leveranciersonafhankelijkheid en exitstrategie (Vlaanderen ch05).
3. Beoordeel lock-in vóór ondertekening — een van de 6 faaloorzaken (Vlaanderen ch05).

## 8. Bestuur & institutionele structuur

**Waarom relevant**: een schoolbestuur/directie en gemeentelijke opdrachtgever zijn geen departement; wie zit in het toezicht en op welk niveau?

- **UK dekt**: ch09 (raad, ethisch comité, AI-inventaris, risicobeheer) — veronderstelt een departementsstructuur.
- **Amsterdam vult aan**: AI-register, standaard openbaar (ch08).
- **Vlaanderen vult aan**: ch04 organisatiemodel (6 dimensies) + overlegorganen (strategisch/tactisch/operationeel, bouw voort op bestaande organen); positionering gecentraliseerd/hybride/gedecentraliseerd.

**Actie**:
1. Stel een AI-inventaris op (UK ch09) en publiceer die als AI-register (Amsterdam ch08).
2. Richt overlegorganen in op drie niveaus, voortbouwend op bestaande organen (schoolraad, directieteam) — Vlaanderen ch04.
3. Voeg leerling- en oudergeleding toe aan het ethisch overleg (combineert UK ch09 + Amsterdam stap 1).

## 9. Regionaal recht & EU AI Act

**Waarom relevant**: de EU AI Act classificeert AI voor toelating en beoordeling van studenten als **hoog-risico**; de UK-skills zijn gebaseerd op UK GDPR/Equality Act.

- **UK dekt**: ch06 (public law, Equality Act) + ch07 (UK GDPR) — andere jurisdictie.
- **Amsterdam dekt**: niet (stedelijk, pre-AI-Act).
- **Vlaanderen vult aan**: **de kernsterkte** — ch03 volledige EU AI Act-risicoclassificatie (4 niveaus), tijdslijn (2/8/2026 rest + bijlage III + FRIA), DPIA **+ FRIA**, AI-geletterdheidsplicht.

**Actie**:
1. Classificeer elke onderwijs-AI op de EU AI Act-schaal (Vlaanderen ch03) — toelating/evaluatie = hoog-risico.
2. Plan FRIA naast DPIA voor hoog-risico systemen (Vlaanderen ch03; UK ch07 voor de DPIA-methodiek).
3. Vervul de AI-geletterdheidplicht (EU AI Act) via opleidingstraject uit Vlaanderen ch04 (opleiding in 5 stappen + AI Readiness Check).

## 10. AI-geletterdheid & curriculum

**Waarom relevant**: het playbook behandelt burgers als gebruikers, niet als lerenden die over AI leren.

- **UK dekt**: ch02 (AI-velden, beperkingen, agentische AI) — bruikbaar als lesmateriaal.
- **Amsterdam vult aan**: stap 9 communicatie & training (ch06) — gebruikerstraining, geen curriculum.
- **Vlaanderen vult aan**: ch03 AI-geletterdheidsplicht + oliyvlekmodel voor GenAI-adoptie (ch02) — kleine testgroep → basisopleiding → ambassadeurs.

**Actie**:
1. Gebruik UK ch02 als inhoudsbasis voor een AI-geletterdheidscurriculum (velden, beperkingen, risico's).
2. Zet het oliyvlekmodel in voor personeelsadoptie (Vlaanderen ch02).
3. Meet AI-geletterdheid met de AI Readiness Check (Vlaanderen ch04).

## 11. Onderzoeksethiek met minderjarigen

**Waarom relevant**: pilots en experimenten met leerlingen vereisen ethische toetsing.

- **UK dekt**: ch05 ethiekthema's (algemeen); ch03 pilot-begeleiding.
- **Amsterdam vult aan**: stap 6 prototype/pilot + stap 7 review (ch05).
- **Vlaanderen vult aan**: ch04 pilot → uitrol (analyse → co-creatie → pilot → verfijnen); ch02 AI-model canvas.

**Actie**:
1. Leg elk leerling-aanraakpunt voor aan de institutionele onderzoeksethische toetsing.
2. Gebruik het Vlaanderen pilot-traject (ch04) + Amsterdam stap 6–7 als processtandaard.
3. Evalueer na de pilot op fairness én accuraatheid (Amsterdam ch05) vóór opschaling.

---

## Werkwijze: de drie skills combineren

1. **Strategie & ambitie** — Vlaanderen ch01 (OKR's, business case, roadmap): waar wil de instelling met AI naartoe?
2. **Use case selectie** — Vlaanderen ch02 (Double Diamond, impact/inspanning, AI-model canvas) + UK ch02/03 (velden, use cases om te vermijden).
3. **Inclusie & toegankelijkheid** — Amsterdam Ten Step 1–2: wie is betrokken, welke barrières?
4. **Juridisch & data** — UK ch06/07 (DPIA) + Vlaanderen ch03 (EU AI Act, FRIA) met kind-bril (§1).
5. **Inkopen of bouwen** — UK ch04 (spec-checklist) + Amsterdam ch04 (toegankelijkheid in bestek) + Vlaanderen ch05 (lock-in, exit).
6. **Governance** — UK ch09 (inventaris, risicobeheer) + Amsterdam ch08 (openbaar AI-register) + Vlaanderen ch04 (overlegorganen).
7. **Monitoren** — Amsterdam outcomes assessment (fairness + accuraatheid) + UK ch08 (model drift) + Vlaanderen ch05 (kosten, architecturale gezondheid).

## Actie-checklist (beknopt)

| # | Minimale actie | Bron |
| --- | --- | --- |
| 1 | Kind-rechtenparagraaf in elke DPIA | UK ch07 + EU Children's Code |
| 2 | Toetsingsbeleid AI + bezwaarroute | Vlaanderen ch03 + UK ch01 |
| 3 | Meetbaar leerdoel vóór elk initiatief | Vlaanderen ch01 |
| 4 | Leraar = eindverantwoordelijke vastleggen | UK ch01 + Vlaanderen ch05 |
| 5 | Proportionaliteitstoets monitoring | UK ch07 + Vlaanderen ch03 |
| 6 | Accessibility review verplicht | Amsterdam ch02–05 |
| 7 | Exitstrategie & datalicenties in bestek | Vlaanderen ch05 |
| 8 | AI-inventaris + openbaar register | UK ch09 + Amsterdam ch08 |
| 9 | EU AI Act-classificatie + FRIA plannen | Vlaanderen ch03 |
| 10 | AI-geletterdheidsopleiding (plicht) | Vlaanderen ch03–04 |
| 11 | Ethische toetsing vóór leerling-pilots | Vlaanderen ch04 + Amsterdam ch05 |

## Verwant

- UK-hoofdstukken: `chapters/ch01–ch10` van deze skill.
- Amsterdam-hoofdstukken: `chapters/ch02–ch08` van de amsterdam-ai-playbook skill.
- Vlaanderen-hoofdstukken: `chapters/ch01–ch06` van de vlaanderen-ai-playbook skill.
- Voor de Vlaamse/Nederlandse onderwijscontext aanvullen met het **IAMA**-skill (impact assessment mensenrechten en algoritmes) en het EU AI Act-kader uit Vlaanderen ch03.
