---
id: ko-ai-fundamentals-fl-001
title: Wat is Federated Learning?
type: definitie
domain: ai_fundamentals
subdomain: machine_learning_basics
summary: Federated learning is een gedistribueerde leervorm waarbij meerdere lokale
  clients en een centrale server samenwerken aan één globaal model — zonder dat de
  ruwe data de cliënt verlaat.
source_centrality: 0.95
source_ref: Ahn et al. (2023). Federated Learning for Predictive Maintenance, §2.4
  (p. 5-6)
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-ai-fund-fl-001
---

# Wat is Federated Learning?

## Definitie

Federated learning (FL) is een technologie waarbij meerdere lokale
clients samen met een centrale server een gedeeld globaal model leren,
terwijl de data **gedecentraliseerd blijft**. Lokale clients zijn
bijvoorbeeld IoT-apparaten, smartphones of edge-nodes.

## Werking

- Elk apparaat houdt zijn data lokaal — geen ruwe data naar de cloud.
- Lokaal wordt een model getraind met de eigen data.
- Alleen **modelparameters** (gewichten, gradiënten) gaan naar een
  centrale server.
- De server combineert de updates tot een globaal model en deelt dit
  terug.
- Dit cyclisch proces herhaalt zich tot convergentie of een vooraf
  ingesteld aantal rondes is bereikt.

## Waarom relevant

FL ontstond om twee fundamentele AI-problemen te beperken:

1. **Privacy** — gevoelige data (medisch, persoonlijk, fabrieks-IP)
   hoeft niet centraal opgeslagen te worden.
2. **Bandbreedte / latency** — aan de netwerkrand wordt enorm veel
   data gegenereerd; alles naar de cloud sturen is vaak onhaalbaar.

## Beperking

De centrale server is een **single point of failure** — valt deze
weg, dan stopt het hele leerproces.


## Praktijkvoorbeeld

FL wordt momenteel het meest actief onderzocht in de medische sector,
omdat patiëntdata privacy-gevoelig is. AI-modellen kunnen daar
getraind worden zonder dat ziekenhuisdata uitwisseld wordt.
