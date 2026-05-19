---
id: ko-spc-106
title: Twee onderwijsregels — operator-regel en teamleider-regel
type: tip
domain: spc
subdomain: variatie_analyse
summary: 'Operator-regel: reageer op signalen, niet op ruis. Teamleider-regel:

  kijk naar patronen die voor de individuele operator niet zichtbaar

  zijn (verschillen tussen shifts, caviteiten, matrijzen, gereedschap).

  Hier verschuift SPC van ''kaart lezen'' naar procesdenken.'
source_centrality: 0.7
source_ref: AIAG SPC Reference Manual; ASQ
status: validated
updated_at: '2026-05-19'
correlation_id: ronde7-lo-spc-106
---

# Twee onderwijsregels — operator-regel en teamleider-regel

## De twee regels

### Operator-regel: reageer op signalen, niet op ruis
- Een signaal = data-patroon dat statistisch onwaarschijnlijk is bij
  normale variatie
- Ruis = normale schommeling binnen de bandbreedte
- Bij een signaal: stop, onderzoek, documenteer
- Bij ruis: niets doen (zie tampering — ko-spc-105)

### Teamleider-regel: kijk naar patronen die de operator mist
Een operator ziet zijn eigen shift, eigen machine. Een teamleider
ziet patronen die alleen ontstaan **boven het individuele niveau**:

| Patroontype | Wat je ziet |
|-------------|-------------|
| Verschil tussen **shifts** | Ploeg A en C produceren stabiel, B niet |
| Verschil tussen **caviteiten** | Caviteit 4 systematisch hoger dan 1-3 |
| Verschil tussen **matrijzen** | Matrijs M2 geeft consistent meer variatie |
| Verschil tussen **gereedschappen** | Specifieke tool faalt na X stuks |
| Verschil tussen **recepturen** | Variant Z heeft hogere afkeur |

Deze patronen zien vraagt om **stratified analysis** — data uitsplitsen
naar relevante factoren.

## Waar SPC verschuift van techniek naar denken
De operator-regel maakt SPC een **uitvoeringsdiscipline**. De
teamleider-regel maakt SPC een **analytische discipline**. Pas op
teamleider-niveau wordt SPC echt **procesdenken** in plaats van
kaart-lezen.

## Implicatie voor module-design
- Module 1 (Gebruik) focus: operator-regel
- Module 2 (Train) focus: meer signaal/ruis-onderscheid + introductie
  teamleider-regel
- Module 3 (Op Maat) focus: stratified analysis, patronen ontwerpen


## Praktijkvoorbeeld

Operator Karim op shift A ziet zijn kaart stabiel — geen actie nodig.
Maar teamleider Sophie ziet aan het einde van de week dat shift A
systematisch 0,3 mm hoger meet dan shift C. Geen enkele losse meting
uit shift A is out-of-control. Maar het patroon is wel betekenisvol:
mogelijk verschil in calibratie of meetmethode tussen shifts.

Sophie escaleert naar engineering voor calibratie-check.
