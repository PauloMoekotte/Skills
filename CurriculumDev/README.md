# ai-curriculum-dev

Pas AI-modellen toe om curriculumontwikkeling en het maken van online cursussen
te versnellen. Gebruik dit bij het ontwerpen van curricula, het in kaart brengen
van leerdoelen, het uitlijnen van Cursusuitkomsten (CU's) en 
programmauitkomsten (PU's), het classificeren van
Bloom-niveaus, het bouwen van kennisgrafen/ontologieën, het sequentiëren van
cursussen, het genereren van toetsen of instructiemateriaal, of het
personaliseren van leerroutes.

> **Kernprincipe:** AI ondersteunt, vervangt nooit, het pedagogisch oordeel van
> de mens. Controleer AI-uitvoer altijd op juistheid, bias en didactische
> geschiktheid voordat je het overneemt.

## Welke aanpak past bij de taak?

| Jouw taak | Aanpak | Referentie |
|-----------|--------|------------|
| Leerdoelen taggen op Bloom-niveau; ontbrekende/oververtegenwoordigde niveaus signaleren | NLP-classificatie | Prompt A |
| Cursusuitkomsten (CU's) aligneren met programma-uitkomsten (PU's); hiaten signaleren | NLP semantische alignering | Prompt B |
| Curriculum koppelen aan standaarden/competentiekaders; overlap/hiaten opsporen | Ontologie / Kennisgraaf | Prompt C, D |
| Volgorde van cursussen adviseren; leerroutes personaliseren; prereq-problemen vinden | Recommender / Graaf | Prompt E |
| Collegeaantekeningen, toetsvragen, casussen schrijven; vereenvoudigen/adapteren | Generatieve AI | Prompt F |

## Werkwijzen

1. **Classificatie & alignering van uitkomsten (NLP)** — Classificeer
   leerdoelen op Bloom-niveau, controleer CU→PU-alignering, breng
   mismatches aan het licht, menselijke review.
2. **Competentie-/standaardenkoppeling (Ontologie + KG)** — Bouw een lichte
   kennisgraaf die uitkomsten koppelt aan kaders (bijv. SFIA, nationale
   kwalificaties); voer gap/overlap-queries uit; aligneer oude↔nieuwe kaders.
3. **Cursusvolgorde & leerroutes (Recommender + Graaf)** — Codeer de
   prerequisite-graaf, adviseer volgende cursussen, valideer tegen harde regels,
   mine succesvolle praktijkroutes.
4. **Contentgeneratie & adaptief ontwerp (Generatieve AI)** — Genereer
   eerste concepten (aantekeningen, MC-vragen, casussen), pas toon/niveau aan
   per cohort, produceer uitlegvarianten; menselijke review van elk item.

## Waarborgen (van toepassing op alle werkwijzen)

- **Hallucinatierisico** — LLM's verzinnen plausibele maar foute koppelingen.
  Combineer met curated kennisbanken + mens-in-de-lus.
- **Vertrouwen** — eis verklaarbaarheid; AI moet redenering tonen, niet alleen
  een oordeel.
- **Gelijkwaardigheid/kwaliteit** — beoordeel AI-content als peer-reviewed OER;
  betrek vakdeskundigen, ontwerpers en studentfeedback.
- **Verantwoordelijkheid blijft menselijk** — AI maakt concepten, de docent
  bezit het definitieve curriculum.

## Bestanden

- `SKILL.md` — beslissingsgids en werkwijzen (het instappunt van deze skill).
- `REFERENCE.md` — copy-paste prompts (A–F) en de onderliggende
  bewijsbasis uit Ratiarson (2025).

## Referentie

Ratiarson (2025), *"AI Models for Accelerating Curriculum Development and
Online Course Creation"* (literatuurstudie) [preprint].
