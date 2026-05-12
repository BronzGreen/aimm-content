---
theme: default
title: Wat SPC is — regelkaart-fundament
info: |
  ## SPC Module 1 — Gebruik
  Instap-workshop over de drie componenten van een regelkaart
  (centrale lijn, UCL/LCL, punten in tijd) en het onderscheid
  stabiel vs. onstabiel proces.
  Doelgroep: operators MBO-3, 40 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Wat staat er op die grafiek bij mijn machine?

### De drie componenten van een regelkaart

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Open de sessie met:
"Op veel werkvloeren hangt ergens een grafiek. Op een bord, op een scherm, in een map.
Vaak loop je er langs. In de komende 40 minuten gaan we kijken wat er eigenlijk op staat —
en wat het voor jou betekent."

Deel wb-01-regelkaart-lezen uit. "Drie fragmenten — drie regelkaarten uit een echte
productieomgeving. Eentje doen we samen, twee doe je zelf. Pak een pen."
-->

---
layout: two-cols
layoutClass: gap-8
---

# Fragment 1 — spuitgietlijn

**Meting:** onderdeelgewicht per uur, in gram.
*(fictieve illustratie ter oefening)*

<v-clicks>

- **Centrale lijn (CL):** 100,0 g
- **UCL:** 100,3 g  · **LCL:** 99,7 g
- **Punten:** schommelen willekeurig
- **Geen enkel punt** buiten grenzen
- **Geen trend** omhoog of omlaag

</v-clicks>

<div v-click class="mt-6 p-3 bg-green-50 rounded-lg text-center">
  <div class="text-xl font-bold text-green-800">Stabiel</div>
  <div class="text-xs opacity-70">Proces doet wat het altijd doet</div>
</div>

::right::

<div class="h-full flex flex-col justify-center text-center">
  <div class="font-mono text-sm text-left bg-gray-50 p-4 rounded-lg">
    <div>UCL ─────────────── 100,3</div>
    <div class="my-1">    •       •   •</div>
    <div>CL  ──•────•───•──── 100,0</div>
    <div class="my-1">        •        •</div>
    <div>LCL ─────────────── 99,7</div>
    <div class="mt-2 opacity-60">tijd → 1 2 3 4 5 6 7 8</div>
  </div>
  <div class="text-xs opacity-50 mt-3">spuitgietlijn · onderdeelgewicht</div>
</div>

<!--
Slide 2 — IK DOE plenair, 4 min.

Wijs met de vinger of laser pointer:
"Eerst kijk ik naar de lijn in het midden. Dat is de centrale lijn — 100,0 gram.
Dan boven en beneden: UCL en LCL, 100,3 en 99,7. Dat zijn procesgrenzen — GEEN
klantgrenzen. Dan de punten: links-naar-rechts in de tijd. Willekeurige schommeling,
geen uitschieters, geen trend. Conclusie: stabiel."

Verwijs naar de A3-print achter in de zaal.

Daarna: "Nu jij. Fragment 2 en 3. Per fragment: zoek CL, grenzen, punten. Kruis aan.
Noteer in één zin waarom. 7 minuten." Timer aan, niet over schouders kijken.

Anti-patroon NIET doen: de theorie nu al geven. Eerst ervaren.
-->

---
layout: section
---

# Reflecteren

## Heb jij ooit zo'n kaart gezien?

<!--
Overgang naar blok 2 (reflecteren), 12 min.

Na buurman-check en plenair turven: "Handen op — wie zei stabiel bij fragment 2?
Wie onstabiel? Wie twijfel?" Tel hardop. Idem fragment 3. Niet beoordelen.
"Komt straks terug in de handout."

Dan: "Regelkaarten zijn geen nieuwe vinding. Op veel werkvloeren hangen ze al —
alleen weet niet iedereen wat het is. We gaan 7 minuten terugkijken op jouw werkvloer."
-->

---
layout: two-cols-header
---

# STARRT — zes korte vragen

::left::

### Wat vul je in?
<v-clicks>

- **S**ituatie — waar hing hij?
- **T**aak — welke meting stond erop?
- **A**ctie — keek je er naar?
- **R**esultaat — wat zag je toen?
- **R**eflectie — zou je het nu anders zien?
- **T**ransfer — naar welke kaart kijk je deze week?

</v-clicks>

::right::

### Hoe vul je in?
<v-clicks>

- Eerlijk — geen "juiste antwoord"
- *"Nog nooit gezien"* is een prima antwoord
- In jouw eigen woorden
- Denk aan je eigen lijn, niet aan wat "hoort"

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  7 min · individueel · wb-02-reflectie
</div>

<!--
Deel wb-02-reflectie uit.
"Zes korte vragen over jouw werkvloer. Eerlijk invullen — 'ik heb er nog nooit eentje
gezien' is een prima antwoord, dat betekent dat we hier met de juiste groep zijn."

