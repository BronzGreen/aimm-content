---
id: lo-data-lit-201-trainee
knowledge_object_id: ko-data-lit-201
version: trainee
title: 'Datatypes herkennen: getallen, categorieen, tijd, tekst'
target_audience: operator
content_level: MBO-3
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: experimenteren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-19'
correlation_id: ronde9-lo-data-lit-201
---

# Hoe herken je het type data dat je hebt, en hoe check je of die data betrouwbaar is?

Als je niet weet welk type data je hebt, kun je er niet goed mee werken. En als je niet checkt of de data klopt, neem je misschien beslissingen op foute informatie. Na deze sessie kun je dat zelf beoordelen.

## Wat leer je?

Je leert vier datatypes herkennen (getallen, categorieën, tijddata, tekst) en drie kwaliteitschecks uitvoeren (volledigheid, consistentie, actualiteit).

## De vier datatypes

Op de werkvloer kom je vier soorten data tegen:

### 1. Getallen
Alles wat je kunt meten of tellen: temperatuur (182,5 graden), gewicht (3,42 kg), OEE (72%). Met getallen kun je **rekenen**: gemiddelde, maximum, trend.

### 2. Categorieën
Labels of groepen: machinetype (CNC-frees, draaibank), foutcode (E-01, E-02), ploeg (ochtend, nacht). Je kunt er niet mee rekenen, maar wel mee **sorteren en tellen**.

### 3. Tijddata
Wanneer iets gebeurde: starttijd (06:30), storingsduur (14 min), datum (2026-04-08). Met tijddata zie je **trends**: wordt het beter of slechter?

### 4. Tekst
Opmerkingen en notities: "Trillingen bij hoog toerental". Lastig om automatisch te verwerken, maar bevat vaak het **waarom**.

## Hoe bepaal je het datatype?

Drie vragen:
1. **Kun je ermee rekenen?** Ja --> getal
2. **Is het een keuze uit een vaste lijst?** Ja --> categorie
3. **Gaat het over wanneer?** Ja --> tijd. Nee --> tekst

## De drie kwaliteitschecks

### Check 1: Volledigheid
Ontbreekt er iets? Lege cellen, ontbrekende diensten, machines die niet meegeteld zijn.

### Check 2: Consistentie
Klopt het met zichzelf? Dezelfde eenheid (kg vs gram)? Dezelfde schrijfwijze ("CNC-01" vs "cnc01")? Logische waarden?

### Check 3: Actualiteit
Is het nog geldig? Wanneer is de data verzameld? Is er sindsdien iets veranderd?

## Na deze sessie

Neem deze week een dataset van je eigen afdeling. Bepaal per kolom het datatype. Voer de drie kwaliteitschecks uit. Noteer je bevindingen en neem ze mee naar de volgende bijeenkomst.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-handout-kwaliteitschecks.md`](./werkbladen/wb-handout-kwaliteitschecks.md) — Kwaliteitschecks
2. [`wb-kwaliteitscheck-oefening.md`](./werkbladen/wb-kwaliteitscheck-oefening.md) — Oefening
3. [`wb-sorteerkaarten-datatypes.md`](./werkbladen/wb-sorteerkaarten-datatypes.md) — Datatypes
4. [`wb-transfer-datatypes-kwaliteit.md`](./werkbladen/wb-transfer-datatypes-kwaliteit.md) — Datatypes kwaliteit

## Verder

- Onderliggend kennisobject: [`ko-data-lit-201`](../../kennisbank/data_literacy/data_begrippen/ko-data-lit-201.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
