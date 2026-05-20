---
id: ko-smart-mfg-101
title: AI voor visuele kwaliteitsinspectie bij spuitgieten
type: voorbeeld
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Bij spuitgieten kan AI-visuele inspectie producten automatisch classificeren
  als goed of defect. De operator behoudt de mogelijkheid om AI-beslissingen te corrigeren.
source_centrality: 0.7
source_ref: Hoch et al. (2024). Artificial Intelligence in Manufacturing, pp. 424-425
status: validated
updated_at: '2026-05-20'
correlation_id: ronde13-lo-smart-mfg-101
---

# AI voor visuele kwaliteitsinspectie bij spuitgieten

Bij de productie van kunststof onderdelen door **spuitgieten** is kwaliteitscontrole cruciaal. Elke fout kost materiaal, tijd en geld. AI-visuele inspectie kan hier veel verbeteren.

### De situatie

In een spuitgietfabriek worden kunststof onderdelen geproduceerd voor de auto-industrie. Na elke cyclus moeten de onderdelen worden gecontroleerd op:
- Vloeisporen in het plastic
- Interne luchtbellen
- Onvolledige vulling van de mal
- Oppervlaktedefecten

### De AI-oplossing

Een camera-systeem maakt foto's van elk geproduceerd onderdeel. Een AI-model analyseert de foto en classificeert het als **OK** of **niet-OK**. Bij niet-OK geeft het model ook het type defect aan.

### De rol van de operator

- De operator kan AI-beslissingen **overrulen** en corrigeren
- Bij twijfelgevallen kan de operator handmatig defecte gebieden **markeren**
- Deze feedback wordt teruggevoerd naar het AI-model, dat hiervan leert

### Voordelen

- Snellere inspectie
- Consistentere beoordeling
- Minder afhankelijkheid van ervaring individuele inspecteur
- Continue verbetering door feedback-loop


## Praktijkvoorbeeld

*(Bron: Hoch et al. 2024, Artificial Intelligence in Manufacturing, pp. 424-425 — case spuitgiet kunststof ventilatierosters.)*

Bij een toeleverancier voor de auto-industrie produceert een spuitgietmachine kunststof ventilatierosters. Het AI-inspectiesysteem detecteert drie categorieën: goed, cosmetisch defect (kan nog worden verkocht) en functioneel defect (moet worden afgekeurd). De operator ziet op zijn scherm de classificatie plus een heatmap die aangeeft waar het model een probleem ziet. In de eerste maand corrigeert de operator 15% van de AI-beslissingen. Na drie maanden is dit gedaald tot 3%.
