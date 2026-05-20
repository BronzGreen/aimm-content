---
theme: default
title: AI voor visuele kwaliteitsinspectie bij spuitgieten
info: |
  ## AI-Kwaliteitscontrole Module 1 — Gebruik
  Workshop-blok over AI-visuele inspectie bij spuitgieten en de rol van de operator.
  Doelgroep: spuitgiet-operators MBO-3, 35 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# AI bij spuitgieten

### Hoe werkt visuele inspectie — en wat is jouw rol?

<div class="mt-12 text-sm opacity-60">
  AI-Kwaliteitscontrole Module 1 (Gebruik) · Workshop-blok · 35 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Spuitgiet-operators MBO-3 · vervolg op LO-006 + LO-010
</div>

<!--
"De komende 35 minuten kijken we naar AI-kwaliteitscontrole bij spuitgieten — jouw werkplek."

Trigger: "Welke defecten kom je het meeste tegen op je lijn?"
Vang 3-4 reacties. Schrijf op flap-over.
-->

---
layout: center
class: text-center
---

# Storingsquiz — spuitgietproducten

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  6 foto's. Goed of afgekeurd?<br/>
  Welk defect zie je?
</div>

<div v-click class="mt-10 grid grid-cols-3 gap-3 text-sm max-w-2xl mx-auto">
  <div class="p-3 bg-amber-50 rounded">Braamvorming</div>
  <div class="p-3 bg-amber-50 rounded">Kleurverschil</div>
  <div class="p-3 bg-amber-50 rounded">Krimp / vervorming</div>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5.5 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01 uitdelen. Toon de 6 foto's.
Zet timer op 5.5 min. Loop rond.

Bij snel klaar: "Bij welke foto twijfelde je het langst?"

Quick-feedback (1.5 min): per foto kort vragen, 1-2 antwoorden.
-->

---
layout: section
---

# Mens versus AI

## Wat doet wie het beste?

<!--
Overgang naar blok 2 — gevoelig moment.
Banen-angst zit hier hoger dan bij andere LO's. Eerlijk over zijn.
-->

---

# Drie vragen — bespreek met je buurman

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-4xl mb-3">🤖</div>
  <div class="text-base font-bold text-blue-700">Wat kan AI beter dan jij?</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-4xl mb-3">👤</div>
  <div class="text-base font-bold text-purple-700">Wat kun jij beter dan AI?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-4xl mb-3">🔑</div>
  <div class="text-base font-bold text-green-700">Waarom blijft de operator belangrijk?</div>
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min duo · 5 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 4 min duo.
Loop rond. Luister naar concrete antwoorden.

Plenair daarna: bouw twee-kolommen-lijst op flap-over op.
-->

---

# AI doet — Mens doet

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="p-6 bg-blue-50 rounded-xl">
  <div class="text-xl font-bold text-blue-700 mb-4">AI doet</div>
  <ul class="text-base space-y-2">
    <li>Snelheid (miljoenen producten)</li>
    <li>Consistentie (geen vermoeidheid)</li>
    <li>Routine-defecten herkennen</li>
    <li>24/7 inspectie</li>
  </ul>
</div>

<div class="p-6 bg-purple-50 rounded-xl">
  <div class="text-xl font-bold text-purple-700 mb-4">Mens doet</div>
  <ul class="text-base space-y-2">
    <li>Twijfelgevallen beoordelen</li>
    <li>Nieuwe defecten herkennen</li>
    <li>Oorzaak achterhalen</li>
    <li>Het AI-model bijstellen</li>
  </ul>
</div>

</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg text-center text-base">
  Bij meerdere spuitgieters in onze regio is dit de praktijk.<br/>
  De rol verandert. Verdwijnt niet.
</div>

<!--
Erken de banen-angst direct. "Bij meerdere spuitgieters in onze regio is dit de praktijk."
Defensief worden = vertrouwen kwijt.

Bouw lijst van wat de groep zegt. Vooraf-gemaakte slide is voorbeeld — vul aan.
-->

---
layout: section
---

# Hoe werkt het?

## Drie hoofdblokken — zes stappen

<!--
Overgang naar blok 3.
"Vóór we naar 6 stappen gaan, eerst drie hoofdblokken."
-->

---

# Drie hoofdblokken

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-4xl mb-3">🎓</div>
  <div class="text-lg font-bold text-blue-700 mb-2">1. Data + training</div>
  <div class="text-sm opacity-80">EENMALIG — voor de productie begint</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-4xl mb-3">🔍</div>
  <div class="text-lg font-bold text-purple-700 mb-2">2. Inspectie</div>
  <div class="text-sm opacity-80">CONTINU — tijdens productie, miljoenen keren</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-4xl mb-3">🔄</div>
  <div class="text-lg font-bold text-green-700 mb-2">3. Feedback</div>
  <div class="text-sm opacity-80">DOORLOPEND — operator verbetert het model</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Drie hoofdblokken — elk met 2 substappen — samen 6 stappen.
</div>

<!--
Eerst de drie blokken landen voordat je 6 stappen detailleert.
-->

---

# Blok 1: Data + training (eenmalig)

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="p-6 bg-blue-50 rounded-xl">
  <div class="text-3xl font-bold text-blue-700 mb-3">Stap 1</div>
  <div class="text-lg font-bold mb-2">Verzamel beelden</div>
  <div class="text-sm opacity-80">Goede én defecte producten — goede zijn er veel, defecte weinig</div>
</div>

