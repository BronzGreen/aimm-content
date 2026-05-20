---
id: ko-spc-501
title: CNC-frees casus — I-MR kaart en gereedschapsslijtage detecteren
type: voorbeeld
domain: spc
subdomain: regelkaarten
summary: 'CNC-operator bewaakt boorgat-diameters (10,00 ± 0,02 mm) op een

  I-MR-kaart omdat elke meting uniek is. Na 40 uur productie:

  6 stijgende metingen (Nelson-regel 3 — trend). Gereedschapscheck

  onthult 0,015 mm slijtage. Tooling-vervanging voorkomt 200 uitvallers.'
source_centrality: 0.7
source_ref: Maakindustrie-praktijk; AIAG SPC Reference Manual; geïllustreerd uit operator-cases
status: validated
updated_at: '2026-05-20'
correlation_id: ronde25-lo-spc-501
---

# CNC-frees casus — I-MR kaart en gereedschapsslijtage detecteren

## Productiecontext
- **Bewerking**: CNC-freescentrum
- **Productie**: seriële bestelling 2000 stuks
- **Kritisch kenmerk**: boorgat-diameter
- **Tolerantie**: 10,00 ± 0,02 mm

## Meetstrategie
- Elk uur: 3 stuks meten met digitale schuifmaat
- Plot op **I-MR-kaart** (Individual + Moving Range)
- Reden voor I-MR: elke meting is uniek, geen natuurlijke subgroep

## Het signaal
Na ~40 uur productie ziet de operator:
- **6 opeenvolgende metingen** geleidelijk stijgend richting bovengrens
- Geen punt buiten control limits
- Patroon = **Nelson-regel 3 (trend)**

## Operator-respons
1. Stop machine
2. Meet het freesgereedschap → blijkt **0,015 mm slijtage**
3. Vervang tooling
4. Documenteer: signaal, oorzaak, actie, effect
5. Hervat productie met monitoring

## Resultaat
Tooling-vervanging voorkomt dat de **volgende 200 stuks** out-of-spec
zouden gaan. Zonder Nelson-regel 3: pas ingrijpen na overschrijding
van UCL (regel 1) — uren later, met afkeur tot gevolg.

## Lessen
- **I-MR is geschikt** voor unieke metingen zonder natuurlijke
  subgroep
- **Trends zijn vroege waarschuwingen** — niet wachten op punt-buiten
- **Gereedschapsslijtage** is een typische trend-veroorzaker
- **Documentatie** van signaal-oorzaak-actie levert organisatie-leren

## Inzetbaarheid in modules
| Module | Inzet |
|--------|-------|
| **1 Gebruik** | Herkenningsoefening: welke regel zie je hier? |
| **2 Train** | Configuratie: hoe richt je deze I-MR-kaart in? |
| **3 Op Maat** | Ontwerp: wat als toleranties wijzigen? Andere chart? |


## Praktijkvoorbeeld

[De casus zelf is het voorbeeld]

Cijfers ter illustratie: bij verlies aan slijtage van 0,0004 mm/uur
(40 uur × 0,0004 = 0,016 mm drift), zou een diameter starten op
9,990 mm en eindigen op 10,006 mm. Net binnen specs (≤ 10,02), maar
de trend was al ver vóór de spec-overschrijding zichtbaar op de kaart.
