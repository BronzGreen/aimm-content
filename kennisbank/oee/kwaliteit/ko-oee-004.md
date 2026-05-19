---
id: ko-oee-004
title: 'Kwaliteit: hoeveel producten zijn goed in een keer?'
type: concept_uitleg
domain: oee
subdomain: kwaliteit
summary: Kwaliteit in OEE meet hoeveel producten in een keer goed zijn. Afkeur en
  herbewerking verlagen dit getal, ook als het product uiteindelijk toch goedgekeurd
  wordt.
source_centrality: 0.7
source_ref: Competentieframework AIMM — SPC & OEE
status: validated
updated_at: '2026-05-19'
correlation_id: ronde5-lo-oee-004
---

# Kwaliteit: hoeveel producten zijn goed in een keer?

**Kwaliteit** is het derde onderdeel van OEE. Het beantwoordt de vraag: van alle producten die de machine maakt, hoeveel zijn er in een keer goed?

### De berekening

**Kwaliteit = Goede producten / Totaal geproduceerde producten**

Bijvoorbeeld:
- De machine maakt 1000 stuks
- 20 stuks zijn afkeur
- 30 stuks moesten herbewerkt worden
- Goed in een keer: 1000 - 20 - 30 = 950
- Kwaliteit: 950 / 1000 = **95%**

### First Pass Yield

Het kwaliteitspercentage in OEE heet ook wel **First Pass Yield** (FPY): het percentage producten dat de eerste keer al goed is. Dit is strenger dan het uiteindelijke afkeurpercentage, want herbewerkte producten tellen als verlies.

### Waarom telt herbewerking als verlies?

Een product dat je moet herbewerken kost:
- **Extra machinetijd** -- de machine had in die tijd nieuwe producten kunnen maken
- **Extra arbeid** -- iemand moet het product opnieuw bewerken
- **Extra materiaal** -- soms gaat er materiaal verloren
- **Extra controle** -- het herbewerkte product moet opnieuw gecontroleerd worden

Ook als het product uiteindelijk goedgekeurd wordt, heb je productietijd verloren.

### Kwaliteitsverlies herkennen

| Type | Wat het is | Voorbeeld |
|---|---|---|
| **Afkeur** | Product is niet te redden | Verkeerde maat, scheur, breuk |
| **Herbewerking** | Product moet opnieuw bewerkt | Nabramen, opnieuw lassen, bijschuren |
| **Opstartverlies** | Eerste producten na opstarten zijn niet goed | Spuitgietmachine moet eerst op temperatuur komen |

### De link met SPC

SPC helpt je om kwaliteitsproblemen **vroegtijdig** te signaleren. Als je regelkaart laat zien dat je proces uit controle raakt, kun je ingrijpen voordat je afkeur produceert. Zo beschermt SPC je OEE-kwaliteitsscore.

## Praktijkvoorbeeld

Een spuitgietbedrijf maakt kunststof behuizingen. Elke ochtend na het opstarten zijn de eerste 15 producten niet goed -- de matrijs is nog niet op temperatuur. Dat zijn 15 x 5 werkdagen = 75 producten per week opstartverlies. Door de matrijs voor te verwarmen met een temperatuurregelaar, daalt het opstartverlies naar 3 producten per ochtend. De kwaliteitsscore stijgt van 97% naar 99%.
