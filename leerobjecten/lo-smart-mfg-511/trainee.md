---
id: lo-smart-mfg-511-trainee
knowledge_object_id: ko-smart-mfg-511
version: trainee
title: 'Trainingsdata labelen: goede en defecte producten markeren'
target_audience: operator
content_level: MBO-3
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: experimenteren
guidance_style: coachen
duration_minutes: 50
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-511
---

# Trainingsdata labelen en model configureren

> **Leervraag:** Hoe label je productfoto's zodat een AI-model ervan kan leren, en hoe stel je het model zo in dat het de juiste balans vindt?

---

## Waarom is dit belangrijk?

In Module 1 heb je gezien wat AI-inspectie kan. Maar wie vertelt de AI wat een goed product is en wat een defect? Dat doe jij. Jouw labels zijn het fundament van het hele systeem. Slechte labels = slecht model. Goede labels = betrouwbare inspectie. Jij hebt de vakkennis om dat verschil te maken.

---

## Deel 1: Foto's labelen (15 min)

Je krijgt 20 productfoto's. Bekijk elke foto systematisch (links-rechts, boven-beneden).

Schrijf per foto op het werkblad:
- **Goed of defect?**
- **Welk type defect?** (kras, deuk, kleurafwijking, vervorming)
- **Hoe zeker ben je?** (1 = helemaal niet zeker, 5 = heel zeker)

Werk zelfstandig. Het gaat om jouw oordeel.

> **Tip:** Kijk zoals je op de werkvloer kijkt. Gebruik dezelfde criteria die je daar ook gebruikt.

---

## Deel 2: Labels vergelijken in duo's (10 min)

Vergelijk je labels met je buurman. Noteer op je werkblad:

- Bij welke foto's waren jullie het **oneens**?
- Waarom koos jij "goed" en je buurman "defect" (of andersom)?
- Wat zijn jullie criteria?

### Waarom dit ertoe doet

Dezelfde foto, twee verschillende labels. Wat betekent dat voor een AI-model? Het model leert van jouw labels. Als jij en je collega het niet eens zijn, raakt het model in de war.

**Consistentie is het belangrijkste.** Niet of je streng of soepel bent, maar dat je altijd hetzelfde oordeelt.

---

## Deel 3: Best practices voor trainingsdata (10 min)

Je krijgt een handout met de vier regels voor goede trainingsdata:

| Regel | Wat het betekent |
|-------|-----------------|
| **Consistente foto's** | Zelfde licht, zelfde achtergrond, zelfde hoek |
| **Duidelijke criteria** | Wanneer is iets een defect? Spreek het af. |
| **Genoeg foto's per categorie** | Minimaal 30% defecten in je set *(vuistregel class balance)* |
| **Verdeling in trainingsset en testset** | 80% om van te leren, 20% om te testen |

> **Waarom een aparte testset?** Stel je voor dat je een toets maakt en je hebt de antwoorden al gezien. Dat is geen eerlijke test. Zo werkt het ook bij een AI-model — je test het met foto's die het nog niet heeft gezien.

---

## Deel 4: Model configureren (15 min)

Nu ga je een model configureren. Je werkt samen met je buurman.

Jullie krijgen de resultaten van een model bij drie drempelwaarden:

| Drempel | Defecten gevonden | Valse alarmen |
|---------|-------------------|---------------|
| **0.3** (soepel) | Veel | Veel |
| **0.5** (midden) | Gemiddeld | Gemiddeld |
| **0.7** (streng) | Weinig | Weinig |

Kies de beste drempel voor jullie product. Schrijf op waarom.

**Denk na:** Wat is erger voor jullie product — een vals alarm (goed product afgekeurd) of een gemist defect (defect product doorgelaten)?

Bereid een pitch van 1 minuut voor om jullie keuze te presenteren aan de groep.

---

## Samenvatting

| Wat je geleerd hebt | Waarom het belangrijk is |
|--------------------|------------------------|
| Foto's consistent labelen | Jouw labels bepalen hoe goed het model wordt |
| Trainingsset vs. testset | Een eerlijke test is nodig om te weten of het model werkt |
| Drempelwaarde kiezen | De balans tussen te streng en te soepel hangt af van je product |

---

## Transferopdracht

Doe dit voor de volgende bijeenkomst:

1. Neem de 10 foto's mee die je in Module 1 op je werkvloer hebt gemaakt
2. Label ze: goed of defect, met type defect
3. Maak 10 extra foto's zodat je minimaal 20 hebt
4. Let op: consistent licht, achtergrond en hoek
5. Neem je gelabelde set mee naar de volgende bijeenkomst

> **Doe ook:** Bespreek met je collega's: welke criteria gebruiken jullie om te bepalen of een product goed of defect is? Zijn jullie het eens?

---

## Werkbladen (Kolb-cyclus)

1. [`wb-handout-trainingsdata.md`](./werkbladen/wb-handout-trainingsdata.md) — Trainingsdata
2. [`wb-labelen.md`](./werkbladen/wb-labelen.md) — wb-labelen
3. [`wb-model-configuratie.md`](./werkbladen/wb-model-configuratie.md) — Configuratie
4. [`wb-reflectie-labelen.md`](./werkbladen/wb-reflectie-labelen.md) — Labelen

## Verder

- Onderliggend kennisobject: [`ko-smart-mfg-511`](../../kennisbank/smart_manufacturing/computer_vision_kwaliteit/ko-smart-mfg-511.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
- Interactief: [`interactive/model.html`](./interactive/model.html)
