---
id: ko-smart-mfg-205
title: 'Van anomaliescores naar onderhoudsplanning: wanneer grijp je in?'
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een anomaliescore vertelt je dat er iets afwijkt, maar niet wanneer je moet
  handelen. Dit framework vertaalt scores naar concrete onderhoudsbeslissingen.
source_centrality: 0.7
source_ref: Gebaseerd op Sesana et al. (2024). Artificial Intelligence in Manufacturing,
  pp. 474-475 + operationele best practices
status: validated
updated_at: '2026-05-20'
correlation_id: ronde18-lo-smart-mfg-205
---

# Van anomaliescores naar onderhoudsplanning: wanneer grijp je in?

In Module 2 heb je geleerd hoe je anomaliescores leest en een model configureert. De volgende stap: **wat doe je met die scores?** Een score van 72 is geen reden voor paniek, maar ook geen reden om niets te doen. Je hebt een beslisframework nodig.

### Het verkeerslichtmodel voor anomaliescores

| Score | Kleur | Actie | Termijn |
|-------|-------|-------|---------|
| 0–30 | 🟢 Groen | Geen actie nodig | — |
| 30–50 | 🟡 Geel | Verhoogde monitoring | Dagelijks checken |
| 50–70 | 🟠 Oranje | Plan onderhoud in | Binnen 2 weken |
| 70+ | 🔴 Rood | Plan inspectie | Binnen 48 uur |

### Eén sensor vs. meerdere sensoren

Een enkele sensor met score 65 is anders dan drie sensoren die samen 65 scoren. Hoe weeg je dat?

- **Eén sensor hoog**: check die specifieke component. Mogelijk een sensorstoring of lokaal probleem.
- **Meerdere sensoren matig verhoogd**: check het systeem als geheel. Dit wijst vaak op slijtage of een systeembreed probleem (bijv. koeling, smering).
- **Combinatie hoog + laag**: kijk welke sensoren samenhangen. Temperatuur hoog + koelmiddeldruk laag = koelprobleem.

### Van score naar werkorder

Als je besluit dat onderhoud nodig is, maak je een werkorder met:

1. **Welke machine** — waar zit het probleem?
2. **Welke sensoren** — wat wees de SHAP-analyse aan?
3. **Urgentie** — groen/geel/oranje/rood
4. **Voorgestelde actie** — inspectie, preventief onderhoud, of vervanging
5. **Deadline** — op basis van het verkeerslichtmodel

### Belangrijk: de score is een advies, geen bevel

Jij kent je machine. Als de score 45 zegt maar jij hoort iets raars, plan dan toch een inspectie. De AI ondersteunt jouw vakkennis — het vervangt die niet.


## Praktijkvoorbeeld

Op maandagochtend checkt operator Marjan het anomaliedashboard voor haar drie CNC-machines. Machine 2 toont een score van 58 — oranje. Ze opent de details en ziet dat twee temperatuursensoren en één trillingssensor bijdragen aan de score. De SHAP-grafiek wijst op het hydraulische systeem.

Marjan maakt een werkorder aan: "Machine 2, hydraulisch systeem, inspectie binnen 2 weken, urgentie oranje." Ze voegt de SHAP-grafiek toe als bijlage. De onderhoudstechnicus kan nu gericht kijken in plaats van de hele machine te controleren.

Twee dagen later stijgt de score naar 73 — rood. Marjan past de werkorder aan: "Inspectie binnen 48 uur." De technicus vindt een lekkende hydrauliekslang. Reparatie duurt 30 minuten. Zonder het framework had Marjan moeten gokken wanneer ze alarm moest slaan.
