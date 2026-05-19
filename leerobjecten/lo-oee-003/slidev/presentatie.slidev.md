---
theme: default
title: Prestatie — draait de machine op volle snelheid?
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over korte stops, snelheidsverlies en de verborgen fabriek.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Prestatie

### Draait de machine op volle snelheid?

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok 3 · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. In LO-002 hebben we beschikbaarheid behandeld.
Eén kaartje (sensor reset, 90 sec) parkeerden we — die komt nu terug.

Korte stops vallen onder PRESTATIE, niet beschikbaarheid.
We gaan vandaag tellen wat er werkelijk gebeurt op een lijn.
-->

---
layout: center
class: text-center
---

# Stop-spotter

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  5 minuten video.<br/>
  Elke keer dat de lijn <span class="font-bold">hapert</span>, <span class="font-bold">stopt</span> of <span class="font-bold">vertraagt</span>: een streepje.
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Geen overleg. Eigen telling.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · turflijst
</div>

<!--
Deel werkblad uit. "Geen overleg met je buurman."

IK DOE — eerste 30 sec mee tellen.
"Daar — sensor flikkert, machine staat 3 seconden — turfje."
"En daar — net iets langzamer dan eerst — twijfel-streepje."

Stop video. "Geen oordelen — alleen turven. We gaan door tot 5 minuten."

Speel video volledig af. Sta achterin, buiten zicht.
-->

---
layout: section
---

# Reflecteren

## Wat zag jij — en wat zag je buurman?

<!--
Overgang naar blok 2.
"Pen neer. Hoeveel streepjes? Schrijf bovenaan. Onthou."
-->

---

# Vergelijk + reken door

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Buurman-check
<v-clicks>

- Hoeveel zag jij?
- Hoeveel zag je buurman?
- Wat zag de een wel, de ander niet?

</v-clicks>

</div>

<div>

### Schaal-rekening
<v-clicks>

- 5 min video → 8 uur dienst?
- × 5 dagen → één week?
- × 20 sec gemiddeld per stop?
- Hoeveel uur per week?

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Niet "wie heeft gelijk" — wel: <span class="font-bold">verschillende waarnemers zien verschillende dingen.</span>
</div>

<!--
Plenaire inventarisatie: "Wie heeft de minste tellingen? Wie de meeste?"
Schrijf spreiding op flap-over.

Schaalrekening — laat de groep rekenen:
- "15 stops in 5 min × 96 = 1440 stops/dienst" (gedachte-experiment)
- Realistisch: 30 stops × 20 sec = 10 min/dienst = 50 min/week

"Verbazing in de buik? Dat is precies de verborgen fabriek."
-->

---
layout: quote
---

# 50 minuten per week

<div class="text-xl mt-6 opacity-80">
  Bij <span class="font-bold">één lijn</span>, <span class="font-bold">één type stop</span>.
</div>

<div v-click class="mt-8 text-base opacity-60">
  En dat is alleen wat je <span class="italic">teld</span>. Wat je niet zag telt nog mee.
</div>

<!--
Pick-and-place voorbeeld uit het kennisobject.
Laat het inzinken met 3 sec stilte.
-->

---
layout: section
---

# Theoretiseren

## Twee verliestypen

<!--
Overgang naar blok 3.
-->

---

# Korte stops

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat het is
<v-clicks>

- Machine stopt — meestal < 5 min
- Start weer op
- Vaak operator-handeling nodig

</v-clicks>

</div>

<div>

### Voorbeelden
<v-clicks>

- Sensor flikkert — reset
- Materiaal klemt — losmaken
- Product valt verkeerd
- Vals alarm

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Probleem: <span class="font-bold">worden meestal niet geregistreerd</span> — maar tellen op.
</div>

<!--
"Wie herkent dit op zijn lijn?" Vang 2-3 voorbeelden.
Maak link met k08 uit LO-002 (sensor reset 90 sec) — dat valt hieronder.
-->

