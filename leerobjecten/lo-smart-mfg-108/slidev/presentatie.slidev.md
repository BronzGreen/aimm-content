---
theme: default
title: SHAP — welke sensor draagt bij aan de anomalie?
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over het lezen van een SHAP-grafiek om bij een anomaliemelding
  de meest verdachte sensor aan te wijzen.
  Doelgroep: operators MBO-3, 30 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# SHAP — welke sensor draagt bij?

### Wat zegt de AI eigenlijk over de anomalie?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 30 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Vandaag krijgen we een melding van de AI: 'er is iets mis op machine 4'.
Maar wat precies? In 30 minuten leer je dat het systeem dat zelf vertelt
met een grafiek die SHAP heet.

Trigger: kijk de groep aan. "Wie heeft wel eens een melding gehad zonder uitleg?
Wat doe je dan?" Vang 1-2 reacties, geen oordeel, doorpakken naar quiz.
-->

---
layout: section
---

# Ervaren

## Storingsquiz: 5 anomaliemeldingen — raden

<!--
Overgang naar blok 1.
"Vijf meldingen, vijf machines. Jij gokt welke sensor het probleem veroorzaakt."
-->

---
layout: center
class: text-center
---

# Melding 1 — Spuitgietmachine 4

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Cyclus 1247.<br/>
  Iets klopt niet.<br/>
  Welke sensor?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  30 seconden — schrijf jouw gok op het werkblad.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  wb-01-ervaren · 5 meldingen
</div>

<!--
Toon de melding. Geef 30 sec. Onthul daarna het juiste antwoord (volgende click).
Bij goed: kort bevestigen. Bij fout: "Niemand kan dit zonder uitleg — dat is normaal."
-->

---
layout: center
class: text-center
---

# Melding 2 — CNC-freesmachine 2

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Spindeltemperatuur loopt langzaam op.<br/>
  Trillingen kloppen ook niet helemaal.<br/>
  Welke sensor zou jij eerst checken?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Melding 2 van 5
</div>

<!--
Geef 30 sec. Onthul antwoord, kort feedback.
Doel is NIET dat ze goed gokken. Doel is dat ze de pijn voelen.
-->

---
layout: center
class: text-center
---

# Melding 3 — Verpakkingslijn 1

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Snelheid daalt onverklaarbaar.<br/>
  Welke sensor heeft het zwaarst?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Melding 3 van 5
</div>

<!--
Geef 30 sec.
-->

---
layout: center
class: text-center
---

# Melding 4 — Spuitgietmachine 7

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Druk in de matrijs schommelt.<br/>
  Trilling is normaal, temperatuur ook.<br/>
  Toch melding. Welke sensor?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Melding 4 van 5
</div>

<!--
Geef 30 sec.
-->

---
layout: center
class: text-center
---

# Melding 5 — CNC-draaibank 5

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Drie sensoren tegelijk lichten geel op.<br/>
  Waar begin jij?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Tel je goeie gokken. Schrijf het op je werkblad.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Melding 5 van 5
</div>

<!--
Verzamelmoment: "Hoeveel had je goed? Schrijf op."
Niet plenair delen. We bespreken in fase 2.
-->

---
layout: section
---

# Reflecteren

## Hoe doe je het nu zonder uitleg-AI?

<!--
Overgang naar blok 2.
"Pak je buurman. Vergelijk wat je nu doet als een machine raar doet."
-->

---
layout: center
class: text-center
---

# Bespreek in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">👀</div>
    <div class="text-lg font-bold text-blue-700">Hoe doe je het nu?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">👂</div>
    <div class="text-lg font-bold text-purple-700">Waar kijk/luister/voel je naar?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">🗺️</div>
    <div class="text-lg font-bold text-green-700">Wat zou je willen weten?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Wat je mist — een soort schatkaart die zegt 'kijk daar eerst' — dat is wat SHAP doet.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  3 min duo · 3 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02 uitdelen. Timer op 3 min.
Loop rond. Luister naar concrete strategieen (kijken, ruiken, voelen, dashboard).

Plenair 3 min: verzamel "wat doe je nu?" en "wat is lastig?".
Schrijf 4-5 sleutelwoorden op flap-over.

Ankerwoord: "schatkaart". Werkt beter dan "visualisatie" of "analyse".
-->

---
layout: section
---

# Theoretiseren

## SHAP-grafiek leren lezen — drie regels

<!--
Overgang naar blok 3. "Pak je markeerstift. We krijgen de kapstok."
-->

---

# Een SHAP-grafiek

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat zie je?

- Per sensor één balk
- Lengte van de balk = impact
- Kleur = richting (hoger of lager dan normaal)

</div>

<div class="p-6 bg-slate-50 rounded-xl border-2 border-slate-200">

### Wat hoef je NIET te onthouden

- Wat SHAP precies betekent
- De formule erachter
- Het vakwoord 'feature importance'

<div class="text-sm opacity-60 mt-3">SHAP = grafiekje dat AI-uitleg geeft. Klaar.</div>

</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Drie dingen om naar te kijken — meer niet.
</div>

