---
id: ko-spc-103
title: SPC in Industry 4.0 — van papieren kaart naar digitale monitoring
type: concept_uitleg
domain: spc
subdomain: ai_integratie
summary: 'Klassieke SPC draaide op handmetingen en papieren kaarten. Industry

  4.0 voegt continue sensordata, IoT, realtime dashboards en AI-modellen

  toe. Het Shewhart-principe blijft hetzelfde — meetfrequentie,

  datastructuur en reactietijd zijn radicaal veranderd.'
source_centrality: 0.7
source_ref: Recente literatuur Industry 4.0 SPC; ISO 7870-2
status: validated
updated_at: '2026-05-19'
correlation_id: ronde3-lo-spc-103
---

# SPC in Industry 4.0 — van papieren kaart naar digitale monitoring

## Wat is veranderd, wat blijft hetzelfde

| Aspect | Klassieke SPC | Moderne SPC (Industry 4.0) |
|--------|---------------|----------------------------|
| Meten | Handmatig, periodiek | Continu via sensors |
| Drager | Papier of spreadsheet | Cloud/MES/SCADA dashboards |
| Detectie | Operator scant kaart | Automatische alarmregels + AI |
| Reactietijd | Uren tot dagen | Seconden tot minuten |
| Datavolume | Tientallen punten/dag | Miljoenen punten/dag |

## Wat blijft hetzelfde
Het **fundamentele Shewhart-principe**: onderscheid tussen verwachte
variatie en betekenisvolle signalen. Een sensor die elke seconde meet
verandert niets aan de vraag "is dit signaal of ruis?".

## Wat dit betekent voor MBO-operators
De operator van vandaag werkt steeds vaker met:
- **Realtime dashboards** in plaats van papieren kaarten
- **Automatische alarmen** in plaats van zelf scannen
- **AI-aanbevelingen** naast (of soms in plaats van) Nelson-rules

Dat verlegt de operator-vaardigheid van *kaart tekenen* naar
*procesgedrag begrijpen ongeacht het scherm*.

## Koppeling aan AIMM-use-cases
- **Predictive Maintenance** (PM) gebruikt vergelijkbare tijdreeksen
- **AI Kwaliteitscontrole** (vision) levert defectdata die in
  p-/np-/c-/u-kaarten passen
- **Data Literacy** is voorwaarde om dashboards betekenisvol te lezen


## Praktijkvoorbeeld

Bij een verpakkingslijn die voorheen elke 2 uur handmatig 5 stuks
woog, meet nu een inline-weegcel elke verpakking. De cel stuurt
duizenden punten per uur naar een MES-dashboard. Een achterliggende
regel berekent X̄-R per minuut. Als de range plotseling stijgt,
verschijnt binnen 30 seconden een alarm op het scherm van de operator.
De operator hoeft niet meer te plotten — wel te begrijpen wat
'range stijgt' betekent.
