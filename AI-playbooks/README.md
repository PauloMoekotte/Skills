# AI Playbooks voor de Vlaamse Onderwijssector

Drie complementaire skills voor AI-governance in onderwijs, gegenereerd via de `book-to-skill` workflow uit officiële overheidsplaybooks.

## Wat zit erin?

| Skill | Bron | Fokus |
|-------|------|-------|
| **uk-government-ai-playbook** | GDS/Cabinet Office (UK, 2025) | Principes, DPIA, security, inkoop, governance — verantwoord AI-proces |
| **amsterdam-ai-playbook** | Amsterdam CTO & World Enabled | Inclusie, toegankelijkheid, stakeholderbetrokkenheid — "nothing about us without us" |
| **vlaanderen-ai-playbook** | Digitaal Vlaanderen | Strategie, use cases, EU AI Act, verandermanagement, architectuur, agentische AI |

Samen dekken ze de volledige keten: **ambitie → use case → juridisch/ethisch → inkoop → governance → monitoring**, met speciale aandacht voor de onderwijscontext.

---

## Snel starten — voor wie?

### 🎯 Bestuurders & Directeuren
> **Bestandsnaam**: `uk-government-ai-playbook/intro-bestuurders-directeuren.md`

**Kernbeslissingen die op uw bureau liggen:**
1. **AI-ambitie** — kies focus via OKR's en business case (niet "we moeten AI", maar "welk probleem lossen we op?")
2. **EU AI Act is verplichting** — AI voor toelating/beoordeling van studenten = **hoog-risico** → DPIA + FRIA
3. **Accountability** — de leraar blijft eindverantwoordelijk; AI = beslissingsondersteuning
4. **Kind-rechten** — elke DPIA krijgt een kind-rechtenparagraaf (Children's Code/UNCRC)
5. **Governance** — AI-inventaris als openbaar register, overlegorganen op 3 niveaus
6. **Inkoop** — dataminimalisatie, exitstrategie, leveranciersonafhankelijkheid in elk bestek

**Eerste stappen:**
- Laat een AI-inventaris maken (incl. schaduw-AI)
- Vraag een quick scan (Vlaanderen playbook ch05)
- Wijs één AI-coördinator aan
- Plan AI-geletterdheid in (wettelijke plicht, EU AI Act)
- Stel vóór elk initiatief een meetbaar leerdoel vast

---

### 👩‍🏫 Onderwijsmanagers & Docenten
> **Bestandsnaam**: `uk-government-ai-playbook/intro-docenten-onderwijsmanagers.md`

**In de klas — do's & don'ts:**

| Doen | Niet doen |
|------|-----------|
| AI als tutor/assistent, jij controleert | Blind vertrouwen op AI-detectie (valse positieven!) |
| Transparant zijn over AI-gebruik | Zelfstandig beoordelen/cijferen door AI |
| Toegankelijkheid checken (SEN) | Gedrag monitoren zonder proportionaliteitstoets |
| AI-geletterdheid samen met leerlingen | Leerlingdata in gratis online tools (schaduw-AI) |

**Toetsing & integriteit:**
- Volg instellingsbeleid: communiceer duidelijk wat wel/niet mag
- Meet **eerlijkheid én accuraatheid**, niet alleen accuraatheid
- Bij twijfel over "AI-werk": het gesprek telt, niet de detector

**Jouw rol in de organisatie:**
- Melden: zet gebruikte tools op de AI-inventaris
- Meebepalen: stem mee in het overlegorgaan (personeel = stakeholder, geen toeschouwer)
- Vragen om ondersteuning: opleiding is recht én plicht (AI Readiness Check)

---

## Diepgang: de gap-analyse

> **Bestandsnaam**: `uk-government-ai-playbook/gaps-education-context.md`

Een gedetailleerde analyse (11 lacunes) die per onderwerp laat zien wat de UK/Amsterdam/Vlaanderen playbooks **wel** dekken en wat **ontbreekt** voor onderwijs — met een actie-checklist van 11 concrete stappen. Combineert de drie skills tot één werkproces:
`Strategie → Use cases → Inclusie → Juridisch → Inkoop → Governance → Monitoring`.

---

## Structuur per skill

Elke skill heeft dezelfde indeling:
```
skill-naam/
├── SKILL.md              # Hoofdindex met frameworks, chapter index, topic index
├── chapters/
│   ├── ch01-...md        # Per hoofdstuk: core idea, frameworks, worked example, takeaways
│   └── ...
├── glossary.md           # Termen met definities
├── patterns.md           # Herbruikbare werkwijzen/patronen
└── cheatsheet.md         # Beslissingsregels, matrices, drempelwaarden
```

**UK playbook** heeft daarbij: `gaps-education-context.md`, `intro-bestuurders-directeuren.md`, `intro-docenten-onderwijsmanagers.md`.

---

## Gebruik in opencode / Claude / andere agents

De skills zijn beschikbaar via skillshare en werken in alle grote AI-tools (opencode, Claude, Cursor, Windsurf, etc.). In opencode:

```
/skill uk-government-ai-playbook        # laad de UK skill
/skill amsterdam-ai-playbook            # laad de Amsterdam skill
/skill vlaanderen-ai-playbook           # laad de Vlaanderen skill
```

Of vraag direct naar een onderwerp:
> "Wat is de EU AI Act tijdslijn voor onderwijs?" → laadt automatisch Vlaanderen ch03  
> "Hoe doe ik een DPIA voor een proctoring-tool?" → laadt UK ch07 + gap-analyse §5

---

## Licentie & bronnen

- **UK playbook**: Crown copyright, Open Government Licence v3.0
- **Amsterdam playbook**: City of Amsterdam / World Enabled, open access
- **Vlaanderen playbook**: Digitaal Vlaanderen, openbaar
- **Deze skills**: gegenereerd via `book-to-skill` (MIT-licentie), geen officiële vertalingen

> **Disclaimer**: Dit zijn beslissingshulpmiddelen, geen juridisch advies. Raadpleeg altijd uw eigen jurist, DPO, examenreglementen en de EU AI Act voor verplichte trajecten.

---

## Bijdragen / Vragen

Issues en PR's welkom op [GitHub](https://github.com/PauloMoekotte/Skills).

Voor vragen over de inhoud: raadpleeg de desbetreffende `chapters/` of de `gaps-education-context.md` voor de onderwijs-specifieke vertaling.