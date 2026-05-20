---
id: ko-ai-fundamentals-ensemble-001
title: 'Ensemble learning voor PdM: aggregatie van zwakke leerders'
type: definitie
domain: ai_fundamentals
subdomain: machine_learning_basics
summary: Ensemble Learning Algorithms (ELAs) combineren meerdere ML-modellen tot één
  voorspeller — voor PdM hebben ze structureel betere voorspelnauwkeurigheid laten
  zien dan losse algoritmen.
source_centrality: 0.85
source_ref: Hung (2021). Improved ELA for PdM, §3.2 (p. 6)
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-ai-fund-ensemble-001
---

# Ensemble learning voor PdM: aggregatie van zwakke leerders

## Definitie

Een Ensemble Learning Algorithm (ELA) is een **integratiemodule die
meerdere ML-algoritmen aggregeert** en de hoogst-presterende
combinatie selecteert om de voorspelkwaliteit te verbeteren.

## Twee hoofdfamilies

- **Bagging (parallel ensemble)** — train onafhankelijke modellen
  op gevarieerde subsets en middel hun voorspellingen. Verlaagt
  **variance**. Voorbeeld: random forest, decision jungle.
- **Boosting (sequentieel ensemble)** — train modellen na elkaar,
  waarbij elk volgende model probeert fouten van zijn voorganger te
  corrigeren. Verlaagt **bias**. Voorbeeld: boosted decision trees.

## Bewezen toepassingen in PdM

- **Aircraft engines / lagers** — Li gebruikte ensemble-prognose voor
  remaining useful lifespan met de laagste voorspelfout.
- **Tool wear in dry milling** — Wu et al. aggregeerden meerdere
  regression-trees (random forest-variant).
- **Pipe failure** — Boosted decision tree was nuttig voor
  uitvalvoorspelling.
- **Software defects** — Decision jungle werd toegepast.

## Waarom ensembles voor PdM?

Onderhoud-data is vaak onevenwichtig (weinig failure-cases) en
heterogeen (meerdere sensors, condities). Ensembles vangen die
diversiteit beter op dan een enkel model.


## Praktijkvoorbeeld

Voor RUL-prognose van aircraft engines bleek de ensemble-aanpak
consequent betere voorspellingen te geven dan elke individuele
regressor — de fout daalde door variance-reductie via bagging.
