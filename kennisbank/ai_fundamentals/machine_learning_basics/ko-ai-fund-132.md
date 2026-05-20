---
id: ko-ai-fund-132
title: Trainingsdata - de brandstof van machine learning
type: concept_uitleg
domain: ai_fundamentals
subdomain: machine_learning_basics
summary: Trainingsdata zijn de voorbeelden waarmee een AI-model leert. De kwaliteit
  en hoeveelheid van trainingsdata bepalen hoe goed het model wordt. Goede data zijn
  belangrijker dan een slim algoritme.
source_centrality: 0.7
source_ref: Russell & Norvig (2021). Artificial Intelligence - A Modern Approach,
  4th ed., Chapter 18, pp. 755-756
status: validated
updated_at: '2026-05-19'
correlation_id: ronde11-lo-ai-fund-132
---

# Trainingsdata - de brandstof van machine learning

Een AI-model leert niet uit het niets. Het heeft **trainingsdata** nodig: een verzameling voorbeelden waarvan het juiste antwoord bekend is. Hoe meer en betere voorbeelden, hoe beter het model wordt.

### Wat zijn goede trainingsdata?

Goede trainingsdata hebben vier kenmerken:

1. **Voldoende hoeveelheid** - te weinig voorbeelden leidt tot onbetrouwbare voorspellingen. Hoe meer data, hoe beter.
2. **Representatief** - de voorbeelden moeten lijken op de situaties die het model straks in de praktijk tegenkomt. Als je alleen foto's bij daglicht traint, werkt het model niet goed bij nachtploegen.
3. **Correct gelabeld** - de antwoorden bij de voorbeelden moeten kloppen. Als een goed product per ongeluk als "afgekeurd" wordt gelabeld, leert het model het verkeerde.
4. **Divers** - de voorbeelden moeten alle variaties bevatten die in de praktijk voorkomen.

### Meer data verslaat beter algoritme

Onderzoek laat zien dat meer trainingsdata vaak belangrijker is dan een slimmer algoritme *(bron: Russell & Norvig 2021, Artificial Intelligence - A Modern Approach; Halevy, Norvig & Pereira 2009, "The Unreasonable Effectiveness of Data")*. Een eenvoudig model met 10 miljoen voorbeelden presteert vaak beter dan een complex model met 1 miljoen voorbeelden.


## Praktijkvoorbeeld

*Fictieve illustratie van het data-kwantiteit-principe — concept uit Russell & Norvig 2021.*

Een voedingsmiddelenfabrikant wil met AI verpakkingsfouten detecteren. Ze beginnen met 200 foto's, maar het model maakt veel fouten. Na het verzamelen van 2.000 foto's - inclusief zeldzame fouttypen en verschillende lichtomstandigheden - verbetert de nauwkeurigheid van 75% naar 95%. De les: investeer eerst in goede data, daarna pas in een beter model.
