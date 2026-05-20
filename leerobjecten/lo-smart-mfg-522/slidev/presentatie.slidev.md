---
theme: default
title: Eigen trainingsdata maken - foto's van jouw producten
info: |
  ## AI-Vision Module 3 — Op Maat
  Workshop over eigen camera-opstelling, consistente foto's en gedeelde labelcriteria.
  Doelgroep: operators MBO-3, 55 minuten, hands-on in teams.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Eigen trainingsdata maken

### Foto's van jouw producten — jouw lijn, jouw data

<div class="mt-12 text-sm opacity-60">
  AI-Vision Module 3 (Op Maat) · Workshop · 55 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · teams van 3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom in Module 3: Op Maat.
In Module 2 leerde je een vision-model gebruiken en trainen.
Vandaag begin je waar het echt om gaat — jouw producten, jouw lijn.

Vandaag bouwen we de fundering: een dataset waarmee je een AI-model
kunt trainen voor je eigen lijn.
-->

---
layout: section
---

# Ervaren

## Bouw zelf een opstelling — maak 20 foto's

<!--
Overgang naar blok 1.
"Geen theorie vooraf. We bouwen, fotograferen, ontdekken."
-->

---
layout: center
class: text-center
---

# Jullie opdracht

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Bouw in teams van 3<br/>
  Maak 20 foto's: helft goed, helft defect<br/>
  Let op: vaste plek, gelijk licht, schone achtergrond
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Je telefoon is goed genoeg. Eenvoud is de kern.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  20 min · team van 3 · wb-01-ervaren
</div>

<!--
Werkblad wb-01. Op tafel: camera, lamp, achtergrond, tape, producten.

Loop langs. Stel coachende vragen:
- "Wat valt je op aan het licht?"
- "Staat het product elke keer op dezelfde plek?"
- "Als je dit morgen herneemt — kun je dat exact zo doen?"

GEEN antwoorden. Ontdekking moet bij hen liggen.
-->

---
layout: section
---

# Reflecteren

## Wat maakt een foto geschikt?

<!--
Overgang naar blok 2.
"Toon je foto's. We kijken naar elkaar's werk en formuleren samen criteria."
-->

---
layout: center
class: text-center
---

# Geschikt voor AI-training?

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Bekijk jullie foto's naast elkaar.<br/>
  Wat valt op?<br/>
  Wat zou een AI-model nodig hebben?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Criteria komen uit jullie eigen ogen — niet uit een lijstje.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · plenair · wb-02-reflecteren + flap-over
</div>

<!--
Vraag elk team 5 foto's te tonen. Laat ze naast elkaar zien.

Kernvraag: "Zijn deze foto's geschikt om een AI-model mee te trainen?"
Tel innerlijk tot 7.

Schrijf criteria die de groep noemt op flap-over.
Bij vage criteria ('ziet er goed uit'): "Wat zou je kunnen meten?"
-->

---
layout: section
---

# Theoretiseren

## De 5 vuistregels + de spuitgieter-casus

<!--
Overgang naar blok 3.
"Jullie hebben het zelf al ontdekt. Ik zet het op een rij."
-->

---

# Vijf vuistregels — niet meer

<div class="grid grid-cols-5 gap-3 mt-8">

<div class="p-3 bg-purple-50 rounded-xl border-2 border-purple-200 text-center">
  <div class="text-2xl mb-2">📍</div>
  <div class="text-sm font-bold text-purple-700 mb-1">1. Vast standpunt</div>
  <div class="text-xs opacity-80">Markeer met tape</div>
</div>

<div class="p-3 bg-amber-50 rounded-xl border-2 border-amber-200 text-center">
  <div class="text-2xl mb-2">💡</div>
  <div class="text-sm font-bold text-amber-700 mb-1">2. Gelijk licht</div>
  <div class="text-xs opacity-80">Geen direct zonlicht</div>
</div>

<div class="p-3 bg-blue-50 rounded-xl border-2 border-blue-200 text-center">
  <div class="text-2xl mb-2">🎨</div>
  <div class="text-sm font-bold text-blue-700 mb-1">3. Schone achtergrond</div>
  <div class="text-xs opacity-80">Geen rommel</div>
</div>

