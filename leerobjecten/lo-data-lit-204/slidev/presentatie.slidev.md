---
theme: default
title: Een simpele data-analyse — van vraag naar antwoord
info: |
  ## Data Literacy Module 2 — Train
  Workshop-blok: vier stappen van vraag naar conclusie. Worked example op Lijn 4 + eigen analyse.
  Doelgroep: operators MBO-3, 48 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Van vraag naar antwoord

### Een simpele data-analyse in vier stappen

<div class="mt-12 text-sm opacity-60">
  Data Literacy Module 2 (Train) · Workshop-blok · 48 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 48 minuten doen jullie ZELF een data-analyse.
Eerst samen op Lijn 4 — daarna op een probleem van je eigen werkvloer.

Open warm: "Wie heeft op zijn werk weleens uitgezocht waarom iets fout ging?"
Vang 1-2 reacties. Reageer alleen met "herkenbaar".
-->

---
layout: center
class: text-center
---

# Vier stappen

<div class="grid grid-cols-4 gap-4 mt-8">
  <div class="p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-3xl mb-2">❓</div>
    <div class="text-base font-bold text-blue-700">1. Vraag</div>
    <div class="text-xs opacity-70 mt-1">Specifiek</div>
  </div>
  <div class="p-4 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-3xl mb-2">📊</div>
    <div class="text-base font-bold text-purple-700">2. Data</div>
    <div class="text-xs opacity-70 mt-1">Wat je nodig hebt</div>
  </div>
  <div class="p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-3xl mb-2">🔍</div>
    <div class="text-base font-bold text-amber-700">3. Analyse</div>
    <div class="text-xs opacity-70 mt-1">Vergelijken / groeperen / tellen</div>
  </div>
  <div class="p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-3xl mb-2">✅</div>
    <div class="text-base font-bold text-green-700">4. Conclusie</div>
    <div class="text-xs opacity-70 mt-1">Beantwoord de vraag</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Ik doe stap 1 voor. Stap 2-3-4 doen jullie zelf.
</div>

<!--
"Vier stappen. Vier ankerpunten.
Ik doe stap 1 voor — een goede vraag formuleren is het lastigste.
Daarna doen jullie het zelf met je buurman."
-->

---
layout: section
---

# Ervaren

## Worked example — Lijn 4

<!--
Overgang naar fase 1.
"Voor je ligt productiedata van Lijn 4. Het afkeurpercentage op dinsdag is 6%. De andere dagen rond de 3%."
-->

---

# Lijn 4 — productie deze week

<div class="mt-4">

| Dag | Productie | Afgekeurd | Afkeur % | Ploeg |
|---|:-:|:-:|:-:|:-:|
| Maandag | 920 | 28 | **3,0%** | A |
| Dinsdag | 880 | 53 | **6,0%** | B |
| Woensdag | 910 | 27 | **3,0%** | A |
| Donderdag | 895 | 54 | **6,0%** | B |
| Vrijdag | 905 | 25 | **2,8%** | A |

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Dinsdag en donderdag = dubbel zo hoog.<br/>
  Hoe komt dat?
</div>

<!--
Toon de dataset rustig. Wijs naar de afkeurkolom.
"Dinsdag 6%. Maandag 3%. Twee keer zo hoog. Hoe komt dat?

Dat is de aanleiding. Nu komt mijn vraag — stap 1."
-->

---
layout: center
class: text-center
---

# Stap 1 — mijn vraag

<div class="text-2xl mt-8 max-w-3xl mx-auto leading-relaxed">
  Waarom is het afkeurpercentage op <span class="font-bold text-blue-600">dinsdag (6%)</span> twee keer zo hoog als op <span class="font-bold text-blue-600">maandag (3%)</span> op <span class="font-bold text-blue-600">Lijn 4</span>?
</div>

<div class="mt-12 grid grid-cols-3 gap-6 text-base">
  <div v-click class="p-3 bg-green-50 rounded-lg">
    <div class="font-bold text-green-700">Specifiek?</div>
    <div class="text-sm opacity-70">tijd · plek · vergelijking</div>
  </div>
  <div v-click class="p-3 bg-green-50 rounded-lg">
    <div class="font-bold text-green-700">Beantwoordbaar?</div>
    <div class="text-sm opacity-70">data is er</div>
  </div>
  <div v-click class="p-3 bg-green-50 rounded-lg">
    <div class="font-bold text-green-700">Relevant?</div>
    <div class="text-sm opacity-70">afkeur = geld</div>
  </div>
</div>

<!--
Dit is stap 1 — IK DOE.
Reken de drie checks hardop af:
- Specifiek? Ja — tijd (dinsdag), plek (Lijn 4), vergelijking (dinsdag vs maandag).
- Beantwoordbaar met data? Ja — ik heb de cijfers.
- Relevant? Ja — afkeur kost geld.

Schrijf de vraag op de flap-over.
"Dit is stap 1. Nu zijn JULLIE aan de beurt — stap 2, 3, 4."
-->

---
layout: center
class: text-center
---

# Jullie beurt — stap 2, 3, 4

