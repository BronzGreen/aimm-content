---
theme: default
title: Trainingsdata — drie vragen aan elke dataset
info: |
  ## AI Fundamentals — Module 1 (Gebruik)
  Workshop-blok over trainingsdata: drie datasets vergelijken, framework drie eigenschappen, eigen lijn-actieplan.
  Doelgroep: operators/teamleiders MBO-4, 45 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Trainingsdata

### Drie vragen aan elke dataset

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 1 (Gebruik) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · krasdetectie · datasituatie → modelkwaliteit
</div>

<!--
[00:00-00:01] Opening.

Welkom. De komende 45 minuten kijken we naar trainingsdata — waar een AI-model van leert.

Tegen het eind weet je welke drie vragen je aan elke dataset moet stellen, en waarom 'meer data is beter' meestal te kort door de bocht is.
-->

---
layout: center
class: text-center
---

# Een leveranciersclaim

<div class="text-2xl mt-10 max-w-2xl mx-auto leading-relaxed opacity-80">
  <span class="italic">"We hebben meer data nodig — geef ons jullie foto's."</span>
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Klinkt redelijk. Maar wat zegt dat over wat jij in huis hebt?
</div>

<!--
[00:01-00:02] Trigger leveranciersclaim.

"Tegen het eind van deze sessie kun je daarop drie vragen terug stellen."

Brug naar fase 1 — drie datasets.
Deel wb-01 uit. "Twijfel mag — vraagteken zetten is welkom."
-->

---

# Drie datasets — welke kies jij?

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-red-50 rounded-lg border-2 border-red-200">

### A · Veel foto's, één ploeg
- 2.000 foto's
- Allemaal ochtendploeg
- Labels kloppen allemaal

<div class="mt-3 text-xs opacity-60">Goed voor productie?</div>

</div>

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### B · Heel veel, fouten erin
- 10.000 foto's
- Dag- en nachtploeg
- 15% labels fout

<div class="mt-3 text-xs opacity-60">Goed voor productie?</div>

</div>

<div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">

### C · Minder, alles klopt
- 800 foto's
- Dag/avond/nacht
- Klein én groot defect
- Labels kloppen allemaal

<div class="mt-3 text-xs opacity-60">Goed voor productie?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-01 · twijfel mag
</div>

<!--
[00:02-00:05] IK DOE — set A voor:
"2.000 foto's, alleen ochtendploeg, labels kloppen.
Veel foto's, fijn. Maar alleen ochtendlicht — wat mis ik straks bij de avond- of nachtploeg?
Vraagteken erbij. Niet of er genoeg foto's zijn, maar of de variatie klopt."

[00:05-00:11] Daarna: "Doe B en C zelf. Zes minuten. Twijfel mag."
Loop rond. Stel vragen. Geef geen antwoorden.

[00:11-00:12] Tussenstand: wie heeft alle drie?
-->

---
layout: center
class: text-center
---

# Stem mee — drie kleuren

<div class="grid grid-cols-3 gap-4 mt-10 text-sm max-w-2xl mx-auto">
  <div class="p-4 bg-red-50 rounded-lg border-2 border-red-200">
    <div class="font-bold text-red-700">Rood</div>
    <div class="mt-2">Set A</div>
    <div class="text-xs mt-1 opacity-60">2.000, ochtendploeg</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">
    <div class="font-bold text-blue-700">Blauw</div>
    <div class="mt-2">Set B</div>
    <div class="text-xs mt-1 opacity-60">10.000, 15% fout</div>
  </div>
  <div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">
    <div class="font-bold text-green-700">Groen</div>
    <div class="mt-2">Set C</div>
    <div class="text-xs mt-1 opacity-60">800, variatie</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Welke zou jij inzetten op de eigen lijn?
</div>

<!--
[00:12-00:15] Eerst 3 minuten tweetallen — vergelijk keuzes. Welk woord uit elke set was doorslaggevend?

[00:15-00:17] Daarna stemmen met kleurkaartjes — schrijf uitslag op flip-over.

