---
theme: default
title: Drempelwaarden instellen — wanneer slaat het systeem alarm?
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over het bepalen, instellen en bijstellen van drempelwaarden
  voor sensoren met de vuistregel gemiddelde + 2x spreiding.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Drempelwaarden instellen

### Wanneer slaat het systeem alarm?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · CNC / draaibank / spuitgieten
</div>

<!--
Welkom. Vorige sessie hebben jullie je eigen basislijn gemeten (LO-201).
Vandaag: vanaf welke waarde slaat het systeem alarm? Dat ga je zelf bepalen.

Trigger: "Wie heeft basislijn-getallen meegenomen?"
Vang 1-2 reacties. Geen oordeel als niemand. "Vandaag krijg je oefendata."
-->

---
layout: section
---

# Ervaren

## Storingsquiz: 6 sensorgrafieken

<!--
Overgang naar blok 1.
"Per grafiek: normaal, waarschuwing of alarm? Geen rekenmachine — gebruik je gevoel."
-->

---
layout: center
class: text-center
---

# 6 grafieken op gevoel

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Per grafiek:<br/>
  <span class="font-bold">normaal</span>,
  <span class="font-bold">waarschuwing</span> of
  <span class="font-bold">alarm</span>?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Geen rekenmachine. Gebruik je gevoel.<br/>
  Schrijf op waarom je dat denkt.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01. Timer op 5 min.
Niet voorzeggen. De waarde zit in de variatie tussen oordelen.

Bij vastlopen: "Waar kijk je naar?"
Bij snel klaar: "Bij welke grafiek twijfelde je het meest? Waarom?"
-->

---
layout: section
---

# Reflecteren

## Hoe bepaalde JIJ de grens?

<!--
Overgang naar blok 2.
"Pak een buurman. Drie vragen op het werkblad."
-->

---
layout: center
class: text-center
---

# Bespreek in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">⚖️</div>
    <div class="text-lg font-bold text-blue-700">Waar verschilden jullie?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">🧭</div>
    <div class="text-lg font-bold text-purple-700">Hoe bepaalde jij de grens?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">⚠️</div>
    <div class="text-lg font-bold text-green-700">Te laag of te hoog — wat dan?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Gevoel is niet genoeg. Er is een rekenmethode nodig.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min duo · 2.5 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Timer op 4 min.
Loop rond. Luister naar concrete redeneringen.

Plenair (2.5 min):
- "Wie had moeite om de grens te bepalen? Wat maakte het lastig?"
- "Wat zou helpen om met meer zekerheid de grens te bepalen?"
  Mik op antwoord: "Een rekenmethode."

Schrijf op flap-over: "Gevoel is niet genoeg."
-->

---
layout: section
---

# Theoretiseren

## 4 stappen + voorbeeld Ahmed

<!--
Overgang naar blok 3. "Markeerstift erbij. Wat is voor jou nieuw?"
-->

---

# De 4 stappen

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-4xl mb-2">📏</div>
  <div class="text-lg font-bold text-blue-700">1. Meten</div>
  <div class="text-sm opacity-80 mt-2">Minimaal 100 cycli onder normale omstandigheden.</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-4xl mb-2">🧮</div>
  <div class="text-lg font-bold text-purple-700">2. Berekenen</div>
  <div class="text-sm opacity-80 mt-2">Gemiddelde + 2x spreiding = drempel.</div>
</div>

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-4xl mb-2">🚦</div>
  <div class="text-lg font-bold text-amber-700">3. Instellen</div>
  <div class="text-sm opacity-80 mt-2">Waarschuwing op 80%. Alarm op 100%.</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-4xl mb-2">🔄</div>
  <div class="text-lg font-bold text-green-700">4. Bijstellen</div>
  <div class="text-sm opacity-80 mt-2">1 week draaien. Valse alarmen tellen. Aanpassen.</div>
</div>

</div>

<div v-click class="mt-6 p-4 bg-slate-50 rounded-lg text-center">

### De vuistregel
<span class="text-2xl font-bold">drempel = gemiddelde + (2 × spreiding)</span><br/>
<span class="text-sm opacity-70">vangt 95% van de normale variatie</span>

</div>

<!--
Loop de 4 stappen één voor één langs.
Wijs naar de flap-over met de formule.

