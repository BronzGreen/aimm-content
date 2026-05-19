---
id: ko-smart-mfg-010
title: AI-gestuurde kwaliteitscontrole bespaart productietijd
type: voorbeeld
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Door AI-gebaseerde visuele inspectie in de productielijn te integreren, worden
  defecte producten automatisch gedetecteerd en uit de lijn gehaald. Dit voorkomt
  onnodige bewerkingen op afgekeurde producten.
source_centrality: 0.7
source_ref: Cruz et al. (2024). Artificial Intelligence in Manufacturing, pp. 139-140
status: validated
updated_at: '2026-05-19'
correlation_id: ronde3-lo-smart-mfg-010
---

# AI-gestuurde kwaliteitscontrole bespaart productietijd

Een van de directe voordelen van AI-gestuurde kwaliteitscontrole is dat defecte producten **vroeg** in het proces worden gedetecteerd. Hoe eerder je een defect vindt, hoe minder tijd en materiaal je verspilt.

### Het probleem

In een traditionele productielijn wordt kwaliteitscontrole vaak aan het einde uitgevoerd. Op dat moment heeft een defect product al alle bewerkingsstappen doorlopen. De tijd en energie die aan dat product besteed zijn, zijn verloren.

### De oplossing

Door AI-gebaseerde visuele inspectie **tussentijds** in de lijn te plaatsen, kun je defecte producten direct na de kritische bewerking identificeren. Het product wordt dan:
- Teruggestuurd voor herbewerking (als het defect herstelbaar is)
- Uit de lijn gehaald (als het product beschadigd is)

### Resultaten uit de praktijk

*(Bron: Cruz et al. 2024, Artificial Intelligence in Manufacturing, pp. 139-140 — gecombineerd pilotresultaat isolatiepanelen.)*

Op een pilotlijn voor isolatiepanelen werd dit systeem getest met drie uitkomsten:
1. **Goed**: paneel gaat door naar de volgende bewerking
2. **Herstelbaar**: paneel gaat terug voor herbewerking van de frees
3. **Beschadigd**: paneel wordt direct verwijderd

Het AI-segmentatiemodel behaalde een nauwkeurigheid van 99,5%. In combinatie met een AutoML-systeem voor procesoptimalisatie werd de doorvoer met 55% verbeterd.

### Waarom werkt dit zo goed?

De combinatie van drie AI-technieken maakt het verschil:
1. **Visuele inspectie** (deep learning): detecteert defecten in real-time
2. **AutoML**: optimaliseert de machine-instellingen voor maximale doorvoer
3. **Fuzzy logic reconﬁgurator**: corrigeert automatisch bij afwijkingen

### Lessen voor de praktijk

- Begin met de meest kritische bewerking in je productielijn
- Verzamel voldoende beelddata (gebruik data augmentatie als je weinig defecten hebt)
- Laat operators het systeem valideren in de eerste weken
- Meet het effect: hoeveel tijd en materiaal bespaar je?


## Praktijkvoorbeeld

*(Bron: Cruz et al. 2024, Artificial Intelligence in Manufacturing, pp. 139-140.)*

Een panelenfabrikant plaatst een camera-inspectiesysteem na de freesbewerking. Voorheen werden beschadigde panelen pas aan het einde ontdekt, na ook de graveerbewerking te hebben doorlopen (90 seconden extra productietijd per paneel). Met het AI-systeem worden beschadigde panelen direct na het frezen verwijderd. Bij een uitvalpercentage van 3% bespaart dit dagelijks 45 minuten productietijd en het bijbehorende energieverbruik.