Zet timer op 7 min. Loop rond. Help bij blokkades met:
- "Denk aan het bord bij jouw lijn. Hangt daar iets?"
- "Kijk op het scherm van je machine — staat daar een grafiekje?"
- "Als het antwoord 'nee' is: schrijf 'nog nooit gezien' — dat is ook een antwoord."

BIJ MBO-3: schaamte over niet-weten is een grote blokkade. Maak expliciet dat
niet-gezien-hebben waardevolle informatie is.
-->

---

# Wat kwam er naar boven?

<div class="mt-8 grid grid-cols-2 gap-6 text-base">

<div v-click class="p-4 bg-blue-50 rounded-lg">
  <div class="font-bold text-blue-700">📋 "Op het bord bij de lijn"</div>
  <div class="text-xs opacity-60 mt-1">klassieke fysieke regelkaart</div>
</div>

<div v-click class="p-4 bg-green-50 rounded-lg">
  <div class="font-bold text-green-700">💻 "Op het scherm van de machine"</div>
  <div class="text-xs opacity-60 mt-1">dashboard, MES-systeem</div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-lg">
  <div class="font-bold text-amber-700">📁 "In een map of ordner"</div>
  <div class="text-xs opacity-60 mt-1">papieren registratie</div>
</div>

<div v-click class="p-4 bg-gray-50 rounded-lg">
  <div class="font-bold text-gray-700">❓ "Nog nooit gezien"</div>
  <div class="text-xs opacity-60 mt-1">= waardevol antwoord</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Of je hem zag of niet — vanaf nu kijk je anders.
</div>

<!--
Plenaire inventarisatie, 4 min.
"Handen op: wie heeft er ooit een kaart of grafiek gezien bij zijn machine?"
Tel hardop. "Wie weet nog waar hij hing?" Vang 2-3 antwoorden, laat kort beschrijven.
Niet beoordelen of het écht een regelkaart was — het gaat om herkenning.

Spiegelvraag (1 min): "En nu je weet dat een regelkaart drie vaste onderdelen heeft —
centrale lijn, UCL/LCL, punten in tijd — zou je dezelfde kaart anders lezen? Eén iemand,
één zin." Vang één antwoord. "Precies. Dat is de hele sessie in één zin."

Bij "ik zag er wel eentje maar ik snapte hem niet": bedank nadrukkelijk — dit is de
ideale opstap naar blok 3.
-->

---
layout: section
---

# Theoretiseren

## Drie componenten. Altijd dezelfde drie.

<!--
Overgang naar blok 3, 13 min.
Onthul (of wijs naar) de A3-print achter in de zaal.
"Hier is wat je de afgelopen 25 minuten hebt gezien, netjes benoemd. Drie componenten.
Altijd dezelfde drie."

Deel wb-03-handout-spc-basics uit.
"Pak je markeerstift. Markeer onderweg wat nieuw voor je is — niet alles, alleen wat
je nog niet had bedacht."
-->

---
layout: image-right
image: ../../trainee/lo-spc-101/diagram-lo-spc-101.svg
backgroundSize: contain
---

# Regelkaart-anatomie

<v-clicks>

1. **Centrale lijn (CL)** — gemiddelde van je proces
2. **UCL en LCL** — grenzen van normaal procesgedrag
3. **Punten in tijd** — metingen in volgorde links-naar-rechts

</v-clicks>

<div v-click class="mt-8 text-sm opacity-70">
  Niet drie willekeurige dingen. <span class="font-bold">Drie onderdelen — elke kaart, elke lijn.</span>
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: Shewhart 1931; ASQ — Control Chart; ISO 7870-1, ISO 7870-2
</div>

<!--
Slide 7 — het diagram zelf, met SVG.
Gebruik dit als ankerbeeld. De drie componenten worden in de volgende drie slides
uitgebouwd. Hier alleen benoemen, niet uitleggen.
-->

---
layout: two-cols
layoutClass: gap-6
---

# 1. De centrale lijn

### Wat is het?
<v-clicks>

- Het gemiddelde van je proces
- De lijn waar metingen "omheen horen"
- Komt uit de historische data van je lijn
- Niet door de klant bepaald

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">➖</div>
    <div class="text-base opacity-70">"Wat doet deze lijn normaal?"</div>
  </div>

  <div v-click class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-800 mb-1">Fragment 1 (wb-01):</div>
    Bij de spuitgietlijn stond CL op <span class="font-mono">100,0 g</span> — het gemiddelde onderdeelgewicht. Metingen schommelen er omheen.
  </div>
</div>

