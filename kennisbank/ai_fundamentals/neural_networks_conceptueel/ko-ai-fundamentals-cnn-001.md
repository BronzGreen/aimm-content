---
id: ko-ai-fundamentals-cnn-001
title: 'Convolutional Neural Network (CNN): architectuur en kernelementen'
type: concept_uitleg
domain: ai_fundamentals
subdomain: neural_networks_conceptueel
summary: 'Een CNN is een feedforward neural network dat via lokale connectiviteit
  en gedeelde gewichten lokale features uit hoog-dimensionale data extraheert; standaardarchitectuur:
  input → convolutielagen → pooling → fully connected → output.'
source_centrality: 0.85
source_ref: Li (2026). Hybrid Data-Model AI for Structural Monitoring, §2.1.1 (p.
  18-19)
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-ai-fund-cnn-001
---

# Convolutional Neural Network (CNN): architectuur en kernelementen

## Definitie

Een Convolutional Neural Network (CNN) is een **feedforward neural
network** dat twee technieken combineert:
- **Lokale connectiviteit** — een neuron in de convolutielaag kijkt
  alleen naar een klein deel van de input (de receptive field).
- **Shared weights** — dezelfde filter (kernel) wordt over de hele
  input geschoven; dat reduceert het aantal parameters drastisch.

Door deze combinatie is CNN bijzonder geschikt voor het extraheren
van **lokale features** uit hoog-dimensionale data (afbeeldingen,
tijdreeksen, sensorsignalen).

## Standaardarchitectuur

```
Input → Convolutielaag → Pooling → ... → Fully connected → Output
```

### Convolutielaag
- Past **leerbare filters** (convolution kernels) toe op de input
- Genereert **feature maps**
- Past een non-lineaire activatie toe (meestal ReLU)
- Formule: c_i = f(w_i · x_i + b_i), waar w_i de filterweights, x_i
  de input, b_i de bias zijn

### Pooling-laag
- **Downsampling** — comprimeert de output van de convolutielaag
- Veelvoorkomend: **max pooling** (neem maximum binnen het venster) of
  average pooling
- Doel: dimensiereductie, overfitting verminderen, robuuster tegen
  kleine verschuivingen

### Fully connected laag
- Integreert alle feature-maps tot een eindvoorspelling
- Voor classificatie of regressie

## Voor- en nadelen

**Voordelen:**
- Aantal parameters drastisch lager dan een standaard fully-connected
  netwerk → snellere training, minder overfitting
- Translation invariance — patroon op locatie A wordt herkend op
  locatie B
- Werkt direct op ruwe data — minder feature-engineering vereist

**Nadelen:**
- Convolutielaag is rekenkundig duur tijdens training
- Vooral effectief bij data met **lokale structuur** (beelden,
  tijdreeksen) — minder geschikt voor data zonder ruimtelijke
  ordening


## Praktijkvoorbeeld

Voor een trillingssignaal van een lager (1D-tijdreeks) extraheert
een 1D-CNN met kernels van bijv. 8 samples lokale frequentie-patronen
zonder dat een ingenieur expliciet FFT-features hoeft te kiezen — het
netwerk leert welke spectrum-banden discrimineren tussen normaal en
defect.
