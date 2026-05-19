---
id: ko-oee-003
title: 'Prestatie: draait de machine op volle snelheid?'
type: concept_uitleg
domain: oee
subdomain: prestatie
summary: Prestatie meet of de machine op de bedoelde snelheid draait. Korte stops
  en vertraagd draaien verlagen dit getal, ook als de machine technisch gewoon draait.
source_centrality: 0.7
source_ref: Competentieframework AIMM — SPC & OEE
status: validated
updated_at: '2026-05-19'
correlation_id: ronde3-lo-oee-003
---

# Prestatie: draait de machine op volle snelheid?

**Prestatie** is het tweede onderdeel van OEE. Het beantwoordt de vraag: als de machine draait, draait hij dan op de snelheid waarvoor hij ontworpen is?

### De berekening

**Prestatie = (Aantal geproduceerde stuks x Ideale cyclustijd) / Draaitijd**

Of eenvoudiger:

**Prestatie = Werkelijke output / Theoretisch mogelijke output**

Bijvoorbeeld:
- De machine kan theoretisch 100 stuks per uur maken
- In een uur draaitijd maakt hij er 85
- Prestatie: 85 / 100 = **85%**

### Wat verlaagt de prestatie?

**Korte stops (micro-stilstanden)**
- De machine stopt even en start weer op
- Een sensor geeft een foutmelding, operator drukt op reset
- Materiaal klemt, operator maakt het los
- Duur: meestal minder dan 5 minuten per keer
- Probleem: ze worden vaak niet geregistreerd, maar tellen op

**Vertraagd draaien (reduced speed)**
- De machine draait, maar langzamer dan de ideale snelheid
- Oorzaken: slijtage, slechte grondstof, bewust teruggeschakeld vanwege kwaliteitsproblemen
- Probleem: het valt niet op omdat de machine gewoon draait

### De verborgen fabriek

Prestatieverlies is vaak **onzichtbaar**. De machine draait, er komen producten uit, niemand staat stil. Maar als je berekent hoeveel de machine **zou kunnen** produceren, blijkt er een groot gat. Dit noemen we de **verborgen fabriek** -- productiecapaciteit die je al hebt maar niet benut.

| Verliestype | Zichtbaar? | Typische omvang |
|---|---|---|
| Storingen | Ja -- iedereen ziet het | 5-15% |
| Korte stops | Nauwelijks | 5-10% |
| Snelheidsverlies | Nee | 5-15% |

## Praktijkvoorbeeld

Op een assemblagelijn voor elektronische componenten draait de pick-and-place machine de hele dag. Maar elke 10-15 minuten stopt hij 20 seconden omdat een feeder vastloopt. De operator tikt ertegen en de machine draait weer. Niemand registreert deze stops. Maar 20 seconden x 30 keer per dienst = 10 minuten per dienst = 50 minuten per week. Door de feeders beter af te stellen, wint het team bijna een uur productietijd per week.
