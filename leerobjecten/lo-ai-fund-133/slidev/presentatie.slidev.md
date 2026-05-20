---
theme: default
title: Classificatie — etiket plus zekerheid
info: |
  ## AI Fundamentals — Module 1 (Gebruik)
  Workshop-blok over classificatie: binair voorbeeld, multi-class, zekerheid-uitleg, twijfelgeval-werkblad.
  Doelgroep: operators MBO-4, 40 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Classificatie

### Wat zegt het systeem als het 'goed' of 'afgekeurd' meldt?

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 1 (Gebruik) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-4 · etiket + zekerheid · twijfelgevallen
</div>

<!--
[00:00-00:01] Opening.

Welkom. De komende 40 minuten kijken we naar classificatie — wat het systeem op je scherm eigenlijk zegt als het 'goed' of 'afgekeurd' meldt. En vooral: wat je doet als het systeem twijfelt.
-->

---
layout: center
class: text-center
---

# Op de werkvloer

<div class="text-xl mt-10 max-w-3xl mx-auto leading-relaxed opacity-80">
  Camera boven de lopende band — <span class="font-bold">"goed"</span> of <span class="font-bold">"afgekeurd"</span>
</div>

<div v-click class="text-xl mt-6 max-w-3xl mx-auto leading-relaxed opacity-80">
  Inspectiesysteem — <span class="font-bold">"kras"</span> / <span class="font-bold">"barst"</span> / <span class="font-bold">"kleurfout"</span> / <span class="font-bold">"vormafwijking"</span>
</div>

<div v-click class="text-xl mt-6 max-w-3xl mx-auto leading-relaxed opacity-80">
  Sensor op de machine — <span class="font-bold">"normaal bedrijf"</span> of <span class="font-bold">"storing type B"</span>
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Wat staat daar nou eigenlijk?
</div>

<!--
[00:01-00:02] Trigger.

"Op steeds meer werkvloeren staat een camera of sensor. Goed of afgekeurd. Kras of barst.
Het scherm geeft een uitslag — maar wat staat daar nou eigenlijk?"

Brug naar fase 1 — IK DOE binair voorbeeld.
Deel wb-01 uit.
-->

---

# Binair voorbeeld — CNC-onderdeel

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-gray-50 rounded-lg border-2 border-gray-200">

### Wat het systeem ziet
- Gefreesd metalen plaatje
- Lichte braam aan de rand

<div class="mt-6 text-xs opacity-50 italic">
  (Foto op scherm)
</div>

</div>

<div class="p-6 bg-blue-50 rounded-lg border-2 border-blue-200">

### Wat het model teruggeeft

<div class="text-lg font-bold text-blue-800 mt-3">
  Klasse: braam gedetecteerd
</div>

<div class="text-lg font-bold text-blue-800 mt-1">
  Zekerheid: 92%
</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min · IK DOE · trainer denkt hardop
</div>

<!--
[00:02-00:06] IK DOE — hardop denken (langzaam):

"Wat zie ik? Een metalen plaatje, lichte braam aan de rand."

"Wat geeft het model terug? Niet een getal — een ETIKET. Een woord. Een categorie.
Het zegt: dit is een braam."

"Wat betekent dat percentage erbij? Het model is voor 92% zeker dat dit een braam is.
Hoge zekerheid."

"Wat zou ik als operator doen? Bij 92% kan ik bijna altijd volgen.
Bij lage zekerheid — bijvoorbeeld 60% — moet ik zelf kijken. Daar komen we straks bij."

"Twee opties hier — goed of braam. Twee klassen. Dat heet BINAIR. Schrijf op."

[00:06-00:07] Notitie: "Schrijf in één zin op — getal of etiket?" 1 minuut, geen plenair.

[00:07-00:08] Transitie naar fase 2.
-->

---

# Multi-class — vier foto's

<div class="grid grid-cols-2 gap-3 mt-4 text-sm">

<div class="p-3 bg-red-50 rounded-lg">

### Foto 1
- **Klasse:** kras
- **Zekerheid:** 78%

</div>

<div class="p-3 bg-amber-50 rounded-lg">

### Foto 2
- **Klasse:** barst
- **Zekerheid:** 85%

</div>

<div class="p-3 bg-blue-50 rounded-lg">

### Foto 3
- **Klasse:** kleurfout
- **Zekerheid:** 91%

</div>

<div class="p-3 bg-green-50 rounded-lg">

### Foto 4
- **Klasse:** vormafwijking
- **Zekerheid:** 66%

</div>

</div>

<div class="mt-6 text-center text-sm opacity-80">
  In duo's: <span class="italic">"hoeveel klassen ziet dit model? Welke heeft de laagste zekerheid?"</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · duo's · wb-02
</div>

