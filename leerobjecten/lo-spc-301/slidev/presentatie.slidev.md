---
theme: default
title: Cp en Cpk — wat zegt het cijfer écht?
info: |
  ## SPC Module 2 — Train
  Workshop-blok over interpretatie van capability-indices (Cp/Cpk).
  Doelgroep: operators MBO-4 + teamleiders MBO-4, 50 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Cp en Cpk

### Wat zegt het cijfer écht?

<div class="mt-12 text-sm opacity-60">
  SPC Module 2 (Train) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-4 + teamleiders · capability-interpretatie
</div>

<!--
Open warm.
"Wie van jullie heeft wel eens 'Cpk = 1,2' gehoord en gedacht: wat zegt dat me eigenlijk?
Of erger: 'Cpk = 0,9 — slecht', en daarna naar de machine gerend om iets te tweaken?"

Wacht. Laat 1-2 mensen knikken. Geen lange verhalen.

In de komende 50 minuten gaan we van 'het cijfer kennen' naar 'het cijfer begrijpen'.
Een Cpk-getal zonder interpretatie is een mooi getal zonder actie — soms zelfs een gevaarlijk getal.

Verwijs naar draaiboek blok 1, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Vandaag leer je

<v-clicks>

- Wat **Cp** zegt over je proces
- Wat **Cpk** zegt over je proces
- Wanneer Cp en Cpk samenvallen
- Welke **actie** past bij welk getal
- Waarom **stabiliteit eerst** komt

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">🎯</div>
    <div class="text-xl font-mono font-bold text-amber-600">Cpk = 1,1</div>
    <div class="text-sm opacity-60 mt-2">wat doe je nu?</div>
  </div>
</div>

<!--
Korte ophaal voorkennis (1 min).
"Snel rondje — wie kan in één zin zeggen wat 'het proces is stabiel' betekent?"
Verwijs naar gisteren — Nelson, common cause, special cause (lo-spc-104, lo-spc-201).

Vang 1-2 antwoorden, bevestig kort.
"Onthou dit. Stabiliteit komt straks terug — op een vervelende manier."

Verwijs naar draaiboek blok 1, instructie 3.
-->

---
layout: center
class: text-center
---

# 🟢 Werkblad — Cpk-puzzel

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Vier mini-casussen.<br/>
  Cp en Cpk zijn gegeven.<br/>
  <span class="font-bold">Geen formules. Wel interpretatie.</span>
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Per casus: probleem? actie? twijfel?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 minuten · individueel · pen
</div>

<!--
Deel wb-01-cpk-puzzel uit (30 sec).
"Vier mini-casussen. Per casus: een Cp-waarde, een Cpk-waarde, en of het proces stabiel is.
Geen formules. Geen berekeningen. Wat is hier aan de hand, en wat zou jij doen?"

Zet timer op 8 min. Loop rond. Beantwoord praktische vragen, GEEN inhoudelijke.
Als iemand vraagt "is mijn antwoord goed?": "Dat gaan we straks samen ontdekken — schrijf vooral op wat jij denkt."

Aan het einde: "Pen neer. Bij welke casus had je de meeste twijfel? Steek je hand op bij casus 1... 2... 3... 4."
Tel hardop, schrijf op flip-over.

Verwijs naar draaiboek blok 1, instructie 4-6.
-->

---
layout: section
---

# Reflecteren

## Wat zit er achter dat cijfer?

<!--
Overgang naar blok 2 (reflecteren).
"Vier verschillende casussen, vier verschillende plaatjes. We bespreken ze één voor één — eerst gokken, dan duiden."

Deel wb-02-reflectie uit:
"Tijdens de bespreking vul je in: wat had je gedacht voordat we de casus bespraken, en wat denk je nu?
Het verschil daartussen — dat is je leeropbrengst van vandaag."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Stem per casus

<div class="grid grid-cols-4 gap-4 mt-6">
  <div class="text-center p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-3xl mb-2">1️⃣</div>
    <div class="text-sm font-bold text-green-700">Niets</div>
    <div class="text-xs opacity-70 mt-1">Alles oké</div>
  </div>
  <div class="text-center p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-3xl mb-2">2️⃣</div>
    <div class="text-sm font-bold text-amber-700">Centrering</div>
    <div class="text-xs opacity-70 mt-1">Staat scheef</div>
  </div>
  <div class="text-center p-4 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-3xl mb-2">3️⃣</div>
    <div class="text-sm font-bold text-red-700">Spreiding</div>
    <div class="text-xs opacity-70 mt-1">Te wijd</div>
  </div>
  <div class="text-center p-4 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-3xl mb-2">4️⃣</div>
    <div class="text-sm font-bold text-purple-700">Stabiliteit</div>
    <div class="text-xs opacity-70 mt-1">Geen geldig getal</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Eerst gokken — dan duiden.
