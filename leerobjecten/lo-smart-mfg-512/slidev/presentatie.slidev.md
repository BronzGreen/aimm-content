---
theme: default
title: Vision-model configureren - parameters instellen
info: |
  ## AI-Vision Module 2 — Train
  Workshop-blok over de drempelwaarde en de afweging tussen recall en valse alarmen.
  Doelgroep: operators MBO-3, 30 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Vision-model configureren

### Hoe stel je de gevoeligheid juist af voor jouw lijn?

<div class="mt-12 text-sm opacity-60">
  AI-Vision Module 2 (Train) · Workshop-blok · 30 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 30 minuten leer je een vision-model afstellen.
Je gaat zelf aan de knoppen draaien.

Trigger: "Stel je voor: AI-camera zegt 'afkeuren' op 1 op 5 producten. Wat denk je?"
Vang reactie. "Vandaag leer je waarom dat gebeurt en wat je eraan doet."
-->

---
layout: center
class: text-center
---

# Drempelwaarde-quiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Schuif de drempelwaarde.<br/>
  Kijk wat er gebeurt.<br/>
  Welke past bij jouw lijn?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Er is geen juiste keuze. Wel een passende.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · simulator + wb-01-ervaren
</div>

<!--
Werkblad wb-01 + simulator (model-lo-smart-mfg-512.html). Zet timer op 6 min.
Loop rond. Bij 'welke is de juiste?' — schud je hoofd.
"Wat is voor jullie erger: weggooien of doorlaten?"
-->

---
layout: section
---

# Reflecteren

## Wat is bij jullie erger?

<!--
Overgang naar blok 2.
"Vergelijk je keuze. Het verschil zit in de context."
-->

---
layout: center
class: text-center
---

# De afweging

<div class="grid grid-cols-2 gap-8 mt-10">
  <div class="p-8 bg-rose-50 rounded-xl border-2 border-rose-200">
    <div class="text-5xl mb-3">⛔</div>
    <div class="text-xl font-bold text-rose-700 mb-2">Streng</div>
    <div class="text-sm opacity-80">Vangt bijna alle defecten<br/>Veel valse alarmen</div>
    <div class="text-xs opacity-60 mt-2">Voedingsmiddelen, medisch, veiligheid</div>
  </div>
  <div class="p-8 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-5xl mb-3">🟢</div>
    <div class="text-xl font-bold text-blue-700 mb-2">Soepel</div>
    <div class="text-sm opacity-80">Weinig productieverstoring<br/>Defecten kunnen door</div>
    <div class="text-xs opacity-60 mt-2">Cosmetisch, niet-veiligheidskritiek</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto text-center">
  Geen gratis lunch. Kies wat erger is.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · in duo's · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 5 min.
Loop rond. Stel verdiepende vragen.

Plenair daarna 2 min: vraag "Wat is bij jullie erger?"
Schrijf 2 voorbeelden op flap-over.
-->

---
layout: section
---

# Theoretiseren

## Recall, valse alarmen, testset

<!--
Overgang naar blok 3.
"Twee getallen helpen om de afweging meetbaar te maken."
-->

---

# Twee getallen + één testset

<div class="grid grid-cols-3 gap-4 mt-8">

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-3xl mb-2">🎯</div>
  <div class="text-lg font-bold text-green-700 mb-2">Recall</div>
  <div class="text-sm opacity-80 mb-2">Hoeveel échte defecten vindt het model?</div>
  <div class="text-xs opacity-60">9 op 10 = 90%</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-3xl mb-2">🔔</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Valse alarmen</div>
  <div class="text-sm opacity-80 mb-2">Hoe vaak schreeuwt model op goed product?</div>
  <div class="text-xs opacity-60">5 op 100 = 5%</div>
</div>

<div class="p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-3xl mb-2">📸</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Testset</div>
  <div class="text-sm opacity-80 mb-2">50-100 foto's met bekende uitkomst</div>
  <div class="text-xs opacity-60">Helft goed, helft defect</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Twee getallen meet je met één testset.
</div>

<!--
Loop de drie begrippen langs.
Tempo strak: 3 min voor uitleg.

Voor MBO-4: parkeer "precision" voor LO-513.
-->

---

# Streng of soepel — wat doet het?

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-rose-50 rounded-xl border-2 border-rose-200">
  <div class="text-xl font-bold text-rose-700 mb-3">Streng</div>
  <ul class="text-sm space-y-1">
    <li>Recall: <strong>hoog</strong> (95%+)</li>
    <li>Valse alarmen: <strong>hoog</strong> (10-20%)</li>
    <li>Resultaat: meer goede producten op afkeur</li>
  </ul>
</div>

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-300">
  <div class="text-xl font-bold text-blue-700 mb-3">Soepel</div>
  <ul class="text-sm space-y-1">
    <li>Recall: <strong>lager</strong> (70-85%)</li>
    <li>Valse alarmen: <strong>laag</strong> (1-5%)</li>
    <li>Resultaat: minder afkeur, defecten kunnen door</li>
  </ul>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Vuistregel: begin in het midden, test met 50 foto's, schuif op basis van wat erger is.
</div>

<!--
Verwijs naar wb-03 (handout). Markeerstiften gebruiken.

Niet ROC-curve, niet F1. Voor MBO-4: kort precision noemen, parkeren.
-->

---
layout: section
---

# Experimenteren

## Jouw product, jouw drempelwaarde

<!--
Overgang naar blok 4.
"Nu wordt het concreet voor jouw lijn."
-->

---

# Actieplan — vier vragen

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-5 bg-blue-50 rounded-xl">
  <div class="text-3xl mb-2">📦</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Welk product?</div>
  <div class="text-sm opacity-70">Specifiek + welk defecttype</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl mb-2">🎚️</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Welke drempelwaarde?</div>
  <div class="text-sm opacity-70">Streng of soepel? Waarom?</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl">
  <div class="text-3xl mb-2">📸</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Welke testset?</div>
  <div class="text-sm opacity-70">50 foto's, helft goed, helft defect</div>
</div>

<div class="p-5 bg-green-50 rounded-xl">
  <div class="text-3xl mb-2">👥</div>
  <div class="text-lg font-bold text-green-700 mb-2">Welke buddy?</div>
  <div class="text-sm opacity-70">Naam — geen 'collega'</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Concreet plan = uitvoerbaar plan.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min individueel + 2 min plenair · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 4 min.
Help concretiseren met doorvragen.

Plenair: 2 deelnemers delen (max 1 min). Zoek contrast: 1 streng, 1 soepel.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bespreek + bouw

<v-clicks>

- Bespreek met leidinggevende welke drempelwaarde
- Maak een testset van 50 foto's
- Vraag een collega om mee te beoordelen

</v-clicks>

</div>

<div>

### Bewaar

<v-clicks>

- Print de handout uit wb-03
- Hang hem op bij je vision-systeem
- Neem testresultaten mee naar LO-513

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende sessie: LO-513 — confusion matrix interpreteren.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende sessie: <span class="font-bold">Confusion matrix interpreteren — LO-513</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Vision Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Streng/soepel-balans van de groep?
- Wie zei "is voor IT"? (1-op-1)
- Bron: Cruz et al. (2024).
-->