Bij vraag over standaarddeviatie / sigma: gebruik woord 'spreiding'.
"Gemiddeld hoeveel wijken waarden af. Niet ingewikkelder."
-->

---

# Voorbeeld: Ahmed op de draaibank

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De berekening
<v-clicks>

- 100 cycli gemeten
- Gemiddelde: **0.3 mm/s**
- Spreiding: **0.1 mm/s**
- Drempel: 0.3 + (2 × 0.1) = **0.5 mm/s**

</v-clicks>

</div>

<div>

### Wat ging er mis?
<v-clicks>

- Week 1: **12 valse alarmen**
- Bij gereedschapwissel: piek tot 0.6
- Drempel te laag

</v-clicks>

</div>

</div>

<div v-click class="mt-6 p-4 bg-blue-50 rounded-lg">

### Wat deed Ahmed?
- Drempel naar **0.8 mm/s** + vertraging 10 sec.
- Alarm pas als waarde langer dan 10 sec boven drempel.
- Resultaat: **1 vals per week**.
- En: detecteerde slijtend lager **2 dagen** voor geplande vervanging.

</div>

<div v-click class="mt-4 text-center text-base font-bold opacity-80">
  De eerste drempel is bijna nooit goed. Bijstellen IS het werk.
</div>

<!--
Vertel langzaam. Concreet. Houd ÉÉN voorbeeld vast.

Na het Ahmed-verhaal: stilte van 3 sec. Laat het landen.

"Twee dingen om te onthouden:
 - eerste drempel is bijna nooit goed
 - bijstellen is geen falen, dat IS het werk."
-->

---
layout: center
class: text-center
---

# Vragen?

<div class="text-base mt-6 opacity-70 max-w-xl mx-auto">
  Over de 4 stappen of over Ahmed.<br/>
  Andere vragen op de parkeerlijst.
</div>

<!--
1.5 min. Beantwoord kort.
Afdwaalende vragen op flap-over "parkeerlijst".
-->

---
layout: section
---

# Experimenteren

## Echte data — bereken, stel in, plan evaluatie

<!--
Overgang naar blok 4. 15 min. Coachen, niet voorzeggen.
-->

---

# Jouw opdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Op het werkblad
<v-clicks>

- 100 metingen van een trillingssensor
- Bereken het gemiddelde
- Bereken de spreiding
- Bepaal je drempel

</v-clicks>

</div>

<div>

### Stel in en plan
<v-clicks>

- Waarschuwing op 80%
- Alarm op 100%
- Schrijf actieplan
- Evaluatiedatum: over 2 weken

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min individueel · 3 min plenair · wb-04-experimenteren
</div>

<!--
Werkblad wb-04 (bevat 100 metingen). Timer op 10 min.
Coach-modus: niet voorzeggen. Berekenfouten = leermomenten.

Bij berekening fout: "Reken het nog eens hardop."
Bij snel klaar: "En als je drempel te laag blijkt — wat doe je dan?"

Plenair 3 min: vraag 2-3 deelnemers
- "Wat was jouw drempel?" + check tegen formule
- "Wanneer ga je evalueren?" — concrete datum
-->

---

# Deze week — jouw transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Doe dit
<v-clicks>

- Kies één sensor op **jouw** machine
- Gebruik je basislijn uit LO-201 OF meet 100 cycli
- Bereken de drempel
- Stel hem in (vraag hulp technische dienst als nodig)

</v-clicks>

</div>

<div>

### Evaluatiemoment
<v-clicks>

- Plan **over 2 weken**
- Tel valse alarmen
- Tel gemiste problemen
- Stel bij — drempel omhoog of omlaag

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg text-center">

### En vraag een collega
Doe hetzelfde voor een andere sensor. Vergelijk jullie aanpak. Wie kreeg de minste valse alarmen?

</div>

<!--
Schrijf afspraak op werkblad: datum + collega als sparringpartner.
LO-202 → LO-205: drempelwaarden worden anomaliescores in verkeerslichtmodel.

Loop rond, check dat het ingevuld is.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Anomaliescores naar onderhoud — LO-205</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Wie heeft welke sensor + drempel toegezegd? (volgmoment LO-205)
- Wie was sceptisch? (1-op-1 in volgende sessie)
- Bron: AIMM Competentieframework v0.1 (drempelwaarden).
-->
