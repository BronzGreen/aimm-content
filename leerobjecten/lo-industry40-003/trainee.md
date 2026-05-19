---
id: lo-industry40-003-trainee
knowledge_object_id: ko-industry40-003
version: trainee
title: Van data naar actie — hoe een AI-systeem op de werkvloer komt
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: onbewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 45
status: validated
updated_at: '2026-05-19'
correlation_id: ronde4-lo-industry40-003
---

# Van data naar actie — hoe komt een AI-systeem op je werkvloer?

Een AI-project op de werkvloer duurt vaak maanden. Niemand op de lijn weet precies waarom. De leverancier zegt: "het komt eraan." Het management zegt: "we zijn al ver." En dan, op het beloofde moment, gebeurt er nog niets. Deze sessie legt uit wat er tussen "we verzamelen data" en "er staat een melding op het scherm" gebeurt. In zes stappen, in 45 minuten, zonder IT-jargon.

## Wat leer je?

Je kunt na deze sessie de zes stappen van een AI-pipeline (de keten van data tot werkende melding) in eigen woorden benoemen. En je kunt aanwijzen in welke stap een AI-project bij jullie vaak vastloopt.

## Een AI-pipeline is net een productielijn

Een AI-pipeline (de keten van stappen om AI op de werkvloer te krijgen) lijkt op een productielijn. Elke stap voegt iets toe. Sla je een stap over? Dan werkt het eindproduct niet. En sommige stappen zijn lastiger dan andere — net als bij echte productie.

Stel je voor: een producent van automotive-onderdelen wil voorspellen wanneer een product afgekeurd wordt. Zes maanden geleden zijn ze begonnen. Vorige maand zou het systeem live gaan. Maar het ging niet live. Wat ligt daar dan tussen? Veel meer dan je denkt.

## De zes stappen

Hieronder de zes stappen die elk AI-project op de werkvloer doorloopt. De stappen komen uit Cutrona et al. (2024), Artificial Intelligence in Manufacturing.

1. **Data voorbereiden.** Verzamel data uit de machines, sensoren en systemen. Maak de data schoon. Verwijder fouten. Vul ontbrekende waarden aan. Zorg dat alles in hetzelfde formaat staat. Dit is bij veel projecten de langste stap.
2. **Model ontwikkelen.** Een data scientist (datadeskundige) bouwt en traint een AI-model met de voorbereide data. Het model leert patronen herkennen. Bijvoorbeeld: welke combinatie van temperatuur en druk leidt tot afkeur.
3. **Model inpakken.** De IT-afdeling verpakt het model zodat het kan draaien in de bedrijfsomgeving. Een technische stap — het model wordt "installeerbaar" gemaakt.
4. **Model valideren.** Het team test het model voordat het in productie gaat. Klopt de nauwkeurigheid? Werkt het betrouwbaar? Geeft het geen rare resultaten?
5. **Model uitrollen.** De IT-afdeling installeert het gevalideerde model in de productieomgeving. Het koppelt aan bestaande systemen zoals MES (Manufacturing Execution System — voor productieplanning) en ERP (Enterprise Resource Planning — voor bedrijfsvoering).
6. **Model gebruiken.** Nu draait het model in de dagelijkse praktijk. Operators zien de resultaten op hun dashboard en kunnen erop handelen.

## Waar gaat het vaak mis?

De stappen 3, 4 en 5 — inpakken, valideren en uitrollen — zijn vaak het knelpunt. Een model dat goed werkt in het lab van de data scientist, werkt niet automatisch op de werkvloer. Een paar redenen waarom dit lastig is:

- **Andere data op de werkvloer dan in het lab.** De data scientist heeft getest met nette historische data. Op de werkvloer staan sensoren soms uit. Of er komt een nieuwe machine bij.
- **Koppeling aan bestaande systemen.** Het model moet praten met het MES, het ERP en de dashboards. Dat is technisch werk.
- **Vertrouwen winnen.** Operators willen zien dat het systeem klopt voordat ze erop vertrouwen. Dat kost weken of maanden.

Platforms zoals KITT4SME (een Europees AI-platform voor het mkb) proberen deze stappen te vereenvoudigen. Ze leveren bouwstenen die de stappen 3, 4 en 5 deels automatiseren.

## Wat betekent dit voor jou?

Je hoeft als operator of teamleider niet alle zes stappen zelf uit te voeren. Maar wie de stappen kent, herkent waar het project zit. Een paar dingen die je dan kunt:

- **Meepraten** als de leverancier of IT met een planning komt. "Welke stap doen jullie nu?"
- **Doorvragen** als beloftes opschuiven. "Zit het bij valideren, of nog bij inpakken?"
- **Herkennen** dat een vertraging logisch is — bij stap 3, 4 of 5 is het vaak normaal.
- **Gerichte vragen** stellen aan IT, onderhoud of de data scientist over wat zij precies aan het doen zijn.

## Een voorbeeld uit de praktijk

Bij een producent van automotive-onderdelen wilde men afkeur voorspellen. Het project liep zo: stap 1 — ze verzamelden zes maanden machine- en kwaliteitsdata. Stap 2 — een data scientist bouwde een voorspelmodel. Stap 3 en 4 — het model werd verpakt en getest op historische data. Stap 5 — het werd gekoppeld aan het MES. Stap 6 — operators zien nu een waarschuwing op hun scherm als de kans op afkeur boven de 80 procent komt.

Tussen stap 1 en stap 6 zaten ongeveer negen maanden. Dat is normaal voor een eerste AI-project. Bij de tweede toepassing op dezelfde lijn ging het sneller — veel werk uit stappen 3 tot 5 was hergebruikbaar.

## Na deze sessie

Kies deze week één AI-traject of slim systeem dat bij jullie loopt. Denk aan een camera-inspectie, een voorspellend onderhoudssysteem of een dashboard met afwijkingsmeldingen. Praat er kort over met IT, de teamleider of de leverancier. Noteer drie dingen: welk systeem het is, in welke pipeline-stap het volgens hen nu zit, en wat de eerstvolgende stap is. Neem je notities mee naar de volgende sessie.

Lees daarnaast deze week één keer een nieuwsbericht over AI in de industrie. Probeer te zien in welke stap dat verhaal zich afspeelt — bij data, bij testen, of al in gebruik.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-casus-automotive-afkeur.md`](./werkbladen/wb-01-casus-automotive-afkeur.md) — Casus automotive afkeur
2. [`wb-02-duo-vergelijking.md`](./werkbladen/wb-02-duo-vergelijking.md) — Duo vergelijking
3. [`wb-03-zes-stappen-handout.md`](./werkbladen/wb-03-zes-stappen-handout.md) — Zes stappen handout
4. [`wb-04-eigen-pipeline.md`](./werkbladen/wb-04-eigen-pipeline.md) — Eigen pipeline

## Verder

- Onderliggend kennisobject: [`ko-industry40-003`](../../kennisbank/industry_4_0/smart_factory_concepten/ko-industry40-003.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