<!--
[00:08-00:09] Deel wb-02 uit (per duo). Toon modeluitvoer hardop.

[00:09-00:15] Zet timer op 6 min. Loop rond.
Stel vragen — geen antwoord:
- "Hoeveel klassen?"
- "Hoe heet dat?"
- "Welke heeft laagste zekerheid? Wat doe je daarmee?"

Laat de term 'multi-class' bottom-up komen — eerst tellen, dan benoemen.
-->

---
layout: center
class: text-center
---

# Plenair

<div class="text-2xl mt-10 max-w-2xl mx-auto leading-relaxed opacity-80">
  <span class="font-bold">Vier klassen</span> — dat heet
</div>

<div v-click class="text-4xl mt-6 font-bold text-blue-700">
  multi-class
</div>

<div v-click class="text-xl mt-10 max-w-2xl mx-auto leading-relaxed opacity-70">
  Foto 4 (66%) heeft de laagste zekerheid.<br/>
  Wat zou jij daarmee doen?
</div>

<!--
[00:15-00:18] Plenair (3 min).

Vraag: "Hoeveel klassen ziet dit model?" Wacht 5-7 sec.
Iemand zegt 'vier' — bevestig: "Klopt — vier klassen. Meer dan twee. Dat heet MULTI-CLASS."
Schrijf op flip-over: 'multi-class = MEER DAN TWEE'.

Daarna: "Welke heeft laagste zekerheid? Foto 4, 66%. Wat zou jij doen?"
Vang 2 antwoorden — bouw door naar fase 3.
-->

---
layout: section
---

# Theoretiseren

## Binair, multi-class, en wat zekerheid betekent

<!--
[00:18-00:19] Overgang naar blok 3.
Deel wb-03 uit. Pak markeerstift erbij.
-->

---

# Classificatie — twee smaken

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-5 bg-blue-50 rounded-lg">

### Binair
- **Twee opties**
- Goed / afgekeurd
- OK / NOK
- Aan / uit
- Normaal / storing

</div>

<div class="p-5 bg-amber-50 rounded-lg">

### Multi-class
- **Meer dan twee**
- Kras / barst / kleurfout / vormafwijking
- Type A / B / C-storing
- Drie of meer klassen

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Allebei: het model krijgt iets, geeft een etiket terug. Nooit een getal.
</div>

<!--
[00:19-00:22] Drie minuten samenvatten.

"Classificatie = AI plakt een ETIKET. Een woord, een categorie. Geen getal."
Schrijf op flip-over: 'classificatie = ETIKET'.

"Twee smaken: binair (twee opties) en multi-class (meer dan twee)."
"Allebei werken hetzelfde — model krijgt iets, geeft een etiket terug."
-->

---

# Wat betekent dat percentage?

<div class="mt-8 p-6 bg-gray-50 rounded-lg border-2 border-gray-300 text-center">

<div class="text-2xl font-bold mb-3">
  Klasse: braam — zekerheid 92%
</div>

</div>

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-5 bg-red-50 rounded-lg border-2 border-red-300">

### NIET
- 92% van het product is een braam
- Iets over de eigenschap van het product
- Een meting

</div>

<div class="p-5 bg-green-50 rounded-lg border-2 border-green-300">

### WEL
- Het model is voor 92% zeker dat dit een braam is
- Iets over het vertrouwen van het MODEL
- Een twijfel-indicator

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Vergelijk: een collega die zegt "ik denk een kras, maar ik twijfel een beetje". Die twijfel = het percentage.
</div>

<!--
[00:22-00:26] Vier minuten — kernpunt van de sessie.

Vraag: "Wat betekent dat percentage?" Wacht 5-7 sec. Vang antwoorden.

Maak expliciet:
"Het zegt NIET dat 92% van het product een braam is.
Het zegt: het model is voor 92% zeker dat dit een braam is.
Het gaat over het vertrouwen van het model in zijn eigen antwoord — niet over de eigenschap van het product."

"Vergelijk: een collega die zegt 'ik denk dat het een kras is, maar twijfel een beetje'.
Die twijfel — dat is wat het percentage uitdrukt."

"Bij hoge zekerheid (boven 90%) kun je bijna altijd volgen.
Bij lage zekerheid wordt het interessant — daar komt de operator in beeld."
-->

---

# Vuistregel

<div class="grid grid-cols-2 gap-8 mt-10">

<div class="p-6 bg-blue-50 rounded-lg text-center">

### Antwoord is een WOORD
*kras, goed, type B*

<div class="mt-3 text-lg font-bold text-blue-700">
  → Classificatie
</div>

</div>

<div class="p-6 bg-purple-50 rounded-lg text-center">

### Antwoord is een GETAL
*23 cycli, 12.000 euro*

