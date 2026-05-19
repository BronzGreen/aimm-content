---
theme: default
title: Common cause vs special cause variatie
info: |
  ## SPC Module 1 — Gebruik
  Workshop-blok over het herkennen van variatie-types in productiedata.
  Doelgroep: operators MBO-3, 50 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Common of special?

### Wanneer moet je ingrijpen — en wanneer niet?

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. In de komende 50 minuten leer je iets dat je waarschijnlijk je hele werkende leven gaat helpen:
het verschil zien tussen wanneer je iets aan je machine moet doen, en wanneer je beter even niets kunt doen.

[Open warm op] "Wie van jullie heeft wel eens een meting gedaan en gedacht: dat klopt niet?"
Vang 2-3 reacties. Reageer alleen met "herkenbaar". Géén oordeel.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Voorbeeldcasus

Spuitgietmachine — onderdeelgewicht.

<v-clicks>

- **Normaal bereik:** 99,8 – 100,2 g
- **Vandaag gemeten:** 100,1 g
- **Wat doe je?**

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">⚙️</div>
    <div class="text-2xl font-mono font-bold text-amber-600">100,1 g</div>
    <div class="text-sm opacity-60 mt-2">één meting</div>
  </div>
</div>

<!--
Worked example — IK DOE.
Denk hardop:
- "Wat zie ik? Eén meting van 100,1 gram."
- "Wat is het normale patroon? 99,8 tot 100,2."
- "Is er iets ánders gebeurd? Niks. Alleen één meting binnen het normale bereik."
- "Mijn antwoord: common cause. Niets doen."

Schrijf op flip-over: "Eén waarde binnen het normale bereik = common cause."
Tempo: rustig. Tel innerlijk tot 2 na elke vraag.
-->

---
layout: center
class: text-center
---

# 🟢 Werkblad — Storingsquiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  10 casussen uit jouw werkomgeving.<br/>
  Per casus: <span class="font-bold text-green-600">common</span>, <span class="font-bold text-red-600">special</span>, of <span class="font-bold text-amber-500">vraagteken</span>.
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Twijfel is geen fout antwoord — twijfel is leerstof.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 minuten · individueel · pen
</div>

<!--
Deel wb-01-storingsquiz uit (1 min).
"Tien casussen. Per casus omcirkel je common, special, of een vraagteken bij twijfel.
Dat vraagteken is geen fout antwoord — het is de meest waardevolle in deze quiz."

Zet timer op 6 min. Loop rond. Beantwoord praktische vragen, GEEN inhoudelijke.
Als iemand vraagt "is dit common of special?": zeg "Dat is precies wat je nu zelf moet wegen."

Aan het einde: "Pen neer. Hoe vaak heb je een vraagteken gezet? Dat aantal is voor jou belangrijk — onthou het."
-->

---
layout: section
---

# Reflecteren

## Waar twijfelde je?

<!--
Overgang naar blok 2 (reflecteren).
We gaan eerst in tweetallen, dan plenair stemmen.
-->

---
layout: two-cols-header
---

# Eerst: buurman-check

::left::

### Wat doen jullie samen?
<v-clicks>

- Vergelijk je antwoorden
- Loop ze één voor één door
- Begrijp **waarom** de ander koos
- Je hoeft het niet eens te worden

</v-clicks>

::right::

### Wat noteer je?
<v-clicks>

- Welke casus blijft lastig?
- Welk woord uit de casus deed je twijfelen?
- Wat viel je op aan jullie verschil?

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · in tweetallen · wb-02-reflectie
</div>

<!--
Zet timer op 5 min. Loop rond. Luister wat er besproken wordt — dit is je input voor de plenaire bespreking.

Halverwege deel je wb-02 uit:
"Dit vul je straks in tijdens de bespreking. Noteer wat je opviel, welke casus nog twijfelachtig is, en welke aanwijzing voor jou doorslaggevend was."
-->

---

# Plenair stemmen

