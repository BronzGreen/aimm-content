---
theme: default
title: Het model verbeteren - meer data, betere labels
info: |
  ## AI-Vision Module 2 — Train
  Workshop-blok over iteratieve modelverbetering: foutenanalyse, gerichte data, peer-gecheckte labels.
  Doelgroep: operators MBO-3/4, 60 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Het model verbeteren

### Meer data, betere labels — itereren zonder leverancier

<div class="mt-12 text-sm opacity-60">
  AI-Vision Module 2 (Train) · Workshop-blok · 60 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3/4 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 60 minuten leer je hoe je een werkend vision-model
zelf beter maakt.

Trigger: "Wie van jullie heeft het idee 'ons model werkt wel, maar mist soms iets'?"
Vang reacties. "Dat 'iets' is wat we vandaag aanpakken — heel specifiek per categorie."
-->

---
layout: section
---

# Ervaren

## Waar gaat je model nog mis?

<!--
Overgang naar blok 1.
"We beginnen niet met theorie. We beginnen met je eigen confusion matrix."
-->

---
layout: center
class: text-center
---

# Foutenanalyse

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Lees je confusion matrix.<br/>
  Vind 2 categorieën met recall onder 80%.<br/>
  Schrijf op: wat pakt het model wel, wat mist het?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  De zwakste categorie is je hefboom.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-01-ervaren + dashboard
</div>

<!--
Werkblad wb-01 + eigen dashboard of model-lo-smart-mfg-514.html.
Zet timer op 8 min. Loop rond.

Geen voorzeggers — laat ze de matrix zelf lezen.
Bij vragen: "Welke rij heeft het laagste percentage rechts onder?"
-->

---
layout: section
---

# Reflecteren

## Waarom faalt het model juist daar?

<!--
Overgang naar blok 2.
"Een laag getal is geen toeval. Er zit een oorzaak achter."
-->

---

# Drie hypothesen

<div class="grid grid-cols-3 gap-4 mt-8">

<div class="p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-3xl mb-2">📉</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Data-tekort</div>
  <div class="text-sm opacity-80">Te weinig foto's van deze categorie in de oorspronkelijke set</div>
</div>

<div class="p-5 bg-rose-50 rounded-xl border-2 border-rose-200">
  <div class="text-3xl mb-2">🏷️</div>
  <div class="text-lg font-bold text-rose-700 mb-2">Label-fouten</div>
  <div class="text-sm opacity-80">Inconsistent gelabeld — verschillende mensen, verschillende criteria</div>
</div>

<div class="p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-3xl mb-2">🆕</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Nieuw defect</div>
  <div class="text-sm opacity-80">Type defect dat niet in de oorspronkelijke trainingsset zat</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Welke hypothese past bij jouw zwakste categorie?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min in duo's + 2 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 5 min.
Loop rond. Stel verdiepende vragen:
- "Hoeveel foto's van die categorie in de oorspronkelijke set?"
- "Zie je dit type tegenwoordig vaker?"
- "Eén persoon of meerdere mensen die labelen?"

Plenair 2 min: 2 duo's hun hypothese delen. Turflijst op flap-over.
-->

---
layout: section
---

# Theoretiseren

## De iteratie-cyclus

<!--
Overgang naar blok 3.
"Er is een vast patroon dat werkt. Vier stappen — geen meer."
-->

---

# Vier stappen — niet meer

<div class="grid grid-cols-4 gap-3 mt-8">

<div class="p-4 bg-purple-50 rounded-xl border-2 border-purple-200 text-center">
  <div class="text-2xl mb-2">🔍</div>
  <div class="text-base font-bold text-purple-700 mb-2">1. Analyse</div>
  <div class="text-xs opacity-80">Confusion matrix: welke categorie onder 80%?</div>
</div>

<div class="p-4 bg-amber-50 rounded-xl border-2 border-amber-200 text-center">
  <div class="text-2xl mb-2">📸</div>
  <div class="text-base font-bold text-amber-700 mb-2">2. Data</div>
  <div class="text-xs opacity-80">30+ gerichte foto's van die categorie</div>
</div>

<div class="p-4 bg-green-50 rounded-xl border-2 border-green-200 text-center">
  <div class="text-2xl mb-2">🏷️</div>
  <div class="text-base font-bold text-green-700 mb-2">3. Labels</div>
  <div class="text-xs opacity-80">Consistent + peer-check (&lt;1 op 10 inconsistent)</div>
</div>