<div class="mt-3 text-lg font-bold text-purple-700">
  → Regressie
</div>

</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70 italic">
  Regressie komt in een volgend leerobject.
</div>

<!--
[00:26-00:27] Eén minuut — onderscheid.

"Classificatie geeft een KLASSE — een woord.
Er bestaat ook AI die een GETAL voorspelt — bv. 23 dagen tot uitval. Dat heet regressie."

"Vuistregel: woord = classificatie, getal = regressie."

[00:27-00:28] Brug naar fase 4: "Nu een twijfelgeval. Wat doe jij?"
-->

---

# Twijfelgeval — metalen frame

<div class="mt-6 p-6 bg-gray-50 rounded-lg border-2 border-amber-400 text-center">

<div class="text-xl font-bold mb-2">
  Klasse: goed — zekerheid 60%
</div>

<div class="text-xl font-bold">
  Klasse: vormafwijking — zekerheid 40%
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Het model leunt naar "goed". Maar nauwelijks.
</div>

<div v-click class="mt-4 text-center text-base opacity-80">
  Wat doe jij?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  7 min · individueel · wb-04
</div>

<!--
[00:28-00:29] Deel wb-04 uit.

"Een metalen frame. Het model zegt: klasse goed — zekerheid 60%. Klasse vormafwijking — zekerheid 40%.
Drie vragen op het werkblad."
-->

---

# Drie vragen op het werkblad

<v-clicks>

- **Wat zegt dit model eigenlijk?**

- **Wat zou jij doen?**
  - Doorlaten
  - Handmatig nakijken
  - Instelling aanpassen

- **Wanneer is een zekerheid "hoog genoeg" voor jouw lijn?**

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  Hulpvragen tijdens rondlopen:<br/>
  Veiligheidscomponent of niet? Wat kost een fout?
</div>

<!--
[00:29-00:36] Zet timer op 7 min. Loop rond.

Stel vragen — geen antwoord:
- "Hoe zeker moet een model zijn voor jij het vertrouwt?"
- "Is dit een veiligheidscomponent of niet?"
- "Wat kost een doorgelaten fout in jullie productie?"

Bij vastloper: ÉÉN hulpvraag, niet drie tegelijk.
-->

---

# Drie handelwijzen

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-green-50 rounded-lg">

### Doorlaten
- Bij lage fout-kosten
- Sierdelen, niet-kritisch
- Vertrouw model grotendeels

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### Handmatig nakijken
- Bij twijfel: bijna altijd veilig
- Veiligheidscomponenten
- Dure onderdelen

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Instelling aanpassen
- Gesprek met teamleider
- Past drempel bij deze lijn?
- Bij veel grensgevallen op dezelfde drempel

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Geen vast getal. Wat een fout kost bepaalt de drempel.
</div>

<!--
[00:36-00:39] Drie minuten plenaire afsluiting.

Vraag 2-3 deelnemers: "wat zou jij doen?"
Verzamel verschillende antwoorden — drie opties zijn alle drie legitiem.

Maak expliciet:
"Doorlaten kan — als fout-kosten laag zijn."
"Handmatig nakijken bij twijfel — vooral veiligheid/duur."
"Instelling aanpassen via teamleider — als veel grensgevallen op dezelfde drempel."

[00:39-00:39:30] Belangrijke conclusie:
"GEEN vast getal voor hoog genoeg. Wat een fout kost bepaalt de drempel.
Doorgelaten kras op sierdeel anders dan op remblok.
Jouw kennis van de lijn maakt het verschil.
Dat is precies waarom operators in beeld blijven."
-->

---

# Deze week — transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Loop langs je inspectiesysteem
<v-clicks>

- Welk type — **binair of multi-class**?
- Welke **klassen** kent het?
- Laagste **zekerheid** die je tegenkomt?

</v-clicks>

</div>

<div>

### Vraag een collega
<v-clicks>

- *"Wat doe jij als het systeem twijfelt?"*
- Iedereen hanteert vaak eigen huisregel
- Mooi gesprek voor het team
- Notities meenemen

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat heb je gezien?
</div>

<!--
[00:39:30-00:40] Transferopdracht meegeven.

"Deze week: kijk langs het kwaliteits- of inspectiesysteem op je lijn.
Drie dingen: type classificatie, welke klassen, laagste zekerheid die week.

Vraag ook aan een collega: 'wat doe jij als het systeem twijfelt?'
Vaak hanteert iedereen een eigen huisregel — mooi gesprek voor het team."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Regressie · Overfitting · ML-paradigma's</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 1 (Gebruik)
</div>

<!--
[00:40] Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Hoeveel interpreteerden het percentage eerst als product-eigenschap?
- Welke huisregels in de groep?
- Welke parkeerlijst-items voor vervolgsessie?
-->
