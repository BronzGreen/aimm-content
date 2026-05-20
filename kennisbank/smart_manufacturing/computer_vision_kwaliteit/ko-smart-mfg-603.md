---
id: ko-smart-mfg-603
title: 'Synthetische data: trainingsfoto''s maken zonder foto''s te nemen'
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Als duizenden foto's verzamelen en labelen te duur of te traag is, kun je
  de foto's laten maken door de computer. Een 3D-scan van je onderdeel plus 3D-software
  levert een getraind AI-systeem in tien minuten in plaats van weken.
source_centrality: 0.7
source_ref: 'Poodt, T. (2026). The Synthetic Offensive: Beyond Manual Data Collection.
  ETNA Coffee Factory. Gebruikt met toestemming RLC-Oost.'
status: validated
updated_at: '2026-05-20'
correlation_id: ronde26-lo-smart-mfg-603
---

# Synthetische data: trainingsfoto's maken zonder foto's te nemen

In de vorige sessie hebben we gezien dat gelabelde foto's de bottleneck zijn bij computer vision. Honderden foto's per defect, elk 1-3 minuten labelen, al snel tientallen uren werk. Voor sommige bedrijven is dat onhaalbaar.

Er bestaat een alternatief: **synthetische data**. In plaats van foto's te maken, laat je de computer ze genereren.

### Wat is synthetische data?

Synthetische data zijn beelden die **niet echt zijn**, maar door een computer gemaakt. Je bouwt een 3D-model van je onderdeel en laat de computer daar honderden foto's van renderen — vanuit verschillende hoeken, met verschillende belichting, op verschillende achtergronden.

De clou: omdat de computer het 3D-model zelf heeft getekend, **weet hij precies waar het onderdeel zit in elk beeld**. De labels komen er automatisch bij, zonder handmatig werk.

### De Etna-case

*(Bron: Poodt, T. (2026). The Synthetic Offensive: Beyond Manual Data Collection. ETNA Coffee Factory. Gebruikt met toestemming RLC-Oost.)*

**ETNA Coffee Factory** (Etten-Leur, maker van koffieapparaten) heeft dit uitgeprobeerd. Hun uitdaging: een AI-systeem trainen dat onderdelen in een koffieapparaat herkent — elektrische printplaten, kabels, connectoren. Traditioneel: duizenden foto's maken van échte koffieapparaten op verschillende productieseries. Onhaalbaar bij elke hardware-wijziging.

Wat ze deden:

1. **3D-scan met een telefoon.** Met een gewone Android-telefoon en een gratis app scannen ze een echte koffieapparaat-module in 3D.
2. **Blender (gratis 3D-software)** genereert vervolgens honderden verschillende foto's van dat 3D-model — op 360 beelden per seconde met een goede laptop-GPU.
3. **Automatische labels.** Omdat de computer het 3D-model bouwde, weet hij op elk beeld precies waar elk onderdeel zit. Labels komen er gratis bij.
4. **YOLO-model trainen.** Het AI-model wordt getraind op de synthetische beelden — en blijkt daarna ook échte foto's van koffieapparaten goed te herkennen.

**Totale tijd: onder de 10 minuten** van 3D-scan tot werkend model. Traditioneel werk: weken tot maanden.

### Waarom dit voor jou belangrijk is

Je hoeft zelf geen Blender te kunnen gebruiken. Maar je moet als operator kunnen herkennen dat **dit een optie is**. Wanneer iemand op jullie werkvloer zegt *'we hebben AI-kwaliteitscontrole willen invoeren, maar 500 foto's labelen lukt niet'*, kun jij zeggen: *'kunnen we synthetische data gebruiken?'*.

### Wat synthetische data NIET is

Het is **geen magische oplossing**. Er zijn beperkingen die jij moet begrijpen:

- Een 3D-model is **nooit precies de echte wereld**. Belichting, stof, oppervlakteslijtage — dat valt er vaak buiten.
- Het getrainde model moet **altijd gevalideerd worden op echte foto's**. Daar blijf jij cruciaal: als operator zie je of het systeem in de praktijk klopt.
- Niet alle defecten zijn synthetisch te maken. Een **nieuw type kras** dat in de productie ontstaat, kent de computer niet — die moet je nog steeds met echte foto's leren.

### De les: kiezen tussen echt en synthetisch

Voor een snel prototype of een eerste versie van een AI-systeem: synthetisch is sneller en goedkoper. Voor een uiteindelijk productiesysteem: meestal een mix — synthetisch om snel te starten, aangevuld met echte foto's voor wat de computer niet kan simuleren.

Het label-probleem van de vorige sessie (5-20 uur handmatig werk) wordt hiermee **verkleind, niet weggenomen**. En jij blijft de eindcheck.


## Praktijkvoorbeeld

Stel: een productiebedrijf wil een camera-inspectiesysteem voor een nieuwe serie metalen beugels. Traditioneel: 450 foto's maken (150 per defect × 3 soorten), 5 uur handmatig labelen, model trainen, testen. Totaal: een week werk.

Met synthetische data: iemand scant één beugel met een telefoon (5 minuten), genereert in Blender 1000 foto's met automatische labels (10 minuten), traint het model (30 minuten). Totaal: één uur werk.

Maar: de operator moet het systeem testen op 50 echte foto's voordat het live mag. Een paar fout-meldingen? Waarschijnlijk iets wat de simulatie niet heeft meegenomen — bijvoorbeeld een type kras dat synthetisch niet goed te maken is. Dan worden die 50 echte foto's alsnog gelabeld en toegevoegd.

Van een week naar één uur + een halve dag validatie. Dat is het verschil dat synthetische data kan maken — als je weet wanneer je het wel en niet gebruikt.
