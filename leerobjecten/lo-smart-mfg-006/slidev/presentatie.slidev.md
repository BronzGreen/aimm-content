---
theme: default
title: Visuele inspectie met deep learning
info: |
  ## AI-Kwaliteitscontrole Module 1 — Gebruik
  Workshop-blok over de drie stappen van AI-inspectie en het verschil tussen classificatie en segmentatie.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Visuele inspectie met deep learning

### Hoe herkent een camera defecten op de lijn?

<div class="mt-12 text-sm opacity-60">
  AI-Kwaliteitscontrole Module 1 (Gebruik) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. De komende 40 minuten kijken we hoe een camera met AI defecten herkent.
Tegen het eind weet je hoe het werkt en waar het op jouw werkplek zou kunnen helpen.

Trigger: "Wie controleert nu zelf producten op kwaliteit? Waar let je dan op?"
Vang 2-3 reacties. Reageer alleen met "herkenbaar". Geen oordeel.
-->

---
layout: center
class: text-center
---

# Storingsquiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Bekijk de 6 foto's.<br/>
  Goedgekeurd of afgekeurd?<br/>
  Schrijf op wat je ziet.
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Er is geen goed of fout. Het gaat om jouw beoordeling.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01 uitdelen. Toon de 6 foto's (of laat op deze slide tonen).
Zet timer op 6 min. Loop rustig rond. Geen sturende vragen.

Bij vastlopen: "Wat zou je doen als je dit op je lijn zag?"

Niet voorzeggen. De waarde zit in de variatie tussen oordelen.
-->

---
layout: section
---

# Reflecteren

## Waar was je het oneens met je buurman?

<!--
Overgang naar blok 2.
"Vergelijken jullie nu in duo's. De plekken waar jullie verschillen zijn de leerwinst."
-->

---
layout: center
class: text-center
---

# Vergelijk in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">👥</div>
    <div class="text-lg font-bold text-blue-700">Eens of oneens?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">🤔</div>
    <div class="text-lg font-bold text-purple-700">Wat maakt het lastig?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">💡</div>
    <div class="text-lg font-bold text-green-700">Wat zou helpen?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Beoordeling met je ogen is werk. En vermoeiend werk is foutgevoelig werk.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · in duo's · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 6 min.
Loop rond. Verzamel 2-3 sterke voorbeelden.

Plenair daarna 3 min:
- "Bij welke foto verschilden jullie het meest?"
- "Wat maakt deze beoordeling lastig?"

Schrijf 3-4 sleutelwoorden op flap-over. Sluit af:
"Dit zijn precies de plekken waar AI kan helpen."

Bij sceptische opmerking ('AI maakt ons overbodig'): erken, parkeer voor fase 3.
-->

---
layout: section
---

# Theoretiseren

## Drie stappen — camera, AI, beslissing

<!--
Overgang naar blok 3.
"Nu krijgen we de kapstok: wat doet AI eigenlijk in zo'n inspectie?"
-->

---

# De drie stappen

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-5xl mb-3">📷</div>
  <div class="text-xl font-bold text-blue-700 mb-2">1. Camera</div>
  <div class="text-sm opacity-80">Foto of video van het product op de lijn</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-5xl mb-3">🧠</div>
  <div class="text-xl font-bold text-purple-700 mb-2">2. AI-analyse</div>
  <div class="text-sm opacity-80">Het model herkent defecten in het beeld</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-5xl mb-3">✅</div>
  <div class="text-xl font-bold text-green-700 mb-2">3. Beslissing</div>
  <div class="text-sm opacity-80">Goed → door · Fout → terug · Stuk → weg</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Eén ketting van drie schakels — meer is het niet.
</div>

<!--
Loop de drie stappen één voor één langs.
Wijs naar de flap-over-kapstok.

"Camera = gewone industriele camera, geen sci-fi.
AI-analyse = het model bekijkt en herkent.
Beslissing = goed/herstellen/afkeuren."

Houd het tempo rustig. Niet meer dan deze drie stappen in de eerste 3 min.
-->

---

# Classificatie of segmentatie?

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-xl font-bold text-amber-700 mb-3">Classificatie</div>
  <div class="text-base mb-3">Het AI-model zegt:</div>
  <div class="text-2xl font-bold text-amber-900">"Goed" of "afgekeurd"</div>
  <div class="text-sm opacity-70 mt-3">Maar laat niet zien WAAR het defect zit.</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-300">
  <div class="text-xl font-bold text-green-700 mb-3">Segmentatie</div>
  <div class="text-base mb-3">Het AI-model kleurt aan:</div>
  <div class="text-2xl font-bold text-green-900">precies welke pixels fout zijn</div>
  <div class="text-sm opacity-70 mt-3">Je kunt het ZIEN. Daardoor controleerbaar.</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold">
  Welke van de twee zou jij willen op jouw lijn?
