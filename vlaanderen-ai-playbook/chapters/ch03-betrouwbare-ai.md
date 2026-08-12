# Hoofdstuk 3: Betrouwbare AI

## Core Idea
Betrouwbare AI vraagt om het identificeren van alle AI-systemen (inclusief schaduw AI), het inschatten van risico's volgens de EU AI Act-risicoclassificatie, het hanteren van een ethisch kader met leidende principes, en doorlopende monitoring op zowel mens- als machinedimensie. Doel: risico's mitigeren, transparantie verzekeren en vertrouwen van burgers behouden.

## Frameworks Introduced
- **Identificatie van AI-systemen (3 types)**:
  - Wanneer gebruiken: als startpunt van de pijler.
  - Hoe: onderscheid doelbewuste AI (zelf gebouwd of aangekocht), incidentele AI (ingebedde AI-componenten in software) en schaduw AI (online tools die medewerkers zonder officieel mandaat gebruiken). Breng schaduw AI via communicatie en opleiding in kaart.
- **EU AI Act — risicoclassificatie (4 categorieën)**:
  - Wanneer gebruiken: voor elk geïdentificeerd AI-systeem.
  - Hoe: bepaal rol (ontwikkelaar vs gebruiker), doel & impact op personen, en risiconiveau:
    1. Verboden praktijken — sociale scoring, emotieherkenning op werkvloer, gedragsmanipulatie.
    2. Hoog-risico — kritieke infrastructuur, politie/justitie, rekrutering, onderwijs, toegang tot publieke diensten.
    3. Beperkt risico/transparantie — GenAI-chatbots; transparantieverplichtingen zoals "je praat met een chatbot".
    4. Minimaal risico — meerderheid van de toepassingen; enkel AI-geletterdheid en vrijwillige gedragscodes.
- **Tijdslijn EU AI Act**: in werking 1/8/2024; verboden praktijken + AI-geletterdheid 2/2/2025; GPAI-modellen 2/8/2025; rest + bijlage III hoog-risico + transparantie + FRIA 2/8/2026; bijlage I hoog-risico 2/8/2027; alle hoog-risico (incl. bestaande) 2/8/2030.
- **Risicostrategie (4 risicotypes)**: oplossingsrisico (focus van EU AI Act — datakwaliteit, beveiligingslekken, schaalbaarheid, synthetische data), technologierisico, projectrisico, organisatierisico.
  - Wanneer gebruiken: bij het opzetten van een risicobeheersingsstrategie.
  - Hoe: pak eerst de meest significante risico's aan, niet elk klein risico.
- **Ethisch kader — 6 leidende principes (Digitaal Vlaanderen)**: democratisch, betrouwbaar, mensgericht, AI-bewustwording, correct datagebruik & -beheer, duurzaam.
  - Wanneer gebruiken: bij elke AI-inzet; vertrek van moraal vs ethiek (ethiek = organisatiespecifieke reflectie).
  - Hoe: koppel principes aan het eigen beleidsplan en maak ze operationeel.
- **8 voorwaarden voor betrouwbare AI (ALTAI)**: maatschappelijk & milieuwelzijn; transparantie & uitlegbaarheid; verantwoording & betwistbaarheid; menselijke controle & toezicht; rechtvaardigheid & non-discriminatie; rechtmatigheid & naleving; robuustheid & veiligheid; privacy & gegevensbescherming.
  - Wanneer gebruiken: als zelfevaluatie-checklist per systeem.
  - Hoe: gebruik ALTAI-checklist, KDM-gids of AI Assessment Tool; betrek ook ALLY (Autonomous Agency/AI).
