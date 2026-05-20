# Handout: Van SHAP-grafiek naar actie
*SHAP-interpretatie — Predictive Maintenance Module 2*

**Naam:** ____________________  **Datum:** __________

---

> **Kernidee:** Na een anomaliemelding vertelt de SHAP-grafiek je welke sensor het meest bijdraagt. Zo weet je waar je moet beginnen. Je hoeft niet alles te checken.

---

## Het 5-stappenplan

| Stap | Wat doe je? | Voorbeeld |
|------|-------------|-----------|
| **1. Open de SHAP-grafiek** | Klik op de anomaliemelding in het dashboard. | Score is 68. Je opent de details. |
| **2. Lees de top-3 sensoren** | Welke sensor, hoeveel procent, welke richting? | Koeltemperatuur 58%, spiltemperatuur 22%, trillingen 12%. |
| **3. Groepeer de sensoren** | Horen de top-sensoren bij hetzelfde systeem? | Koeltemperatuur + spiltemperatuur = koelsysteem. |
| **4. Bepaal je actie** | Kies wat je als eerste checkt. | Koelsysteem checken: filter, pomp, slangen. |
| **5. Documenteer** | Schrijf je bevinding in de werkorder. | "Verstopt koelfilter gevonden en gereinigd." |

---

## Vuistregels

| Situatie | Wat betekent het? | Wat doe je? |
|----------|-------------------|-------------|
| Een sensor boven 70% | Lokaal probleem of sensorstoring | Check die ene sensor of dat onderdeel |
| 2-3 sensoren uit een systeem | Systeemprobleem | Check het hele systeem |
| Veel sensoren, elk klein % | Algemene slijtage | Vergelijk met vorige metingen |

---

## Voorbeeld: Operator Dennis

Dennis krijgt een melding: score 68.
Hij opent de SHAP-grafiek:

- Koelmiddeltemperatuur: **58%** (te hoog)
- Spiltemperatuur: **22%** (te hoog)
- Trillingen: **12%** (normaal)

Dennis ziet: twee sensoren wijzen op het koelsysteem.
Hij checkt de koelunit en vindt een verstopt filter.
Na schoonmaken daalt de score naar 15.

---

## Vergelijk met je quiz

*Kijk terug naar je antwoorden op de storingsquiz (werkblad 1). Wat zou je nu anders doen?*

_______________________________________________

_______________________________________________

---
*Bron: SHAP — Lundberg & Lee (2017) | AIMM Predictive Maintenance Module 2 | v1.0*