Tel innerlijk tot 7 na elke vraag.
Bij stilte: noem zelf de eerste 'hand omhoog' om ijs te breken.
Bevestig elk antwoord zonder oordeel.
-->

---

# Het antwoord

<div class="grid grid-cols-3 gap-3 mt-6 text-xs">

<div class="p-3 bg-red-50 rounded-lg">

### A · Faalt op diversiteit
- 2.000 is genoeg
- Labels kloppen
- Maar: alleen ochtendlicht
- → Werkt slecht 's nachts

</div>

<div class="p-3 bg-blue-50 rounded-lg">

### B · Faalt op kwaliteit
- 10.000 is heel veel
- Variatie zit erin
- Maar: 15% labels fout
- → Model leert verkeerd

</div>

<div class="p-3 bg-green-50 rounded-lg">

### C · Wint op balans
- Minste foto's (800)
- Maar variatie + kwaliteit
- Op orde
- → Beste keuze

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Minder data, betere data. "Meer is beter" klopt alleen als de andere twee vragen positief zijn.
</div>

<!--
[00:17-00:21] Bespreking — 4 minuten.

Vraag eerst iemand die A koos: "welk woord deed jou kiezen?" Wacht 5-7 sec.
Daarna iemand die C koos. Daarna iemand die B koos (indien aanwezig).

Maak expliciet:
"A heeft veel foto's, maar één licht-situatie — diversiteit faalt.
B heeft veel foto's én variatie, maar 15% verkeerde labels — kwaliteit faalt.
C heeft minder foto's, maar kwaliteit én variatie op orde — winnaar."

"Minder data, betere data. Dat is het tegenovergestelde van wat veel mensen denken."

[00:21-00:22] Brug naar fase 3: "Nu de drie vragen op een rij."
-->

---
layout: section
---

# Theoretiseren

## Drie vragen aan elke dataset

<!--
[00:22-00:23] Overgang naar blok 3.

Deel wb-03 uit. Pak markeerstift erbij.
-->

---

# Drie eigenschappen

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### 1 · Kwantiteit
- **Hoeveel voorbeelden?**
- Vuistregel: 100-300 per klasse
- Set C: 800 — genoeg
- Set A: 2.000 — meer dan genoeg

</div>

<div class="p-4 bg-yellow-50 rounded-lg">

### 2 · Kwaliteit
- **Kloppen de labels?**
- Garbage in, garbage out
- Russell & Norvig (2021)
- Set B: 15% fout — gevaar

</div>

<div class="p-4 bg-green-50 rounded-lg">

### 3 · Diversiteit
- **Genoeg variatie?**
- Dag/avond/nacht
- Oud/nieuw, klein/groot
- Set A faalt hier

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Niet één — alle drie. Eén falen is genoeg om een model onbruikbaar te maken.
</div>

<!--
[00:23-00:31] Acht minuten voor de drie eigenschappen.

Kwantiteit (2 min): vuistregel 100-300 per klasse. Verbind aan A en C.

Kwaliteit (3 min): garbage in, garbage out — Russell & Norvig 2021.
Vraag: "wie controleert eigenlijk de labels op jullie lijn?"
Wacht 5-7 sec.

Diversiteit (3 min): dag/avond/nacht, oud/nieuw, klein/groot defect.
Een model leert alleen wat het ziet. Set A faalde hier.

Schrijf elke eigenschap op flip-over met steekwoord:
HOEVEEL / KLOPPEN / GENOEG VERSCHIL.

Vermijd technische termen (overfitting, train/test-split) — die komen later.
-->

---

# Praktische realiteit

<div class="grid grid-cols-2 gap-4 mt-8 text-sm">

<div class="p-4 bg-amber-50 rounded-lg">

### Wie controleert de labels?
- Op veel werkvloeren: open vraag
- Daar zit de eerste winst
- Operators zien als eerste de fout

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Operators weten dingen niemand anders weet
- Welke foto van welke ploeg
- Welke producten écht goed waren
- Welke variatie er die week was

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Die kennis is goud waard bij elk AI-project.
</div>

