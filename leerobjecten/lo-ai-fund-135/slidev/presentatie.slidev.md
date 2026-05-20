---
theme: default
title: Overfitting — wanneer 99% een alarmbel is
info: |
  ## AI Fundamentals — Module 1 (Gebruik)
  Workshop-blok over overfitting: twee scorekaarten vergelijken, framework drie signalen + drie tegenmaatregelen, eigen leveranciersvraag.
  Doelgroep: operators/teamleiders MBO-4, 42 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Overfitting

### Wanneer 99% een alarmbel is

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 1 (Gebruik) · Workshop-blok · 42 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · leveranciersclaim → kritisch lezen
</div>

<!--
[00:00-00:01] Opening.

Welkom. De komende 42 minuten kijken we naar het belangrijkste alarmbel-signaal in AI — overfitting.

Tegen het eind ken je de drie signalen, drie tegenmaatregelen, en de vraag die je voortaan aan elke leverancier stelt.
-->

---
layout: center
class: text-center
---

# Een leveranciersclaim

<div class="text-2xl mt-10 max-w-2xl mx-auto leading-relaxed opacity-80">
  <span class="italic">"Ons model is 99% nauwkeurig."</span>
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Klinkt geweldig. Maar wat zegt dat eigenlijk?
</div>

<!--
[00:01-00:02] Trigger.

"Een leverancier komt aanzetten met 99% nauwkeurig.
Tegen het eind van deze sessie kun je daarop een betere vraag stellen."

Brug naar fase 1 — twee scorekaarten.
Deel wb-01 uit.
-->

---
layout: center
class: text-center
---

# Wil je het zien gebeuren?

<div class="text-xl mt-10 max-w-xl mx-auto opacity-80">
  90 seconden video
</div>

<div v-click class="mt-8 text-lg opacity-70">
  Twee curves: een blijft stijgen, de ander zakt af.<br/>
  De gap tussen leren en productie groeit in beeld.
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion · <code>OverfittingVideo</code>)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
[OPTIONEEL] Toon de 90s video.
Stop bij voorkeur NA scene 2 (~35s) — divergerende curves zijn de visuele anker.
GEEN term 'overfitting' noemen — die komt bottom-up in fase 2.
-->

---

# Model A

<div class="grid grid-cols-2 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-lg border-2 border-blue-300 text-center">

### Training-score
<div class="text-5xl font-bold text-blue-800 mt-4">
  99%
</div>
<div class="text-xs mt-3 opacity-60">
  Op de trainingsdata
</div>

</div>

<div class="p-6 bg-red-50 rounded-lg border-2 border-red-300 text-center">

### Nieuwe machine
<div class="text-5xl font-bold text-red-800 mt-4">
  60%
</div>
<div class="text-xs mt-3 opacity-60">
  Op onbekende data
</div>

</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-80 italic">
  99% klinkt geweldig. Maar kijk hier — wat zegt dat?
</div>

<!--
[00:02-00:04] IK DOE.

Toon Model A. Denk hardop (langzaam):
"99% klinkt geweldig. Maar kijk hier — op een andere machine zakt het naar 60%. Wat zegt dat?"

Pauze. GEEN antwoord geven.
-->

---

# Model B

<div class="grid grid-cols-2 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-lg border-2 border-blue-300 text-center">

### Training-score
<div class="text-5xl font-bold text-blue-800 mt-4">
  88%
</div>
<div class="text-xs mt-3 opacity-60">
  Op de trainingsdata
</div>

</div>

<div class="p-6 bg-green-50 rounded-lg border-2 border-green-300 text-center">

### Nieuwe machine
<div class="text-5xl font-bold text-green-800 mt-4">
  86%
</div>
<div class="text-xs mt-3 opacity-60">
  Op onbekende data
</div>

</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-80">
  Welke vertrouw je? En waarom?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min · individueel · wb-01
</div>