<div class="grid grid-cols-2 gap-8 mt-6">
  <div class="text-center p-8 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-6xl mb-3">🟢</div>
    <div class="text-2xl font-bold text-green-700">Common</div>
    <div class="text-sm opacity-70 mt-2">Normaal patroon — laat met rust</div>
  </div>
  <div class="text-center p-8 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-6xl mb-3">🔴</div>
    <div class="text-2xl font-bold text-red-700">Special</div>
    <div class="text-sm opacity-70 mt-2">Iets ánders dan normaal — onderzoek</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Bij twijfel: <span class="font-bold">beide kaartjes omhoog.</span>
</div>

<!--
Werk de 10 casussen door met stemkaartjes.
- Bij eensgezindheid (casus 1, 2, 4, 6, 9): kort bevestigen, max 20 sec.
- Bij verdeeldheid (casus 3, 5, 7, 8, 10): laat één deelnemer per kant uitleggen, dan duiden.

KERNCASUSSEN om extra tijd aan te besteden:
- Casus 5 (cluster — 7 van 8 boven gemiddelde): leg de "run rule" uit met getal ("statistisch onwaarschijnlijk dat dit toeval is").
- Casus 10 (tampering): teken op flip-over de twee lijnen — vlakke ruis vs. wild slingerende lijn door bijstellen. Dít is de casus van de sessie.

Stem zelf NOOIT mee. Tel innerlijk tot 7 bij stilte.
-->

---
layout: center
class: text-center
---

# Casus 10 — let op

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  De machine produceerde <span class="font-bold">common cause</span> variatie.<br/>
  Door op één meting te reageren versterkte de operator de schommelingen.
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-amber-100 text-amber-900 rounded-lg font-bold">
  Dit heet overcontrol — of tampering.
</div>

<div v-click class="mt-6 text-sm opacity-60 max-w-lg mx-auto">
  Deming noemt het een van de duurste fouten in de procesindustrie.
</div>

<!--
Neem hier extra tijd. Dit is dé casus van de sessie.

Visualiseer op flip-over:
- Lijn 1: vlakke band met willekeurige ruis (de machine zonder bijsturing)
- Lijn 2: wild slingerende lijn (dezelfde machine met bijsturing op elke meting)

Zeg: "De machine deed niks raars — de operator wel."

Voor wie meer wil weten: verwijs naar Deming's Funnel Experiment (Out of the Crisis, hfst 11).
-->

---
layout: section
---

# Theoretiseren

## Het patroon achter de twijfel

<!--
Overgang naar blok 3.
"Twijfel is geen domheid — het is precies waar het leren begint.
We gaan nu kijken naar wat de boeken hierover zeggen,
en dan zie je hoe je twijfel patronen krijgt."
-->

---
layout: two-cols
layoutClass: gap-6
---

# De twee patronen

### 🟢 Common cause
<v-clicks>

- Willekeurige spreiding
- Rond een centrumlijn
- Geen onwaarschijnlijke patronen
- = systeemvariatie

</v-clicks>

::right::

### 🔴 Special cause
<v-clicks>

- Sprong
- Trend
- Cluster (lange reeks aan één kant)
- Punt buiten grenzen

</v-clicks>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: Deming (1986), Wheeler (1993)
</div>

<!--
Onthul het A3-diagram achter in de zaal.

Toon de twee patronen. Twee duidelijk verschillende beelden.
Verwijs naar het diagram (lo-spc-104 SVG) — dit is het visuele anker.

Deel wb-03-handout-theorie uit. "Pak je markeerstift. Markeer wat voor jou nieuw is."
-->

---

# Koppel terug naar de quiz

| Quizcasus | Patroon | Type signaal |
|-----------|---------|--------------|
| Casus 1 — gewicht 100,1 g | binnen bereik | 🟢 common |
| Casus 3 — drie cycli 100,5 g na matrijswissel | sprong | 🔴 special |
| Casus 5 — 7 van 8 boven gemiddelde | cluster | 🔴 special |
| Casus 7 — vulgewicht zakt 5 metingen lang | trend | 🔴 special |
| Casus 8 — diameter 25,15 mm | buiten grenzen | 🔴 special |
| Casus 10 — bijstellen op losse meting | overcontrol | 🔴 tampering |

<!--
Loop één voor één door. Maak de koppeling expliciet:
"Casus 3 — gewicht kroop omhoog na de matrijswissel — dat is dus een sprong, en die staat hier in de tabel als signaal voor special cause."

