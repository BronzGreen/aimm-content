---
theme: default
title: Datakwaliteit beoordelen — drie checks die je zelf kunt doen
info: |
  ## Data Literacy Module 2 — Train
  Workshop-blok: drie checks (volledigheid, consistentie, actualiteit) op een productiedataset.
  Doelgroep: operators MBO-3, 30 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Datakwaliteit beoordelen

### Drie checks die je zelf kunt doen

<div class="mt-12 text-sm opacity-60">
  Data Literacy Module 2 (Train) · Workshop-blok · 30 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 30 minuten leer je in drie stappen of data te vertrouwen is.
Geen theorie eerst — je gaat het direct doen op een dataset uit een spuitgieterij.

Open warm: "Wie heeft weleens gewerkt met data die niet klopten?"
Vang 1-2 reacties. Reageer alleen met "herkenbaar". Niet bespreken.
-->

---
layout: center
class: text-center
---

# Drie checks

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-5xl mb-3">📋</div>
    <div class="text-xl font-bold text-blue-700">Volledigheid</div>
    <div class="text-sm opacity-70 mt-2">Is de dataset compleet?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-5xl mb-3">⚖️</div>
    <div class="text-xl font-bold text-purple-700">Consistentie</div>
    <div class="text-sm opacity-70 mt-2">Kloppen de waarden?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-5xl mb-3">⏰</div>
    <div class="text-xl font-bold text-green-700">Actualiteit</div>
    <div class="text-sm opacity-70 mt-2">Hoe oud is de data?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Drie geheugenankers. Werkt op elke dataset.
</div>

<!--
Drie checks groot in beeld. Niet uitleggen — alleen benoemen.
"Vandaag oefen je deze drie. Geen theorie eerst."
-->

---
layout: section
---

# Ervaren

## Doe de drie checks zelf

<!--
Overgang naar fase 1.
"Voor je ligt productiedata van een spuitgietmachine. 25 batches.
Pak werkblad 1. Tien minuten. Doe alle drie de checks."
-->

---

# Voorbeelddataset — spuitgieten

<div class="mt-4 text-sm">

| Batch | Datum | Cyclustijd (s) | Afkeur (%) | Operator |
|---|---|---|---|---|
| LOT-2026-0411 | 22-04 | 38 | 3,2 | Karim |
| LOT-2026-0412 | 22-04 | — | 2,8 | Sven |
| LOT-2026-0413 | 23-04 | 41 | **200** | Karim |
| LOT-2026-0414 | 23-04 | 39 | 3,5 | Mariska |
| LOT-2026-0415 | 24-04 | — | 2,9 | S. de Boer |
| ... | ... | ... | ... | ... |

</div>

<div v-click class="mt-6 text-base opacity-70 text-center">
  Wat valt je op? Tel, kijk, vergelijk.<br/>
  Werkblad 1 — 8 minuten — individueel.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · individueel · wb-01-ervaren
</div>

<!--
Deel werkblad 1 + dataset uit. Zet timer op 8 min.
Loop rond. Coach met vragen, geef GEEN antwoorden.

Bij vastlopers: "Tel even kolom 3 — hoeveel cellen zijn leeg?"
Concrete telopdracht haalt de drempel weg.

NIET zeggen: "die afkeur 200% is duidelijk een typfout."
WEL: "Wat denk je dat hier gebeurd is?"
-->

---
layout: section
---

# Reflecteren

## Wat zag je? Wat was lastig?

<!--
Overgang naar fase 2.
"Nu vergelijk je met je buurman. Werkblad 2 — drie vragen."
-->

---

# Wat viel op?

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Volledigheid
- Lege cellen tellen
- Welke kolom mist data?
- Hoeveel procent leeg?

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Consistentie
- Eenheden vergelijken
- Buitenproporties zoeken
- Typfouten herkennen

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Actualiteit
- Datum laatste rij
- Past dat bij je beslissing?
- Hoe oud mag data zijn?

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Bespreek met je buurman: wat zag jij, wat zag hij?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · in tweetallen · wb-02-reflecteren
</div>

<!--
Deel werkblad 2 uit. Zet timer op 5 min.
Loop rond. Verzamel 2-3 sterke voorbeelden voor de plenaire ronde.

Plenair daarna 2 min — vang per check 1-2 voorbeelden.
Schrijf op flap-over alleen wat de groep zegt.
-->

---

# Plenair — sleutelwoorden op de flap-over

<div class="mt-6">

> **Vul met de groep in. Schrijf op de flap-over.**

</div>

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Volledigheid
- _________________
- _________________
- _________________

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Consistentie
- _________________
- _________________
- _________________

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Actualiteit
- _________________
- _________________
- _________________

</div>

</div>

<!--
Vraag per check een voorbeeld:
- "Wat viel op bij volledigheid?" — 1-2 voorbeelden
- "Wat bij consistentie?" — 1-2
- "Wat bij actualiteit?" — 1-2

Tel innerlijk tot 5 na elke vraag. Stilte trekt antwoorden los.
Schrijf alleen wat de groep zegt — niet wat jij denkt.
-->

---
layout: section
---

# Theoretiseren

## Vuistregels en stoplicht

<!--
Overgang naar fase 3.
"Jullie hebben de drie checks net zelf gedaan. Nu krijgen ze een naam."
-->

---

# Drie vuistregels

