---
id: ko-ai-fund-022
title: Wat is een neuraal netwerk?
type: concept_uitleg
domain: ai_fundamentals
subdomain: neural_networks_conceptueel
summary: Een neuraal netwerk is een AI-model dat patronen leert herkennen in data,
  vergelijkbaar met hoe je hersenen patronen herkennen. Het wordt gebruikt voor beeldherkenning,
  activiteitenherkenning en voorspellingen.
source_centrality: 0.7
source_ref: Soldatos, J. (ed.) (2024). Artificial Intelligence in Manufacturing, Ch.
  17-18, pp. 306-310, 321-323
status: validated
updated_at: '2026-05-19'
correlation_id: ronde10-lo-ai-fund-022
---

## Wat is een neuraal netwerk?

Een neuraal netwerk is een computerprogramma dat leert door voorbeelden.
Net zoals jij leert om een goed lasje te herkennen door honderden lassen
te bekijken, leert een neuraal netwerk door duizenden voorbeelden te zien.

### Hoe werkt het (simpel)?

1. **Input** — het netwerk krijgt data binnen (een foto, sensordata,
   een meting)
2. **Lagen** — de data gaat door meerdere lagen die elk een stukje
   van het patroon herkennen. De eerste laag ziet lijnen, de tweede
   vormen, de derde objecten
3. **Output** — het netwerk geeft een antwoord: "dit is een defect"
   of "deze activiteit is lopen"

### Soorten neurale netwerken in de fabriek

- **CNN (Convolutional Neural Network)** — gespecialiseerd in beelden.
  Wordt gebruikt voor kwaliteitscontrole met camera's en het herkennen
  van objecten
- **RNN (Recurrent Neural Network)** — gespecialiseerd in reeksen
  data over tijd. Wordt gebruikt voor sensordata en voorspellingen

### Waarom heet het "neuraal"?

Het is geïnspireerd op hoe je hersenen werken: miljoenen zenuwcellen
(neuronen) die met elkaar verbonden zijn. Elk neuron ontvangt signalen,
verwerkt ze, en stuurt het resultaat door. In een computerneuraal netwerk
werkt het vergelijkbaar — maar dan met rekenkracht in plaats van
hersencellen.

### Wat moet je weten als operator?

- Je hoeft niet te begrijpen hoe een neuraal netwerk precies rekent
- Wel is het goed om te weten: **het model is zo goed als de data
  waarmee het getraind is**
- Jij levert de trainingsdata — door aan te geven wat "goed" en
  "fout" is
- Zonder jouw kennis kan het model niet leren
