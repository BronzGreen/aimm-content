---
id: ko-spc-107
title: Control limits versus specificatiegrenzen — het kritische onderscheid
type: concept_uitleg
domain: spc
subdomain: regelkaarten
summary: 'Control limits (UCL/LCL) zeggen of het PROCES statistisch stabiel is.

  Specificatiegrenzen zeggen of het PRODUCT functioneel of contractueel

  voldoet. NIST: nooit control limits uit klanttoleranties afleiden.

  Veelgemaakte fout die signaaldetectie ondermijnt.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Engineering Statistics Handbook; ISO 7870-2
status: validated
updated_at: '2026-05-19'
correlation_id: ronde8-lo-spc-107
---

# Control limits versus specificatiegrenzen — het kritische onderscheid

## Het verschil

| | Control limits (UCL/LCL) | Specificatiegrenzen |
|---|--------------------------|---------------------|
| **Wat ze zeggen** | Is het PROCES stabiel? | Voldoet het PRODUCT? |
| **Vanwaar afgeleid** | Berekend uit procesdata (gemiddelde ± 3σ) | Gegeven door klant of ontwerp |
| **Plaats op kaart** | Op de regelkaart | NIET op de regelkaart (apart) |
| **Beslissing** | "Grijp ik in op het proces?" | "Mag dit product naar klant?" |

## NIST waarschuwt expliciet
Een proces kan **stabiel** zijn (binnen control limits) en toch
**te dicht bij specificatiegrens** zitten (lage capability).
Omgekeerd: een proces kan incidenteel binnen specs produceren
terwijl het proces **al uit controle** is.

## De kritieke fout
**Nooit control limits uit klanttoleranties afleiden.** Wie dat doet:
- Tekent geen kaart van procesgedrag meer
- Maakt een versimpelde pass/fail-grafiek
- Verbergt verstoringen die wel binnen specs blijven maar het proces
  signaleren
- Mist daardoor de waarde van SPC volledig

## Hoe wel?
Control limits berekenen uit het werkelijke procesgedrag:
```
UCL = gemiddelde + 3σ
LCL = gemiddelde − 3σ
```
Specs apart op de kaart tonen (of helemaal niet — sommige scholen
doen dit bewust om verwarring te voorkomen).


## Praktijkvoorbeeld

Bij een spuitgietlijn vraagt de klant onderdeelgewicht 100 ± 1g
(specs: 99-101). De operator berekent control limits uit 100 cycli
productiedata: gemiddelde 99,9 g, σ = 0,12 → UCL = 100,26, LCL = 99,54.

De control limits liggen ruim binnen de specificatiegrenzen. Het
proces is **stabiel** (UCL/LCL gehaald) en bovendien **bekwaam**
(specs ruimer dan UCL/LCL).

Verkeerde aanpak: control limits gelijk aan 99-101 zetten. Dan zou
een trend van 99,8 → 99,9 → 100,0 → 100,1 nooit een signaal geven,
ook al wijst hij op een procesverandering.
