---
id: ko-ai-fund-133
title: Classificatie - AI die dingen in categorieën indeelt
type: concept_uitleg
domain: ai_fundamentals
subdomain: supervised_vs_unsupervised
summary: Classificatie is een machine learning taak waarbij een AI-model leert om
  dingen in categorieën in te delen, zoals goed/afgekeurd, storingstype A/B/C, of
  productklasse. Het model leert dit van gelabelde voorbeelden.
source_centrality: 0.7
source_ref: Russell & Norvig (2021). Artificial Intelligence - A Modern Approach,
  4th ed., Chapter 18, pp. 723-727
status: validated
updated_at: '2026-05-20'
correlation_id: ronde12-lo-ai-fund-133
---

# Classificatie - AI die dingen in categorieën indeelt

Bij **classificatie** leert een AI-model om dingen in categorieën te sorteren. Het model krijgt voorbeelden met een label (de categorie) en leert welke kenmerken bij welke categorie horen.

### Hoe werkt classificatie?

Stel dat je een AI wilt trainen om storingen te herkennen. Je verzamelt data van je machines: temperatuur, trillingen, geluidsniveau, stroomverbruik. Bij elke meting noteer je of er een storing was, en welk type. Het model leert verbanden tussen de meetwaarden en het storingstype.

Na het trainen kan het model nieuwe meetwaarden beoordelen: "Deze combinatie van hoge temperatuur en onregelmatige trillingen lijkt op storingstype B."

### Twee of meer categorieën

- **Binaire classificatie**: twee categorieën - ja/nee, goed/fout, aan/uit
- **Multiclass classificatie**: meerdere categorieën - storingstype A, B, C of D

### Beslissingsgrens

Het model trekt als het ware een lijn (of vlak) tussen de categorieën. Dit heet de **beslissingsgrens**. Alles aan de ene kant is categorie A, aan de andere kant categorie B. Hoe beter het model, hoe nauwkeuriger deze grens.


## Praktijkvoorbeeld

Bij een metaalbewerkingsbedrijf worden CNC-gefreesde onderdelen automatisch gecontroleerd. Een camera maakt foto's en een classificatiemodel deelt elk onderdeel in: "goed", "braam gedetecteerd", "maatafwijking" of "oppervlaktefout". Operators hoeven alleen nog de afgekeurde onderdelen handmatig te controleren.
