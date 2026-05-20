---
id: ko-smart-mfg-093
title: 'Autoencoder: AI leert wat normaal is'
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een autoencoder is een type AI-model dat zichzelf leert om data samen te
  vatten en weer uit te breiden. Afwijkingen worden herkend doordat het model ze niet
  goed kan reproduceren.
source_centrality: 0.7
source_ref: Scholz et al. (2024). Artificial Intelligence in Manufacturing, pp. 370-374
status: validated
updated_at: '2026-05-20'
correlation_id: ronde12-lo-smart-mfg-093
---

# Autoencoder: AI leert wat normaal is

Een **autoencoder** is een speciaal type neuraal netwerk dat gebruikt wordt voor anomaliedetectie. Het werkt als volgt:

### Het principe

Stel je voor dat je iemand vraagt om een foto te beschrijven in drie woorden, en daarna de foto opnieuw te tekenen op basis van die drie woorden. Als de foto een standaard productierun is, lukt dat redelijk goed. Maar als de foto een ongebruikelijke situatie toont, wordt de tekening veel slechter.

Dat is precies wat een autoencoder doet:
1. **Encoder**: comprimeert de data tot een klein formaat (de drie woorden)
2. **Decoder**: probeert de originele data te herstellen vanuit het compacte formaat

### Hoe detecteert het afwijkingen?

Het model wordt getraind op normale productiedata. Na training kan het normale patronen goed comprimeren en herstellen. Maar als er een afwijking is:
- De data past niet in het geleerde patroon
- De herstelde versie wijkt sterk af van het origineel
- Het verschil (de **reconstructiefout**) is groot
- Het systeem slaat alarm

### Drempelwaarde

Om te bepalen wanneer een alarm afgaat, wordt een drempel ingesteld. Bijvoorbeeld: als de reconstructiefout meer dan drie keer de standaardafwijking is, is het een anomalie. Deze drempel kan worden aangepast op basis van ervaring.


## Praktijkvoorbeeld

Bij de productie van brandstoftanks via blaasgieten analyseert een autoencoder de sensordata van elke productiecyclus. Het model heeft geleerd hoe een normale cyclus eruitziet qua temperatuur, druk en energie. Wanneer een cyclus afwijkt - bijvoorbeeld door een verstopte luchttoevoer - kan het model de data niet goed reproduceren. De hoge reconstructiefout triggert een alarm, waarna de operator de machine kan controleren voordat er defecte tanks worden geproduceerd.