<div class="p-4 bg-blue-50 rounded-xl border-2 border-blue-200 text-center">
  <div class="text-2xl mb-2">🔁</div>
  <div class="text-base font-bold text-blue-700 mb-2">4. Hertest</div>
  <div class="text-xs opacity-80">Train opnieuw, vergelijk per categorie</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Geen transfer learning, geen hyperparameters. Twee acties: gerichte data + consistente labels.
</div>

<!--
Loop de vier stappen langs.
Tempo: 3 min voor uitleg.

Niet uitwijden. Voor MBO-4: kort 'data-centric AI' noemen als achtergrond.
-->

---

# Lakdefect-casus

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-rose-50 rounded-xl border-2 border-rose-200">
  <div class="text-xl font-bold text-rose-700 mb-3">Vóór iteratie</div>
  <ul class="text-sm space-y-2">
    <li>Krassen: <strong>95%</strong> recall</li>
    <li>Kleurafwijkingen: <strong>60%</strong> recall</li>
    <li>40% van kleurafwijkingen ging door</li>
  </ul>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-300">
  <div class="text-xl font-bold text-green-700 mb-3">Na iteratie</div>
  <ul class="text-sm space-y-2">
    <li>Krassen: <strong>95%</strong> recall (gelijk)</li>
    <li>Kleurafwijkingen: <strong>85%</strong> recall</li>
    <li>+25 procentpunt</li>
  </ul>
</div>

</div>

<div v-click class="mt-6 text-center text-base">
  <strong>Actie:</strong> 80 extra foto's met kleurafwijkingen + peer-gecheckte labels.
</div>

<div v-click class="mt-4 text-center text-base font-bold opacity-80">
  Gerichte data van zwakste categorie heft prestatie omhoog — zonder andere categorieën te verslechteren.
</div>

<!--
Verwijs naar wb-03 (handout). Markeerstiften.

Stap voor stap doorlopen. Inzicht expliciet benoemen:
"Dit is waarom data-centric werkt — je voegt waar het écht ontbreekt."
-->

---
layout: section
---

# Experimenteren

## Jouw iteratie — 30+ foto's, peer-check, plan

<!--
Overgang naar blok 4.
"Nu doen we het echt. Geen oefening — eigen lijn, eigen categorie, eigen foto's."
-->

---

# Vier stappen — voor jou

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-5 bg-purple-50 rounded-xl">
  <div class="text-2xl mb-2">🎯</div>
  <div class="text-lg font-bold text-purple-700 mb-2">1. Categorie + plan</div>
  <div class="text-sm opacity-70">Welke shift? Welke camera? Hoeveel foto's?</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl">
  <div class="text-2xl mb-2">📸</div>
  <div class="text-lg font-bold text-amber-700 mb-2">2. Foto's verzamelen</div>
  <div class="text-sm opacity-70">30+ — nu of gedetailleerd plan</div>
</div>

<div class="p-5 bg-green-50 rounded-xl">
  <div class="text-2xl mb-2">👥</div>
  <div class="text-lg font-bold text-green-700 mb-2">3. Labels + peer-check</div>
  <div class="text-sm opacity-70">5 labels door collega — &lt;1 op 10 inconsistent</div>
</div>

<div class="p-5 bg-blue-50 rounded-xl">
  <div class="text-2xl mb-2">🔁</div>
  <div class="text-lg font-bold text-blue-700 mb-2">4. Hertrainings-plan</div>
  <div class="text-sm opacity-70">Datum + eigenaar + hoe meten?</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Concreet plan = uitvoerbaar plan.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  30 min · individueel + duo-peer-check · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Vier stappen.

Stap 1 (5 min) — concretiseren: shift, camera, hoeveelheid.
Stap 2 (10 min) — fotograferen of gedetailleerd plan.
Stap 3 (8 min) — duo's wisselen 5 labels.
Stap 4 (3 min) — hertrainings-moment plannen.

Concreet maken is de competentie. Vage plannen terugsturen.
-->

---

# Deze week + komende weken

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Deze week

<v-clicks>

- Iteratie afronden of uitvoeren als gepland
- Vóór en na meten: recall + precision per categorie
- Notuleer welke categorie de hefboom was

</v-clicks>

</div>

<div>

### Volgende kwaliteitsoverleg

<v-clicks>

- Resultaten delen (vóór/na getallen)
- Iteratie-frequentie afspreken (wekelijks/maandelijks)
- Collega van naburige lijn vragen hetzelfde te doen

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende sessie: LO-094 — human-in-the-loop bij anomalies.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende sessie: <span class="font-bold">Human-in-the-loop — LO-094</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Vision Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke categorieën waren breed zwak in de groep?
- Wie had geen toegang tot eigen model? (1-op-1)
- Bron: Cruz et al. (2024); Ng (2021) Data-centric AI.
-->
