---
id: lo-ai-fund-117-trainee
knowledge_object_id: ko-ai-fund-117
version: trainee
title: Drie vormen van machine learning — welke past bij welk maakindustrie-probleem?
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 42
status: validated
updated_at: '2026-05-19'
correlation_id: ronde9-lo-ai-fund-117
---

# Hoe leert AI? Twee systemen op jouw lijn, één leerprincipe

Op Lijn B bij Van Daalen Plastics werken twee AI-systemen. **InspectAI** kijkt met een camera naar elk zijpaneel. **CycleAdvise** geeft advies over de cyclustijd. Beide leren uit data. Maar de data ziet er totaal anders uit. In deze sessie kijk je voor het eerst onder de motorkap.

## Wat leer je?

Je leert de drie vormen van machine learning herkennen. Je ziet dat InspectAI en CycleAdvise hetzelfde leerprincipe gebruiken — met heel andere data. Je weet welke vraag je kunt stellen over de data op jouw lijn.

## Sanne kijkt mee — twee systemen, één principe

Sanne is operator op Lijn B. Vandaag laat Joyce van kwaliteit haar de trainingsset van InspectAI zien. En Karim van onderhoud opent het bestand van CycleAdvise. Twee laptops naast elkaar.

### InspectAI — leren van foto's

Joyce klikt een map open. Er staan 4.000 foto's in. Foto's van zijpanelen die de afgelopen maanden langs de camera kwamen. Bij elke foto staat een label. Joyce wijst:

- Foto 0001 → **GOED**
- Foto 0002 → **TWIJFEL** (lichte krasvorming)
- Foto 0003 → **AFGEKEURD** (vlekken)
- Foto 0004 → **GOED**

"Iemand heeft bij elke foto het antwoord gezet," zegt Joyce. "Wij van kwaliteit. We hebben drie maanden gelabeld voordat InspectAI live ging."

Sanne snapt het. *Dít is waar mijn oordeel in het systeem komt.* InspectAI heeft die 4.000 voorbeelden uit het hoofd geleerd. Nu kan de camera nieuwe foto's herkennen.

### CycleAdvise — leren van een tabel

Karim opent een ander bestand. Geen foto's. Een tabel met 4.000 rijen. Elke rij is één cyclus van de spuitgietmachine.

| Rij | Mal-temperatuur | Druk | Cyclustijd | Uitval | Label |
|---|---|---|---|---|---|
| 1 | 64 °C | 820 bar | 22,1 sec | 0,8 % | NIET BIJSTELLEN |
| 2 | 67 °C | 815 bar | 22,3 sec | 2,1 % | BIJSTELLEN |
| 3 | 71 °C | 810 bar | 22,8 sec | 4,4 % | BIJSTELLEN |
| 4 | 63 °C | 820 bar | 22,0 sec | 0,7 % | NIET BIJSTELLEN |

"Ik heb zes maanden meegekeken," zegt Karim. "Bij elke rij heb ik genoteerd: moest je hier bijstellen of niet? Dat is mijn antwoord per cyclus."

Sanne kijkt. *Geen foto's. Wel hetzelfde idee.* Iemand heeft per voorbeeld een antwoord gezet. CycleAdvise heeft uit die 4.000 rijen geleerd. Nu geeft het systeem advies bij elke nieuwe cyclus.

### Het contrast — andere data, zelfde principe

Twee systemen. Heel andere data. Maar één ding is gelijk: **bij elk voorbeeld staat een antwoord erbij**. Dat heet **supervised learning** — leren met gelabelde voorbeelden.

| Wat | InspectAI | CycleAdvise |
|---|---|---|
| Data-vorm | Foto's | Tabel met meetwaarden |
| Wie labelt? | Joyce (kwaliteit) | Karim (onderhoud) |
| Aantal voorbeelden | 4.000 | 4.000 |
| Antwoord per voorbeeld | GOED / TWIJFEL / AFGEKEURD | BIJSTELLEN / NIET BIJSTELLEN |
| Leerprincipe | Supervised | Supervised |