</div>

<!--
Werk de 4 casussen door met stemkaartjes (cijfers of kleuren).

KERNAANPAK per casus (exact gesynchroniseerd met wb-01):
- Casus 1 (spuitgiet, Cp = 1,39 / Cpk = 1,11): klassiek centreer-patroon. Bij verdeeldheid: laat uitleggen waarom Cp > Cpk = scheef. Teken op flip-over de smalle klok verschoven naar LSL.
- Casus 2 (CNC-frees, Cp = 0,85 / Cpk = 0,85): gelijke Cp en Cpk = gecentreerd, maar < 1,0 = spreidingsprobleem. Teamleider/engineering-gesprek.
- Casus 3 (verpakking, Cp = 1,67 / Cpk = 1,67): bij eensgezindheid 'niets': kort bevestigen, max 30 sec. Niet onnodig tweaken.
- Casus 4 (automotive PPAP, Cp = 1,45 / Cpk = 0,90): inhoudelijk = centreren, maar PPAP-context maakt het escalatie-waardig. Laat de stilte vallen na 'wat vindt de autobouwer hiervan?'.

Stem zelf NOOIT mee. Tel innerlijk tot 7 bij stilte.

NB: wb-01 bevat geen instabiele casus. Stabiliteit komt aan bod in blok 3 (drie veelgemaakte fouten, fout #1).

Verwijs naar draaiboek blok 2, instructie 2-5 (volledige bespreking per casus).
-->

---
layout: center
class: text-center
---

# Casus 4 — automotive let op

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Cp = 1,45 ; Cpk = 0,90<br/>
  Inhoudelijk: <span class="font-bold">centreer-patroon</span> (gemiddelde 49,87 g zit te dicht tegen LSL 49,80 g).
</div>

<div v-click class="mt-8 inline-block px-6 py-3 bg-red-100 text-red-900 rounded-lg font-bold">
  Maar de klant is een autobouwer (PPAP).
</div>

<div v-click class="mt-6 text-base opacity-80 max-w-lg mx-auto">
  PPAP eist <span class="font-bold">Cpk ≥ 1,67.</span><br/>
  Een Cpk van 0,90 is contractueel <span class="font-bold">afgekeurd</span>.
</div>

<div v-click class="mt-4 text-sm opacity-60 max-w-lg mx-auto">
  Eerste actie: centreren naar 50,00 g. Daarna nog Cpk ≈ 1,4 — nog steeds &lt; 1,67.<br/>
  Vervolg: <span class="font-bold">escaleren naar engineering</span>; lijn niet vrijgeven voor klantleveringen.
</div>

<div v-click class="mt-3 text-xs opacity-50 max-w-md mx-auto">
  Klantcontext meewegen — Ford PPAP · automotive
</div>

<!--
Dit is dé casus van de sessie — niet door een instabiliteits-trick maar door de klantcontext.

Veel deelnemers zien Cp = 1,45 / Cpk = 0,90 en denken 'oh, lijkt op casus 1 — centreren'.
Inhoudelijk klopt dat, maar de klantcontext maakt het zwaarder.

"Wat denken jullie dat de autobouwer van Cpk = 0,90 vindt?"
Stilte. Tel innerlijk tot 5.

Onthul stapsgewijs:
1. Inhoudelijk = centreer-patroon, eerste actie: centreren naar 50,00 g.
2. Maar klant = autobouwer, eis = PPAP-niveau Cpk ≥ 1,67.
3. Centreren brengt je hooguit naar Cpk ≈ 1,4 — nog steeds onacceptabel.
4. Vervolg: escaleren naar engineering voor procesverbetering, lijn niet vrijgeven.

De les: dezelfde getallen kunnen totaal verschillende beslissingen vragen, afhankelijk van klantcontext.

NB: stabiliteit komt aan bod in blok 3 (drie veelgemaakte fouten, fout #1).

Verwijs naar draaiboek blok 2, instructie 5.
-->

---
layout: section
---

# Theoretiseren

## Waar komt dat verschil vandaan?

<!--
Overgang naar blok 3 (theoretiseren).
"Drie verschillende problemen, drie verschillende acties — en één gemene gemeenschappelijke deler:
zonder context zegt een Cpk-getal niets.

We gaan nu kijken naar de formules — niet om te rekenen, maar om te zien waar dat verschil tussen Cp en Cpk vandaan komt."

Deel wb-03-cpk-handout uit. "Pak je markeerstift. Markeer wat voor jou nieuw is."

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-6
---

# Cp — is de fles smal genoeg?

<div class="text-3xl font-mono mt-4 mb-6 text-amber-700">
  Cp = (USL − LSL) / 6σ
</div>

<v-clicks>

- Tolerantie / spreiding
- "Hoe vaak past de spreiding in het tolerantievak?"
- Zegt **niets** over positie
- Alleen: is het in **potentie** smal genoeg?

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-6xl mb-4">📏</div>
    <div class="text-base opacity-70 max-w-xs mx-auto">
      Cp = 1,33 → past met<br/>33% marge
    </div>
  </div>
</div>

<!--
Schrijf op flip-over: Cp = (USL − LSL) / 6σ.

"Bovenkant min onderkant van de tolerantie, gedeeld door zes keer de procesvariatie.
In operator-taal: hoe vaak past de spreiding van mijn proces in het tolerantievak?"

- Cp = 1 → past nipt
- Cp = 1,33 → past met 33% marge
- Cp = 1,67 → past ruim, Ford-niveau

Geen berekening hier — alleen de leesregel.

Verwijs naar draaiboek blok 3, instructie 3.
-->

---
layout: two-cols
layoutClass: gap-6
---

# Cpk — staat hij midden op de tafel?

<div class="text-2xl font-mono mt-4 mb-6 text-amber-700">
  Cpk = min[<br/>
  &nbsp;&nbsp;(USL − μ) / 3σ,<br/>
  &nbsp;&nbsp;(μ − LSL) / 3σ<br/>
  ]
</div>

<v-clicks>

- Afstand tot dichtstbijzijnde grens
- Gemeten in spreidingseenheden
- Hoe groter het verschil **Cp − Cpk**…
- …hoe **schever** het proces staat

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-6xl mb-4">🎯</div>
    <div class="text-base opacity-70 max-w-xs mx-auto">
      Cpk = Cp →<br/>gecentreerd<br/><br/>
      Cpk &lt; Cp →<br/>verschoven
    </div>
  </div>
</div>

<!--
Schrijf op flip-over: Cpk = min[(USL−μ)/3σ, (μ−LSL)/3σ].

"Twee afstanden: van het gemiddelde naar de bovengrens, en van het gemiddelde naar de ondergrens —
beide gedeeld door 3σ. Het kleinste van die twee is je Cpk.

Cpk vertelt: hoe ver zit ik van de dichtstbijzijnde tolerantiegrens, gemeten in spreidingseenheden?
Hoe groter het verschil tussen Cp en Cpk, hoe schever het proces staat."

Verwijs naar draaiboek blok 3, instructie 4.
-->

---
layout: two-cols-header
---

# Het centrale onderscheid

::left::

### 🟢 Smal én gecentreerd
<div class="mt-4 text-sm opacity-80">

- Cp **hoog**
- Cpk **hoog**
- Cp ≈ Cpk

</div>

<div class="mt-6 p-4 bg-green-50 rounded-lg text-center">
  <div class="text-xs opacity-70 mb-1">Tolerantievak</div>
  <div class="font-mono text-sm">|—————•—————|</div>
  <div class="text-xs mt-1 opacity-70">smalle klok in het midden</div>
</div>

::right::

### 🔴 Smal maar verschoven
<div class="mt-4 text-sm opacity-80">

- Cp **hoog**
- Cpk **laag**
- Verschil → schever

</div>

<div class="mt-6 p-4 bg-red-50 rounded-lg text-center">
  <div class="text-xs opacity-70 mb-1">Tolerantievak</div>
  <div class="font-mono text-sm">|——•——————————|</div>
  <div class="text-xs mt-1 opacity-70">smalle klok tegen ondergrens</div>
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Diagram lo-spc-301 — twee verdelingen
</div>

<!--
Onthul het A3-diagram achter in de zaal (slide 7 + diagram-lo-spc-301.svg).

"Twee verdelingen.
Links: smal en gecentreerd — Cp hoog, Cpk hoog.
Rechts: even smal, maar verschoven — Cp hetzelfde, Cpk laag.
Dat is precies casus 2 uit jullie puzzel.

Cp vraagt: is de fles smal genoeg?
Cpk vraagt: staat hij ook midden op de tafel?"

Dit is de centrale didactische slide. Stilte van 3 sec na de uitleg.

Verwijs naar draaiboek blok 3, instructie 1.
-->

---

# Interpretatietabel

| Cp / Cpk | Interpretatie | Praktijk |
|----------|---------------|----------|
| **< 1,0** | Niet capabel | Structureel afkeur waarschijnlijk |
| **= 1,0** | Theoretisch passend | Eén procesdrift en je bent buiten |
| **≥ 1,33** | Industriële ondergrens | Veel klanten accepteren minimaal dit |
| **≥ 1,67** | Zwaar / kritisch | Ford PPAP, automotive |
| **≈ 2,0** | Six sigma | Gecentreerd kortetermijnproces |

<div v-click class="mt-6 text-sm opacity-70 text-center">
  Een getal alleen zegt niets — koppel altijd aan stabiliteit en rol van de meting.
</div>

<!--
Loop snel door:
- Onder 1,0 — niet capabel
- Precies 1,0 — kwetsbaar
- 1,33 — industriële ondergrens
- 1,67 — Ford PPAP, automotive
- 2,0 — luxepositie

Voor MBO-4 / teamleider: noem PPAP-term. Operators negeren, teamleiders onthouden.

Verwijs naar draaiboek blok 3, instructie 5.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Spuitgiet-voorbeeld

Spuitgietlijn — onderdeelgewicht.

<v-clicks>

- **USL = 100,5 g**
- **LSL = 99,5 g**
- Stabiele lijn (regelkaart oké)
- Gemeten μ = **99,9 g**
- σ = **0,12 g**

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">⚙️</div>
    <div class="text-sm opacity-60 mt-2">één meetwaarde,<br/>twee getallen</div>
  </div>
</div>

<!--
"Concrete casus. Spuitgietlijn, onderdeelgewicht moet tussen 99,5 en 100,5 gram liggen.
Stabiele lijn — regelkaart zegt: alleen common cause.
Gemiddelde van 50 metingen: 99,9 gram. σ van die metingen: 0,12 gram."

Bouw spanning op — laat de getallen even staan voordat je de uitkomst onthult op de volgende slide.

Verwijs naar draaiboek blok 3, instructie 6.
-->

---

# Spuitgiet — de twee getallen

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">

### Cp
<div class="font-mono text-base mt-2 mb-3 opacity-80">
  (100,5 − 99,5) / (6 × 0,12)<br/>
  = 1,00 / 0,72
</div>
<div class="text-3xl font-bold text-green-700">≈ 1,39</div>
<div class="text-xs mt-2 opacity-70">spreiding zit goed (boven 1,33)</div>

</div>

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">

### Cpk
<div class="font-mono text-sm mt-2 mb-3 opacity-80">
  min[(100,5 − 99,9) / 0,36 ;<br/>
  (99,9 − 99,5) / 0,36]<br/>
  = min[1,67 ; 1,11]
</div>
<div class="text-3xl font-bold text-amber-700">= 1,11</div>
<div class="text-xs mt-2 opacity-70">verschuiving naar ondergrens</div>

</div>

</div>

<div v-click class="mt-8 text-center text-base p-4 bg-blue-50 text-blue-900 rounded-lg">
  De pers schiet niet te wijd — de pers staat <span class="font-bold">scheef</span>.<br/>
  <span class="text-sm opacity-80">Actie: centreren naar 100,0 — niet sleutelen aan spreiding.</span>
</div>

<!--
Toon Cp-berekening: 1,39 — boven 1,33, spreiding zit goed.
Toon Cpk-berekening: 1,11 — boven 1,0 maar onder 1,33.

Stilte. "Wat zien we? Cp is mooi, maar Cpk lager — verschil zit in centrering.
De pers staat te dicht tegen de ondertolerantie aan."

KERNZIN — herhaal:
"Operatorles: de juiste actie is centreren — gemiddelde naar 100,0 brengen,
niet harder proberen de spreiding te verkleinen.
Dat is de hele les van vandaag in één voorbeeld."

Schrijf de uitkomsten op de flip-over zodat ze blijven staan voor blok 4.

Verwijs naar draaiboek blok 3, instructie 6.
-->

---

# Drie veelgemaakte fouten

<div class="grid grid-cols-1 gap-4 mt-6">

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">1. Capability op een instabiel proces</div>
  <div class="text-sm opacity-80 mt-1">Eén mooi getal over data uit meerdere toestanden = appels en peren. Verboden — eerst stabiliteitscheck (lo-spc-201, Nelson). Niet rapporteren als capabel.</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">2. Slechte subgroepering</div>
  <div class="text-sm opacity-80 mt-1">Kortetermijn- en langetermijnvariatie door elkaar — komt in module 3 terug.</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">3. Slecht meetsysteem</div>
  <div class="text-sm opacity-80 mt-1">Cpk zegt evenveel over de meter als over de machine. Heet MSA / Gage R&R.</div>
</div>

</div>

<!--
Loop snel door (1 min 30):
1. Capability op een instabiel proces — gisteren behandeld (lo-spc-201). Stel plenair: 'Stel: in casus 4 was de regelkaart instabiel geweest — wat had je dan gedaan?' Antwoord: niets, geen capability uitspraak doen.
2. Subgroepering — kortetermijn vs langetermijn variatie, komt in module 3.
3. Meetsysteem — MSA / Gage R&R, onderwerp voor kwaliteitsdienst of module 3.

NIET dieper op MSA ingaan. Eén zin volstaat.

Verwijs naar draaiboek blok 3, instructie 7. Let op valkuil vk-05 (te diep op MSA) en vk-07 (Pp/Ppk).
-->

---
layout: section
---

# Experimenteren

## Eén meetwaarde van jouw lijn

<!--
Overgang naar blok 4.
"Nu is het bekend. Tijd om het op je eigen lijn los te laten — maar wel met de stabiliteits-vraag erbij."

Deel wb-04-eigen-cpk-analyse uit.
"Kies één meetwaarde waarvan je weet of vermoedt dat de tolerantie bekend is —
onderdeelgewicht, diameter, vulhoogte, druk, temperatuur."

Verwijs naar draaiboek blok 4, instructie 1.
-->

---

# Jouw eigen Cpk-analyse

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen
<v-clicks>

1. Welke meetwaarde + USL/LSL?
2. Is je proces **stabiel**? Hoe weet je dat?
3. Welke Cp/Cpk verwacht je / vraag je op?
4. Jouw interpretatie + welke actie?

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Welke meting doe ik elke shift al?
- Waar vermoed ik dat het gemiddelde zit t.o.v. specs?
- Wat zou ik doen bij Cpk = 1,0?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-04-eigen-cpk-analyse
</div>

<!--
Zet timer op 8 min.

Inventarisatie-vraag (1 min): "Even rondkijken: noem in één zin welke meetwaarde je kiest, en wat de tolerantie is."
Vang 4-5 voorbeelden. Niet bespreken — alleen verzamelen.

Loop rond. Help met:
- "Welke meetwaarde controleren jullie sowieso al elke shift?"
- "Heb je een idee waar het gemiddelde zit ten opzichte van de specs?"
- "Wat zou je gaan doen als je hoort: Cpk = 1,0?"

Bevestig dat 'ik moet dit eerst opvragen' een geldig antwoord is — vaak het juiste.
NIET zelf meedenken over instellingen — autonomie is de werkende component.

Verwijs naar draaiboek blok 4, instructie 2-3.
-->

---
layout: center
class: text-center
---

# Transferopdracht — deze week

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Vraag bij je teamleider of kwaliteitsdienst<br/>
  de <span class="font-bold">Cp/Cpk-waarden</span> op van jouw meetwaarde,<br/>
  plus de <span class="font-bold">stabiliteits-status</span>.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-2xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Stabiel?</div>
    <div class="text-xs opacity-70 mt-1">ja / nee</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Probleem?</div>
    <div class="text-xs opacity-70 mt-1">centrering / spreiding / beide / geen</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Actie?</div>
    <div class="text-xs opacity-70 mt-1">welke past?</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-70 max-w-lg mx-auto">
  Bonus: praat er deze week één keer met een collega over.<br/>
  <span class="text-sm opacity-80">"Wat zou jij doen bij Cpk = 1,1 met Cp = 1,4?"</span>
</div>

<!--
Korte deel-ronde (2 min): "Wie wil in één zin vertellen welke meetwaarde je gaat onderzoeken?"
3-4 deelnemers, max 30 sec per persoon.

Sluit af met de transferopdracht en de bonus-collega-vraag.
"Volgende workshop bespreken we per persoon."

Verwijs naar draaiboek blok 4, instructie 4-5.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende blok in module 2: <span class="font-bold">groepsreflectie configuratiebesluit eigen lijn</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 2 (Train) · Cp/Cpk
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (groepsreflectie configuratiebesluit).

Vergeet niet werkbladen in te nemen of foto's te maken voor learning analytics.

Notities voor jezelf na afloop:
- Welke casussen waren voor déze groep het lastigst?
- Welke meetwaardes hebben deelnemers gekozen voor de eigen analyse?
- Bij teamleider-deelnemers: warm overdragen naar groepsreflectie configuratiebesluit (volgend blok).

Verwijs naar draaiboek "Checklist na de sessie".
-->
