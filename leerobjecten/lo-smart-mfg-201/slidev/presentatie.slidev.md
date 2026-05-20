---
theme: default
title: Sensordata lezen — temperatuur, druk en trillingen
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over basislijn bepalen, trends herkennen en pieken van ruis onderscheiden.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Sensordata lezen

### Wat is normaal voor JOUW machine?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · CNC / spuitgieten / draaibank
</div>

<!--
Welkom. De komende 40 minuten leer je sensordata lezen op JOUW machine.
Niet op een gemiddelde fabriek-machine. Op de jouwe.

Trigger: "Wie heeft wel eens een storing gehad die niemand zag aankomen?"
Vang 1-2 reacties. Reageer met "herkenbaar". Geen oordeel.
Doorpakken naar fase 1.
-->

---
layout: section
---

# Experimenteren

## Meet zelf — bepaal je basislijn

<!--
Overgang naar blok 1.
"In duo's. Een meet, de ander schrijft. Halverwege wisselen."
-->

---
layout: center
class: text-center
---

# In duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">🌡️</div>
    <div class="text-lg font-bold text-blue-700">Meet 6 waarden</div>
    <div class="text-sm opacity-70 mt-2">Temperatuur · druk · trillingen</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">🧮</div>
    <div class="text-lg font-bold text-purple-700">Bereken basislijn</div>
    <div class="text-sm opacity-70 mt-2">Gemiddelde van jullie metingen</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">🔍</div>
    <div class="text-lg font-bold text-green-700">Beoordeel 6 waarden</div>
    <div class="text-sm opacity-70 mt-2">Normaal · trend · piek?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Halverwege wisselen — eerst meet jij, dan je buurman.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · in duo's · wb-01-experimenteren
</div>

<!--
Werkblad wb-01 uitdelen. Timer op 10 min.
Coach-modus: niet voorzeggen.

Bij vastlopen: "Wat zou je doen als je dit getal op je werk zag?"
Bij snelle duo's: "Welke variabele zou je OOK willen meten die niet in de sensoren zit?"
-->

---
layout: center
class: text-center
---

# Jouw basislijn — wat valt op?

<div class="text-2xl mt-8 max-w-xl mx-auto leading-relaxed opacity-80">
  Wie deelt zijn getallen?
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Zelfde machinetype, andere getallen.<br/>
  <span class="font-bold">Jouw machine heeft eigen normaalwaarden.</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Plenair · 1.5 min
</div>

<!--
Vang 2-3 reacties. Schrijf 2-3 getallen op de flap-over.
"Zelfde machinetype, andere getallen. Dat IS het inzicht."

Bij scepsis ('die getallen staan toch al ingesteld?'):
"Klopt — fabriek heeft een standaard. Maar jouw machine, jouw productie,
jouw omgeving wijken af. Vandaag meten we de echte."
-->

---
layout: section
---

# Ervaren

## Storingsquiz — 4 scenario's

<!--
Overgang naar blok 2. "Vier scenario's. Per scenario: type afwijking + actie."
-->

---
layout: center
class: text-center
---

# 4 scenario's

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Per scenario:<br/>
  <span class="font-bold">Wat zie je</span> — basislijn, trend, piek, ruis?<br/>
  <span class="font-bold">Wat doe je</span> — welke actie?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Drie keer of vaker = signaal.<br/>
  Eén losse piek die verdwijnt = ruis.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  7 min · individueel · wb-02-ervaren
</div>

<!--
Werkblad wb-02. Timer op 7 min.
Geen antwoorden geven — wel vragen stellen:
- "Waar kijk je naar — gemiddelde of laatste meting?"
- "Hoe lang zie je dit al?"
- "Drie keer of vaker = signaal — geldt dat hier?"

Niet plenair antwoorden bespreken na deze fase.
Dat doen we in fase 3.
-->

---
layout: center
class: text-center
---

# Tel je correcte antwoorden

<div class="text-xl mt-8 opacity-80">
  Iedereen heeft fouten gemaakt.<br/>
  <span class="font-bold">Dat is goed.</span>
</div>

<div v-click class="mt-8 text-base opacity-70">
  Daar leren we van in de duo-bespreking.
</div>

<!--
Anker-moment. Voorkomt faalangst.
"Niemand heeft 4 op 4 — dit is oefenen, niet toetsen."
-->

---
layout: section
---

# Reflecteren

## Vergelijk met je oefenpartner

<!--
Overgang naar blok 3. "Zelfde duo als in fase 1. Vergelijk."
-->

---
layout: center
class: text-center
---

