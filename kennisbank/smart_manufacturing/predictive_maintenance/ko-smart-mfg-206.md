---
id: ko-smart-mfg-206
title: 'Jouw sensordata interpreteren met SHAP: welke sensor telt het meest?'
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Na een anomaliemelding gebruik je de SHAP-grafiek om te bepalen welke sensor
  het meest bijdraagt. Zo weet je waar je moet beginnen met zoeken.
source_centrality: 0.7
source_ref: Gebaseerd op Sesana et al. (2024). Artificial Intelligence in Manufacturing,
  pp. 474-475 + operationele best practices
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-smart-mfg-206
---

# Jouw sensordata interpreteren met SHAP: welke sensor telt het meest?

In ko-smart-mfg-108 heb je geleerd wat SHAP is en wat het laat zien. Nu leer je het **gebruiken**. Dit is procedurele kennis: je volgt stappen om van een SHAP-grafiek naar een concrete actie te komen.

### Stappenplan: van SHAP-grafiek naar actie

**Stap 1: Open de SHAP-grafiek na een anomaliemelding**

Je krijgt een melding dat de anomaliescore boven de drempel zit. Open het detailscherm. De SHAP-grafiek toont alle sensoren, gesorteerd op bijdrage.

**Stap 2: Lees de top-3 sensoren**

Kijk naar de drie sensoren met de hoogste bijdrage. Lees af:
- **Welke sensor** is het? (bijv. "koelmiddeltemperatuur")
- **Hoeveel procent** draagt die bij? (bijv. "60%")
- **In welke richting** wijkt de waarde af? (te hoog of te laag?)

**Stap 3: Groepeer de sensoren**

Horen de top-sensoren bij hetzelfde systeem?
- Drie temperatuursensoren bij de koeling → **koelprobleem**
- Trillingssensor + druksensor bij de hydrauliek → **hydrauliekprobleem**
- Sensoren uit verschillende systemen → **check elke sensor apart**

**Stap 4: Bepaal je actie**

- "De SHAP-grafiek zegt dat temperatuur 60% bijdraagt aan de anomaliescore. Dus ik check eerst de koeling."
- "Trillingen dragen 45% bij, druk 30%. Beide zitten op de hydrauliek. Dus ik check de hydrauliek."
- "Eén sensor draagt 80% bij. Dat kan een sensorstoring zijn. Ik check eerst of de sensor zelf goed werkt."

**Stap 5: Documenteer je bevinding**

Noteer in de werkorder:
- Welke sensoren de SHAP-grafiek aanwees
- Wat je gecheckt hebt
- Wat je gevonden hebt (of niet)

Dit helpt de volgende keer: het model leert niet van jouw actie, maar jij leert van het patroon.

### Vuistregels

| Situatie | Interpretatie | Actie |
|----------|--------------|-------|
| Eén sensor > 70% bijdrage | Lokaal probleem of sensorstoring | Check die ene sensor/component |
| Twee-drie sensoren uit één systeem | Systeemprobleem | Check het systeem als geheel |
| Veel sensoren, elk klein percentage | Algemene slijtage of drift | Vergelijk met historische data |
| Sensor bijdrage negatief | Die sensor werkt juist beter dan verwacht | Niet relevant voor de storing |


## Praktijkvoorbeeld

Operator Dennis krijgt een anomaliemelding voor de freesmachine: score 68 (oranje). Hij opent de SHAP-grafiek en leest:

1. Koelmiddeltemperatuur: 58% bijdrage (te hoog)
2. Spiltemperatuur: 22% bijdrage (te hoog)
3. Koelmiddeldruk: 12% bijdrage (te laag)

Dennis groepeert: alle drie hangen samen met het koelsysteem. Zijn conclusie: "Het koelsysteem werkt niet goed genoeg. De koelmiddeldruk is te laag, waardoor de temperaturen oplopen."

Hij checkt het koelsysteem en vindt een filter dat voor 70% verstopt zit. Na het vervangen van het filter dalen alle drie de sensorwaarden naar normaal. De anomaliescore zakt naar 15.

Dennis noteert in de werkorder: "SHAP wees koelsysteem aan. Filter verstopt. Vervangen. Advies: filter elke 3 maanden checken."