<!--
Toon het diagram (diagram-lo-smart-mfg-108.svg op deze slide indien beschikbaar).
"Per sensor een balk. Drie dingen om naar te kijken."

Bij vraag "wat staat SHAP voor?":
"Komt uit een formule, hoef je niet te onthouden."
-->

---

# De drie leesregels

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-300">
  <div class="text-5xl mb-3">📏</div>
  <div class="text-xl font-bold text-amber-700 mb-2">1. Groot = belangrijk</div>
  <div class="text-sm opacity-80">Hoe groter de balk, hoe meer die sensor bijdraagt aan de melding.</div>
</div>

<div class="p-6 bg-red-50 rounded-xl border-2 border-red-300">
  <div class="text-5xl mb-3">🔴</div>
  <div class="text-xl font-bold text-red-700 mb-2">2. Rood = hoger</div>
  <div class="text-sm opacity-80">Sensor meet meer dan de AI verwachtte.</div>
</div>

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-300">
  <div class="text-5xl mb-3">🔵</div>
  <div class="text-xl font-bold text-blue-700 mb-2">3. Blauw = lager</div>
  <div class="text-sm opacity-80">Sensor meet minder dan de AI verwachtte.</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Wijs naar de flap-over. Deze drie regels blijven hangen.
</div>

<!--
Eén regel per keer hardop voorlezen.
Wijs naar de flap-over-kapstok met dezelfde drie regels.

Bij MBO-3: niet doorvragen op feature importance.
Bij MBO-4: noem kort Lundberg & Lee (2017).
-->

---

# Voorbeeldgrafiek hardop lezen

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat zie je?

<v-clicks>

- **Trillingssensor** — grote rode balk
- **Temperatuursensor** — middel rode balk
- **Druksensor** — kleine groene balk

</v-clicks>

</div>

<div>

### Wat betekent dat?

<v-clicks>

- Hoofdverdachte: trilling, sterk verhoogd
- Tweede verdachte: temperatuur, ook verhoogd
- Druk: niet verdacht

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-blue-50 rounded-lg text-center">

### Conclusie
Eerst trillingsmotor controleren. Daarna temperatuur.

</div>

<!--
Lees de voorbeeldgrafiek hardop voor — dit is het demonstratiemodel voor fase 4.
Vraag: "Welke sensor zou jij eerst checken?" Vang 1-2 antwoorden.

Houd het bij groot/rood/blauw. Niet uitweiden.
-->

---
layout: quote
---

# SHAP = advies, geen bevel

<div class="text-xl mt-6 opacity-80">
  Het systeem zegt waar de meest verdachte sensor zit.
</div>

<div v-click class="mt-8 text-base opacity-70">
  Maar <span class="font-bold">jij</span> kijkt nog steeds zelf.<br/>
  Klopt het met wat je hoort en voelt?
</div>

<div v-click class="mt-8 text-sm opacity-60">
  Bij conflict: jouw oordeel telt.<br/>
  Schrijf het op voor het team.
</div>

<!--
Belangrijk moment. Maak expliciet:
- SHAP wijst de richting
- Operator vergelijkt met de machine
- Bij conflict: operator wint

Voorkomt blind vertrouwen + voorkomt afwijzing van het systeem.
-->

---
layout: section
---

# Experimenteren

## Drie nieuwe SHAP-grafieken — actie

<!--
Overgang naar blok 4. "Nu zelf — drie nieuwe grafieken."
-->

---

# Drie grafieken — drie acties

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📊</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Grafiek A</div>
  <div class="text-sm opacity-70">Welke sensor controleer je eerst?</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📊</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Grafiek B</div>
  <div class="text-sm opacity-70">Welke sensor controleer je eerst?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📊</div>
  <div class="text-lg font-bold text-green-700 mb-2">Grafiek C</div>
  <div class="text-sm opacity-70">Welke sensor controleer je eerst?</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Minimaal 1 grafiek. Twee is mooi. Drie is bonus.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min individueel · 1.5 min duo · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Timer op 4 min.
Loop rond. Help met de drie leesregels:
- "Welke balk is het grootst?"
- "Welke kleur — rood of blauw?"
- "Wat betekent dat?"

Daarna 1.5 min duo-bespreking, dan 1 min plenair afsluiten.
Kwaliteit boven snelheid.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bij een melding
<v-clicks>

- Vraag aan je leidinggevende:<br/>"Is er een SHAP-grafiek beschikbaar?"
- Bekijk hem samen
- Maak een foto
- Noteer welke sensor bovenaan stond

</v-clicks>

</div>

<div>

### Volgende sessie
<v-clicks>

- We bespreken jouw foto's
- Volgende stap: van anomaliescore naar werkorder
- LO-205 — onderhoudsplanning

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
"Wat je deze week ziet nemen we mee naar de volgende sessie."

LO-108 → LO-205 = van uitleg naar werkorder.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Van anomaliescore naar onderhoud — LO-205</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Wie raadde 4-5 goed in fase 1? Kandidaat voor module 3.
- Bron: Lundberg & Lee (2017). A Unified Approach to Interpreting Model Predictions.
        Molnar (2022). Interpretable Machine Learning.
-->
