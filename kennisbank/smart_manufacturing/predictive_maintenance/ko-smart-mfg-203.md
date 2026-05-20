---
id: ko-smart-mfg-203
title: 'Modelresultaten interpreteren: wat betekent een anomaliescore?'
type: concept_uitleg
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een praktische handleiding om anomaliescores van een predictief model te
  interpreteren en om te zetten in concrete acties op de werkvloer.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1
status: validated
updated_at: '2026-05-20'
correlation_id: ronde16-lo-smart-mfg-203
---

# Modelresultaten interpreteren: wat betekent een anomaliescore?

Je predictieve model draait en geeft een **anomaliescore** per machine. Dat is een getal tussen 0 en 100 dat aangeeft hoe **ongewoon** het gedrag van de machine is. Maar wat doe je met dat getal? En wanneer kun je het vertrouwen?

### Wat de score betekent

De anomaliescore werkt als een verkeerslicht:

**Score 0-30: Groen — normaal, geen actie**
De machine draait binnen de verwachte waarden. Alle sensoren zijn stabiel. Je hoeft niets te doen.

**Score 30-70: Oranje — let op, monitor extra**
Er is iets veranderd, maar het is nog niet kritiek. Dit kan betekenen:
- Een sensor begint langzaam af te wijken.
- De machine gedraagt zich net iets anders dan normaal.
- Er is een verandering in de omgeving (temperatuur hal, ander materiaal).

Wat doe je: bekijk **welke sensor** de score omhoog drijft. Check of er een logische verklaring is. Verhoog de meetfrequentie. Meld het bij de volgende overdracht.

**Score 70-100: Rood — ingrijpen, plan onderhoud**
De machine wijkt sterk af van normaal. De kans op een storing neemt toe.

Wat doe je: check direct welke sensor afwijkt. Plan een inspectie of onderhoudsmoment. Overleg met de technische dienst. Documenteer wat je ziet.

### Wanneer vertrouw je de score?

Een model is niet altijd gelijk goed. Houd rekening met deze situaties:

- **Na een productwissel**: het model kent de nieuwe instellingen misschien nog niet. Een hoge score kan een vals alarm zijn.
- **Na onderhoud**: nieuwe onderdelen geven andere sensorwaarden. Het model moet even wennen.
- **Seizoensveranderingen**: in de zomer is de omgevingstemperatuur hoger, dat beinvloedt de sensordata.

De vuistregel: vertrouw de score als de machine al minimaal **2 weken stabiel draait** onder dezelfde omstandigheden.

### Score omzetten in actie

Gebruik dit stappenplan bij een hoge score:
1. Kijk welke sensor de hoogste bijdrage levert aan de score.
2. Controleer of er een logische verklaring is (productwissel, omgeving).
3. Vergelijk met eerdere situaties: heeft deze sensor eerder zo gedaan?
4. Beslis: monitoren of ingrijpen?
5. Documenteer je beslissing en het resultaat.


## Praktijkvoorbeeld

Een freesmachine scoort plotseling 82. De operator opent het dashboard en ziet dat de trillingssensor op de Y-as de grootste bijdrage levert. Hij checkt: is er een productwissel geweest? Nee, hetzelfde product als gisteren. Is er onderhoud geweest? Nee. Hij kijkt naar de trend: de trillingen stijgen al 3 dagen. Hij plant een inspectie met de technische dienst voor dezelfde middag. Bij inspectie blijkt een geleidingsrail versleten. Vervanging duurt 45 minuten — gepland in de lunchpauze. Zonder het model had dit een ongeplande stilstand van 3 uur kunnen worden, midden in een productierun.
