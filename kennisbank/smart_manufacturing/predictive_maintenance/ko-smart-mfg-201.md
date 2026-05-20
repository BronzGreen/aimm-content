---
id: ko-smart-mfg-201
title: 'Sensordata lezen: temperatuur, druk en trillingen interpreteren'
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een stapsgewijze procedure om sensordata van je machine te lezen, een basislijn
  te bepalen, trends te herkennen en pieken van ruis te onderscheiden.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1
status: validated
updated_at: '2026-05-20'
correlation_id: ronde14-lo-smart-mfg-201
---

# Sensordata lezen: temperatuur, druk en trillingen interpreteren

Als operator werk je dagelijks met machines die sensoren hebben. Die sensoren meten continu dingen zoals **temperatuur**, **druk** en **trillingen**. Maar wat zeggen die getallen eigenlijk? En wanneer moet je je zorgen maken?

Met deze drie stappen leer je sensordata lezen en begrijpen.

### Stap 1: Basislijn bepalen — wat is normaal voor DEZE machine?

Elke machine heeft zijn eigen normaalwaarden. Een CNC-freesmachine draait misschien normaal op 65 graden, terwijl een andere machine op 80 graden prima functioneert. Je kunt normaalwaarden niet uit een boekje halen — je moet ze **meten op jouw machine**.

Zo doe je dat:
- Draai de machine een volle shift onder normale omstandigheden.
- Schrijf elke 30 minuten de sensorwaarden op (of lees ze uit het systeem).
- Doe dit minimaal 5 werkdagen.
- Bereken het gemiddelde: dat is jouw **basislijn**.

### Stap 2: Trends herkennen — stijgt het langzaam?

Een enkele hoge meting is vaak niet erg. Maar als de temperatuur **elke week een beetje hoger** wordt, dan is er iets aan de hand. Dat noemen we een **trend**.

Waar let je op:
- Vergelijk de waarden van deze week met vorige week.
- Stijgt de waarde steeds een klein beetje? Dan is er een trend.
- Een trend van 1-2 graden per week kan wijzen op slijtage van een lager of vervuiling van een filter.

### Stap 3: Pieken vs ruis onderscheiden

Soms springt een waarde plotseling omhoog en dan weer terug. Is dat een probleem? Niet altijd.

- **Ruis** is een korte, willekeurige schommeling die vanzelf verdwijnt. Bijvoorbeeld: een trillingspiek wanneer een heftruck langsrijdt.
- **Een echte piek** herhaalt zich, wordt groter, of blijft langer aanhouden. Bijvoorbeeld: trillingen die elke cyclus hoger worden.

De vuistregel: zie je het **drie keer of vaker**, dan is het geen ruis maar een signaal.


## Praktijkvoorbeeld

Op een CNC-freesmachine meet een temperatuursensor de spindeltemperatuur. De basislijn is 65 graden. In week 1 meet de operator gemiddeld 66 graden, in week 2 is het 68 graden, in week 3 is het 72 graden. Dat is een duidelijke trend: 2-3 graden stijging per week. De operator meldt dit bij de technische dienst. Bij inspectie blijkt het smeermiddel van het spindellager bijna op. Na bijvullen daalt de temperatuur weer naar 65 graden. Door de trend vroeg te herkennen is een ongeplande stilstand voorkomen.
