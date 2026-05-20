---
id: lo-ai-fund-135-trainee
knowledge_object_id: ko-ai-fund-135
version: trainee
title: Overfitting — wanneer een AI-model te-goed-leert
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 42
status: validated
updated_at: '2026-05-20'
correlation_id: ronde13-lo-ai-fund-135
---

# Waarom is een AI-model met 99% nauwkeurigheid soms niet te vertrouwen op de werkvloer?

Een leverancier komt aanzetten met 99%. Dat klinkt geweldig. Maar als dat getal alleen geldt op de eigen historie, valt het model om zodra er een nieuwe batch of een nieuwe machine bij komt. Wie dit patroon kent, stelt de juiste vraag aan de leverancier. En voorkomt een dure teleurstelling.


## Wat leer je?

Je kunt overfitting (te-goed-leren) herkennen. Je weet aan welk verschil tussen twee getallen je het ziet. Je kunt drie oorzaken en drie tegenmaatregelen benoemen.


## Twee modellen naast elkaar

Stel je hebt twee AI-modellen voor trillingsherkenning. Allebei moeten ze normaal van abnormaal onderscheiden. Op papier zien ze er zo uit:

| Model | Trainings-score (leren) | Score op nieuwe machine |
|---|---|---|
| Model A | 99% | 60% |
| Model B | 88% | 86% |

Welk model zou jij vertrouwen op de productievloer?

Veel mensen kiezen eerst voor Model A. Het is het hoogste getal. Maar Model A zakt op een nieuwe machine in tot 60%. Model B blijft stabiel. Het verschil tussen leren en onbekende data is bij Model A enorm. Bij Model B is het klein.

Dat verschil is het signaal. Niet de hoogte van het getal.


## Wat is overfitting?

Overfitting (te-goed-leren) betekent dat een AI-model de trainingsdata uit het hoofd heeft geleerd. Het model herkent de voorbeelden waarop het is getraind. Het herkent niet het onderliggende patroon. Op nieuwe data valt het stil.

Vergelijk het met een nieuwe collega. Die heeft tien producten gezien op één machine. Hij herkent die tien feilloos. Maar zet hem op een ander machinetype, dan staat hij stil. Hij heeft de voorbeelden onthouden. Hij heeft het patroon niet door.


### Drie signalen

Je herkent overfitting (te-goed-leren) aan drie dingen:

1. **Groot verschil tussen leren en onbekende data** — bijvoorbeeld 99% op de training, 60% op een nieuwe situatie
2. **Klein dataset met een complex model** — weinig voorbeelden, veel rekenkracht. Het model heeft te veel ruimte om voorbeelden uit het hoofd te leren
3. **Het model faalt op een nieuwe machine of een nieuwe batch** — wat in het lab werkte, werkt niet op de werkvloer


### Drie tegenmaatregelen

Tegen overfitting (te-goed-leren) helpen drie dingen:

1. **Meer voorbeelden** — meer data uit verschillende situaties dwingt het model om het echte patroon te leren
2. **Een simpeler model** — minder ingewikkelde modellen kunnen minder ruis vasthouden
3. **Cross-validatie** — test het model steeds op data die het nog niet zag. Zo zie je het verschil tussen leren en onbekende data

In het voorbeeld uit het boek van Russell en Norvig (2021) was een trillings-model getraind op 50 voorbeelden van één machine. Score op de training: 99%. Score op een nieuwe machine: 60%. Na het toevoegen van data van vijf machines steeg de score op nieuwe machines naar 90%. Meer voorbeelden, minder overfitting (te-goed-leren).


## Wat dit voor jou betekent

Als operator zie je het AI-systeem in productie. Jij bent degene die merkt of het werkt. Wie dit patroon kent, kan:

- De juiste vraag stellen aan een leverancier
- De score op leren en de score op onbekende data uit elkaar houden
- Eerlijk inschatten of een proefopstelling ook op de eigen lijn werkt


## Zelf zien gebeuren?

Twee extra hulpmiddelen die bij dit leerobject horen — beide maken overfitting tastbaar:

- **Video (~90 seconden):** zie hoe trainingsfout (groen) blijft dalen terwijl productiefout (rood) na het knikpunt weer omhoog gaat — letterlijk de divergentie van Model A in beeld. Bestand: `video/composition.tsx` (Remotion-project).
- **Interactief "Overfitting-sliders":** schuif aan modelcomplexiteit (1-10) en aantal trainingsvoorbeelden (10-1000), en zie live hoe de sweet spot verschuift. Bestand: `model-overfitting-sliders.jsx`.

Vraag je trainer welke variant in jouw sessie gebruikt wordt.

## Na deze sessie

Zoek deze week één concreet AI-systeem in jouw fabriek. Een inspectiecamera, een trillings-monitor, een kwaliteits-classificatie of een voorspelmodel. Vraag aan de leverancier of aan IT drie dingen. Op welke data is het model getraind — hoeveel voorbeelden, van welke machine? Op welke onbekende data is het getest, en wat was daar de score? Hoe groot is het verschil tussen training (leren) en test (onbekende data)? Schrijf de drie antwoorden op en neem ze mee naar de volgende sessie. Praat ook even met een collega-operator: *"Heb jij ooit gezien dat een meting of inspectie het op de ene machine wel deed en op een nieuwe niet?"* Vaak is het probleem herkenbaar — alleen had niemand er een naam voor.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-scorekaarten.md`](./werkbladen/wb-01-scorekaarten.md) — Scorekaarten
2. [`wb-02-reflectie.md`](./werkbladen/wb-02-reflectie.md) — Reflectie
3. [`wb-03-handout-overfitting.md`](./werkbladen/wb-03-handout-overfitting.md) — Handout overfitting
4. [`wb-04-diagnose.md`](./werkbladen/wb-04-diagnose.md) — Diagnose

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-135`](../../kennisbank/ai_fundamentals/machine_learning_basics/ko-ai-fund-135.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