<div class="text-2xl mt-8 max-w-2xl mx-auto leading-relaxed opacity-80">
  Welke <span class="font-bold">data</span> heb je nodig?<br/>
  Hoe ga je <span class="font-bold">analyseren</span>?<br/>
  Wat is je <span class="font-bold">conclusie</span>?
</div>

<div v-click class="mt-12 text-base opacity-70">
  Tien minuten — met je buurman — werkblad 1
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · in tweetallen · wb-01-ervaren
</div>

<!--
Zet timer op 10 min. Loop rond.
Coach met vragen — GEEN antwoorden:
- Stap 2: "Welke data heb je nodig? Waar zou je kijken?"
- Stap 3: "Wat valt je op als je vergelijkt? En als je per ploeg groepeert?"
- Stap 4: "Wat is je conclusie? Waarom denk je dat?"

Bij vastlopen: drie analyse-werkwoorden — "vergelijken, groeperen, tellen".
-->

---
layout: section
---

# Reflecteren

## Wat ging goed, wat was lastig?

<!--
Overgang naar fase 2.
"Pak je buurman — vijf minuten reflecteren. Welke stap was makkelijk, welke lastig?"
-->

---

# Drie reflectievragen

<div class="grid grid-cols-1 gap-4 mt-6">

<div class="p-4 bg-blue-50 rounded-lg">

### 1. Bij welke stap ging het makkelijkst?
*Wat maakte het makkelijk?*

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### 2. Bij welke stap moest je het meest nadenken?
*Wat maakte het lastig?*

</div>

<div class="p-4 bg-green-50 rounded-lg">

### 3. Wat zou je de volgende keer anders doen?

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · in tweetallen · wb-02-reflecteren
</div>

<!--
Deel werkblad 2 uit. Zet timer op 5 min duo + 5 min plenair.
Loop rond, luister mee, verzamel observaties.

Plenair: vraag 2-3 duo's te delen.
Vat samen: "De meeste mensen vinden stap 1 en stap 3 het lastigst. Dat is normaal."
-->

---
layout: section
---

# Theoretiseren

## Tips per stap

<!--
Overgang naar fase 3.
"Jullie hebben de stappen net zelf gedaan. Nu krijgen ze tips."
-->

---

# Stap 1 — een goede vraag

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Goed
<v-clicks>

- Specifiek (tijd, plek, vergelijking)
- Beantwoordbaar met data
- Relevant voor productie

</v-clicks>

<div v-click class="mt-4 p-3 bg-green-50 rounded-lg text-sm">
  *"Waarom is afkeur op dinsdag dubbel zo hoog als op maandag op Lijn 4?"*
</div>

</div>

<div>

### Niet goed
<v-clicks>

- Vaag ("waarom gaat het soms fout?")
- Niet meetbaar ("wat is er aan de hand?")
- Niet relevant ("hoe oud is de machine?")

</v-clicks>

<div v-click class="mt-4 p-3 bg-red-50 rounded-lg text-sm">
  *"Waarom gaat het soms fout?"*
</div>

</div>

</div>

<!--
Verwijs naar fase 1: "Karim's vraag had alle drie de kenmerken."
Maakt het herkenning, geen lesje.
-->

---

# Stap 2 — alleen wat je nodig hebt

<div class="mt-8 text-center text-2xl">

Vier ankerpunten

</div>

<div class="grid grid-cols-4 gap-4 mt-8">

<div v-click class="p-4 bg-blue-50 rounded-xl text-center">
  <div class="text-3xl mb-2">📅</div>
  <div class="font-bold">Periode</div>
  <div class="text-xs opacity-70 mt-1">Welke dagen / weken?</div>
</div>

<div v-click class="p-4 bg-purple-50 rounded-xl text-center">
  <div class="text-3xl mb-2">⚙️</div>
  <div class="font-bold">Machine</div>
  <div class="text-xs opacity-70 mt-1">Welke lijn / cel?</div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-xl text-center">
  <div class="text-3xl mb-2">👥</div>
  <div class="font-bold">Ploeg</div>
  <div class="text-xs opacity-70 mt-1">A / B / C?</div>
</div>

<div v-click class="p-4 bg-green-50 rounded-xl text-center">
  <div class="text-3xl mb-2">📦</div>
  <div class="font-bold">Product</div>
  <div class="text-xs opacity-70 mt-1">Welke variant?</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Niet alle data verzamelen — alleen wat past bij je vraag.
</div>

<!--
"Verzamel ALLEEN wat je nodig hebt. Niet alles.
De vraag bepaalt de data — niet andersom."
-->

---

# Stap 3 — drie werkwoorden

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl">
  <div class="text-4xl mb-3">↔️</div>
  <div class="text-xl font-bold text-blue-700 mb-2">Vergelijken</div>
  <div class="text-sm opacity-80">Twee getallen naast elkaar</div>
  <div class="text-xs italic opacity-60 mt-3">dinsdag (6%) vs maandag (3%)</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl">
  <div class="text-4xl mb-3">📊</div>
  <div class="text-xl font-bold text-purple-700 mb-2">Groeperen</div>
  <div class="text-sm opacity-80">Per categorie</div>
  <div class="text-xs italic opacity-60 mt-3">ploeg A (3%) vs ploeg B (6%)</div>