<!--
Component 1 (1,5 min).
"Het gemiddelde van je proces. De lijn waar de metingen 'omheen horen te liggen'
als alles normaal draait. Bij Fragment 1 stond die op 100,0 gram — dat is het
gemiddelde van de spuitgietlijn."

Schrijf op flip-over kolom CENTRALE LIJN: "Gemiddelde — wat je proces normaal doet"
-->

---
layout: two-cols
layoutClass: gap-6
---

# 2. UCL en LCL

### Grenzen van **normaal procesgedrag**
<v-clicks>

- **UCL** — Upper Control Limit (boven)
- **LCL** — Lower Control Limit (onder)
- Statistisch bepaald uit je proces
- Typisch op enkele standaarddeviaties van CL

</v-clicks>

<div v-click class="mt-4 p-3 bg-amber-50 rounded-lg text-sm">
  <span class="font-bold text-amber-800">⚠️ Geen klantspecificaties.</span> USL/LSL staan op de tekening — UCL/LCL komen uit je proces.
</div>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">📏</div>
    <div class="text-base opacity-70">"Wat is normaal — niet wat mag?"</div>
  </div>

  <div v-click class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-800 mb-1">Fragment 1:</div>
    UCL <span class="font-mono">100,3 g</span> · LCL <span class="font-mono">99,7 g</span>. Dat is wat <em>deze lijn</em> normaal doet — niet wat de klant accepteert.
  </div>
</div>

<!--
Component 2 (2 min) — de moeilijkste van de drie.

"Upper Control Limit en Lower Control Limit. Boven- en ondergrens van normaal
procesgedrag. Let op — dit is een valkuil: UCL/LCL zijn GEEN klantspecificaties.
Ze komen uit jouw proces zelf, statistisch bepaald op basis van historische data,
typisch op enkele standaarddeviaties van de centrale lijn (bron: Shewhart 1931).

Klantspecificaties (USL/LSL) zijn wat-mag-wel-verkocht-worden — UCL/LCL zijn
wat-is-normaal-voor-deze-lijn. Twee verschillende vragen."

Verwijs naar wb-03 tabel UCL/LCL vs. USL/LSL voor wie het later wil nalezen.
Schrijf op flip-over kolom UCL/LCL: "Procesgrenzen — niet klantgrenzen"

[MBO-4]: verwijs naar NIST/SEMATECH Engineering Statistics Handbook hoofdstuk 6
voor de formule-onderbouwing (CL ± 3σ).
-->

---
layout: two-cols
layoutClass: gap-6
---

# 3. Punten in tijd

### Volgorde telt
<v-clicks>

- Links-naar-rechts = volgorde van meten
- Punt 1 was eerst, punt 2 daarna
- De kaart **onthoudt de tijdvolgorde**
- Patroon zie je pas over meerdere metingen

</v-clicks>

<div v-click class="mt-4 text-sm italic opacity-80">
  "Eén meting van 100,3 g zegt weinig.<br/>Tien metingen die langzaam stijgen zegt veel."
</div>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">📊</div>
    <div class="text-base opacity-70">"Tijdreeks — geen losse getallen"</div>
  </div>

  <div v-click class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-800 mb-1">Fragment 2 (CNC):</div>
    Losse meting 24,98 mm lijkt prima. Maar acht metingen op rij die stijgen — <span class="font-bold">trend</span>. Dat is alleen zichtbaar als je de volgorde bewaart.
  </div>
</div>

<!--
Component 3 (1,5 min).

"De metingen staan van links naar rechts in de volgorde waarin je ze hebt gedaan.
Punt 1 eerst, punt 2 daarna. Dat is belangrijk: de kaart onthoudt de tijdvolgorde.
Daarom zie je patronen die je op losse metingen nooit zou zien."

Schrijf op flip-over kolom PUNTEN IN TIJD: "Tijdreeks — patroon zegt meer dan losse meting"

Vuistregel (naslag, niet nu expliciet noemen): voor een nieuwe observatie heb je
minstens 5-10 opeenvolgende metingen nodig voordat je een patroon zinnig kunt
beoordelen. Staat in wb-03 — te valideren per werkvloer.
-->

---

# Terug naar de fragmenten

<div class="mt-6 grid grid-cols-3 gap-4 text-sm">

