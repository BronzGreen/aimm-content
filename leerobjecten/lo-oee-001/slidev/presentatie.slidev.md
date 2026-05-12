---
theme: default
title: Wat is OEE? Hoe goed draait jouw machine echt?
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over de drie OEE-componenten en het multiplicatie-effect.
  Doelgroep: operators MBO-3, 38 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Wat is OEE?

### Hoe goed draait jouw machine echt?

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok · 38 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 38 minuten gaan we kijken naar één getal dat in veel fabrieken op het bord staat: OEE.
Tegen het eind weet je wat het is, welke drie vragen erin zitten, en hoe het er bij jouw eigen machine ongeveer uitziet.

[Open warm op] "Wie heeft op zijn lijn ergens een OEE-getal of een grafiek hangen?"
Vang 2-3 reacties. Reageer alleen met "herkenbaar". Géén oordeel.
-->

---
layout: center
class: text-center
---

# Plak je schatting op de lijn

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Hoe goed draait jouw machine?<br/>
  Schrijf een percentage op je gele kaartje.
</div>

<div class="mt-10 flex justify-center items-center gap-6">
  <div class="text-3xl font-bold text-red-500">0%</div>
  <div class="flex-1 h-2 bg-gradient-to-r from-red-300 via-amber-300 to-green-400 rounded-full max-w-md"></div>
  <div class="text-3xl font-bold text-green-600">100%</div>
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Buikgevoel is genoeg. Geen onderbouwing nodig.
</div>

<!--
IK DOE eerst — pak een geel kaartje, schrijf 85, plak op de lijn:
"Mijn voorbeeldmachine — verpakkingslijn — draait volgens mij ongeveer 85% van de tijd. Ik plak hem hier."

Daarna kaartjes uitdelen. 3 minuten plakken.
Praat niet — laat het stil gebeuren.
Eindig met: "Pen neer. Kijk naar de lijn. Wat zie je?"

NIET interpreteren. Bewaar voor fase 4.
-->

---
layout: section
---

# Drie vragen

## Wat zit er eigenlijk in dat getal?

<!--
Overgang naar blok 2 (reflecteren).
-->

---
layout: center
class: text-center
---

# OEE beantwoordt drie vragen

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-5xl mb-3">⚙️</div>
    <div class="text-xl font-bold text-blue-700">Draait hij?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-5xl mb-3">⏱️</div>
    <div class="text-xl font-bold text-purple-700">Snel genoeg?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-5xl mb-3">✅</div>
    <div class="text-xl font-bold text-green-700">Goed product?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Bespreek met je buurman: welke vraag zie je het sterkst op jouw lijn?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · in tweetallen · werkblad drie vragen
</div>

<!--
Deel werkblad uit. Zet timer op 6 min.
Loop rond. Luister, verzamel sterke voorbeelden voor de plenaire ronde.

Als iemand vastloopt:
- "Wanneer staat jouw machine wel eens stil zonder dat het de bedoeling is?"
- "Wanneer zou hij sneller kunnen draaien?"

Plenair daarna 3 min — vang per vraag 1-2 voorbeelden, schrijf sleutelwoorden op flap-over.
-->

---

# Voorbeelden van de werkvloer

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Draait hij?
- Storing (matrijs vast)
- Omstellen (productwissel)
- Wachten op materiaal
- Opstarten / opwarmen

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Snel genoeg?
- Korte stops (sensor reset)
- Materiaal klemt even
- Slijtage — net wat trager
- Bewust teruggeschakeld

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Goed product?
- Afkeur (scheuren, maatfout)
- Herbewerking (nabramen)
- Opstartverlies (eerste stuks)
- Materiaalfout

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Drie verliessoorten — drie OEE-componenten.
</div>

<!--
Bespreek met de groep welke voorbeelden zij hebben opgeschreven.
Schrijf 1-2 sleutelwoorden per vraag op flap-over.
Maak de koppeling: deze drie voorbeeldgroepen zijn precies de drie OEE-componenten.
-->

---
layout: section
---

# Theoretiseren

## De formule en wat de tabel zegt

<!--
Overgang naar blok 3.
"De drie vragen krijgen nu een naam — en een formule."
-->

---
layout: center
class: text-center
---

# De formule

<div class="text-3xl mt-10 font-mono">
  <span class="text-blue-600 font-bold">B</span>
  <span class="opacity-60 mx-2">×</span>
  <span class="text-purple-600 font-bold">P</span>
  <span class="opacity-60 mx-2">×</span>
  <span class="text-green-600 font-bold">K</span>
  <span class="opacity-60 mx-3">=</span>
  <span class="text-amber-600 font-bold">OEE</span>
</div>

<div class="mt-12 grid grid-cols-3 gap-6 text-base">
  <div><span class="text-blue-600 font-bold">B</span>eschikbaarheid</div>
  <div><span class="text-purple-600 font-bold">P</span>restatie</div>
  <div><span class="text-green-600 font-bold">K</span>waliteit</div>
</div>

<div v-click class="mt-10 text-sm opacity-60">
  Drie percentages — vermenigvuldigen — één getal.
</div>

<!--
Schrijf op flap-over: B x P x K = OEE
Spreek de namen langzaam uit — Beschikbaarheid, Prestatie, Kwaliteit.

"Drie vragen — drie namen.
Beschikbaarheid = draait hij. Prestatie = snel genoeg. Kwaliteit = goed product.
Elk getal is een percentage. We vermenigvuldigen ze."
-->

---

# Voorbeeld: verpakkingslijn

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De situatie
- Dienst: 8 uur (480 min)
- Stilstand: 1 uur
- Snelheid: 90% van max
- Goed product: 98%

</div>

<div>

### De berekening
<v-clicks>