</div>

<div class="p-6 bg-amber-50 rounded-xl">
  <div class="text-4xl mb-3">🔢</div>
  <div class="text-xl font-bold text-amber-700 mb-2">Tellen</div>
  <div class="text-sm opacity-80">Hoe vaak komt iets voor?</div>
  <div class="text-xs italic opacity-60 mt-3">storingen per dag</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Begin altijd met vergelijken — twee getallen naast elkaar.
</div>

<!--
"Vergelijken is de makkelijkste start.
Groeperen daarna — patroon zoeken.
Tellen als je hoeveelheden moet weten."
-->

---

# Stap 4 — eerlijke conclusie

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Goed
<v-clicks>

- Beantwoordt de vraag
- Niet meer, niet minder
- Eerlijk over onzekerheid

</v-clicks>

<div v-click class="mt-4 p-3 bg-green-50 rounded-lg text-sm">
  *"Op de twee dagen dat ploeg B werkt, is afkeur dubbel zo hoog. Volgende vraag: ligt het aan de ploeg of aan iets anders?"*
</div>

</div>

<div>

### Niet goed
<v-clicks>

- "Lijkt erop dat..."
- Conclusie is een mening
- Conclusie wijst persoon aan

</v-clicks>

<div v-click class="mt-4 p-3 bg-red-50 rounded-lg text-sm">
  *"Het lijkt erop dat ploeg B het slechter doet."*
</div>

</div>

</div>

<!--
Belangrijk: een conclusie zegt WAT de data laat zien — niet wat jij gelooft.
"De data laat zien dat..." = goed.
"Het lijkt erop dat..." = geen conclusie, alleen gevoel.

Een eerlijke conclusie kan ook zeggen: "We weten het nog niet — meer data nodig."
-->

---
layout: section
---

# Experimenteren

## Jouw eigen werkvloer

<!--
Overgang naar fase 4.
"De afgelopen 33 minuten waren oefening. Nu pas je het toe op een echt probleem van je werkvloer."
-->

---

# Kies een probleem van je werk

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het werkblad
<v-clicks>

- Stap 1 — formuleer een vraag
- Stap 2 — welke data heb je nodig?
- Stap 3 — vergelijk, groepeer, tel
- Stap 4 — wat is je conclusie?

</v-clicks>

</div>

<div>

### Coach-vragen
<v-clicks>

- Is je vraag specifiek?
- Welke data heb je?
- Wat zie je als je vergelijkt?
- Wat is je eerlijke conclusie?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  15 min · in tweetallen · wb-04-experimenteren
</div>

<!--
Deel werkblad 4 uit. Zet timer op 10 min duo + 4 min plenair + 1 min afsluiting.

Geef GEEN voorbeeld-probleem.
Bij twijfel: "Wat ergert je deze week op het werk?"
Daar zit een goed analyse-onderwerp.

Bij klacht-sessie: maak het feitelijk.
"Welke vraag wil je hier mee beantwoorden?"
-->

---
layout: center
class: text-center
---

# Mini-presentaties

<div class="text-2xl mt-8 max-w-xl mx-auto leading-relaxed">
  Twee duo's delen<br/>
  hun analyse
</div>

<div class="mt-12 grid grid-cols-3 gap-4 text-base opacity-80">
  <div>Vraag</div>
  <div>→ Data + analyse</div>
  <div>→ Conclusie</div>
</div>

<div v-click class="mt-12 text-base opacity-60">
  Reageer met *"helder"* of een doorvraag.<br/>
  Geen oordeel, geen correctie.
</div>

<!--
Twee duo's, elk 1 min. Vraag, data, conclusie.

Trainer reageert ALLEEN met:
- "Helder geformuleerd"
- "Wat zou je nodig hebben om het zekerder te maken?"

ZWIJG na de presentatie. Laat de groep reageren — niet jij.
-->

---

# Deze week — transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Doe het echt
<v-clicks>

- Kies een probleem op je werk
- Doorloop de vier stappen
- Schrijf je conclusie op
- Bespreek met je teamleider

</v-clicks>

</div>

<div>

### Volgende bijeenkomst
<v-clicks>

- Presenteer je analyse
- Klopt mijn conclusie?
- Wat zou de teamleider anders doen?
- Module 3 — op je hele afdeling

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
"Module 3 (Op maat) bouwt hierop voort — daar pas je dezelfde stappen toe op je hele afdeling."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende stap: <span class="font-bold">Module 3 — Op maat</span>
</div>

<div class="mt-6 text-sm opacity-60">
  Je leert de vier stappen toepassen op je eigen afdeling, met een eigen dataplan
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Data Literacy Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notities voor jezelf:
- Welke duo's hadden de scherpste vraag? (sterke kandidaten voor Module 3)
- Wie kwam met "lijkt op"-conclusie? (kandidaat voor extra coaching)
- Welke werkvloer-problemen werden genoemd? (input voor module 3 cases)
-->