<!--
[00:04-00:05] Toon Model B.

Vraag: "Welke vertrouw je? En waarom?"
Stilte 5-7 sec. Geen aanwijzing.

[00:05-00:09] Zet timer op 4 min. Loop rond.
Stel verdiepende vragen — geen hint:
- "Wat valt je op?"
- "Welk getal vertel je aan je teamleider?"
- "Wat zou je willen weten voor je kiest?"

[00:09-00:10] Tussenstand. Wie heeft gekozen? Wie twijfelt nog? Schuren mag.
-->

---
layout: center
class: text-center
---

# Stem mee — twee kleuren

<div class="grid grid-cols-2 gap-6 mt-10 text-sm max-w-xl mx-auto">
  <div class="p-5 bg-red-50 rounded-lg border-2 border-red-300">
    <div class="font-bold text-red-700 text-lg">Rood</div>
    <div class="mt-3">Model A</div>
    <div class="text-xs mt-1 opacity-60">99% / 60%</div>
  </div>
  <div class="p-5 bg-blue-50 rounded-lg border-2 border-blue-300">
    <div class="font-bold text-blue-700 text-lg">Blauw</div>
    <div class="mt-3">Model B</div>
    <div class="text-xs mt-1 opacity-60">88% / 86%</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Welke zou jij op de productievloer vertrouwen?
</div>

<!--
[00:10-00:15] Eerst 5 minuten in tweetallen.
"Vergelijk je keuze en je reden. Welk getal of welk verschil verraadt voor jullie wat hier scheef zit?"

[00:15-00:16] Daarna plenaire stemming met kleurkaartjes.
Tel hardop. Schrijf uitslag op flip-over.

Tel innerlijk tot 7 na elke vraag.
Bij stilte: noem zelf 'wie heeft Model A?' om ijs te breken.
-->

---

# Het signaal

<div class="grid grid-cols-2 gap-6 mt-8 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### Model A — 99% / 60%
- Scoreverschil: **39 punten**
- Model heeft trainingsdata uit hoofd geleerd
- Valt stil op nieuwe data

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Model B — 88% / 86%
- Scoreverschil: **2 punten**
- Heeft het patroon door
- Stabiel op onbekende data

</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold text-blue-700">
  Het VERSCHIL is het signaal — niet de hoogte.
</div>

<div v-click class="mt-4 text-center text-base opacity-70 italic">
  Dat heet overfitting — te-goed-leren.
</div>

<!--
[00:16-00:19] Plenair benoemen (3 min).

Vraag eerst een duo dat voor A koos: "wat overtuigde jullie?" Wacht 5-7 sec.
Daarna een duo dat voor B koos.

Maak expliciet:
"Wat verraadt het verschil tussen 99% en 60%?
Het MODEL heeft de trainingsdata uit het hoofd geleerd in plaats van het patroon.
Op nieuwe data valt het stil. Dat heet OVERFITTING — te-goed-leren."

Schrijf op flip-over: 'Overfitting = voorbeelden onthouden, niet patroon zien'.

Vergelijking: "Stel een nieuwe collega heeft tien producten op één machine gezien.
Herkent die feilloos. Zet hem op een ander machinetype — hij staat stil.
Voorbeelden onthouden, geen patroon door."

[00:19-00:20] Brug naar fase 3.
-->

---
layout: section
---

# Theoretiseren

## Drie signalen + drie tegenmaatregelen

<!--
[00:20-00:21] Overgang naar blok 3.

Deel wb-03 uit. Pak markeerstift erbij.
-->

---

# Drie signalen voor overfitting

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### 1 · Groot scoreverschil
- **Training vs onbekende data**
- Bv. 99% → 60%
- Verschil 39 punten
- Sterk alarm-signaal

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### 2 · Klein dataset, complex model
- **Weinig voorbeelden + veel rekenkracht**
- Bv. 50 cases, één machine
- Model heeft ruimte om te onthouden
- In plaats van patroon te leren

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### 3 · Faalt op nieuw
- **Lab werkt, vloer niet**
- Showroom-effect
- Nieuwe machine, nieuwe batch
- → onverwacht foutpercentage

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Niet één — alle drie samen bouwen het verhaal.
</div>

