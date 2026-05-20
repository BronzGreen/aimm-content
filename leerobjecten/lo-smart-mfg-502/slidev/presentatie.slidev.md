---
theme: default
title: Eigen productiedata verzamelen en beoordelen
info: |
  ## Predictive Maintenance Module 3 — Op Maat
  Workshop-blok over de data-audit op de eigen machine.
  Doelgroep: operators MBO-3, 55 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Eigen productiedata verzamelen en beoordelen

### Heb ik genoeg goede data om een PM-pilot te starten?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 3 (Op Maat) · Workshop-blok · 55 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Module 3 begint nu echt voor jou.
We gaan van voorbeelddata naar JOUW machine.

Trigger: "Hoeveel sensoren denk je dat er op jouw machine zitten?"
Vang 2-3 ruwe schattingen. Schrijf op flap-over.
-->

---
layout: center
class: text-center
---

# Verken jouw machine

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Welke sensoren zitten erop?<br/>
  Werken ze allemaal?<br/>
  Wordt de data opgeslagen?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Wat je weet is een goed begin.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  12 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01 uitdelen. Zet timer op 12 min.
Loop rustig rond. Geen voorzeggers.

Coachende vragen:
- "Weet je zeker dat er geen sensoren in de PLC zitten?"
- "Heb je de technische dienst al gevraagd?"
-->

---
layout: section
---

# Reflecteren

## Wat viel op?

<!--
Overgang naar blok 2.
"Vergelijk met je buurman. Wat is hetzelfde? Wat anders?"
-->

---
layout: center
class: text-center
---

# Vergelijk in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">📋</div>
    <div class="text-lg font-bold text-blue-700">Wat ontdekte je?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">⚖️</div>
    <div class="text-lg font-bold text-purple-700">Wat hetzelfde, wat anders?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">💡</div>
    <div class="text-lg font-bold text-green-700">Tips voor elkaar?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Wat ik niet weet, weet hij misschien wel.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · in duo's · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 10 min.
Loop rond. Verzamel 2-3 sterke voorbeelden voor plenair.

Plenair daarna 3 min: 2 duo's delen hun ontdekking.
Vat samen op flap-over: 3-4 sleutelwoorden.
-->

---
layout: section
---

# Theoretiseren

## Vier criteria voor goede data

<!--
Overgang naar blok 3.
"Nu krijgen we de kapstok: vier dingen die data goed maken."
-->

---

# Vier criteria voor datakwaliteit

<div class="grid grid-cols-2 gap-4 mt-6">

<div class="p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-2xl mb-2">📅</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Volledigheid</div>
  <div class="text-sm opacity-80">Geen gaten. Elke 5 min meten = 288 metingen per dag.</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-2xl mb-2">🔄</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Consistentie</div>
  <div class="text-sm opacity-80">Eenheden en formaten kloppen. Altijd °C, niet soms °F.</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-2xl mb-2">🎯</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Nauwkeurigheid</div>
  <div class="text-sm opacity-80">Sensor is gekalibreerd, meting klopt met werkelijkheid.</div>
</div>

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-2xl mb-2">⏰</div>
  <div class="text-lg font-bold text-green-700 mb-2">Tijdstempel</div>
  <div class="text-sm opacity-80">PLC-tijd, sensor-tijd, ERP-tijd op elkaar afgestemd.</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Vier criteria — werkt voor élke sensor.
</div>

<!--
Loop de 4 criteria langs met telkens hetzelfde fabrieksvoorbeeld.
Wijs naar de flap-over.

Niet uitweiden — visueel + voorbeeld is genoeg.
-->

---

# Hoe scoort jouw machine?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Kijk terug naar je werkblad

<v-clicks>

- Welk criterium scoort goed?
- Welk criterium scoort slecht?
- Wat verraste je?

</v-clicks>

</div>

<div>

### Voor een PM-pilot heb je nodig

<v-clicks>

- Minimaal 3 maanden historie (liever 6)
- Frequentie hoog genoeg (vaak 1 per minuut)
- Sensoren rond de faaltype

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-blue-50 rounded-lg text-center">
  Een pilot zonder data-audit = experiment met onbekende grondstof.
</div>

<!--
Vraag: "Kijk naar je eigen scores. Waar scoor je goed? Waar niet?"
Vang 2-3 reacties.

Voor MBO-4: "data drift" parkeren voor LO-504.
-->

---
layout: section
---

# Experimenteren

## Wat heb ik nog nodig?

<!--
Overgang naar blok 4.
"Nu wordt het concreet. Welke actie deze week?"
-->

---

# Actieplan — vier vragen

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-5 bg-blue-50 rounded-xl">
  <div class="text-3xl mb-2">❓</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Wat ontbreekt?</div>
  <div class="text-sm opacity-70">Welke specifieke sensor of welke periode?</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl mb-2">👥</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Wie kan helpen?</div>
  <div class="text-sm opacity-70">Naam — geen 'IT' of 'technische dienst'</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl">
  <div class="text-3xl mb-2">📅</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Wanneer?</div>
  <div class="text-sm opacity-70">Datum deze week</div>
</div>

<div class="p-5 bg-green-50 rounded-xl">
  <div class="text-3xl mb-2">✅</div>
  <div class="text-lg font-bold text-green-700 mb-2">Hoe weet je dat het klaar is?</div>
  <div class="text-sm opacity-70">Concreet eindresultaat</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Vaag plan = leeg plan.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min individueel + 3 min duo · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 10 min.
Loop rond. Help concretiseren met doorvragen.

Daarna 3 min duo-feedback: "Is het plan haalbaar? Mist er iets?"
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Ga langs je machine

<v-clicks>

- Check of je scoringsformulier klopt
- Praat met de technische dienst
- Vraag welke data wordt opgeslagen

</v-clicks>

</div>

<div>

### Vul aan en plan

<v-clicks>

- Vul je actieplan aan met wat je leert
- Vraag je teamleider om een sensor-overzicht
- Neem alles mee naar LO-504

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: LO-504 — van pilot naar productie.
"De data-audit van vandaag is het startpunt voor je pilotplan."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Van pilot naar productie — LO-504</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 3 (Op Maat)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke sensoren werden genoemd? (input voor LO-504)
- Wie was sceptisch? (1-op-1)
- Bron: Cruz et al. (2024). AI in Manufacturing.
-->
