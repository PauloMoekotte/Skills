# Hoofdstuk 5: AI-Architectuur

## Core Idea
AI-architectuur verbindt strategie, data, processen en technologie en vormt de basis voor elk AI-initiatief. Meer dan 80% van de AI-initiatieven faalt vóór productie (RAND, 2024) — vaak door vermijdbare architecturale problemen. De AI-architect bewaakt randvoorwaarden op organisatieniveau en stuurt architecturale keuzes op projectniveau, van probleemvalidatie tot operationele bewaking.

## Frameworks Introduced
- **6 probleemstellingen (waarom AI-projecten falen)**:
  - Wanneer gebruiken: om architecturale risico's te herkennen en te voorkomen.
  - Hoe: (1) tegenstrijdige data — geen unieke bron van waarheid → data governance & interoperabiliteit; (2) ongecontroleerde toegang → autorisatielaag met CISO/DPO; (3) onuitlegbare beslissingen → monitoringsysteem dat factoren, zekerheid en gebruikte data logt; (4) vendor lock-in → open formaten & standaarden eisen; (5) AI-modeldrift → monitoring & bijsturingsstrategie; (6) schaalbaarheid → schaalbaarheidsanalyse, caching, goedkopere modellen voor eenvoudige taken.
- **Rollen in AI-architectuur**: AI-architect (coördinator: AI-governance, infrastructuur- & modelkeuzes, agentische architectuur, AI-risico's), data architect, enterprise architect, solution architect.
  - Hoe: de AI-architect opereert op 2 niveaus — organisatie (structurele randvoorwaarden) en project (concrete keuzes). Kan een aparte functie zijn of door een bestaande architect worden opgenomen.
- **Quickscan AI-architectuur**: eerste inschatting van gereedheid.
  - Wanneer gebruiken: bij elk AI-project.
  - Hoe: organisatieniveau — strategie, data, processen, technologie & leveranciers; projectniveau — autonomie, databronnen & integratie, schaal, operationele continuïteit. Meer vinkjes → AI-architect vroeg betrekken.
- **Organisatieniveau — 4 grondstoffen**: verwachtingen & strategie (gedeeld realistisch beeld, 3 kernvragen: welk probleem lossen we op, is AI adequaat & proportioneel, hoe meten we succes; polarisatie wantrouwen vs overmatig vertrouwen), data (kwaliteit & herkomst, toegang vs gebruik vs hergebruik — modeltraining vereist expliciete licentie; datastandaarden & levenscyclus; centraal vs decentraal), processen (explicitering incl. uitzonderingen/escalaties/randgevallen; validatie & versiebeheer), technologie & leveranciers (cloudsoevereiniteit, leveranciersonafhankelijkheid, exitstrategie).
- **AI-systeemcategorisering (3 categorieën)**:
  - Wanneer gebruiken: tijdens projectvoorbereiding.
  - Hoe: (1) workflowintegratie — AI voert deeltaak uit in bestaande workflow (orkestratie door workflow); (2) beslissingsondersteuning — expert is orkestmeester, AI ondersteunt (human-in-the-loop); (3) agentische systemen — AI-agent is orkestmeester, vereist organisatiekunde (zie ch06). Maak per categorie een schets: procesdiagram, systeemdiagram of organigram.
- **Projectniveau — voorbereiding (3 stappen)**: probleemvalidatie (kernvragen: concreet probleem? meerwaarde AI vs eenvoudiger alternatief? versnelling van verkeerde werkwijze?), AI-systeemcategorisering, en gereedheidscheck (strategie/data/processen/technologie op projectniveau met budget, tijdspad, stakeholders, escalatiepunt, draagvlak).
- **Projectuitvoering (architecturale sturing)**: informatiestromen (traceerbaarheid van wie welke informatie krijgt), integratie tussen componenten (API's, event-driven), monitoring & prestatiebewaking (modeldrift detecteren), uitlegbaarheid (inbouwen tijdens ontwerp, niet achteraf), documentatie & wettelijke vereisten (DPIA + FRIA vóór ontwikkelfase), toegangscontrole & beveiliging (autorisatielaag; AI leert van data waartoe het toegang heeft).
- **Valideren vóór live (5 checks)**: beveiligingsvalidatie, baselinebepaling (verwachte antwoordkwaliteit, latentie, nauwkeurigheid), alarmering & drempelwaarden (bv. >5% foutief gerouteerde aanvragen → alarm), schaalbaarheidsvalidatie (tokenverbruik/API-kosten schalen exponentieel), noodstopprocedures.
- **Operationeel bewakingskader**: oorzaakanalyse bij degradatie (inputdata veranderd? context? model?), kostenbewaking (kostengrenzen & alerts; kostenexplosie bij lage gebruikersaantallen = architecturaal signaal), impact van wijzigingen (nieuwe modelversie/prompt kan bijwerkingen hebben), evoluerende regelgeving (EU AI Act wordt strenger over tijd).
- **Architecturale gezondheid — indicatoren**: % projecten met 4 gereedheidschecks doorlopen, % met AI-architect vanaf start, incidenten per kwartaal (architecturale oorzaak), afwijking geraamde vs werkelijke infrastructuurkosten, % met gedocumenteerde exitstrategie, % actieve systemen met actuele architectuurdocumentatie, % periodieke bias-checks. Bespreek per kwartaal in stuurgroep/architectuurboard.

## Key Concepts
- **Modeldrift**: model getraind op data van een moment, maar de wereld verandert → model degradeert; zonder feedback neerwaartse spiraal.
- **Unieke bron van waarheid / golden dataset**: referentieset van correcte input-outputcombinaties waartegen AI-output getoetst wordt.
- **Cloudsoevereiniteit**: waar draait de data, welke wetgeving is van toepassing.
- **Vendor lock-in**: vastzitten in leverancierspecifieke formaten waardoor migratie alles herbouwen betekent.
- **Exitstrategie**: hoe makkelijk kan men van leverancier wisselen zonder expertise te verliezen.
- **DPIA / FRIA**: gegevensbeschermings- resp. grondrechtenimpactbeoordeling (EU AI Act).
- **Architectuurplan**: technisch ontwerp + governance framework + operationeel model.

## Mental Models
- "Architectuur = een bouwwerk dat tegelijk een blokkendoos blijft: continu uitbreidbaar, veranderingen kunnen herbergen."
- "Wat je een AI-systeem niet vertelt, vult het zelf in — met aannames die niet zichtbaar en niet noodzakelijk correct zijn."
- "De kloof tussen persoonlijke productiviteit en organisatorische inzet: organisatorische AI moet integreren, voldoen aan regelgeving en consistent presteren op schaal."
- "Schaalbaarheid: een systeem dat werkt met 10 gebruikers kan falen met 5.000 — kosten schalen niet lineair maar exponentieel."

## Anti-patterns
- Procesdocumentatie uitstellen ("we bouwen eerst de app, documenteren later") → project stopt halverwege.
- Referentie nemen naar persoonlijke AI-tools → onderschatte tijdlijnen en budgetten.
- Geen exitstrategie → opgesloten bij één leverancier.
- Autorisatielaag vergeten → AI-agenten die data raadplegen waar ze geen toegang toe hebben.
- Geen baseline & alarmering → degradatie onzichtbaar tot het te laat is.
- AI-projecten starten zonder quickscan en zonder AI-architect.

## Worked Example
Een organisatie bouwt een AI-assistent voor dossierbehandeling (OCMW-voorbeeld). Zonder architectuur krijgt het systeem toegang tot alle dossiers — dossierbehandelaars kunnen plots vragen stellen over dossiers waar ze geen toegang toe hebben: een AVG-overtreding. De AI-architect ontwerpt samen met CISO & DPO een autorisatielaag die vastlegt wie wat mag opvragen, hoe dat gelogd wordt en hoe gecontroleerd wordt dat het systeem zich aan de regels houdt. Verder: uitlegbaarheid (loggen welke factoren wegen), modeldrift-monitoring, baseline voor antwoordkwaliteit, en een noodstop. Het systeem gaat pas live na de 5 validatiechecks.

## Key Takeaways
1. Herken de 6 klassieke faaloorzaken en adresseer ze vroeg.
2. Gebruik de quickscan om de gereedheid te bepalen op organisatie- en projectniveau.
3. Borg op organisatieniveau: verwachtingen/strategie, data, processen, technologie & leveranciers.
4. Categoriseer elk systeem (workflowintegratie, beslissingsondersteuning, agentisch) en teken de juiste schets.
5. Valideer vóór live: beveiliging, baseline, alarmering, schaalbaarheid, noodstop.
6. Bewaak na live: drift, kosten, impact van wijzigingen, evoluerende regelgeving.

## Connects To
- **Ch 1 (Visie & strategie)**: verwachtingen & strategie als eerste grondstof.
- **Ch 3 (Betrouwbare AI)**: DPIA/FRIA, betrouwbaarheid & monitoring.
- **Ch 4 (Mens & organisatie)**: rollen & overlegorganen als organisatorische randvoorwaarden.
- **Ch 6 (Agentische organisatie)**: agentische systemen als derde categorie.