---

# Snelheidsverlies

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat het is
<v-clicks>

- Machine draait
- Maar langzamer dan ideaal
- Niemand staat stil
- Niemand merkt het

</v-clicks>

</div>

<div>

### Oorzaken
<v-clicks>

- Slijtage onderdelen
- Slechte grondstof
- Bewust teruggeschakeld (trillingen)
- Niet goed afgesteld

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Hoe weet je hoe snel hij theoretisch kan? Daar gaan we in LO-005 op in.
</div>

<!--
"Snelheidsverlies herken je alleen als je weet wat de ideale cyclustijd is.
Daar gaan we in LO-005 op in."

Bewust frustrerend punt — niet oplossen, bewaar voor LO-005.
-->

---

# Wat zie je — en wat niet?

<div class="mt-6">

| Verliestype | Zichtbaar? | Typisch |
|---|---|---|
| **Storingen** | Ja — iedereen ziet het | 5-15% |
| **Korte stops** | Nauwelijks | 5-10% |
| **Snelheidsverlies** | Nee | 5-15% |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Het meest sluipend? <span class="font-bold">Snelheidsverlies.</span><br/>
  De machine draait gewoon — niemand merkt het.
</div>

<!--
Tabel als anker — laat hem op het scherm staan tijdens fase 4.
-->

---
layout: center
class: text-center
---

# De verborgen fabriek

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed">
  Wat de machine <span class="font-bold">zou kunnen</span> minus wat hij <span class="font-bold">echt doet</span>.
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-md mx-auto">
  Geen nieuwe machine. Geen extra ploeg.<br/>
  <span class="font-bold">Capaciteit die je al hebt.</span>
</div>

<!--
Hoofdconcept van het LO. Stilte van 3 sec.

"Welke korte stops gebeuren op jouw lijn die jullie nu nooit registreren?"
1-2 deelnemers kort delen.
-->

---
layout: section
---

# Experimenteren

## Mijn verborgen fabriek

<!--
Overgang naar blok 4.
-->

---

# Plan jouw turfsessie

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Welk tijdslot?
<v-clicks>

- Eerste uur na opstart?
- Na de pauze?
- Eind van de ochtend?
- Kies wat voor jou werkt

</v-clicks>

</div>

<div>

### Wat schrijf je op?
<v-clicks>

- Je verwachting (vooraf)
- Streepje per korte stop
- "Voelt traag" markeren
- Aan het eind: tellen + doorrekenen

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · actieplan
</div>

<!--
Inventarisatie van tijdslots — vang 4-5 voorbeelden, niet bespreken.

Zet timer op 6 min.

Help bij blokkades:
- "Wat verwacht je qua aantal stops?"
- "Welk tijdslot?"

Bevestig: klein beginnen mag.
-->

---
layout: center
class: text-center
---

# Welk tijdslot, hoeveel verwacht?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Eén zin per persoon.
</div>

<!--
Korte deel-ronde — 1 min 30.
3-4 deelnemers, max 30 sec per persoon.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Turf je verborgen fabriek
<v-clicks>

- Eén tijdslot van 30-60 min
- Streepje per korte stop
- "Voelt traag" markeren
- Reken door naar dienst + week

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Praat met de monteur of TD'er
- Over één structureel terugkerende stop
- Vraag: "Is hier iets aan te doen?"
- Vaak blijken oplossingen kleiner dan gedacht

</v-clicks>

</div>

</div>

<!--
Sluit af.
Volgende workshop: LO-004 over kwaliteit — afkeur, herbewerking, opstartverlies.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Kwaliteit — hoeveel is in een keer goed?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Notitie voor jezelf:
- Spreiding van tellingen (laag - hoog)
- Welke voorbeelden van korte stops genoemd? (input voor LO-005 worked example)
- Welke deelnemers waren het meest verrast?
-->
