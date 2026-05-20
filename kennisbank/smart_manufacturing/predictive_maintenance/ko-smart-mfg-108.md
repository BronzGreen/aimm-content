---
id: ko-smart-mfg-108
title: 'SHAP: welke sensor draagt bij aan de anomalie?'
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: SHAP-visualisaties tonen de bijdrage van elke sensor aan een gedetecteerde
  anomalie. Dit helpt de operator om de oorzaak van het probleem snel te vinden.
source_centrality: 0.7
source_ref: Sesana et al. (2024). Artificial Intelligence in Manufacturing, pp. 474-475
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-smart-mfg-108
---

# SHAP: welke sensor draagt bij aan de anomalie?

Als een AI-model een anomalie detecteert, is de volgende vraag: **welke sensor heeft hier het meest aan bijgedragen?** De SHAP-techniek (SHapley Additive exPlanations) beantwoordt deze vraag.

### Wat laat SHAP zien?

SHAP berekent per sensor de bijdrage aan de anomaliescore. Je krijgt een overzicht:
- **Hoge bijdrage**: deze sensor wijkt sterk af van normaal
- **Lage bijdrage**: deze sensor gedraagt zich normaal
- **Kleur en grootte**: rode, grote punten = sterke afwijking in de richting van anomalie

### Drie niveaus van uitleg

1. **Individueel**: waarom is dit specifieke meetpunt een anomalie?
2. **Groep**: welke combinatie van sensoren wijst op een probleem?
3. **Globaal**: welke sensoren zijn over alle anomalieën heen het belangrijkst?

### Voor de operator

De SHAP-visualisatie vertaalt een abstracte anomaliescore naar een **concreet aanknopingspunt**: "Sensor 23 (koelmiddeltemperatuur) draagt het meest bij aan de anomalie. Controleer het koelsysteem."

### Voor de teamleider

Het globale overzicht toont welke sensoren structureel het meest bijdragen aan anomalieën. Dit helpt bij het plannen van preventief onderhoud en het prioriteren van verbeterprojecten.


## Praktijkvoorbeeld

Na een anomaliemelding op de Heller 400 CNC-machine opent de operator de XAI-webapplicatie. De SHAP-grafiek toont de bijdrage van alle 76 sensoren, gesorteerd op impact. De top-3 sensoren zijn allemaal gerelateerd aan het hydraulische systeem. De operator weet nu dat hij het hydraulische systeem moet controleren, in plaats van de hele machine te doorzoeken. De gemiddelde diagnosetijd daalt van 45 minuten naar 12 minuten.