<!--
[00:21-00:26] Vijf minuten — drie signalen.

Signaal 1 (2 min): "Training 99% → nieuwe machine 60%. Verschil 39 punten.
Bij Model B: 88% → 86%. Verschil 2 punten.
Het VERSCHIL is het signaal — niet de hoogte. Een leverancier die alleen één getal noemt, is verdacht."

Signaal 2 (1.5 min): "50 trillings-voorbeelden van één machine + complex neuraal netwerk.
Model heeft te veel ruimte om voorbeelden te onthouden in plaats van patroon te leren."

Signaal 3 (1.5 min): "Wat in het lab werkte, werkt niet op de werkvloer.
Wat bij de leverancier werkt, faalt bij jullie. Het showroom-effect."

Schrijf elk signaal op flip-over.
-->

---

# Drie tegenmaatregelen

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-green-50 rounded-lg">

### 1 · Meer voorbeelden
- **DIVERSE data**
- Niet alleen meer foto's
- Meer ploegen, machines, situaties
- Bron: Russell & Norvig (2021)

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### 2 · Simpeler model
- **Minder complexiteit**
- Kan minder ruis vasthouden
- Soms is eenvoudiger robuuster
- Niet de mooiste — wel werkbaar

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### 3 · Cross-validatie
- **Testen op data die niet in training zat**
- Standaard professionele werkwijze
- Vraag aan leverancier:<br/>"hoe heeft u dit gedaan?"

</div>

</div>

<div v-click class="mt-6 text-center text-sm opacity-70">
  In Russell & Norvig 2021: 50 voorbeelden van 1 machine → 5 machines toegevoegd → score op nieuwe machines steeg naar 90%.
</div>

<!--
[00:26-00:30] Vier minuten — drie tegenmaatregelen.

Tegenmaatregel 1 (1.5 min): "Niet alleen meer foto's — meer DIVERSE voorbeelden.
Variatie zoals we in trainingsdata-LO zagen: meer ploegen, machines, situaties.
Russell & Norvig 2021: 50 voorbeelden van 1 machine → 5 machines toegevoegd → 90% op nieuwe machines."

Tegenmaatregel 2 (1 min): "Minder complexiteit. Soms eenvoudiger algoritme robuuster."

Tegenmaatregel 3 (1.5 min): "Cross-validatie — test herhaald op data die het NIET tijdens training zag.
Standaard onderdeel van professioneel AI-werk.
Vraag aan leverancier: hoe heeft u dit gedaan?"

Schrijf elke tegenmaatregel op flip-over.
-->

---

# Praktische realiteit

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### Leveranciers tonen één getal
- 99% nauwkeurig — klinkt indrukwekkend
- Maar: in welke context?
- Vraag door naar het verschil

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### Showroom-modellen
- Werken op één machine
- Vaak overfitted
- Productie-deployment toont realiteit

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Operator-vaardigheid
- Patroon herkennen bespaart jaren ervaring
- Voor je een dure leverancier kiest
- Voor je verkeerd model in productie gaat

</div>

</div>

<!--
[00:30-00:31] Eén minuut — praktische realiteit.

"Leveranciers tonen vaak één hoog getal. Jouw rol als operator:
vraag door naar het verschil. Showroom-modellen op één machine zijn vaak overfitted.
Het herkennen van dit patroon is een vaardigheid die jaren ervaring bespaart."

[00:31-00:32] Brug naar fase 4: "Nu drie nieuwe scenario's. Jij beoordeelt."
-->

---
layout: section
---

# Experimenteren

## Diagnose op drie scorekaarten

