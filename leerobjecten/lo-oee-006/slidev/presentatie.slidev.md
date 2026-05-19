---
theme: default
title: De zes grote verliezen — waar gaat productietijd verloren?
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over het zes-grote-verliezen framework + Pareto eigen lijn.
  Doelgroep: operators MBO-3, 45 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# De zes grote verliezen

### Waar gaat productietijd verloren?

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok 6 — afsluiter · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Vorige sessie hebben we OEE doorgerekend.
Daarvoor: drie componenten apart.

Nu sluiten we module 1 af met structuur — alle verliezen op een rij.
Maar eerst: jullie maken je eigen indeling.
Daarna kijken we hoe dat zich verhoudt tot wat de boeken zeggen.
-->

---
layout: center
class: text-center
---

# Sorteer de kaartjes

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  12 gebeurtenissen uit de werkvloer.<br/>
  Maak <span class="font-bold">je eigen indeling</span> — zoveel stapels als jullie willen.
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Geef elk stapeltje een naam. Geen goed of fout.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6,5 min · in tweetallen · 12 kaartjes
</div>

<!--
IK DOE eerst — pak één kaartje, denk hardop.
"Matrijswissel — wissel-actie, eigen stapeltje."

Zet timer op 6,5 min. Loop rond.
Stel alleen vragen, geen oordeel.

Bij vraag "is dit goed?" — "Vertel me waarom JIJ deze hier legt."
-->

---
layout: section
---

# Reflecteren

## Wat zien we als groep?

<!--
Overgang naar blok 2.
"Pen neer. Hoeveel stapels heb je? Welke namen?"
-->

---

# Vergelijk indelingen

<div class="mt-6 text-sm">

| Tweetal | Aantal stapels | Namen |
|---------|----------------|-------|
| 1 | _ | _ |
| 2 | _ | _ |
| 3 | _ | _ |
| 4 | _ | _ |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Welke kaartjes belandden meestal bij elkaar?<br/>
  Welke werden anders ingedeeld?
</div>

<!--
Vraag elk tweetal kort: "Hoeveel stapels? Welke namen?"
Schrijf op het whiteboard NAAST elkaar.

Patroon-zoeken:
- "Welke kaartjes belandden meestal bij elkaar?" (k01+k05+k08 = wissel)
- "Welke kaartjes werden anders ingedeeld?" (k06 slijtage, k09 opwarmtijd)

Schrijf overeenkomsten op flap-over.
-->

---
layout: center
class: text-center
---

# Patroon herkenbaar?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Tussen jullie groepen zit veel overlap.<br/>
  Zoals: <span class="font-bold">wissel-cluster, storing-cluster, kort-stop-cluster.</span>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-md mx-auto">
  Het officiële framework heeft jullie indeling al opgeschreven.<br/>
  Hoeveel ervan zit al in jullie sortering?
</div>

<!--
"Jullie hebben dit grotendeels zelf al ontdekt.
Klein verschil tussen de groepen, sterke overlap.
We gaan nu naar het officiële framework — kijk hoeveel ervan al in jullie indeling zit."

Discovery-learning effect — bewust opbouwen.
-->

---
layout: section
---

# Theoretiseren

## Het officiële framework

<!--
Overgang naar blok 3.
-->

---

# De zes grote verliezen

<div class="grid grid-cols-3 gap-4 mt-6">

<div class="p-4 bg-blue-50 rounded-lg">

### B — Beschikbaarheid
<v-clicks>

1. **Storingen**
2. **Omstellen**

</v-clicks>

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### P — Prestatie
<v-clicks>

3. **Korte stops**
4. **Snelheidsverlies**

</v-clicks>

</div>

<div class="p-4 bg-green-50 rounded-lg">

### K — Kwaliteit
<v-clicks>

5. **Opstartverlies**
6. **Productieafkeur**

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-sm opacity-60">
  Bron: Nakajima (1988), TPM-traditie. Wereldwijd gebruikt.
</div>

<!--
"Dit framework heet de Zes Grote Verliezen — TPM-traditie, wereldwijd gebruikt."

"Kijk naar jullie indeling op het whiteboard. Wat zien jullie?"
Wacht. Verwacht: "Wij hadden er vier of vijf, en die kloppen ongeveer."
-->

---

# Welk kaartje hoort waar?

<div class="mt-4 text-sm">

| # | Verlies | OEE | Kaartjes uit jullie sortering |
|---|---------|-----|-------------------------------|
| 1 | **Storingen** | B | k02 hydrauliek |
| 2 | **Omstellen** | B | k01 matrijs, k05 gereedschap, k08 kalibratie |
| 3 | **Korte stops** | P | k03 sensor, k07 materiaal, k11 vals alarm |
| 4 | **Snelheidsverlies** | P | k06 slijtage |
| 5 | **Opstartverlies** | K | k04 eerste stuks |
| 6 | **Productieafkeur** | K | k10 breukmaat, k12 oppervlaktefout |

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  k09 (opwarmtijd) — twijfelkaart. Daarover zo.
</div>

<!--
Behandel verlies voor verlies.
Per verlies: "Wie had dit kaartje hier?" Korte handen omhoog.

k09 (opwarmtijd) bewaar voor volgende slide.
-->

---
layout: center
class: text-center
---

# Twijfelkaart — k09 opwarmtijd

