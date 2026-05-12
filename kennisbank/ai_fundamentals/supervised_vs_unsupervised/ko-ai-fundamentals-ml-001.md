---
id: ko-ai-fundamentals-ml-001
title: Vier ML-leerklassen voor Predictive Maintenance
type: framework
domain: ai_fundamentals
subdomain: supervised_vs_unsupervised
summary: ML-gebaseerde PdM gebruikt vier leerklassen — supervised, unsupervised, semi-supervised
  en reinforcement learning — afhankelijk van of failure-data gelabeld, deels gelabeld
  of helemaal afwezig is.
source_centrality: 0.85
source_ref: Nacchia et al. (2021). Systematic Mapping of ML for PdM, §3.2 (p. 11-12)
status: validated
updated_at: '2026-05-12'
correlation_id: marathon-2026-05-12-lo-ai-fund-ml-001
---

# Vier ML-leerklassen voor Predictive Maintenance

## Vier leerklassen

### Supervised learning
Trainingsdata bevat **gelabelde failure-events**. Het algoritme leert
de relatie tussen sensordata en het bekende uitval-label. Voor PdM
het meest accuraat — als er voldoende historische uitvaldata beschikbaar is.

### Unsupervised learning
Logistieke en proces-data zijn beschikbaar, maar **geen failure-labels**.
Het algoritme zoekt verborgen patronen in de input. Bij PdM gebruikt
wanneer uitval-events zeldzaam of niet gedocumenteerd zijn.

### Semi-supervised learning
Combineert weinig gelabelde met veel ongelabelde voorbeelden — leert
de kansverdeling van de input en optimaliseert tegelijk de voorspelling
op de gelabelde voorbeelden. Recent populair in PdM-onderzoek.

### Reinforcement learning
Combineert leren en handelen in **online-leren** met self-optimization.
Leert een optimale relatie tussen input en beslissing/prestatie. Geschikt
voor adaptieve onderhoudsbeslissingen.

## Toepassing op PdM-probleemtypen

- **Classification** (supervised) — kans dat een onderdeel uitvalt voor n volgende cycli
- **Regression** (supervised) — voorspel Remaining Useful Life (RUL)
- **Clustering** (unsupervised) — groepeer datapunten op (dis)similariteit


## Praktijkvoorbeeld

Een fabriek met goede uitval-historie kan supervised regression
gebruiken om RUL te voorspellen; een fabriek zonder failure-labels
gebruikt unsupervised clustering om afwijkende patronen te isoleren.
