---
id: ko-smart-mfg-094
title: Human-in-the-loop bij anomaliedetectie
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Bij anomaliedetectie is feedback van de operator essentieel. De mens helpt
  het AI-systeem om vals alarm te verminderen en echte problemen beter te herkennen.
source_centrality: 0.7
source_ref: Scholz et al. (2024). Artificial Intelligence in Manufacturing, pp. 373-374
status: validated
updated_at: '2026-05-19'
correlation_id: ronde5-lo-smart-mfg-094
---

# Human-in-the-loop bij anomaliedetectie

AI-systemen voor anomaliedetectie zijn niet perfect. Ze geven soms **vals alarm** (false positives): het systeem denkt dat er een probleem is, maar er is niets aan de hand. Of ze missen soms echte problemen.

### De rol van de operator

De operator kent de machine en het proces. Die kennis is onmisbaar om het AI-systeem te verbeteren:

1. **Resultaten beoordelen**: de operator beoordeelt of een gedetecteerde anomalie echt een probleem is
2. **Drempels bijstellen**: als er te veel vals alarm is, kan de gevoeligheid worden verlaagd. Als echte problemen worden gemist, moet de gevoeligheid omhoog
3. **Labels geven**: door aan te geven wat echt een anomalie was, krijgt het model gelabelde data om van te leren

### Van ongesuperviseerd naar gesuperviseerd

Veel anomaliedetectiemodellen beginnen zonder labels (ongesuperviseerd). Door de feedback van de operator ontstaan er gelabelde voorbeelden. Met deze labels kan het model worden bijgetraind en worden de detecties steeds nauwkeuriger.

### Het resultaat

Door mens en machine samen te laten werken:
- Minder vals alarm (minder onnodige onderbrekingen)
- Betere detectie van echte problemen
- Een systeem dat steeds slimmer wordt


## Praktijkvoorbeeld

Een anomaliedetectiesysteem bij een blaasgieter geeft regelmatig alarm bij de start van een nieuwe productiedag. De operator herkent dit als het normale opwarmproces en markeert deze meldingen als vals alarm. Het systeem leert hiervan en past de drempelwaarden aan voor de opwarmfase. Na enkele weken geeft het systeem alleen nog alarm bij echte problemen, wat de operator tijd bespaart en het vertrouwen in het systeem vergroot.