<div class="text-xl mt-10 max-w-2xl mx-auto leading-relaxed">
  Sommige fabrieken: <span class="font-bold text-blue-600">opstarten = stilstand → B</span><br/>
  Andere fabrieken: <span class="font-bold text-green-600">opstartverlies = eerste stuks → K</span>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Beide goed te beargumenteren.<br/>
  <span class="font-bold">Kies als fabriek een lijn — en houd hem aan.</span>
</div>

<!--
Maak conventie expliciet.
"k09 — opwarmtijd 25 min. Sommige fabrieken zetten dit onder beschikbaarheid (opstarten = stilstand). Andere onder kwaliteit (opstartverlies = eerste stuks). Beide goed te beargumenteren. Kies een lijn — en houd hem aan."

Niet oplossen — bewust dubbelzinnig.
-->

---

# Per verlies een aanpak

<div class="grid grid-cols-2 gap-4 mt-6 text-sm">

<div class="p-3 bg-red-50 rounded-lg">

**1. Storingen**<br/>
→ Preventief / predictive maintenance

</div>

<div class="p-3 bg-amber-50 rounded-lg">

**2. Omstellen**<br/>
→ SMED (Shingo)

</div>

<div class="p-3 bg-purple-50 rounded-lg">

**3. Korte stops**<br/>
→ Poka-Yoke + registratie

</div>

<div class="p-3 bg-blue-50 rounded-lg">

**4. Snelheidsverlies**<br/>
→ Slijtage-monitoring

</div>

<div class="p-3 bg-green-50 rounded-lg">

**5. Opstartverlies**<br/>
→ Voorverwarmen + eerste-stuks-procedure

</div>

<div class="p-3 bg-teal-50 rounded-lg">

**6. Productieafkeur**<br/>
→ SPC (Wheeler / Deming)

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Vandaag: herkennen. Module 2 (Train): aanpakken.
</div>

<!--
Niet uitwerken. Bewaak scope.
"Vandaag: herkennen. Module 2: aanpakken."

MBO-4: noem boekreferenties (Shingo, Wheeler, Deming).
-->

---
layout: section
---

# Experimenteren

## Pareto van mijn eigen lijn

<!--
Overgang naar blok 4.
"Theorie staat. Nu jouw eigen lijn — welke verliezen zijn bij jou het grootst?"
-->

---

# Voorbeeld: verpakkingslijn

<div class="mt-6">

| Verlies | Aandeel |
|---------|---------|
| **Omstellen** | 35% |
| **Storingen** | 25% |
| **Korte stops** | 20% |
| **Snelheidsverlies** | 10% |
| **Opstartverlies** | 5% |
| **Productieafkeur** | 5% |

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Bij jouw lijn kan het anders zijn. Schat.
</div>

<!--
Toon verpakkingsvoorbeeld uit kennisobject.
"Voorbeeld van een verpakkingslijn — omstellen op 1, storingen op 2.
Bij jouw lijn kan het anders zijn. Schat."
-->

---

# Jouw eigen Pareto

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Top-3 voor jouw lijn
<v-clicks>

1. Welk verlies is het grootst?
2. Op nummer 2?
3. Op nummer 3?

</v-clicks>

</div>

<div>

### Per top-3
<v-clicks>

- Markeer één concrete oorzaak
- Welk verlies zou je het EERST aanpakken?
- Waarom?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · werkblad eigen Pareto
</div>

<!--
Zet timer op 8 min.

Help bij blokkades:
- "Wat zie je het meest in een week — storing of wissel?"
- "Hoeveel keer per week wissel je? Hoe lang?"
- "Welke korte stops zie je elke dienst?"

Bevestig: schatten is genoeg.
-->

---
layout: center
class: text-center
---

# Welk verlies is bij jou nummer 1?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Handen omhoog per verlies.<br/>
  We kijken naar het patroon van de groep.
</div>

<!--
Plenaire deel-ronde — 2,5 min.
Tel handen per verlies.
Schrijf op flap-over: groeps-Pareto.

Vraag 2-3 deelnemers: "Welk verlies zou je het eerst willen aanpakken? Waarom?"
-->

---

# Deze week + module 2

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Houd een week-logboek
<v-clicks>

- Top-3 verliezen op jouw lijn
- Per voorval: welk type
- Hoe lang
- Vermoede oorzaak

</v-clicks>

</div>

<div>

### Volgende module
<v-clicks>

- Module 2: **Train**
- Aanpakken van top-1 verliezen
- SMED, Poka-Yoke, SPC, preventief
- Praat met de monteur of TD'er

</v-clicks>

</div>

</div>

<!--
Sluit module 1 af.
"In module 2 (Train) gaan we juist die top-1-verliezen aanpakken — met SMED, Poka-Yoke of preventief onderhoud."

Module 1-afsluiting: badge aimm-oee-module-1-gebruik.
-->

---
layout: end
---

# Module 1 — Klaar

<div class="mt-8 text-base opacity-70">
  Volgende: <span class="font-bold">Module 2 — Train</span><br/>
  <span class="text-sm opacity-60">van herkennen naar verbeteren</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik) — afsluiter
</div>

<!--
Bedank de groep.
Module 1 (Gebruik) is afgerond. Badge toekennen aan deelnemers die alle 6 LOs hebben afgerond.

Notitie:
- Welke verliezen kwamen het vaakst op nummer 1? (input voor module 2 keuzes)
- Welke deelnemers hadden moeite met framework-koppeling?
- Hoe goed kwam de spontane indeling overeen met het officiële framework?
-->