- **GenAI-risicotypologie**: bias, hallucinaties, gebrek aan transparantie, copyrightschending, gegevensbescherming (AVG), automatiseringsparadox, beheer van externe systemen, overfitting.
  - Wanneer gebruiken: bij het opstellen van richtlijnen voor (Gen)AI-gebruik.
  - Hoe: vertaal elk risico naar een concrete richtlijn (bescherm gevoelige info, dubbelcheck output, voeg eigen waarde toe, wees transparant over AI-gebruik, veilig aan de slag, milieubewustzijn, scheid professioneel/persoonlijk gebruik, word voldoende ervaren).
- **Risico- & controleraamwerk**: mitigeer via 3 complementaire elementen — technische maatregelen, richtlijnen & procedures, en cultuur ("culture eats policies for breakfast").

## Key Concepts
- **EU AI Act**: eerste horizontale AI-wetgeving; risicogebaseerde benadering.
- **DPIA**: gegevensbeschermingseffectbeoordeling (AVG).
- **FRIA**: grondrechtenimpactbeoordeling (EU AI Act).
- **Automatiseringsparadox**: hoe beter GenAI presteert, hoe meer we vertrouwen en hoe minder kritisch we worden.
- **Schaduw AI**: niet-goedgekeurde AI-tools die toch gebruikt worden.
- **AI-risicoregister**: levend register van geïdentificeerde AI-systemen, hun risiconiveau en mitigatiemaatregelen.

## Mental Models
- "AI kan niets 'vergeten': data zit onomkeerbaar in het model — vooraf goed nadenken over datagebruik."
- "Transparantie is het fundament van vertrouwen; risicomitigatie is geen administratieve overlast maar een vertrouwensinvloed."
- "Hoe geavanceerder GenAI, hoe groter de automatiseringsparadox — kritisch blijven op output."

## Anti-patterns
- Schaduw AI negeren i.p.v. bespreekbaar maken via communicatie/opleiding.
- GenAI-output klakkeloos overnemen zonder dubbelcheck (hallucinaties).
- Gevoelige/privacygevoelige data in publieke tools invoeren.
- Enkel technische maatregelen inzetten zonder cultuurverandering.
- AI-gebruik geheimhouden voor burgers i.p.v. transparantie in te bouwen.

## Worked Example
Een overheidsorganisatie wil een chatbot voor burgers over subsidies. Identificatie: doelbewuste AI (zelf gebouwd). Classificatie volgens EU AI Act: beperkt risico → transparantieverplichtingen (burger moet weten dat hij met AI praat). Risicoanalyse op oplossingsniveau: hallucinaties en datakwaliteit zijn de grootste risico's → richtlijn "dubbelcheck output", menselijk toezicht en een duidelijke disclaimer. Er wordt een ethisch kader toegepast (6 principes), en de 8 ALTAI-voorwaarden dienen als zelfevaluatie. Monitoring: menselijke dimensie (aantal incidenten, % medewerkers dat richtlijnen kent) en machinedimensie (bias/fairness-checks, transparantie van output). Resultaat: risico's zijn gemitigeerd en vertrouwen blijft behouden.

## Key Takeaways
1. Breng alle AI-systemen in kaart, inclusief schaduw AI.
2. Classificeer elk systeem volgens de EU AI Act en ken de tijdslijnen.
3. Pas een ethisch kader toe met 6 principes en evalueer met de 8 ALTAI-voorwaarden.
4. Stel GenAI-richtlijnen op die elke risico in de typologie adresseren.
5. Monitor doorlopend op mens- én machinedimensie; gebruik een AI-risicoregister.

## Connects To
- **Ch 1 (Visie & strategie)**: risico- en ethisch kader beïnvloeden de ambitie.
- **Ch 2 (Innovatie)**: juridische/ethische haalbaarheid en DPIA maken deel uit van use case ontwikkeling.
- **Ch 4 (Mens & organisatie)**: AI-bewustwording en opleiding ondersteunen schaduw AI-beheer.
- **Ch 5 (AI-Architectuur)**: toegangscontrole, uitlegbaarheid en monitoring zijn architecturale verantwoordelijkheden.
