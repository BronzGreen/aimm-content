---
id: ko-spc-101
title: Wat SPC is — procesgedrag in tijd, niet inspectie achteraf
type: definitie
domain: spc
subdomain: fundament
summary: 'SPC (Statistical Process Control) volgt procesdata in volgorde van tijd

  op een regelkaart met centrale lijn en boven-/ondergrenzen. Het bepaalt

  of variatie consistent en voorspelbaar is, of dat er onvoorspelbare

  verstoringen optreden.'
source_centrality: 0.7
source_ref: ASQ Control Chart definitie; ISO 7870-1, 7870-2; Shewhart (1931); NIST/SEMATECH
  Engineering Statistics Handbook
status: validated
updated_at: '2026-05-12'
correlation_id: sprint3-acceptance-2
---

# Wat SPC is — procesgedrag in tijd, niet inspectie achteraf

## Wat SPC is — en wat niet

SPC is **geen inspectiemethode achteraf**. Het is een manier om een
proces in de tijd te volgen via een regelkaart. Op die kaart staat:
- Een **centrale lijn** (gemiddeld procesgedrag)
- Een **bovengrens** (UCL) en **ondergrens** (LCL)
- **Punten** in volgorde van tijd

ASQ-definitie: een control chart is een grafiek waarmee je kunt
beoordelen of variatie **consistent en voorspelbaar** is, of dat er
**onvoorspelbare verstoringen** optreden. ISO 7870-1 en 7870-2 plaatsen
diezelfde gedachte centraal.

## Historische basis
Walter Shewhart formuleerde in de jaren 1920 het algemene model: een
centrumlijn met grenzen op een aantal standaarddeviaties. Zijn boek
*Economic Control of Quality of Manufactured Product* (1931) is nog
altijd fundamenteel.

## Waarom werkt het?
SPC garandeert geen perfecte kwaliteit. Het maakt de **normale
bandbreedte** van procesgedrag zichtbaar. Wanneer data binnen die
bandbreedte blijven, is er geen sterk signaal dat het proces is
veranderd. Wanneer punten daarbuiten komen of een onwaarschijnlijk
patroon vormen, is dat een aanwijzing dat een **andere oorzaak meedoet**.

## Didactische kern voor operators
SPC gaat **niet eerst over productspecificaties halen**. Het gaat
eerst over **procesgedrag begrijpen**.


## Praktijkvoorbeeld

Bij een spuitgietlijn meet de operator elke 2 uur 5 onderdeelgewichten.
Die gemiddelden komen op de regelkaart. Zolang ze schommelen tussen
99,8 en 100,2 g (binnen UCL/LCL), is er geen reden om in te grijpen.
Wanneer drie gemiddelden achter elkaar boven 100,3 g uitkomen, is dat
een signaal dat er iets in het proces is veranderd.
