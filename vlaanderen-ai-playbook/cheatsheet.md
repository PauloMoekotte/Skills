# Cheatsheet

## Volgorde bij een nieuw AI-traject
1. Inspiratie & bewustzijn (ch04) → 2. AI-ambitie (ch01) → 3. OKR-doelstellingen (ch01) → 4. Use case identificatie (ch02) → 5. Business case + roadmap (ch01) → 6. Classificatie & risico (ch03) → 7. Architectuur & gereedheid (ch05) → 8. Piloot & uitrol (ch02, ch04).

## Wanneer wél of geen AI?
- Probleem eerst: is er een concreet probleem? Nee → stop.
- Is eenvoudigere oplossing (beslissingsboom, regel) voldoende? Ja → geen AI.
- Is het versnellen van een slechte werkwijze de motivatie? Ja → herteken het proces, niet AI.
- AI = geschikt als: patroonherkenning, taal, voorspelling, personalisatie, automatisering van deeltaak.

## Haalbaarheidscheck (5 dimensies)
Business waarde · Technisch · Praktisch · Juridisch · Ethisch — alle 5 moeten haalbaar zijn (of een mitigatieplan hebben).

## Prioritering impact/inspanning
| Kwadrant | Actie |
|---|---|
| Grote impact, kleine inspanning | Quick win — eerst doen |
| Grote impact, grote inspanning | Big project — plan zorgvuldig |
| Kleine impact, kleine inspanning | Fill-in job — lage prioriteit |
| Kleine impact, grote inspanning | Thankless task — vermijden |

## EU AI Act — risiconiveau bepalen
Rol (ontwikkelaar/gebruiker) + doel & impact op personen →
- Sociale scoring, emotieherkenning werkvloer, gedragsmanipulatie → **verboden**.
- Kritieke infrastructuur, politie/justitie, rekrutering, onderwijs, toegang publieke diensten → **hoog-risico** (DPIA + FRIA).
- GenAI-chatbot met burgerinteractie → **beperkt** (transparantieverplichtingen).
- Overige → **minimaal** (AI-geletterdheid + vrijwillige code).

## EU AI Act — tijdslijn
1/8/2024 in werking · 2/2/2025 verboden + geletterdheid · 2/8/2025 GPAI · 2/8/2026 rest + bijlage III + FRIA · 2/8/2027 bijlage I · 2/8/2030 alle hoog-risico.

## 8 voorwaarden betrouwbare AI (checklist)
Welzijn · Transparantie · Verantwoording · Menselijke controle · Rechtvaardigheid · Rechtmatigheid · Robuustheid · Privacy.

## GenAI-risico's — herkennen
Bias (scheve data) · Hallucinaties (foutief, zelfverzekerd) · Copyright · AVG (gevoelige data) · Automatiseringsparadox (te veel vertrouwen) · Overfitting (te veel op trainingsdata).

## Stakeholder kwadranten (impact × invloed)
| | Hoge invloed | Lage invloed |
|---|---|---|
| **Hoge impact** | Samenwerken & actief betrekken | Intensief ondersteunen & begeleiden |
| **Lage impact** | Proactief meenemen | Niet uit het oog verliezen |

## Case for change — 4 vragen
WAT & HOE (gewenste situatie) · WAAROM (context & uitdagingen) · WAAROM NU (voordelen/risico's) · HOE (aanpak & impact).

## Positioneringsmodel kiezen
| Situatie | Model |
|---|---|
| Lage AI-maturiteit | Gecentraliseerd |
| Innovatiecultuur, autonomie, snelheid | Gedecentraliseerd |
| Meestal, evenwicht | Hybride |
| Minder mature/kleine organisatie | Overweeg externe partners |

## Overlegorgaan — per orgaan vastleggen
Doel (informeren/beslissen/kennisdelen) · Voorbeeldbeslissingen · Aanwezigen (functietitels) · Eigenaar · Frequentie & duurtijd.

## Quickscan — wanneer AI-architect betrekken?
Organisatie: strategie/data/processen/technologie onduidelijk → betrek vroeg. Project: autonomie, meerdere databronnen, schaal, operationele continuïteit → betrek vanaf start.

## AI-systeemcategorisering
- Workflow bestaat, AI doet deeltaak → **workflowintegratie** (procesdiagram).
- Expert beslist, AI adviseert → **beslissingsondersteuning** (systeemdiagram, mens centraal).
- Agent orkestreert, handelt autonoom → **agentisch** (organigram).

## Valideren vóór live — 5 checks
Beveiliging · Baseline (kwaliteit/latentie/accuraatheid) · Alarmering & drempels (bv. >5% foutief gerouteerd → alarm) · Schaalbaarheid (kosten schalen exponentieel) · Noodstop.

## 6 faaloorzaken — herkennen (tells)
1. Zelfde vraag, ander antwoord → geen unieke bron van waarheid.
2. "Wie kan hier allemaal bij?" → autorisatielaag ontbreekt.
3. Geen uitleg voor AI-beslissing → black box, geen logging.
4. "We kunnen niet meer weg" → leverancierspecifieke formaten.
5. Steeds vaker mis → modeldrift, geen monitoring.
6. Werkt met 10 gebruikers, faalt met 5.000 → geen schaalbaarheidsanalyse.

## Agentische AI — 3 documenten vóór livegang
Taakomschrijving (doel + bevoegdheidsgrenzen) · Escalatieprotocol (wanneer/wie neemt mens over) · Verantwoordingslog (waarom handelde de agent). Plus grenzen van aandacht (wanneer start/stopt handelen).

## Maturiteitsniveaus — indicatief
AI verkenner: use cases verkennen, basistraining. AI piloot: 1–3 use cases, roadmap, ethisch kader. AI expert: meerdere use cases, governancekader, innovatiebudget, AI-expertgroep.