- B = 7 / 8 = **87,5%**
- P = **90%**
- K = **98%**
- OEE = 0,875 × 0,90 × 0,98

</v-clicks>

<div v-click class="mt-4 p-3 bg-amber-100 text-amber-900 rounded-lg text-center font-bold text-2xl">
  = 77%
</div>

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Drie keer een hoog getal — samen 77%. Dat is het multiplicatie-effect.
</div>

<!--
Reken hardop voor.
Tel langzaam: nul-komma-acht-zeven-vijf maal nul-komma-negen.
Reken-tempo is denk-tempo.

Stilte van 3 sec na het 77%-getal.
Het verschil tussen drie hoge cijfers en het multiplicaire eindresultaat is hét didactische scharnier.
-->

---

# Wat betekent het getal?

<div class="mt-6">

| OEE | Betekenis |
|---|---|
| **100%** | Perfecte productie — geen stilstand, max snelheid, nul afkeur |
| **85%** | World class — doel voor de meeste fabrieken |
| **60%** | Typisch voor veel bedrijven — verbeterruimte |
| **40%** | Veel productietijd verloren — actie nodig |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Loop in gedachten naar je gele kaartje.<br/>
  In welk gebied valt jouw schatting?
</div>

<!--
Geef de tabel door op de handout. Markeerstift hand.
Vraag: "Waar valt jouw schatting? Markeer dat gebied."

Niet duiden of het hoog of laag is — laat de deelnemer dat zelf doen.
-->

---
layout: quote
---

# OEE = spiegel

<div class="text-xl mt-6 opacity-80">
  Het laat zien <span class="font-bold">waar tijd verloren gaat.</span>
</div>

<div v-click class="mt-8 text-base opacity-70">
  Niet om <span class="font-bold">een persoon</span> te beoordelen.
</div>

<div v-click class="mt-8 text-sm opacity-50">
  Lage OEE = ergens in het systeem zit verlies.<br/>
  Niet: operator doet slecht werk.
</div>

<!--
Belangrijk moment. Maak expliciet dat OEE een verbeter-instrument is, geen afrekentool.

Als iemand sceptisch reageert: valideer eerst.
"Ik snap dat het zo voelt — in sommige fabrieken gebeurt dat ook.
Wij gebruiken het hier om verbeterkansen te zien."

Schrijf op flap-over: spiegel, geen rapport.
-->

---
layout: section
---

# Experimenteren

## Jouw eigen machine — ruwe schatting

<!--
Overgang naar blok 4.
"De afgelopen 28 minuten waren de theorie. Nu kijken we wat het voor JOUW lijn betekent."
-->

---

# Schat voor jouw eigen lijn

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-2xl font-bold text-blue-700 mb-3">Beschikbaarheid</div>
  <div class="text-sm opacity-70">Hoeveel % draait hij van de geplande tijd?</div>
  <div class="mt-4 text-3xl font-mono">___ %</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-2xl font-bold text-purple-700 mb-3">Prestatie</div>
  <div class="text-sm opacity-70">Hoe snel ten opzichte van het maximum?</div>
  <div class="mt-4 text-3xl font-mono">___ %</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-2xl font-bold text-green-700 mb-3">Kwaliteit</div>
  <div class="text-sm opacity-70">Hoeveel % is in een keer goed?</div>
  <div class="mt-4 text-3xl font-mono">___ %</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Vermenigvuldig de drie. Vergelijk met je gele kaartje.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · werkblad ruwe schatting
</div>

<!--
Inventarisatie-vraag eerst (1 min): "Wat is jouw soort lijn?"
Vang 4-5 antwoorden — niet bespreken, alleen verzamelen.

Zet timer op 6 min.

Bij twijfel:
- "Halfuur stil op 8 uur = 6%, dus beschikbaarheid 94%."
- "Vol gas of rek? 95% of 85%?"
- "Afkeur + herbewerking samen — promille of paar procent?"

Bevestig: ruwe schatting is genoeg.
-->

---
layout: center
class: text-center
---

# Vergelijk

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed">
  Geel kaartje = <span class="font-bold">buikgevoel</span><br/>
  Werkblad = <span class="font-bold">drie keer doorgerekend</span>
</div>

<div v-click class="mt-10 text-xl opacity-80">
  Wat valt je op?
</div>

<!--
Stilte. 10 seconden.

Vraag: "Wat valt op?"
Laat 2-3 deelnemers kort delen.

Vaak: "het is lager dan ik dacht."
Dat is het aha-moment. Bevestig: "Drie keer 90% is samen 73%. Dat is wat OEE zichtbaar maakt."
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Ga zoeken
<v-clicks>

- Loop langs het OEE-bord van jouw lijn
- Schrijf op: wat is de OEE?
- Wat zijn de drie onderliggende getallen?
- Vergelijk met je schatting van vandaag

</v-clicks>

</div>

<div>

### Geen bord?
<v-clicks>

- Vraag aan je teamleider:<br/>"zijn er ergens cijfers van mijn machine?"
- En de bonus:<br/>vraag een collega welk onderdeel híj denkt dat de grootste verliespost is
- Je gaat ontdekken dat collega's verschillende intuïties hebben

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: LO-002 over beschikbaarheid.

"In de volgende sessie bespreken we kort: wat heb je gevonden? Klopte je schatting?
Daarna gaan we dieper in op de eerste van de drie componenten."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Beschikbaarheid — hoeveel draait jouw machine echt?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Gemiddelde fase 1 vs gemiddelde fase 4 (verschil = leerwinst)
- Welke voorbeelden van stilstand werden genoemd? (input voor LO-002)
- Wie schatte heel hoog/laag? (kandidaten voor differentiatie)
-->