<!--
[00:32-00:33] Overgang naar blok 4.

Deel wb-04 uit. Zet de scope: "Twee vragen per scenario — is dit overfitting?
Welke tegenmaatregel? Twijfel mag."
-->

---

# Drie scenario's — beoordeel

<div class="grid grid-cols-3 gap-3 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Scenario A
- Training **95%**
- Test **92%**
- 200 voorbeelden
- 4 machines

<div class="mt-3 text-xs opacity-60">Overfitting?</div>

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### Scenario B
- Training **97%**
- Test **65%**
- 30 voorbeelden
- 1 machine

<div class="mt-3 text-xs opacity-60">Overfitting?</div>

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Scenario C
- Training **80%**
- Test **78%**
- 500 voorbeelden
- 2 machines

<div class="mt-3 text-xs opacity-60">Overfitting?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-04 <span class="opacity-60">of tablet · model-overfitting-sliders</span> · twijfel mag
</div>

<!--
[00:33-00:34] Drie scenario's toelichten (1 min).

[00:34-00:40] Zet timer op 6 min. Loop rond.
Help bij twijfel met ÉÉN vraag: "hoe groot is het verschil tussen leren en onbekende data?"
Bevestig dat twijfel een goed antwoord is.
-->

---

# De diagnose

<div class="grid grid-cols-3 gap-3 mt-6 text-sm">

<div class="p-3 bg-green-50 rounded-lg">

### A · Gezond
- Verschil 3 punten
- 200 voorbeelden, 4 machines
- Generaliseert prima

</div>

<div class="p-3 bg-red-50 rounded-lg">

### B · Overfitting
- Verschil 32 punten
- Klein dataset, 1 machine
- → meer diverse voorbeelden

</div>

<div class="p-3 bg-amber-50 rounded-lg">

### C · Gezond — lage score
- Verschil 2 punten
- Geen overfitting
- Wel: ander model overwegen

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Scenario C is het contra-intuïtieve geval: lage score is geen synoniem voor overfitting.
</div>

<!--
[00:40-00:42] Twee minuten plenair vergelijken.

Per scenario: "wie zegt overfitting, wie zegt nee, wie twijfelt?"
Tel handen, geen lange bespreking.

Maak per scenario kort de diagnose:
"A — gezond. Verschil 3 punten, 200 voorbeelden over 4 machines."
"B — overfitting. Verschil 32 punten, klein dataset. Tegenmaatregel: meer diverse voorbeelden."
"C — gezond ondanks lage score. Geen overfitting — wel andere model overwegen."

[00:41:30-00:42] Transferopdracht.
-->

---

# Deze week — transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Drie vragen aan leverancier / IT
<v-clicks>

- Op welke data is dit model **getraind**? Hoeveel voorbeelden, welke machines?
- Op welke onbekende data is het **getest**?
- Wat is het **verschil** tussen die twee scores?

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Vraag een collega-operator:<br/>*"Heb jij ooit gezien dat iets op één machine wel deed en op een nieuwe niet?"*
- Vaak: herkenbaar verhaal
- Alleen had niemand er een naam voor
- Nu wel: overfitting

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat heb je gevonden?
</div>

<!--
[00:41:30-00:42] Transferopdracht meegeven.

"Deze week: zoek één AI-systeem in jouw fabriek.
Vraag aan leverancier of IT drie dingen.
Drie antwoorden meenemen naar de volgende sessie.

Bonus: vraag een collega — vaak herkenbaar verhaal, geen naam voor."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Cross-validatie · CNN · RNN · Ensemble methods</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 1 (Gebruik)
</div>

<!--
[00:42] Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Hoeveel kozen Model A vóór de bespreking? (hardnekkigheid 'hoogste wint')
- Welke leveranciers worden bevraagd?
- Welke systemen onderzocht?
- Welke parkeerlijst-items voor vervolgsessie?
-->
