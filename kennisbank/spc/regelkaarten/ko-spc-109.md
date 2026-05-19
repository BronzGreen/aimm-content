---
id: ko-spc-109
title: Rationele subgroepering — wát samenvoegen bepaalt of de kaart werkt
type: framework
domain: spc
subdomain: regelkaarten
summary: 'Een rationele subgroep is een kleine set eenheden onder vrijwel

  dezelfde omstandigheden, dicht in de tijd. Doel: spreiding binnen

  groep = kortetermijnvariatie, verschillen tussen groepen = shifts

  en verstoringen. Verkeerd subgroeperen vernietigt detectiekracht.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Handbook; Minitab documentation; Ford PPAP 4th ed.; AIAG
  SPC Reference Manual
status: validated
updated_at: '2026-05-19'
correlation_id: ronde10-lo-spc-109
---

# Rationele subgroepering — wát samenvoegen bepaalt of de kaart werkt

## Wat een rationele subgroep is
Een subgroep is een **kleine set eenheden**:
- Onder vrijwel **dezelfde omstandigheden** gemaakt
- **Dicht in de tijd** verzameld
- Bij voorkeur uit dezelfde caviteit, lijn, machine, ploeg

## Waarom dit cruciaal is

| Variatiebron | Waar moet die zichtbaar worden? |
|--------------|----------------------------------|
| Kortetermijn-variatie (gewone ruis) | Binnen subgroep |
| Shifts/verstoringen | Tussen subgroepen |

Als je **dat omdraait** door verkeerd te subgroeperen, krijg je het
tegenovergestelde:
- Subgroep over meerdere shifts → control limits worden kunstmatig
  breed
- Subgroep over meerdere caviteiten → caviteit-verschillen verdwijnen
  in 'ruis'
- Subgroep over instelcondities → setup-effecten onzichtbaar

Resultaat: kaart geeft geen alarmen meer, ook bij echte verstoringen.

## Praktische richtlijnen

| Bron | Aanbeveling |
|------|-------------|
| **NIST/Minitab** | Initiële studie: 4-5 stuks per uur, ca 100 observaties of 25 subgroepen |
| **Ford PPAP** | Capabilitydemonstratie: minimaal 25 subgroepen van minimaal 5 |
| **Snapshot-principe** | Subgroep = momentopname van proces |

## De didactische kern voor operators
"Een goede kaart begint **vóór** het plotten — bij de vraag wát je
samenvoegt."

## Veelgemaakte fouten

1. **Subgroep over shifts** — vermengt operator-effecten met procesvariatie
2. **Subgroep over caviteiten** — verbergt caviteit-specifieke problemen
3. **Te kleine n (<3)** — instabiele variatieschattingen
4. **Mengen van setup-condities** — setup-effecten worden 'ruis'


## Praktijkvoorbeeld

Een spuitgietlijn met 4 caviteiten heeft een operator die elk uur
4 stuks meet (1 per caviteit). De operator denkt: "n=4, dat is
genoeg voor X̄-R."

Verkeerd: deze subgroep mengt vier verschillende caviteiten. Als
caviteit 3 een drift heeft, gaat dat verloren in de ruis tussen de
4 caviteiten.

Beter: meet 4 stuks **uit dezelfde caviteit** per uur (op rotatie:
uur 1 caviteit 1, uur 2 caviteit 2, etc.). Of: maak vier aparte
kaarten, één per caviteit.