Tempo aanhouden: 12 min is krap. Niet vertragen door eigen anekdotes.
-->

---
layout: center
class: text-center
---

# Geen losse meetwaarde

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed">
  Eén punt zegt <span class="line-through opacity-50">alles</span> <span class="font-bold text-amber-600">niks</span>.<br/>
  Het patroon over tijd zegt alles.
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-md mx-auto">
  SPC kijkt naar <span class="font-bold">tijdreeksen</span>, niet naar losse waardes.
</div>

<!--
Slide 12 — kernregel.
Laat dit even inzinken. Stilte van 3 sec.

Overgang naar Deming-context.
-->

---
layout: quote
---

# 94%

<div class="text-xl mt-6 opacity-80">
  van procesproblemen zijn <span class="font-bold">common cause</span> — ze zitten in het systeem zelf.
</div>

<div v-click class="mt-8 text-base opacity-60">
  Maar 94% van de operator-reacties richten zich op de losse meting.
</div>

<div v-click class="mt-8 text-sm opacity-50">
  — W.E. Deming, Out of the Crisis (1986)
</div>

<!--
Het 94%-percentage is bewust opvallend.
Laat het inzinken met een korte stilte.

"Daar zit precies de winst voor jou als operator: leren stoppen met reageren op losse waardes."

Korte vraagronde: "Welke casus uit de quiz zie je nu anders dan voordat we begonnen?"
2-3 mensen kort delen.

Overgang: "Theorie is mooi, maar pas bruikbaar als je het op je eigen lijn toepast."
-->

---
layout: section
---

# Experimenteren

## Eén meetwaarde van jouw lijn

<!--
Overgang naar blok 4.
Deel wb-04-actieplan uit.
"De afgelopen 37 minuten waren een oefening. Nu gaan we kijken wat dit voor JOUW lijn betekent."
-->

---

# Jouw actieplan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat ga je doen?
<v-clicks>

- Kies één meetwaarde die je sowieso al meet
- Noteer 10 opeenvolgende metingen
- Met datum + tijd
- Markeer per meting: normaal of anders

</v-clicks>

</div>

<div>

### Vragen voor jezelf
<v-clicks>

- Welke meting doe ik dagelijks al?
- Wat noem ik "normaal"?
- Wanneer twijfel ik nu of ik moet ingrijpen?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  9 min · individueel · wb-04-actieplan
</div>

<!--
Zet timer op 9 min.

Inventarisatie-vraag (1 min): "Even rondkijken: noem in één zin welke meting je dagelijks doet."
Vang 4-5 voorbeelden op (gewicht, diameter, druk, temperatuur, vulgewicht). Niet bespreken — alleen verzamelen.
Dit helpt deelnemers die niet weten wat ze moeten kiezen.

Loop rond. Help met deze vragen:
- "Welke meting doe je sowieso al?"
- "Wanneer twijfel je nu of je moet ingrijpen?"
- "Wat zou je als 'normaal' beschrijven voor die meting?"

Bevestig dat klein beginnen prima is — één meetwaarde, niet drie.
NIET zelf meedenken over instellingen — autonomie is de werkende component.
-->

---
layout: center
class: text-center
---

# Volgende sessie

<div class="text-xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Neem je 10 metingen mee.<br/>
  We bespreken per deelnemer kort:<br/>
  <span class="font-bold">wat zag je, wat deed je?</span>
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-base">
  Bonus: praat er deze week één keer met een collega over.<br/>
  <span class="text-sm opacity-70">"Wat is voor jou normaal op deze machine?"</span>
</div>

<!--
Korte deel-ronde (2 min): "Wie wil in één zin vertellen welke meetwaarde je gaat volgen?"
3-4 deelnemers, max 30 sec per persoon.

Sluit af met de transferopdracht en de bonus-collega-vraag.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">van herkennen naar dashboard lezen</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik)
</div>

<!--
Bedank de groep. Kondig de volgende sessie aan.
Vergeet niet werkbladen in te nemen of foto's te maken voor learning analytics.

Notitie voor jezelf na afloop:
- Welke casussen waren voor déze groep het lastigst?
- Hoeveel vraagtekens gemiddeld?
- Welke meetwaardes hebben deelnemers gekozen voor het actieplan?
-->
