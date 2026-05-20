---
id: ko-smart-mfg-092
title: Anomaliedetectie in de productie
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Anomaliedetectie is het automatisch opsporen van afwijkingen in machinegedrag
  of productiedata. Het helpt om problemen vroeg te signaleren voordat ze schade veroorzaken.
source_centrality: 0.7
source_ref: Scholz et al. (2024). Artificial Intelligence in Manufacturing, pp. 366-374
status: validated
updated_at: '2026-05-20'
correlation_id: ronde11-lo-smart-mfg-092
---

# Anomaliedetectie in de productie

Stel je voor: een machine voert elke dag dezelfde beweging uit, duizenden keren. Op een dag werkt een motor niet goed meer. Het product raakt beschadigd. Hoe langer het duurt voordat je dit merkt, hoe meer schade er ontstaat.

**Anomaliedetectie** is het automatisch herkennen van dit soort afwijkingen. Het AI-systeem leert wat "normaal" is en slaat alarm als er iets ongewoons gebeurt.

### Drie soorten anomalieën

1. **Puntanomalie**: een enkel meetpunt dat afwijkt (bijv. een plotselinge temperatuurpiek)
2. **Contextuele anomalie**: een waarde die normaal is in de ene situatie maar afwijkend in een andere (bijv. hoge temperatuur bij opstart vs. tijdens productie)
3. **Collectieve anomalie**: een reeks metingen die samen een patroon laten zien dat afwijkt

### Hoe werkt het?

Het proces van anomaliedetectie heeft drie stappen:
1. **Voorbereiding**: data wordt verzameld en in het juiste formaat gebracht
2. **Training**: het AI-model leert wat normaal gedrag is
3. **Detectie**: het model vergelijkt nieuwe data met het geleerde patroon en geeft een alarm als er een afwijking is

### Waarom is dit belangrijk?

Vroege detectie van afwijkingen voorkomt:
- Beschadigde producten
- Ongeplande stilstand
- Hoge reparatiekosten
- Veiligheidsrisico's


## Praktijkvoorbeeld

Bij een fabrikant van brandstoftanks bewaakt een AI-systeem meer dan 100 sensorwaarden tijdens het blaasgieten. De sensoren meten temperatuur, druk, positie en energieverbruik. Als het systeem een afwijkend patroon detecteert - bijvoorbeeld een ongebruikelijke combinatie van druk en temperatuur - krijgt de operator direct een melding. Zo kan er worden ingegrepen voordat er defecte tanks van de lijn komen.