<div class="grid grid-cols-1 gap-3 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Volledigheid
**Tel lege cellen per kolom.** Meer dan **10% leeg = oranje**. Meer dan **25% leeg = rood**.

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Consistentie
**Klopt de waarde met de eenheid?** Mengsel van eenheden? Buitenproporties (200% afkeur)? Typfouten?

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Actualiteit
**Hoe oud is het laatste record?** Past dat bij je beslissing? Dagelijks rapport vraagt verse data.

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Drie geheugenankers — drie vuistregels.
</div>

<!--
Verwijs ELKE keer terug naar wat de groep zelf heeft genoemd.
"Karim zei net: lege cellen. Dat is volledigheid."
Maakt het framework hun eigen ontdekking.

Markeerstiften uitdelen — laat ze meemarkeren in de handout.
-->

---

# Voorbeeld: spuitgiet-dataset doorgerekend

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De observaties
<v-clicks>

- 3 lege cellen in cyclustijd (12%)
- Twee batches afkeur 200% — typfout
- Operator-naam soms voornaam, soms achternaam
- Laatste rij van vorige week

</v-clicks>

</div>

<div>

### De stoplichten
<v-clicks>

- Volledigheid: **oranje** (12% leeg)
- Consistentie: **oranje** (typfouten)
- Naam-consistentie: **oranje**
- Actualiteit: **oranje** voor dagelijks

</v-clicks>

<div v-click class="mt-4 p-3 bg-amber-100 text-amber-900 rounded-lg text-center font-bold">
  Eindoordeel: oranje
</div>

</div>

</div>

<div v-click class="mt-4 text-center text-sm opacity-70 italic">
  Bruikbaar mits met aandacht — meld het voorbehoud in je conclusie.
</div>

<!--
Reken hardop voor. Wijs naar de dataset.
"Drie lege cellen op 25 = 12%. Dat is meer dan 10%. Dus oranje."

Het stoplichtsysteem is bewust eenvoudiger dan ++/+/-/--.
Voor MBO-3 werkt minder onderscheid beter.
-->

---
layout: center
class: text-center
---

# Stoplichtsysteem

<div class="grid grid-cols-3 gap-6 mt-8">
  <div class="p-6 bg-green-100 rounded-xl">
    <div class="text-5xl mb-3">🟢</div>
    <div class="text-xl font-bold text-green-700 mb-2">Groen</div>
    <div class="text-sm opacity-80">Bruikbaar zonder<br/>voorbehoud</div>
  </div>
  <div class="p-6 bg-amber-100 rounded-xl">
    <div class="text-5xl mb-3">🟠</div>
    <div class="text-xl font-bold text-amber-700 mb-2">Oranje</div>
    <div class="text-sm opacity-80">Bruikbaar mits<br/>met aandacht</div>
  </div>
  <div class="p-6 bg-red-100 rounded-xl">
    <div class="text-5xl mb-3">🔴</div>
    <div class="text-xl font-bold text-red-700 mb-2">Rood</div>
    <div class="text-sm opacity-80">Niet gebruiken —<br/>eerst aanvullen</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Bij oranje: meld het voorbehoud expliciet in je conclusie.
</div>

<!--
Belangrijk: oranje is GEEN excuus om data te negeren.
Het is een verplichting om het voorbehoud te benoemen.

"Onze afkeur is gemiddeld 3% deze week — let op: cyclustijd-data is 12% incompleet."
Dat is een eerlijke conclusie.
-->

---
layout: section
---

# Experimenteren

## Jouw eigen werkvloer

<!--
Overgang naar fase 4.
"De afgelopen 25 minuten waren oefening. Nu ga je het toepassen op je eigen data."
-->

---

# Actieplan eigen werkvloer

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen
<v-clicks>

- **Welke dataset** ga ik checken?
- **Wanneer** doe ik het?
- **Wat doe ik** met een rood stoplicht?
- **Met wie** deel ik de uitkomst?

</v-clicks>

</div>

<div>

### Coach-vragen
<v-clicks>

- Welke data zie je elke dag?
- Voor of na de ploegwissel?
- Bij rood: wie kan helpen?
- Teamleider? Collega?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel + peer-check · wb-04-experimenteren
</div>

<!--
Deel werkblad 4 uit. Zet timer op 3 min individueel + 1 min peer-check.

Coach met vragen:
- "Welke data gebruik je het vaakst om een beslissing te nemen?"
- "Wanneer is dat morgen mogelijk — voor of na de ploegwissel?"

Bij vaag plan: "Welke dataset, welke dag, welk uur?"
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Doe het echt
<v-clicks>

- Voer je actieplan uit
- Drie checks op de gekozen dataset
- Stoplicht-oordeel: groen / oranje / rood
- Bespreek met je teamleider

</v-clicks>

</div>

<div>

### Verder?
<v-clicks>

- Module 3 — lo-data-lit-302:<br/>audit op je hele afdeling
- Vraag een collega om dezelfde checks
- Vergelijk de scores

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: lo-data-lit-203 over data-presentatie.

"In de volgende sessie bespreken we kort: welke check verraste je het meest?
Wie heeft een rood stoplicht gevonden? Wat doe je ermee?"
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">data presenteren — van getal naar grafiek</span>
</div>

<div class="mt-6 text-sm opacity-60">
  Verdiepingsroute: lo-data-lit-302 — audit op je eigen afdeling
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Data Literacy Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke check viel het meest op? (input voor lo-data-lit-203)
- Wie scoorde alles groen? (mogelijk te oppervlakkig — kandidaat voor coaching)
- Wie scoorde alles rood? (mogelijk verlamd — kandidaat voor extra steun)
-->