# Bespreek in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">🤔</div>
    <div class="text-lg font-bold text-blue-700">Waar verschilden jullie het meest?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">🧭</div>
    <div class="text-lg font-bold text-purple-700">Trend of piek — hoe wist je dat?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">💡</div>
    <div class="text-lg font-bold text-green-700">Wat ga je nu anders doen?</div>
  </div>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min duo · 3 min plenair · wb-03-reflecteren
</div>

<!--
Werkblad wb-03. Timer op 6 min.
Loop rond. Luister naar concrete redeneringen.
Verzamel 2-3 sterke voorbeelden voor plenair.

Plenair (3 min):
- "Bij welk scenario verschilden jullie het meest?"
- "Hoe bepaalde je trend vs piek?"
- "Wie heeft op zijn eigen machine ooit een trend gezien
   die hij nu anders zou interpreteren?"

Schrijf 3 sleutelwoorden op flap-over.
-->

---
layout: section
---

# Theoretiseren

## De 3 stappen — kapstok voor jouw werkvloer

<!--
Overgang naar blok 4. 5 minuten — geen seconde meer.
"Dit is wat jullie net zelf hebben gedaan."
-->

---

# De 3 stappen

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-5xl mb-3">📏</div>
  <div class="text-xl font-bold text-blue-700 mb-2">1. Basislijn</div>
  <div class="text-sm opacity-80">Wat is normaal voor JOUW machine?</div>
  <div class="text-xs opacity-60 mt-2">5 dagen meten · elke 30 min · gemiddelde</div>
</div>

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-5xl mb-3">📈</div>
  <div class="text-xl font-bold text-amber-700 mb-2">2. Trend</div>
  <div class="text-sm opacity-80">Stijgt het langzaam over weken?</div>
  <div class="text-xs opacity-60 mt-2">Vergelijk deze week met vorige week</div>
</div>

<div class="p-6 bg-red-50 rounded-xl border-2 border-red-200">
  <div class="text-5xl mb-3">⚡</div>
  <div class="text-xl font-bold text-red-700 mb-2">3. Piek vs ruis</div>
  <div class="text-sm opacity-80">Drie keer of vaker = signaal</div>
  <div class="text-xs opacity-60 mt-2">Eén losse piek die verdwijnt = ruis</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Dit is wat jullie net zelf hebben gedaan.
</div>

<!--
Lees de handout SAMEN — niet voor.
Wijs naar de flap-over-kapstok.
"Stap 1 = wat jullie maten. Stap 2 = wat in scenario 2 stond.
Stap 3 = wat jullie in duo bespraken."
-->

---

# Voorbeeld: CNC-spindeltemperatuur

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De data
<v-clicks>

- Basislijn: **65 graden**
- Week 1: 66 graden
- Week 2: 68 graden
- Week 3: **72 graden**

</v-clicks>

</div>

<div>

### De redenering
<v-clicks>

- Stijging 2-3 graden per week
- Vier keer hoger gemeten — geen ruis
- Trend = signaal

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-blue-50 rounded-lg">

### Wat deed de operator?
- Meldde bij technische dienst.
- Smeermiddel spindellager bijna op.
- Na bijvullen: weer 65 graden.
- **Ongeplande stilstand voorkomen.**

</div>

<!--
Concreet voorbeeld. Houd het bij dit ene voorbeeld — niet wisselen.
Bij vraag over andere sensoren: "Werkt hetzelfde voor druk en trilling."

Bij MBO-4: noem bron AIMM Competentieframework v0.1 PM-02.
-->

---

# Deze week — jouw transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Doe dit
<v-clicks>

- Kies **één machine**
- Doe **5 metingen** in 3 werkdagen
- Meet temperatuur, druk, trilling
- Bereken het gemiddelde

</v-clicks>

</div>

<div>

### Stuur dit
<v-clicks>

- Drie getallen in de **groepsapp**
- Binnen 3 dagen
- Volgende sessie: vergelijken
- Bouwen we voort: drempelwaarden (LO-202)

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg text-center">

### Let ook op
Niet-numerieke signalen — geluid, geur, vibratie die je voelt.
Vraag de onderhoudstechnicus welke sensorwaarden hij belangrijk vindt.

</div>

<!--
Schrijf op het werkblad: welke machine, welke 5 meetmomenten.
Dat is je commitment.

Loop rond, check dat het ingevuld is.
LO-201 → LO-202: basislijn-getallen worden drempelwaarden.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Drempelwaarden instellen — LO-202</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Wie heeft basislijn-getallen toegezegd? (volgmoment LO-202)
- Wie was sceptisch? (1-op-1 in volgende sessie)
- Bron: AIMM Competentieframework v0.1 (PM-02).
-->
