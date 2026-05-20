---
theme: default
title: Gelabelde data is de echte bottleneck - MBO-4 variant
info: |
  ## AI-Vision Module 1 — Gebruik (MBO-4 variant)
  Workshop-blok over de economische realiteit van AI-vision: drie getallen
  voor het gesprek met je teamleider — labeltijd, jaarlijkse inspectietijd, ratio.
  Doelgroep: operators MBO-4 / aanstaande teamleiders, 40 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Gelabelde data is de bottleneck

### Drie getallen voor het gesprek met je teamleider

<div class="mt-12 text-sm opacity-60">
  AI-Vision Module 1 (Gebruik) · MBO-4 variant · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-4 / aanstaande teamleiders · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 40 minuten ontdek je waarom AI-vision systemen
bij veel bedrijven nog niet draaien.

Het probleem is niet het AI-model — dat is gratis.
Het probleem is jullie data.

Vandaag krijg je drie getallen om dat gesprek te voeren met je teamleider.

Trigger: "Wie heeft al eens 'we kopen een AI-camera' gehoord? Wat ging er door je hoofd?"
-->

---
layout: section
---

# Ervaren

## Zelf labelen — met de stopwatch erbij

<!--
Overgang naar blok 1.
"Geen theorie vooraf. Pak een fotoset, label, meet de tijd."
-->

---
layout: center
class: text-center
---

# Jullie opdracht

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  10 foto's metalen beugels per duo<br/>
  Label elke foto: kras / geen defect / scheurtje<br/>
  Eén van jullie houdt de tijd per foto bij
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Welk getal noteer jij straks? Gemiddelde seconden per foto.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · in duo's · wb-01 + fotoset A
</div>

<!--
Werkblad wb-01 met handgeschreven extra kolom 'tijd per foto (sec)'.
Stopwatch via telefoon van één duo-lid.

Loop rond. Vragen:
- "Welke foto duurde het langst? Waarom?"
- "Waar twijfelden jullie?"
- "Bij 1000 zulke foto's — past dat in één werkdag?"

Geen jargon (YOLO, F1-score). Drie woorden vandaag.
-->

---
layout: section
---

# Reflecteren

## Jouw productielijn — de rekensom

<!--
Overgang naar blok 2.
"Nu de brug naar je werkvloer. Cijfers, niet alleen ervaring."
-->

---

# 15 uur versus 1222 uur

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-xl font-bold text-amber-700 mb-3">Eenmalige investering</div>
  <ul class="text-sm space-y-2">
    <li>3 defecten × 150 foto's = 450 foto's</li>
    <li>2 min per foto</li>
    <li><strong>= 15 uur eenmalig</strong></li>
  </ul>
</div>

<div class="p-6 bg-rose-50 rounded-xl border-2 border-rose-200">
  <div class="text-xl font-bold text-rose-700 mb-3">Jaarlijkse inspectietijd</div>
  <ul class="text-sm space-y-2">
    <li>1000 prod/dag × 20 sec = 20000 sec/dag</li>
    <li>× 220 werkdagen</li>
    <li><strong>= ± 1222 uur per jaar</strong></li>
  </ul>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Het contrast is de boodschap.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  12 min · plenair + duo · wb-02 + flipover
</div>

<!--
Plenaire rekensom op flipover.
Vraag de groep om eigen getallen — niet zelf invullen.

Daarna 3 min duo-overleg: "Hoeveel producten/dag op jullie lijn?
Hoeveel seconden/product?"

Plenaire deel-ronde 1.5 min: 1-2 deelnemers hun getallen.
-->

---
layout: section
---

# Theoretiseren

## Data flywheel + variatie-factor

<!--
Overgang naar blok 3.
"Twee concepten — niet meer. Maar het tweede verandert de rekensom."
-->

---

# Het data flywheel

<div class="text-center mt-8">

```mermaid
graph LR
    A[Meer gebruikers] --> B[Meer gelabelde data]
    B --> C[Beter model]
    C --> D[Beter product]
    D --> A
```

</div>

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="p-5 bg-blue-50 rounded-xl border border-blue-200">
  <div class="text-base font-bold text-blue-700 mb-2">Wat dit betekent</div>
  <div class="text-sm opacity-80">Data wordt strategisch voordeel — niet het model. Modellen zijn gratis. Data is jouw fabriek.</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl border border-purple-200">
  <div class="text-base font-bold text-purple-700 mb-2">Google's reCAPTCHA</div>
  <div class="text-sm opacity-80">Miljoenen mensen leverden onbewust labels. Dat was Google's voorsprong — niet hun model.</div>
</div>

</div>

<!--
Teken de cirkel of toon mermaid-graaf.
30 seconden, niet meer.

reCAPTCHA-anekdote als anker.
"Strategisch voordeel zit in de data."
-->

