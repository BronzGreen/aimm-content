---
theme: default
title: Sensordata interpreteren met SHAP
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over het 5-stappenplan voor SHAP-grafieken bij anomaliemeldingen.
  Doelgroep: operators MBO-3, 25 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Sensordata interpreteren met SHAP

### Hoe lees je een SHAP-grafiek bij een anomaliemelding?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 25 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · CNC / freesbank / spuitgieten
</div>

<!--
Welkom. De komende 25 minuten leer je een SHAP-grafiek lezen.
Tegen het eind weet je in 5 stappen waar je moet beginnen met zoeken.

Trigger: "Wat doe jij nu als er een anomaliemelding komt?"
Vang 1-2 reacties. Reageer alleen met "herkenbaar".
-->

---
layout: center
class: text-center
---

# Storingsquiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  3 SHAP-grafieken.<br/>
  Welke sensor draagt het meest bij?<br/>
  Wat is je eerste actie?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Werk alleen. Je mag fouten maken.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01 uitdelen. Zet timer op 5 min.
Loop rustig rond. Geen sturende vragen.

Bij vastlopen: "Welke sensor staat bovenaan? Wat zegt het percentage?"
Niet voorzeggen.
-->

---
layout: section
---

# Reflecteren

## Waar verschilden jullie het meest?

<!--
Overgang naar blok 2.
"Vergelijk in duo's. Het verschil is de leerwinst."
-->

---
layout: center
class: text-center
---

# Vergelijk in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">📊</div>
    <div class="text-lg font-bold text-blue-700">Welke top-1?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">🔗</div>
    <div class="text-lg font-bold text-purple-700">Welke samen?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">🎯</div>
    <div class="text-lg font-bold text-green-700">Welke actie?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  SHAP geeft de getallen. Jij geeft de richting.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min · in duo's · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 4 min.
Loop rond. Verzamel sterke voorbeelden.

Plenair daarna 2 min:
- "Bij welke casus verschilden jullie het meest?"
- "Welke sensoren horen bij elkaar?"

Schrijf 3-4 sleutelwoorden op flap-over (spilsysteem, koelsysteem).
-->

---
layout: section
---

# Theoretiseren

## Het 5-stappenplan

<!--
Overgang naar blok 3.
"Nu krijgen we de kapstok: 5 stappen die altijd werken."
-->

---

# Het 5-stappenplan

<div class="grid grid-cols-5 gap-3 mt-8">

<div class="p-4 bg-blue-50 rounded-xl border-2 border-blue-200 text-center">
  <div class="text-3xl mb-2">📖</div>
  <div class="text-sm font-bold text-blue-700">1. Lees</div>
  <div class="text-xs opacity-70 mt-1">Top-1 sensor?</div>
</div>

<div class="p-4 bg-purple-50 rounded-xl border-2 border-purple-200 text-center">
  <div class="text-3xl mb-2">🔗</div>
  <div class="text-sm font-bold text-purple-700">2. Groepeer</div>
  <div class="text-xs opacity-70 mt-1">Welk systeem?</div>
</div>

<div class="p-4 bg-amber-50 rounded-xl border-2 border-amber-200 text-center">
  <div class="text-3xl mb-2">↕️</div>
  <div class="text-sm font-bold text-amber-700">3. Richting</div>
  <div class="text-xs opacity-70 mt-1">Te hoog/laag?</div>
</div>

<div class="p-4 bg-green-50 rounded-xl border-2 border-green-200 text-center">
  <div class="text-3xl mb-2">🎯</div>
  <div class="text-sm font-bold text-green-700">4. Oorzaak</div>
  <div class="text-xs opacity-70 mt-1">Vuistregel</div>
</div>

<div class="p-4 bg-rose-50 rounded-xl border-2 border-rose-200 text-center">
  <div class="text-3xl mb-2">⚡</div>
  <div class="text-sm font-bold text-rose-700">5. Actie</div>
  <div class="text-xs opacity-70 mt-1">Check / meld</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Vijf stappen — werkt voor élke SHAP-grafiek.
</div>

<!--
Loop de 5 stappen rustig langs.
Wijs naar de flap-over-kapstok.

Niet meer dan deze 5 stappen in de eerste 3 min.
Bij vraag over Shapley values: parkeer.
-->

---

# Vuistregeltabel — voorbeeld casus 1

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-xl font-bold text-amber-700 mb-3">SHAP-output</div>
  <ul class="text-sm space-y-1">
    <li>Spiltemperatuur 55% — te hoog</li>
    <li>Trillingen Y-as 25% — te hoog</li>
    <li>Koelmiddelniveau 12% — te laag</li>
    <li>Voedingssnelheid 8% — normaal</li>
  </ul>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-300">
  <div class="text-xl font-bold text-green-700 mb-3">Stap 2 + 4 + 5</div>
  <div class="text-sm space-y-2">
    <div><strong>Groep:</strong> spilsysteem (temp + trilling)</div>
    <div><strong>Vuistregel:</strong> koeling check + lager toerental</div>
    <div><strong>Actie:</strong> melden bij teamleider, niet zelf draaien</div>
  </div>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Het stappenplan vervangt het "ik kijk maar wat".
</div>

<!--
Verwijs naar wb-03 (handout). Markeerstift gebruiken.
Casus 1 als voorbeeld — niet wisselen.

Voor MBO-4: "feature attribution" parkeren voor LO-207.
-->

---
layout: section
---

# Experimenteren

## Wat doe jij bij de eerstvolgende melding?

<!--
Overgang naar blok 4.
"De afgelopen 20 minuten was de oefening. Nu wordt het concreet voor jouw machine."
-->

---

# Actieplan — drie vragen

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-4xl mb-3">🏭</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Welke machine?</div>
  <div class="text-sm opacity-70">Wees specifiek — geen 'alle machines'</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-4xl mb-3">🔍</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Welke sensor vaak?</div>
  <div class="text-sm opacity-70">Spil, koeling, voeding, druk?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-4xl mb-3">⚡</div>
  <div class="text-lg font-bold text-green-700 mb-2">Eerste actie?</div>
  <div class="text-sm opacity-70">Check, melden, of ingrijpen?</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Concreet maken is de oefening.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  3 min · individueel · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 3 min.
Help concretiseren met doorvragen:
- "Welke sensor zit er meestal achter een storing?"

Plenair daarna 1 min: 2 deelnemers delen kort (max 30 sec).
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bij de eerstvolgende melding
<v-clicks>

- Open de SHAP-grafiek
- Loop de 5 stappen langs
- Noteer je bevinding in de werkorder

</v-clicks>

</div>

<div>

### Hang op
<v-clicks>

- Print de vuistregeltabel uit wb-03
- Hang hem bij je werkplek
- Bewaar het stappenplan

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: LO-207 — zelf grenswaarden bepalen.

"Wat je deze week ontdekt nemen we mee naar de volgende sessie."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Zelf grenswaarden bepalen — LO-207</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke sensoren werden genoemd? (input voor LO-207)
- Wie was sceptisch? (1-op-1-aandacht)
- Bron: Lundberg & Lee (2017). SHAP. Cruz et al. (2024).
-->
