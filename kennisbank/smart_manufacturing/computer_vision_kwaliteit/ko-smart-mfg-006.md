---
id: ko-smart-mfg-006
title: Visuele inspectie met deep learning
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Deep learning kan camera-beelden van producten automatisch analyseren om
  defecten te herkennen. Een segmentatiemodel markeert precies waar het probleem zit,
  wat de beslissing transparant maakt.
source_centrality: 0.7
source_ref: Cruz et al. (2024). Artificial Intelligence in Manufacturing, pp. 129-131
status: validated
updated_at: '2026-05-18'
correlation_id: ronde2-lo-smart-mfg-006
---

# Visuele inspectie met deep learning

Kwaliteitscontrole is een van de meest voorkomende AI-toepassingen in de maakindustrie. In plaats van elk product handmatig te inspecteren, kan een camera met een AI-model dit automatisch doen.

### Hoe werkt visuele inspectie met AI?

**Stap 1: Camera-opname**
Een camera maakt een foto of video van het product op de productielijn.

**Stap 2: AI-analyse**
Een deep learning model analyseert het beeld. Er zijn twee hoofdbenaderingen:
- **Classificatie**: het model zegt "goed" of "afgekeurd" (maar legt niet uit waarom)
- **Segmentatie**: het model markeert precies welke pixels van het beeld een defect tonen

Segmentatie heeft de voorkeur in de industrie omdat je kunt **zien** waarom het model een beslissing neemt. Dit maakt het resultaat controleerbaar en vertrouwenwekkend.

**Stap 3: Beslissing**
Op basis van de segmentatie wordt een beslissing genomen:
- Product goedgekeurd? Door naar de volgende stap
- Defect dat hersteld kan worden? Terug naar bewerking
- Product beschadigd? Uit de lijn halen

### Data augmentatie: meer leren van minder data

Een veelvoorkomende uitdaging: je hebt maar weinig voorbeelden van defecte producten (gelukkig!). **Data augmentatie** lost dit op door bestaande trainingsbeelden te variëren:
- Horizontaal spiegelen
- Willekeurig stukken weglaten
- Helderheid en contrast variëren

In de praktijk kan data augmentatie de nauwkeurigheid spectaculair verbeteren: van 89% naar 99,5% in sommige gevallen *(bron: Cruz et al. 2024, Artificial Intelligence in Manufacturing, pp. 129-131 — case isolatiepanelen)*.

### Architectuur: U-net

Het meest gebruikte model voor industriele beeldsegmentatie is de **U-net architectuur**. Dit model is speciaal ontworpen om nauwkeurige segmentaties te maken, ook met relatief weinig trainingsdata. Het combineert een "inzoompad" (details herkennen) met een "uitzoompad" (context begrijpen).


## Praktijkvoorbeeld

*(Bron: Cruz et al. 2024, Artificial Intelligence in Manufacturing, pp. 129-131 — casus isolatiepanelenfabriek.)*

Op een productielijn voor isolatiepanelen fotografeert een camera elk paneel na de freesbewerking. Het AI-model (U-net segmentatie) markeert de zijkanten van het paneel. Als het model twee rechthoeken detecteert, is de freesbewerking correct. Bij slechts een rechthoek is er een defect: het paneel gaat terug voor herbewerking of wordt afgekeurd. Met data augmentatie behaalt het model een nauwkeurigheid van 99,5% en een F1-score van 0,992.