## Drie vormen van machine learning

Bij beide systemen zit er een antwoord bij elk voorbeeld. Dat is supervised. Maar er bestaan twee andere vormen.

### 1. Supervised — leren met voorbeelden

Bij supervised heeft een mens vooraf het antwoord gezet. Het systeem leert het verschil tussen de klassen. Daarna kan het nieuwe data beoordelen.

Kerngedachte: **je hebt labels nodig**. Geen labels, geen supervised.

InspectAI en CycleAdvise zijn allebei supervised. De data-vorm verschilt — foto's tegenover een tabel — maar het leerprincipe is hetzelfde.

### 2. Unsupervised — patronen ontdekken zonder labels

Bij unsupervised heeft niemand antwoorden gezet. Het systeem zoekt zelf naar groepen of afwijkingen.

Een voorbeeld: een lasrobot maakt zes maanden lang 50.000 lasnaden. Niemand heeft gemarkeerd welke goed of fout waren. Toch wil de productieleider weten of bepaalde dagen anders lopen. Het systeem ontdekt zelf dat er twee soorten dagen zijn.

Kerngedachte: **geen labels, wel patronen**.

### 3. Reinforcement — leren door proberen

Bij reinforcement probeert het systeem iets en krijgt direct een score. Lukt het? Beloning. Mislukt het? Straf. Door duizenden pogingen leert het de beste strategie.

Een voorbeeld: een verpakkingsrobot mag zelf zijn grijpkracht aanpassen. Product heel: +1 punt. Product beschadigd: -1 punt. Na duizenden pogingen weet hij hoe hard hij moet knijpen.

Kerngedachte: **leren door te doen, score per actie**.

> Vuistregel: op de werkvloer kom je als operator vooral supervised en unsupervised tegen. Reinforcement is bijzonder en vaak alleen bij geavanceerde robots.

## Hoe herken je welke vorm past?

Stel deze drie vragen over de data op jouw lijn:

1. **Staat er bij elk voorbeeld een antwoord?** Ja → supervised. Nee → ga naar vraag 2.
2. **Krijgt het systeem een score na elke poging?** Ja → reinforcement. Nee → ga naar vraag 3.
3. **Zoeken we groepen of afwijkingen in de data?** Ja → unsupervised.

Een leverancier die zegt "wij doen supervised" verwacht dat jullie gelabelde voorbeelden leveren. Heb je die niet, dan stokt het project. Een leverancier die unsupervised werkt, vraagt geen labels — maar levert ook geen kant-en-klare voorspelling. Wie het verschil kent, leidt zo'n gesprek.

## Na deze sessie

Kies deze week één plek op Lijn B of op jouw eigen lijn. Bijvoorbeeld het inspectiestation, de spuitgietmachine of een sensor in het magazijn. Schrijf drie dingen op. Eén: welke data verzamelen we daar? Twee: staat er bij elk voorbeeld een antwoord? Drie: welke vorm past — supervised, unsupervised of reinforcement? Neem dat blaadje mee.

Praat er deze week ook één keer over met een collega van onderhoud of kwaliteit: *"Houden wij ergens vast wanneer er iets misgaat — en zo ja, hoe?"* Vaak zit die informatie al ergens. In logboeken of vrije tekstvelden. Maar nog niet zo geordend dat een AI ervan kan leren. Dat is een waardevolle ontdekking.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-scenarios-drie-vormen.md`](./werkbladen/wb-01-scenarios-drie-vormen.md) — Scenarios drie vormen
2. [`wb-02-reflectie-signaalwoorden.md`](./werkbladen/wb-02-reflectie-signaalwoorden.md) — Reflectie signaalwoorden
3. [`wb-03-handout-drie-vormen.md`](./werkbladen/wb-03-handout-drie-vormen.md) — Handout drie vormen
4. [`wb-04-eigen-lijn-verkenning.md`](./werkbladen/wb-04-eigen-lijn-verkenning.md) — Eigen lijn verkenning

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-117`](../../kennisbank/ai_fundamentals/machine_learning_basics/ko-ai-fund-117.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
