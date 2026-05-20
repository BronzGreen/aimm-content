---
id: ko-ai-fund-135
title: Overfitting - wanneer een AI-model te goed leert
type: concept_uitleg
domain: ai_fundamentals
subdomain: machine_learning_basics
summary: Overfitting betekent dat een AI-model de trainingsdata te precies heeft geleerd,
  inclusief de ruis en toevalligheden. Het model presteert dan uitstekend op de trainingsdata,
  maar slecht op nieuwe data.
source_centrality: 0.7
source_ref: Russell & Norvig (2021). Artificial Intelligence - A Modern Approach,
  4th ed., Chapter 18, pp. 695-697, 721, 736
status: validated
updated_at: '2026-05-20'
correlation_id: ronde13-lo-ai-fund-135
---

# Overfitting - wanneer een AI-model te goed leert

Een AI-model kan **te goed** leren. Dat klinkt raar, maar het is een veelvoorkomend probleem. Het heet **overfitting** (overaanpassing).

### Wat is overfitting?

Stel je voor dat je een nieuwe operator inwerkt. Je laat 10 voorbeelden zien van goede en slechte producten. Als die operator alleen die 10 specifieke producten herkent, maar niet kan generaliseren naar nieuwe producten, dan is er sprake van overfitting. De operator heeft de voorbeelden uit het hoofd geleerd, maar niet het achterliggende patroon begrepen.

Hetzelfde gebeurt bij AI-modellen. Het model past zich zo precies aan op de trainingsdata dat het ook de **ruis** leert - toevallige afwijkingen die niets te maken hebben met het echte patroon.

### Hoe herken je overfitting?

- Het model scoort bijna **perfect** op de trainingsdata
- Maar op **nieuwe data** (testdata) scoort het veel slechter
- Het verschil tussen trainingsscore en testscore is groot

### Hoe voorkom je overfitting?

1. **Meer trainingsdata** - meer voorbeelden helpen het model om echte patronen te onderscheiden van ruis
2. **Eenvoudiger model** - een simpeler model kan minder ruis vastleggen
3. **Regularisatie** - een techniek die het model bestraft voor te complexe oplossingen
4. **Cross-validatie** - test het model op data die het nog niet heeft gezien


## Praktijkvoorbeeld

*Fictieve illustratie van overfitting — concept uit Russell & Norvig 2021, Artificial Intelligence - A Modern Approach.*

Een machinebouwer traint een AI-model om trillingen te classificeren als normaal of abnormaal. Met slechts 50 voorbeelden scoort het model 99% op de trainingsdata. Maar bij inzet op een andere machine van hetzelfde type herkent het slechts 60% van de abnormale trillingen correct. Het model had de specifieke kenmerken van die ene machine geleerd, niet het generieke patroon van abnormale trillingen. Na het toevoegen van data van 5 machines verbetert de score op nieuwe machines naar 90%.