<div class="p-3 bg-green-50 rounded-xl border-2 border-green-200 text-center">
  <div class="text-2xl mb-2">📸</div>
  <div class="text-sm font-bold text-green-700 mb-1">4. Genoeg foto's</div>
  <div class="text-xs opacity-80">Min. 50 per categorie</div>
</div>

<div class="p-3 bg-rose-50 rounded-xl border-2 border-rose-200 text-center">
  <div class="text-2xl mb-2">🏷️</div>
  <div class="text-sm font-bold text-rose-700 mb-1">5. Labelafspraken</div>
  <div class="text-xs opacity-80">Meetbaar, eenduidig</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Jullie hebben de meeste van deze regels zelf al genoemd.
</div>

<!--
Verwijs naar flap-over: "Jullie noemden net..."

Loop de 5 langs. Niet meer dan 3 minuten.
-->

---

# Spuitgieter-casus

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-xl font-bold text-blue-700 mb-3">Wat hadden ze?</div>
  <ul class="text-sm space-y-2">
    <li>3 operators bij kunststofverwerker</li>
    <li>Tafel + witte achtergrond</li>
    <li>2 TL-lampen</li>
    <li>Telefoon op statief</li>
  </ul>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-300">
  <div class="text-xl font-bold text-green-700 mb-3">Wat deden ze?</div>
  <ul class="text-sm space-y-2">
    <li>Afspraak: kras &gt; 2mm = defect</li>
    <li>3 dagen werk</li>
    <li>300 foto's: 150 goed, 150 defect</li>
    <li>60 krassen, 50 vloeisporen, 40 inzinkingen</li>
  </ul>
</div>

</div>

<div v-click class="mt-6 text-center text-base font-bold opacity-80">
  Geen dure apparatuur. Heldere afspraken. Bruikbare dataset.
</div>

<!--
Vertel de casus stap voor stap.

Inzicht expliciet benoemen:
"Eenvoudige opstelling + heldere afspraken = bruikbare dataset."
-->

---
layout: section
---

# Experimenteren

## Labelcriteria + actieplan voor jouw lijn

<!--
Overgang naar blok 4.
"Nu het concreet: drie criteria, één plan, één peer-check."
-->

---

# Drie taken voor je team

<div class="grid grid-cols-3 gap-6 mt-6">

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-3xl mb-2">📏</div>
  <div class="text-lg font-bold text-purple-700 mb-2">1. Labelcriteria</div>
  <div class="text-sm opacity-70">Minstens 3 — meetbaar (mm, kleur, zichtbaar op 30cm)</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl">
  <div class="text-3xl mb-2">📅</div>
  <div class="text-lg font-bold text-amber-700 mb-2">2. Actieplan</div>
  <div class="text-sm opacity-70">Wie + wanneer + hoeveel + welke shift</div>
</div>

<div class="p-5 bg-green-50 rounded-xl">
  <div class="text-3xl mb-2">👥</div>
  <div class="text-lg font-bold text-green-700 mb-2">3. Peer-check</div>
  <div class="text-sm opacity-70">Welke collega? Wanneer? Hoeveel labels?</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Concreet plan = uitvoerbaar plan.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  15 min · team + plenair · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Drie taken.

8 min team-werk, dan 5 min plenaire deel-ronde (1.5 min per team).

Concreet maken is de competentie.
"Wie, wanneer, hoeveel" — terugsturen tot het er staat.
-->

---

# Komende week + volgende sessie

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Komende week

<v-clicks>

- Voer je actieplan uit
- 50+ foto's met jullie opstelling
- Label samen — gebruik je eigen criteria
- Collega die er niet bij was 10 labels laten geven (peer-check)

</v-clicks>

</div>

<div>

### Volgende sessie

<v-clicks>

- LO-523: eigen model trainen
- Neem je gelabelde dataset mee
- Vergelijk je opstelling met andere teams

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende sessie: LO-523 — eigen model trainen met eigen data.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende sessie: <span class="font-bold">Eigen model trainen — LO-523</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Vision Module 3 (Op Maat)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.
Foto van flap-over (criteria-lijst) — input voor LO-523.

Notitie:
- Welke teams hadden moeite met meetbare criteria?
- Bron: Rožanec et al. (2024); Ng (2021) Data-centric AI.
-->
