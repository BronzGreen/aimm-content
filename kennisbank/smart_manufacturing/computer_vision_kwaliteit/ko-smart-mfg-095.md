---
id: ko-smart-mfg-095
title: Visuele kwaliteitscontrole met AI
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: AI-camera's kunnen producten automatisch controleren op defecten. Ze zijn
  sneller en consistenter dan het menselijk oog, maar hebben menselijke feedback nodig
  om goed te blijven werken.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397,
  409
status: validated
updated_at: '2026-05-19'
correlation_id: ronde6-lo-smart-mfg-095
---

# Visuele kwaliteitscontrole met AI

**Visuele kwaliteitscontrole** is het beoordelen van producten op zichtbare gebreken: krassen, scheuren, kleurafwijkingen, verkeerde afmetingen. Traditioneel doen menselijke inspecteurs dit met hun ogen. Maar dat heeft nadelen:

- **Vermoeidheid**: na uren kijken neemt de aandacht af
- **Inconsistentie**: twee inspecteurs kunnen verschillend oordelen
- **Schaalbaarheid**: je kunt niet onbeperkt inspecteurs inzetten

### Hoe werkt AI-visuele inspectie?

1. **Camera's** maken foto's van elk product op de productielijn
2. Een **AI-model** (meestal een deep learning model) analyseert elke foto
3. Het model classificeert het product als **goed** of **defect**
4. Bij twijfel wordt het product doorgestuurd naar een **menselijke inspecteur**

### Soorten defecten die AI kan detecteren

- Krassen en deuken op oppervlakken
- Foutieve opdrukken (bijv. logo's)
- Ontbrekende onderdelen
- Kleurafwijkingen
- Maatafwijkingen

### Uitdagingen

- Er is geen universele oplossing: elk product heeft een eigen model nodig
- Het model heeft **gelabelde voorbeelden** nodig (foto's waarvan je weet of ze goed of defect zijn)
- Nieuwe types defecten worden niet automatisch herkend


## Praktijkvoorbeeld

Bij Philips in Drachten controleert een AI-systeem drie producten: logo-afdrukken op scheerapparaten (zijn ze compleet en scherp?), decoratieve kapjes (zitten er vloeisporen in het plastic?) en tandenborstelschachten (zitten er deuken of strepen op?). Voor elk product is een apart model getraind met honderden voorbeeldfoto's. De operator hoeft alleen nog de twijfelgevallen te bekijken, waardoor de inspectietijd met 60% is verminderd.