</div>

<div v-click class="mt-3 text-center text-sm opacity-70 italic">
  In de industrie: bijna altijd segmentatie — omdat je het kunt controleren.
</div>

<!--
Maak het visueel. Vraag actief: "Welke van de twee zou jij willen?"
Bijna altijd komt: segmentatie.

Bevestig: "Segmentatie is in de industrie de voorkeur, omdat je het kunt zien."
-->

---

# Voorbeeld: isolatiepanelen

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De situatie
- Camera fotografeert elk paneel
- Na de freesbewerking
- AI markeert de zijkanten

</div>

<div>

### De beslissing
<v-clicks>

- **Twee rechthoeken** zichtbaar → OK
- **Eén rechthoek** zichtbaar → freesfout
- Terug voor herbewerking, of afkeur

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-blue-50 rounded-lg">

### Een trucje: data augmentatie
- Weinig defecte voorbeelden? Variëer ze: spiegelen, helderheid aanpassen, stukken weglaten.
- In de praktijk: van **89% naar 99,5% nauwkeurig** dankzij data augmentatie.

</div>

<!--
Vertel langzaam. Het isolatiepaneel-voorbeeld is concreet en hanteerbaar.
Houd hetzelfde voorbeeld vast — niet wisselen.

Data augmentatie: bij MBO-3 niet uitleggen wat het technisch is. Wel: "een trucje om met weinig data toch goed te leren."

Stilte van 3 sec na 99,5%. Dan: "En toch heb jij straks nog steeds werk — daar gaat fase 4 over."
-->

---
layout: quote
---

# AI = extra paar ogen

<div class="text-xl mt-6 opacity-80">
  Het ziet de routine.
</div>

<div v-click class="mt-8 text-base opacity-70">
  Jij ziet de <span class="font-bold">twijfelgevallen,</span><br/>
  de <span class="font-bold">nieuwe fouten,</span><br/>
  de <span class="font-bold">oorzaken.</span>
</div>

<div v-click class="mt-8 text-sm opacity-50">
  Een AI met 99,5% nauwkeurigheid betekent nog steeds:<br/>
  1 op de 200 producten heeft jouw oordeel nodig.
</div>

<!--
Belangrijk moment. Sceptische deelnemers hebben dit nodig.

"AI doet de routine. Jij doet wat AI niet kan: twijfel, nieuwheid, oorzaak."

Schrijf op flap-over: AI = extra paar ogen.
-->

---
layout: section
---

# Experimenteren

## Waar zou AI helpen op jouw lijn?

<!--
Overgang naar blok 4.
"De afgelopen 30 minuten was de theorie. Nu wordt het concreet voor jouw werk."
-->

---

# Actieplan — drie vragen

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📦</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Welk product?</div>
  <div class="text-sm opacity-70">Wees specifiek — geen 'alle producten'</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-4xl mb-3">🔍</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Welk defect?</div>
  <div class="text-sm opacity-70">Krassen, maatfout, kleur, vorm, breuk?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📷</div>
  <div class="text-lg font-bold text-green-700 mb-2">Welke camerapositie?</div>
  <div class="text-sm opacity-70">Voor of na welke bewerking?</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Concreet maken is de oefening. Vaag actieplan = leeg actieplan.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 5 min.
Loop rond. Help concretiseren met doorvragen:
- "Welk product specifiek?"
- "Welk defect zoek je nu met je ogen?"
- "Voor of na de bewerking?"

Plenair daarna 3 min: 3-4 deelnemers delen hun toepassing kort (max 30 sec per persoon).
Vat samen op flap-over: product, defect, plek camera.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Ga kijken
<v-clicks>

- Sta één keer bewust bij een kwaliteitscontrole op je lijn
- Welke defecten zoek je?
- Hoe lang duurt het?
- Zou een camera dit ook kunnen zien?

</v-clicks>

</div>

<div>

### Ga vragen
<v-clicks>

- Vraag je teamleider:<br/>"Zijn er al plannen voor AI-inspectie?"
- Vraag een collega:<br/>"Wat zou jij willen automatiseren?"
- Bewaar het antwoord voor de volgende sessie

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: LO-010 — hoeveel productietijd bespaart AI-kwaliteitscontrole?

"Wat je deze week ontdekt nemen we mee naar de volgende sessie."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">AI bespaart productietijd — LO-010</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI-Kwaliteitscontrole Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke toepassingen werden genoemd? (input voor LO-010 en LO-101)
- Wie was sceptisch? (1-op-1-aandacht in volgende sessie)
- Bron: Cruz et al. (2024). Artificial Intelligence in Manufacturing, pp. 129-131.
-->