<!--
[00:31-00:33] Twee minuten — praktische realiteit.

Belangrijk inzicht: "Wie controleert de labels?" is op veel werkvloeren een open vraag.
Daar zit de eerste winst. Operators zijn vaak de enige met dit overzicht.

[00:33-00:34] Brug naar fase 4: "Nu jouw eigen lijn."
-->

---
layout: section
---

# Experimenteren

## Welke data heb ik eigenlijk?

<!--
[00:34-00:35] Overgang naar blok 4.
"Laatste 11 minuten — eigen lijn-actieplan."
-->

---

# Eigen actieplan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen op het werkblad
<v-clicks>

- Welke **voorbeelden** zou je nodig hebben?
- Heb je nu al **foto's of metingen** — hoeveel?
- Zijn de **antwoorden bijgehouden** — door wie?
- Zit er genoeg **variatie** in?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Waar staan de foto's nu opgeslagen?
- Wie zou kunnen vertellen of de labels kloppen?
- Denk je dat alle ploegen erin zitten?
- 'Weet ik niet' is waardevol

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  7 min · individueel · wb-04
</div>

<!--
[00:35-00:36] Inventarisatie-vraag (1 min):
"Bij wie op de eigen lijn loopt een inspectiecamera, dashboard, defectherkenning?
Of zou er een kunnen komen? Spuitgieten, CNC, verpakking?"
Vang 4-5 antwoorden, niet bespreken.

[00:36-00:43] Zet timer op 7 min.
'Ik weet het niet zeker' is een GELDIGE uitkomst.
Help formuleren als concrete IT-vraag.

Loop rond. Stel concretiserende vragen.
-->

---

# Plenaire mini-ronde

<div class="text-center mt-10 text-base opacity-80">
  Twee deelnemers — kort:
</div>

<div class="grid grid-cols-3 gap-4 mt-8 text-sm max-w-3xl mx-auto">

<div class="p-4 bg-blue-50 rounded-lg">

### 1
Jouw toepassing
*"Inspectiecamera bij spuitgieten..."*

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### 2
Grootste vraagteken
*"Kwantiteit / kwaliteit / diversiteit?"*

</div>

<div class="p-4 bg-green-50 rounded-lg">

### 3
Welke IT-vraag
*"Vraag aan IT / onderhoud / kwaliteit"*

</div>

</div>

<!--
[00:43-00:45] Twee minuten — vang 2 voorbeelden.
Niet bespreken, alleen noteren voor volgende sessie.

De plenaire ronde is goud — geeft signaal welke onderwerpen in de groep leven.
-->

---

# Deze week — transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Drie vragen aan IT / onderhoud / kwaliteit
<v-clicks>

- Welke **voorbeelden** gebruikt dit systeem om te leren?
- Wie **controleert** of de antwoorden kloppen?
- Zitten alle **ploegen en machines** erin?

</v-clicks>

</div>

<div>

### Bonus-praatje
<v-clicks>

- Vraag iemand van onderhoud:<br/>*"Welke foto's of metingen bewaren wij eigenlijk?"*
- Vaak: data zit ergens
- Maar niemand weet of het de goede zijn
- Dat ontdekken = waardevol voor elk AI-project

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat heb je gevonden?
</div>

<!--
[00:44-00:45] Transferopdracht meegeven (30 sec).

Drie vragen — concreet en stelbaar deze week.
Bonus-praatje: vaak ontdek je dat data ergens staat maar niemand weet of het klopt.

Daarna door naar lo-ai-fund-133 (classificatie) en lo-ai-fund-135 (overfitting),
die op deze foundation bouwen.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Classificatie · Overfitting · Machine Learning paradigma's</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 1 (Gebruik)
</div>

<!--
[00:45] Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Hoeveel deelnemers kozen B vóór de bespreking? (hardnekkigheid 'meer is beter')
- Stemming-uitslag op flip-over (verdeling = groepsbegrip)
- Welke IT-vragen aangekondigd?
- Welke parkeerlijst-items voor vervolgsessie?
-->
