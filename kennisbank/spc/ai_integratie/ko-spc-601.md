---
id: ko-spc-601
title: Digitale SPC en sensordata — uitbreiding, geen vervanging
type: concept_uitleg
domain: spc
subdomain: ai_integratie
summary: 'Digitale SPC voegt continue sensoren, hogere meetfrequentie, grotere

  datavolumes en multivariate analyse toe aan klassieke SPC. Industry

  4.0-era (vanaf ~2011) bracht nieuwe kansen door sensing,

  connectiviteit, cyber-fysieke systemen. Het Shewhart-principe blijft.'
source_centrality: 0.7
source_ref: Technometrics review 2024 over Industry 4.0 SPC; ISO 7870-2
status: validated
updated_at: '2026-05-20'
correlation_id: ronde26-lo-spc-601
---

# Digitale SPC en sensordata — uitbreiding, geen vervanging

## Wat verandert er?

| Aspect | Klassieke SPC | Digitale SPC (Industry 4.0) |
|--------|---------------|------------------------------|
| **Meetfrequentie** | Laag (uurlijks/per shift) | Continu (seconde/minuut) |
| **Datastroom** | Beperkt (tientallen punten/dag) | Groot (miljoenen punten/dag) |
| **Analyse** | Univariaat (één variabele tegelijk) | Multivariaat mogelijk |
| **Data-bron** | Handmetingen | IoT-sensoren, MES, SCADA |
| **Detectie** | Operator scant kaart | Auto-alarmen + AI |
| **Dimensionaliteit** | Lage dimensie | Hoge dimensie |

## Wat blijft hetzelfde
Het **fundamentele Shewhart-principe**: onderscheid tussen
verwachte variatie en betekenisvolle signalen. Een sensor die
elke seconde meet verandert niets aan de vraag "is dit signaal of
ruis?".

## Tijdslijn
De Technometrics-review (2024) plaatst de **Industry 4.0-era**
grofweg vanaf **2011** — toen sensing, connectiviteit en
cyber-fysieke systemen breed beschikbaar werden voor productie.

## Praktische verandering voor de operator
Operator van vandaag werkt steeds vaker met:
- **Realtime dashboards** in plaats van papieren kaarten
- **Automatische alarmen** in plaats van zelf scannen
- **AI-aanbevelingen** naast (of soms in plaats van) Nelson-rules
- **Multi-variabele displays** in plaats van één kaart per kenmerk

Dat verlegt de operator-vaardigheid van **kaart tekenen** naar
**procesgedrag begrijpen ongeacht het scherm**.

## Wat de digitale verschuiving NIET doet
- **Niet**: Nelson-rules verouderd maken (ze blijven correct, maar
  zien soms te weinig van complexe patronen)
- **Niet**: capability-redenering vervangen
- **Niet**: behoefte aan reactieplannen wegnemen
- **Niet**: rationele subgroepering overbodig maken

## Implicatie voor curriculumdesign
Operators moeten nog steeds de fundamenten leren — maar het
werkmateriaal verschuift van papieren kaarten naar dashboards en
alarmsystemen.


## Praktijkvoorbeeld

Een verpakkingslijn die voorheen elke 2 uur handmatig 5 stuks woog,
meet nu continu via inline-weegcel:

- **Vroeger**: 12 metingen/dag → één papieren X̄-R-kaart
- **Nu**: 60 metingen/minuut → MES-dashboard met X̄-R per minuut +
  capability-update per uur
- Een achterliggende regel berekent stijgende range → alarm binnen
  30 seconden op operator-scherm

De operator hoeft niet meer te plotten — wel te begrijpen wat
"stijgende range" betekent en wat de juiste respons is. Het
Shewhart-denken is belangrijker dan ooit, juist omdat de
automatisering het signaaldetectiewerk overneemt.
