---
id: ko-oee-002
title: 'Beschikbaarheid: hoeveel van de geplande tijd draait de machine?'
type: concept_uitleg
domain: oee
subdomain: beschikbaarheid
summary: Beschikbaarheid meet welk deel van de geplande productietijd de machine ook
  echt draait. Stilstand door storingen en omstellen verlaagt dit getal.
source_centrality: 0.7
source_ref: Competentieframework AIMM — SPC & OEE
status: validated
updated_at: '2026-05-18'
correlation_id: ronde2-lo-oee-002
---

# Beschikbaarheid: hoeveel van de geplande tijd draait de machine?

**Beschikbaarheid** is het eerste onderdeel van OEE. Het beantwoordt de vraag: hoeveel van de tijd die we hadden **ingepland** voor productie, draaide de machine ook echt?

### De berekening

**Beschikbaarheid = Draaitijd / Geplande productietijd**

Bijvoorbeeld:
- Geplande productietijd: 8 uur (= 480 minuten)
- De machine stond 60 minuten stil
- Draaitijd: 480 - 60 = 420 minuten
- Beschikbaarheid: 420 / 480 = **87.5%**

### Wat telt als stilstand?

Stilstand is alle tijd dat de machine niet draait terwijl dat wel gepland was:

- **Storingen**: de machine is kapot en moet gerepareerd worden
- **Omstellen**: de machine wordt ingesteld voor een ander product
- **Wachten**: de machine wacht op materiaal, gereedschap of een operator
- **Opstarten**: de machine moet opwarmen of kalibreren

### Wat telt NIET als stilstand?

- Geplande pauzes (lunch, ploegwissel)
- Gepland onderhoud (als het buiten de productietijd valt)
- Weekenden of feestdagen (geen geplande productie)

Deze tijd zit niet in de geplande productietijd, dus ook niet in de berekening.

### Waar zit het verbeterpotentieel?

| Type stilstand | Typische oorzaak | Verbetering |
|---|---|---|
| Storingen | Slijtage, gebrek aan onderhoud | Preventief onderhoud, predictive maintenance |
| Omstellen | Lange wisseltijden | SMED (Single Minute Exchange of Die) |
| Wachten | Materiaaltekort, logistiek | Betere planning, buffervoorraden |
| Opstarten | Lange opwarmtijd | Standaard opstartprocedures |

## Praktijkvoorbeeld

Bij een plaatwerkerij staat de ponsmachine elke ochtend 20 minuten stil omdat de operator moet wachten op materiaal uit het magazijn. Dat is 20 minuten per dag, 5 dagen per week, 52 weken per jaar = 87 uur per jaar aan verloren productietijd. Door een kleine materiaalbuffer bij de machine neer te zetten, verdwijnt deze wachttijd volledig.