<div v-click class="p-4 bg-green-50 rounded-lg">
  <div class="font-bold text-green-800 mb-2">Fragment 1 — spuitgieten</div>
  <div class="text-xs mb-2">Gewicht rond CL 100,0 g</div>
  <div class="font-bold text-green-900">Stabiel</div>
  <div class="text-xs opacity-70 mt-1">Willekeurig binnen grenzen</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg">
  <div class="font-bold text-red-800 mb-2">Fragment 2 — CNC-diameter</div>
  <div class="text-xs mb-2">Punten kruipen omhoog</div>
  <div class="font-bold text-red-900">Onstabiel</div>
  <div class="text-xs opacity-70 mt-1">Trend — signaal (Shewhart 1931)</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg">
  <div class="font-bold text-red-800 mb-2">Fragment 3 — vulgewicht</div>
  <div class="text-xs mb-2">Punt 8 op 506 g</div>
  <div class="font-bold text-red-900">Onstabiel</div>
  <div class="text-xs opacity-70 mt-1">Punt buiten UCL (ASQ, ISO 7870-2)</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Geen inspectie achteraf. <span class="font-bold">Procesgedrag in de tijd volgen.</span>
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Fictieve illustraties ter oefening — getallen ontworpen voor leerdoel
</div>

<!--
Koppeling terug naar wb-01, 3 min.

Loop de drie fragmenten nog één keer door:
- Fragment 1 (spuitgieten): stabiel. Punten schommelen willekeurig binnen de grenzen.
- Fragment 2 (CNC-diameter): onstabiel. Trend omhoog. Dat is precies wat Shewhart
  in 1931 een signaal noemde dat een andere oorzaak meedoet
  (bron: Shewhart, Economic Control of Quality of Manufactured Product).
- Fragment 3 (verpakking-vulgewicht): onstabiel. Punt 8 springt boven UCL.
  Eén punt buiten grenzen is per definitie een signaal (bron: ASQ, ISO 7870-2).

Vraag: "Wie had dit zo? Wie had er eentje anders?" Bespreek kort waar de groep
verdeeld was. Geen schaamte bij foute antwoorden — "Dit leren we nu net."

Benoem bij fragmenten 2 en 3: dit zijn fictieve oefenvoorbeelden.
-->

---
layout: quote
---

# "SPC is geen inspectie achteraf.
# SPC is procesgedrag in de tijd volgen."

<div class="mt-6 text-sm opacity-60">
  American Society for Quality (ASQ) — Control Chart definitie<br/>
  ISO 7870-1 & ISO 7870-2 — dezelfde kerngedachte internationaal
</div>

<!--
De kernboodschap, 2 min.

"Dat staat zo in de ASQ-definitie (American Society for Quality) en in de
internationale norm ISO 7870-1 en 7870-2. De kerntaak: beoordelen of variatie
consistent en voorspelbaar is, of dat er onvoorspelbare verstoringen optreden
(bron: ASQ — Control Chart; ISO 7870-1, ISO 7870-2)."

Laat deze zin bezinken. Geen volgende slide terwijl de groep nog leest.

Bij verwarring stabiel ≠ goed: "Een proces kan stabiel draaien én tóch onderdelen
maken die de klant afkeurt. SPC kijkt naar het proces, niet naar het onderdeel."
-->

---
layout: center
class: text-center
---

# Deze week op de werkvloer

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Kijk één keer bewust naar <span class="font-bold">een grafiek bij jouw machine.</span><br/>
  Noteer: welke meting, is er een CL, zijn er grenzen,<br/>
  in welke richting loopt <span class="font-bold">de tijd?</span>
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-base">
  Bonus: vraag een collega<br/>
  <span class="text-sm opacity-70">"Wat betekent die grafiek eigenlijk voor jou?"</span>
</div>

<!--
Afsluiting + transfer, 1 min 30.

"Deze week: kijk één keer bewust naar een grafiek, regelkaart of dashboard bij jouw
machine. Noteer: welke meting, is er een centrale lijn, zijn er grenzen, in welke
richting loopt de tijd? Neem je notities mee naar de volgende sessie (lo-spc-102).

Bonus: vraag één keer aan een collega 'wat betekent die grafiek eigenlijk voor jou?'
Vaak leer je zo sneller wat de lokale afspraken zijn."

Verwijs naar wb-03 als naslag — niet innemen, meenemen naar werkvloer.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop-blok: <span class="font-bold">variatie — common vs. special cause (lo-spc-102)</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik) · lo-spc-101
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (lo-spc-102, variatie + common/special cause).

Vergeet niet werkbladen 1-2 in te nemen of foto's te maken voor learning analytics.
Werkblad 3 (handout) gaat MEE naar de werkvloer — niet innemen.

Notitie voor jezelf na afloop:
- Bij welke component was de meeste verwarring? (meestal: UCL/LCL vs. klantspec)
- Welke deelnemers hadden fragment 2 en 3 goed? (= voorkennis, potentiële MBO-4 tempo)
- Welke werkvloer-voorbeelden kwamen op tafel in blok 2? (nuttig voor lo-spc-102)

Bronnen-check tijdens Q&A:
- Shewhart 1931 = grondslag
- ASQ = definitie
- ISO 7870-1/-2 = internationale norm
- NIST/SEMATECH = verdieping voor MBO-4
-->