---

# Variatie-factor — de MBO-4 verdieping

<div class="grid grid-cols-3 gap-4 mt-8">

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-3xl mb-2">🟢</div>
  <div class="text-lg font-bold text-green-700 mb-2">Lage variatie</div>
  <div class="text-sm opacity-80"><strong>150</strong> foto's per klasse</div>
  <div class="text-xs opacity-60 mt-2">Uniforme producten, weinig batches</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-3xl mb-2">🟡</div>
  <div class="text-lg font-bold text-amber-700 mb-2">Middel variatie</div>
  <div class="text-sm opacity-80"><strong>200-300</strong> per klasse</div>
  <div class="text-xs opacity-60 mt-2">Gemiddelde productlijn</div>
</div>

<div class="p-5 bg-rose-50 rounded-xl border-2 border-rose-200">
  <div class="text-3xl mb-2">🔴</div>
  <div class="text-lg font-bold text-rose-700 mb-2">Hoge variatie</div>
  <div class="text-sm opacity-80"><strong>300-500</strong> per klasse</div>
  <div class="text-xs opacity-60 mt-2">Veel kleuren, batches, lichtcondities</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Hoge variatie verdriedubbelt je labeltijd. Dat verandert de ROI.
</div>

<!--
Variatie-factor IS de MBO-4-toevoeging.
Niet skippen.

Anker: Philips Drachten — 3 producten, 3 modellen, elk apart getraind.
Geen "one model fits all".

Voeg toe: twee labelaars leveren niet dubbele data — consistentie schaalt slecht.
-->

---
layout: section
---

# Experimenteren

## Op jouw werkvloer — drie getallen

<!--
Overgang naar blok 4.
"Nu jij. Drie getallen. Eén KPI. Eén teamleider."
-->

---

# Vier delen voor je werkblad

<div class="grid grid-cols-2 gap-4 mt-6">

<div class="p-4 bg-purple-50 rounded-xl">
  <div class="text-2xl mb-1">📦</div>
  <div class="text-base font-bold text-purple-700 mb-1">1. Jouw product</div>
  <div class="text-xs opacity-70">+ 3 defect-typen</div>
</div>

<div class="p-4 bg-blue-50 rounded-xl">
  <div class="text-2xl mb-1">🔢</div>
  <div class="text-base font-bold text-blue-700 mb-1">2. Drie getallen</div>
  <div class="text-xs opacity-70">Labeltijd · jaarlijkse inspectie · ratio</div>
</div>

<div class="p-4 bg-amber-50 rounded-xl">
  <div class="text-2xl mb-1">📊</div>
  <div class="text-base font-bold text-amber-700 mb-1">3. KPI</div>
  <div class="text-xs opacity-70">OEE · FPY · klachten · doorlooptijd</div>
</div>

<div class="p-4 bg-green-50 rounded-xl">
  <div class="text-2xl mb-1">👤</div>
  <div class="text-base font-bold text-green-700 mb-1">4. Teamleider-naam</div>
  <div class="text-xs opacity-70">Voornaam — geen 'mijn manager'</div>
</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70">
  Orde-van-grootte. Niet derde decimaal.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min individueel + 1.5 min plenair · wb-04-roi-afweging
</div>

<!--
Werkblad wb-04 (MBO-4 specifiek).

5 min individueel. Help met schattingen.
1.5 min plenair: 1-2 deelnemers hun cijfers.

Concreet maken is de competentie.
"Wie ga jij dit voorleggen? Naam."
-->

---

# Deze week — de teamleider-vraag

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Binnen 1 week

<v-clicks>

- Leg je drie getallen voor aan je teamleider
- Vraag: "Is deze afweging realistisch voor onze lijn?"
- Noteer welke getallen zij aanvullen of bijstellen
- Let op niet-getalsmatige factoren (contracten, budget, weerstand)

</v-clicks>

</div>

<div>

### Volgende sessie

<v-clicks>

- 5 min aan begin: plenaire correctie-bespreking
- Waar wijken schattingen het meest af van praktijk?
- Welke niet-getalsmatige factoren kwamen bovendrijven?

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende sessie: bespreken correcties plenair.

Optioneel: zoek artikel "ROI AI quality inspection" — Engelse bron oké.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende sessie: <span class="font-bold">Correcties van de teamleiders + LO-006 visuele inspectie</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Vision Module 1 (Gebruik) · MBO-4 variant
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.
Foto van flipover — input voor correctie-bespreking.

Notitie:
- Wie had moeite met variatie-factor? (1-op-1 follow-up)
- Wie noteerde een KPI? Wie liet 'm leeg?
- Bron: RLC-Oost (2026); Ng (2021) Data-centric AI; Davenport & Ronanki (2018) HBR.
-->
