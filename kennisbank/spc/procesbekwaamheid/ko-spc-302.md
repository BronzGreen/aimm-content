---
id: ko-spc-302
title: Pp en Ppk — langetermijn-bekwaamheid voor de klantervaring
type: concept_uitleg
domain: spc
subdomain: procesbekwaamheid
summary: 'Pp en Ppk lijken op Cp/Cpk maar gebruiken de **langetermijn-spreiding**

  die de klant uiteindelijk ervaart. Bij een stabiel proces liggen Cpk

  en Ppk dichter bij elkaar. Ford eist Ppk ≥ 1,67 voor relevante

  automotive-capability in actuele PPAP-documentatie.'
source_centrality: 0.7
source_ref: Ford PPAP 4th edition; AIAG SPC Reference Manual; NIST/SEMATECH Handbook
status: validated
updated_at: '2026-05-20'
correlation_id: ronde19-lo-spc-302
---

# Pp en Ppk — langetermijn-bekwaamheid voor de klantervaring

## Het verschil: korte vs lange termijn

| Index-paar | Spreiding | Wat het meet |
|------------|-----------|--------------|
| **Cp/Cpk** | Binnen-subgroep σ (kortetermijn) | Wat het proces **kan** als het stabiel is |
| **Pp/Ppk** | Totale σ (langetermijn) | Wat de **klant uiteindelijk ervaart** |

## Waarom dit onderscheid bestaat
Tussen subgroepen gebeuren shifts en drifts die binnen één subgroep
niet zichtbaar zijn:
- Materiaalbatch-wissels
- Operator-overdracht ploeg A → B
- Setup-aanpassingen
- Temperatuurschommelingen door dag/nacht

Deze "tussen-subgroep variatie" telt mee in Pp/Ppk maar niet in
Cp/Cpk. Daarom geldt bijna altijd: **Cpk ≥ Ppk**.

## Wanneer liggen ze dicht bij elkaar?
Bij een **stabiel proces** liggen Cpk en Ppk dicht bij elkaar — er
is dan weinig tussen-subgroep variatie bovenop de binnen-subgroep
variatie. Een groot verschil tussen Cpk en Ppk is dus zelf een
diagnostisch signaal: het proces is niet stabiel of er zijn
betekenisvolle subgroep-effecten.

## Industriële eisen
- **Ford PPAP** (4th edition, actueel): **Ppk ≥ 1,67** voor relevante
  automotive-capability
- **AIAG SPC Reference Manual**: vergelijkbare eisen per kritisch
  kenmerk
- **General Motors / VW**: vaak zelfde of strengere drempels

## Operator-implicatie
Als de Cpk goed is (≥1,33) maar de Ppk laag (<1,33): het proces is
kortstondig wel capabel, maar de praktijk is dat door batch-wissels
en shift-overdracht alsnog scope-uitval ontstaat. Actie: kijk naar
de **stabiliteit tussen subgroepen** in plaats van de spreiding
binnen.

## Pp (zonder centrering)
Pp = (USL − LSL) / (6 × σ_totaal). Net als Cp meet dit alleen de
potentie, niet de centrering. Cpk en Ppk corrigeren wél voor
centrering — daarom altijd beide rapporteren.


## Praktijkvoorbeeld

Een lijn meet over een week: Cpk = 1,42 (binnen elke shift goed),
Ppk = 1,05 (over de hele week onvoldoende). Het verschil van 0,37
is groot.

Onderzoek wijst uit: ploeg B stelt de machine systematisch 0,15 mm
hoger in dan ploeg A. Binnen elke shift is het proces stabiel
(goede Cpk), maar de wissel zorgt voor effectieve drift in de week
(lage Ppk).

Actie: standaardiseer de set-up procedure per ploeg, train ploeg B
op de juiste instelling. Niet het proces zelf aanpakken — wel het
systeem rond shift-wissels.
