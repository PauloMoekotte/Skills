# Hoofdstuk 6: Agentische organisatie

## Core Idea
Agentische AI-systemen krijgen een doel in plaats van een stappenplan: ze bepalen zelf de weg en handelen ook zonder dat iemand hen een vraag stelt. Dit verandert wat vóór livegang gedocumenteerd moet zijn — van volledige logica naar grenzen — en vereist architectuur die lijkt op organisatiekunde.

## Frameworks Introduced
- **3 documenten vóór livegang (taakomschrijving, escalatieprotocol, verantwoordingslog)**:
  - Wanneer gebruiken: voor elk agentisch AI-systeem.
  - Hoe: (1) taakomschrijving — wat is het doel van de agent en waar stopt zijn bevoegdheid; (2) escalatieprotocol — wanneer neemt een mens het over en wie is dat; (3) verantwoordingslog — hoe weet je achteraf waarom de agent zo handelde. Ze lijken op documenten bij aanwerving van een medewerker (functiebeschrijving, werkinstructie, contact bij twijfel), maar bepalen hier de architectuur van het systeem.
- **Grenzen van aandacht**: niet alleen wat de agent doet, maar ook wanneer hij begint en stopt met handelen.
  - Wanneer gebruiken: bij het vastleggen van proactief gedrag.
  - Hoe: definieer de trigger voor handelen én de stopvoorwaarde; een agent die zonder vraag handelt (bv. ontdekt 2 maanden voor deadline dat er slechts één inschrijving is bij een overheidsopdracht en waarschuwt het aankoopteam) vereist expliciete grenzen van zijn aandacht.
- **Multi-agent samenwerking als organigram**:
  - Wanneer gebruiken: voor complexe processen met meerdere agenten.
  - Hoe: vertaal teamvragen naar een organigram — wie stuurt aan, wie escaleert bij conflict, wie neemt de eindbeslissing, wie neemt over als het misloopt. Bv. omgevingsvergunning: agent 1 haalt documenten op, agent 2 controleert volledigheid, agent 3 toetst aan regelgeving, agent 4 bereidt communicatie voor.
- **AI-architect als verkenner van het mogelijke**: naast bewaker en stuurman toont de AI-architect welke processen te duur zijn voor continue menselijke opvolging, welke dossiers vastlopen op opvolging die niemand als hoofdtaak heeft, en waar werk bleef liggen door gebrek aan VTE.

## Key Concepts
- **Agentische AI**: AI die een doel krijgt, zelf de weg bepaalt en ook handelt zonder dat er een vraag gesteld wordt.
- **Taakomschrijving**: doel en bevoegdheidsgrenzen van de agent.
- **Escalatieprotocol**: wanneer en door wie een mens overneemt.
- **Verantwoordingslog**: registratie waarom de agent handelde zoals hij handelde.
- **Grenzen van aandacht**: start- en stopvoorwaarden van de agent.
- **Organigram-architectuur**: diagram van bevoegdheden en overnamepaden (vs processchema).
- **Multi-agent systeem**: meerdere samenwerkende AI-agenten.

## Mental Models
- "Klassiek AI = volledige logica uittekenen (als-dan); agentisch AI = grenzen beschrijven (tot hier, en anders...)."
- "Denk aan een agent als een nieuwe medewerker: functiebeschrijving, werkinstructie en contactpunt bij twijfel — maar voor software."
- "Mensen voor werk dat oordeel, contact en empathie vraagt; agenten voor continuïteit, consistentie en volume."
- "De slimste organisaties zetten mensen en agenten in waar ze het beste in zijn."

## Anti-patterns
- Een agent proberen te besturen met volledig uitgetekende logica (dat is klassiek AI, geen agentisch).
- Geen escalatieprotocol → bij conflict tussen agenten of onvoorziene situatie is er geen menselijke overname.
- Geen verantwoordingslog → achteraf onverklaarbare acties van de agent.
- Autonoom handelen zonder grenzen van aandacht → agent handelt onbeperkt of start nooit.

## Worked Example
Een aanvraag voor een omgevingsvergunning: een eerste agent haalt de documenten op, een tweede controleert of alles aanwezig is, een derde toetst de inhoud aan de regelgeving, een vierde bereidt de communicatie naar de aanvrager voor. De AI-architect tekent dit als een organigram: wie stuurt aan, wie escaleert wanneer agenten het oneens zijn (bv. ontbrekend document vs automatische weigering), wie neemt de eindbeslissing. Vooraf zijn de taakomschrijvingen, het escalatieprotocol en de verantwoordingslog vastgelegd. Daarnaast signaleert een agent proactief een overheidsopdracht met slechts één inschrijving, 2 maanden vóór de deadline, zodat het aankoopteam nog kan bijsturen.

## Key Takeaways
1. Stel voor livegang 3 documenten op: taakomschrijving, escalatieprotocol, verantwoordingslog.
2. Leg de grenzen van aandacht vast: wanneer begint en stopt de agent.
3. Modelleer multi-agent systemen als organigram, niet als processchema.
4. Gebruik de AI-architect als verkenner van wat haalbaar is voor de organisatie.
5. Verdeel werk tussen mensen en agenten op basis van hun sterktes.

## Connects To
- **Ch 5 (AI-Architectuur)**: agentische systemen als derde categorie; architectuur = organisatiekunde.
- **Ch 3 (Betrouwbare AI)**: verantwoordingslog ondersteunt transparantie & uitlegbaarheid.
- **Ch 4 (Mens & organisatie)**: escalatie en verantwoordelijkheden als organisatorische principes.