<div class="p-6 bg-blue-50 rounded-xl">
  <div class="text-3xl font-bold text-blue-700 mb-3">Stap 2</div>
  <div class="text-lg font-bold mb-2">Train het AI-model</div>
  <div class="text-sm opacity-80">Het model leert op basis van die beelden wat goed is en wat niet</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Eenmalig werk — voordat de productielijn begint.
</div>

<!--
Houd het concreet. Vermijd termen als 'neural network', 'epochs', 'loss function'.
-->

---

# Blok 2: Inspectie tijdens productie (continu)

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl font-bold text-purple-700 mb-2">Stap 3</div>
  <div class="text-base font-bold mb-1">Camera fotografeert</div>
  <div class="text-xs opacity-80">Elk product apart</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl font-bold text-purple-700 mb-2">Stap 4</div>
  <div class="text-base font-bold mb-1">AI beoordeelt</div>
  <div class="text-xs opacity-80">Goed, twijfel, of defect</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl font-bold text-purple-700 mb-2">Stap 5</div>
  <div class="text-base font-bold mb-1">Beslissing</div>
  <div class="text-xs opacity-80">Door, terug, of weg</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Miljoenen producten per maand — zonder pauze.
</div>

<!--
Nu komen de drie stappen die continu draaien tijdens productie.
-->

---

# Blok 3: Feedback (doorlopend)

<div class="mt-8 p-8 bg-green-50 rounded-xl text-center">
  <div class="text-3xl font-bold text-green-700 mb-3">Stap 6</div>
  <div class="text-2xl font-bold mb-3">De operator corrigeert</div>
  <div class="text-base opacity-80">
    Bij twijfelgevallen en nieuwe defecten —<br/>
    het AI-model wordt bijgewerkt op basis van jouw correcties
  </div>
</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg text-center">
  Zonder jouw feedback wordt het AI-model langzaam slechter —<br/>
  bij nieuwe materialen, nieuwe defecten.
</div>

<!--
Stap 6 is voor MBO-3 het belangrijkste — rol-bevestiging.
"Zonder jouw feedback wordt het model langzaam slechter."

Bij vraag 'kunnen wij het model bijwerken?': bevestig + verwijs naar module 2.
-->

---
layout: center
class: text-center
---

# De cyclus

<div class="text-base opacity-70 mt-4">
  Drie hoofdblokken — zes stappen — één doorlopend proces
</div>

<div class="mt-12 flex justify-center items-center gap-3 text-sm">
  <div class="p-3 bg-blue-100 rounded">1. Data</div>
  <div>→</div>
  <div class="p-3 bg-blue-100 rounded">2. Train</div>
  <div>→</div>
  <div class="p-3 bg-purple-100 rounded">3. Foto</div>
  <div>→</div>
  <div class="p-3 bg-purple-100 rounded">4. Oordeel</div>
  <div>→</div>
  <div class="p-3 bg-purple-100 rounded">5. Beslissing</div>
</div>

<div class="mt-6 flex justify-center items-center gap-3">
  <div class="p-3 bg-green-100 rounded text-sm">6. Operator-feedback</div>
  <div class="text-2xl">↻</div>
  <div class="text-sm opacity-70">terug naar de training</div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Markeer in je handout: welke stap is voor JOUW rol het belangrijkst?
</div>

<!--
Cyclus-diagram. Verbinden met de handout.
-->

---
layout: section
---

# Experimenteren

## Waar zou dit op jouw lijn werken?

<!--
Overgang naar blok 4.
-->

---

# Actieplan — drie vragen

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📦</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Welk product?</div>
  <div class="text-sm opacity-70">Wees specifiek</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-4xl mb-3">🔍</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Welk defect?</div>
  <div class="text-sm opacity-70">Braam, kleur, krimp, anders?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-4xl mb-3">👤</div>
  <div class="text-lg font-bold text-green-700 mb-2">Wat is JOUW rol?</div>
  <div class="text-sm opacity-70">Bij welke twijfel zou jouw oog nodig zijn?</div>
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  3.5 min individueel · 2.5 min plenair · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 3.5 min individueel.
Loop rond. Help concretiseren:
- "Welk specifiek product?"
- "Welk defect zoek je nu met je ogen?"
- "Bij welke twijfel zou jouw oog nodig zijn?"

Plenair daarna 2.5 min: 3-4 deelnemers delen kort.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Ga kijken
<v-clicks>

- Sta bij een collega-spuitgieter op de lijn
- Welk defect kwam vaak voor?
- Zou een camera dit kunnen zien?
- Wat zou jouw rol erbij zijn?

</v-clicks>

</div>

<div>

### Vraag rond
<v-clicks>

- Vraag een collega: wat denk jij van AI-inspectie?
- Vraag de teamleider: hebben we al een proefopstelling?
- Schrijf antwoorden op voor de volgende sessie

</v-clicks>

</div>

</div>

<div v-click class="mt-10 p-4 bg-blue-50 rounded-lg text-center">
  Volgende: <span class="font-bold">Module 2 (Train) — autoencoder LO-093</span>
</div>

<!--
Sluit af met de transferopdracht.
"Module 2 gaat over zelf trainen. Eerste LO daar: autoencoder."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Autoencoder — AI leert wat normaal is — LO-093</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Kwaliteitscontrole Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Welke defecten werden genoemd? (input voor module 2)
- Wie was sceptisch? (1-op-1)
- Wie noemde een specifieke operator-rol? (good practice voor volgend cohort)
-->
