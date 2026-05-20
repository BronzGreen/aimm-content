---
id: lo-ai-fund-132-trainee
knowledge_object_id: ko-ai-fund-132
version: trainee
title: Trainingsdata — waarom kwaliteit en variatie zwaarder wegen dan hoeveelheid
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 45
status: validated
updated_at: '2026-05-19'
correlation_id: ronde11-lo-ai-fund-132
---

# Waarom levert meer trainingsdata niet vanzelf een beter AI-model op?

Leveranciers zeggen vaak: *"we hebben meer data nodig."* Maar of een AI-systeem op je lijn werkt, hangt zelden alleen af van hoeveelheid. Het hangt vaker af van of de voorbeelden kloppen. En of er genoeg variatie in zit. Wie de juiste vragen stelt aan een dataset, herkent loze claims. En weet welke data op de eigen lijn wél bruikbaar is.


## Wat leer je?

Je kunt uitleggen wat trainingsdata (leerdata) zijn. En je kunt de drie eigenschappen benoemen die bepalen of een model goed leert: hoeveelheid, kwaliteit en variatie.

## Wat zijn trainingsdata eigenlijk?

Een AI-model leert niet uit het niets. Het krijgt voorbeelden waarvan het juiste antwoord bekend is. Die voorbeelden heten **trainingsdata** (leerdata).

Een voorbeeld uit de maakindustrie: een inspectiecamera boven de lopende band moet krassen herkennen op metalen beugels. De camera krijgt honderden foto's te zien. Bij elke foto staat het antwoord erbij: *"goed"* of *"kras"*. Dat antwoord noemen we een **label** (antwoord bij een voorbeeld). Het model leert door honderden van die foto-met-label-combinaties te bekijken.

Zonder die labels weet het model niet wat goed of fout is. De labels zijn dus minstens zo belangrijk als de foto's zelf.

## Drie vragen aan elke dataset

Voor elke trainingsdataset zijn drie vragen belangrijk. Niet één — alle drie.

### 1. Kwantiteit — hoeveel voorbeelden zijn er?

Een model heeft genoeg voorbeelden nodig om patronen te zien. Te weinig voorbeelden leidt tot onbetrouwbare voorspellingen.

Vuistregel uit branche-publicaties: ongeveer 100 tot 300 voorbeeldfoto's per klasse als startpunt (te valideren per bedrijf). Voor een krasdetectie betekent dat: 100 tot 300 foto's met krassen, plus 100 tot 300 foto's zonder.

Maar — en hier wordt het interessant — meer is niet altijd beter. Hoeveelheid is pas een voordeel als de andere twee vragen ook positief zijn.

### 2. Kwaliteit — kloppen de labels?

Dit is de vraag die vaak vergeten wordt. Stel: in een dataset van 10.000 foto's staat 15% op het verkeerde label. Een goed product heet *"kras"*. Of een kras heet *"goed"*. Het model leert dan de verkeerde patronen.

Een veelgehoorde uitspraak in de AI-wereld: **garbage in, garbage out** (bron: Russell & Norvig 2021). Rommel erin, rommel eruit. Zelfs één op de tien foute labels kan een model serieus uit balans brengen.

Wie controleert eigenlijk of de labels kloppen? Op veel werkvloeren is dat een open vraag. En precies daar zit vaak de eerste winst voor een AI-project.

### 3. Diversiteit — zit er genoeg variatie in?

Een model leert alleen wat het ziet. Als je trainingsdata alleen foto's van de ochtendploeg bevat, werkt het model slecht in de nachtploeg. Andere lichtval, andere schaduwen, ander resultaat.

Wat hoort er allemaal in te zitten?

- Dag-, avond- en nachtploeg
- Oude én nieuwe machines
- Kleine én grote defecten
- Zeldzame fouten, niet alleen veelvoorkomende

Een kleinere dataset met veel variatie verslaat vaak een grote dataset zonder variatie.

## Drie datasets vergeleken

Drie fictieve datasets voor de krasdetectie-camera. Welke werkt het beste?

| Dataset | Aantal | Labels kloppen? | Variatie | Bruikbaar? |
|---|---|---|---|---|
| **A** | 2.000 foto's | Ja, allemaal | Alleen ochtendploeg | Beperkt — werkt slecht 's nachts |
| **B** | 10.000 foto's | Nee, 15% fout | Dag en nacht | Risicovol — model leert fouten |
| **C** | 800 foto's | Ja, allemaal | Dag/avond/nacht, klein/groot | Best bruikbaar |

Set C is de kleinste. Toch is dat vaak de winnaar. Minder data, betere data.

Dat is het tegenovergestelde van wat veel mensen denken. *"Meer data is beter"* klopt alleen als de kwaliteit en variatie op orde zijn.

## Waarom dit ertoe doet

Als operator zie je als eerste of de data klopt. Je weet welke foto's van welke ploeg komen. Je weet welke producten écht goed waren. En je herkent variatie in wat er die week geproduceerd is.

Die kennis is goud waard bij elk AI-project. Wie de drie vragen kan stellen, kan:

- **Meepraten** als IT of leverancier over data begint
- **Aanwijzen** waar de zwakke plek zit in een dataset
- **Voorkomen** dat een AI-systeem op verkeerde voorbeelden wordt getraind

Dat is iets anders dan accepteren wat de leverancier aanlevert.

## Na deze sessie

Kijk deze week één keer naar één concrete AI-toepassing op je eigen lijn. Een inspectiecamera, een defectherkenningssysteem of een dashboard met voorspellingen. Stel drie vragen aan een collega of teamleider. Welke voorbeelden gebruikt dit systeem om te leren — foto's, metingen, beide? Wie controleert of de antwoorden bij die voorbeelden kloppen? Zitten er voorbeelden in van alle ploegen, van nieuwe én oude producten, en van zeldzame fouten? Schrijf de antwoorden kort op en neem ze mee naar de volgende sessie. Praat er ook even over met iemand van onderhoud of kwaliteit: *"Welke foto's of metingen bewaren wij eigenlijk — en weet iemand of het de goede zijn?"* Vaak ontdek je dat de data wel ergens staat. Maar dat niemand zeker weet of de labels kloppen. Dat is een waardevolle ontdekking voor elk AI-project.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-drie-datasets.md`](./werkbladen/wb-01-drie-datasets.md) — Drie datasets
2. [`wb-02-reflectie-buurman.md`](./werkbladen/wb-02-reflectie-buurman.md) — Reflectie buurman
3. [`wb-03-handout-drie-vragen.md`](./werkbladen/wb-03-handout-drie-vragen.md) — Handout drie vragen
4. [`wb-04-actieplan-eigen-lijn.md`](./werkbladen/wb-04-actieplan-eigen-lijn.md) — Actieplan eigen lijn

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-132`](../../kennisbank/ai_fundamentals/machine_learning_basics/ko-ai-fund-132.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
