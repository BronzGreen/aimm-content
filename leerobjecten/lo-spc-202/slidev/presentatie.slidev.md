---
theme: default
title: Gevoeligheid versus vals alarm
info: |
  ## SPC Module 2 — Train
  Workshop-blok over de afweging gevoeligheid versus vals alarm op regelkaarten.
  Doelgroep: operators MBO-3 (primair), 40 minuten, rekenen-reflecteren-theorie.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Gevoeligheid vs vals alarm

### Waarom levert méér regels niet automatisch een betere kaart op?

<div class="mt-12 text-sm opacity-60">
  SPC Module 2 (Train) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · ARL en signaalregels
</div>

<!--
Open warm.
"Wie van jullie heeft deze week op de eigen lijn een alarm meegemaakt waarvan achteraf bleek dat er niks aan de hand was?"

Wacht. Laat 2-3 mensen kort knikken of een kort woord zeggen. Geen lange verhalen.

Vandaag in 40 minuten: het verschil begrijpen tussen 'gevoeligheid' en 'vals alarm'.
We doen het niet met theorie eerst — we beginnen met rekenen op een fictieve lijn.

Verwijs naar draaiboek blok 1, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Vandaag leer je

<v-clicks>

- Wat **ARL** is (Average Run Length)
- Hoeveel vals alarm je krijgt bij **Kale Shewhart**
- Hoeveel bij **+ WECO** en **+ Nelson**
- Waarom **alarm-fatigue** een echt risico is
- Waarom AIMM regels **gefaseerd** leert

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">🚨</div>
    <div class="text-xl font-mono font-bold text-amber-600">ARL = 91,75</div>
    <div class="text-sm opacity-60 mt-2">wat betekent dat voor jouw lijn?</div>
  </div>
</div>

<!--
Korte ophaal voorkennis (1 min).
"Snelle check: wat is een regelkaart? Wie kan in één zin zeggen wat die ±3σ-band op de kaart doet?"

Vang 1-2 antwoorden, bevestig kort. Verwijs naar ko-spc-201.
Dit is geen hertoetsing — alleen herinnering.

Verwijs naar draaiboek blok 1, instructie 3.
-->

---
layout: center
class: text-center
---

# 🟢 Werkblad — Alarm-rekenoefening

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Fictieve verpakkingslijn B.<br/>
  <span class="font-bold">96 metingen per dag.</span><br/>
  Drie regelsets — hoeveel vals alarm krijg je?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Rekensom: metingen per dag ÷ ARL
</div>

<div v-click class="mt-4 text-xs opacity-50 max-w-md mx-auto">
  Fictieve case — bedoeld voor rekenoefening, niet gebaseerd op een echte lijn
</div>

<div class="abs-br m-6 text-xs opacity-40">
  15 minuten · individueel · rekenmachine
</div>

<!--
Deel wb-01-oefening uit (30 sec).
"Eén fictieve verpakkingslijn. 8 uur per dag, meet elke 5 minuten = 96 metingen per dag.
Proces in werkelijkheid stabiel — alle alarmen die afgaan zijn dus vals.
Hoeveel krijg je er per dag bij drie verschillende regelsets?"

IK DOE — demonstreer scenario A plenair:
Schrijf op flip-over: "Scenario A: ARL = 371".
"96 / 371 ≈ 0,26 vals alarm per dag. Dus ~1 per 4 dagen. Goed te doen."
Schrijf op flip-over: "0,26/dag → ~1 per 4 dagen → goed te doen".

JIJ DOET — individueel scenario B en C (8 min):
"Pak je rekenmachine. Scenario B: WECO, ARL = 91,75. Scenario C: Nelson, schat ARL = 50."

Loop rond. Help alleen bij technische struikelingen. GEEN interpretatie-hints.

Korte plenaire check (1 min 30): oogst antwoorden B en C.

Verwijs naar draaiboek blok 1, instructie 4-7.
-->

---

# Drie regelsets — wat krijg je?

<div class="grid grid-cols-3 gap-4 mt-6">
  <div class="text-center p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-3xl mb-2">1️⃣</div>
    <div class="text-sm font-bold text-green-800">Kale Shewhart</div>
    <div class="text-2xl font-mono font-bold text-green-900 mt-2">ARL = 371</div>
    <div class="text-xs opacity-70 mt-2">~1 per 4 dagen</div>
    <div class="text-xs opacity-50 mt-1">Goed te doen</div>
  </div>
  <div class="text-center p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-3xl mb-2">2️⃣</div>
    <div class="text-sm font-bold text-amber-800">+ WECO (4 regels)</div>
    <div class="text-2xl font-mono font-bold text-amber-900 mt-2">ARL = 91,75</div>
    <div class="text-xs opacity-70 mt-2">~1 per dag</div>
    <div class="text-xs opacity-50 mt-1">Voelbaar</div>
  </div>
  <div class="text-center p-4 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-3xl mb-2">3️⃣</div>
    <div class="text-sm font-bold text-red-800">+ Nelson (8 regels)</div>
    <div class="text-2xl font-mono font-bold text-red-900 mt-2">ARL ≈ 50</div>
    <div class="text-xs opacity-70 mt-2">~2 per dag</div>
    <div class="text-xs opacity-50 mt-1">Alarm-fatigue-risico</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Elk extra regeltje = meer signaal, meer ruis. De vraag is: waar ligt jouw grens?
</div>

<!--
Dit is het brugblad tussen blok 1 en blok 2.
De cijfers komen direct uit wb-01 — oogst eerst de antwoorden voordat je doorloopt naar dit overzicht.

Deze slide wordt pas bereikt na de plenaire oogst van blok 1.

Laat stilte vallen bij 'alarm-fatigue-risico'. Die term gaat terugkomen in blok 3.

Verwijs naar draaiboek blok 1, instructie 7.
-->

---
layout: section
---

# Reflecteren

## Mijn ervaring met vals alarm

<!--
Overgang naar blok 2 (reflecteren).
"Die getallen die jullie net uitrekenden — waarschijnlijk herken je er iets in van je eigen werkdag.
Nu gaan we kijken naar één concrete herinnering."

Deel wb-02-reflectie uit. Normaliseer meteen:
"Bijna iedereen heeft wel eens een alarm genegeerd dat achteraf niks was. Dat is alarm-fatigue in actie.
Geen slechte mentaliteit — een reëel effect van een te gevoelige regelset."

Verwijs naar draaiboek blok 2, instructie 1-2.
-->

---

# STARRT — zes korte stappen

<div class="grid grid-cols-3 gap-3 mt-6">
  <div class="p-3 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-900">S — Situatie</div>
    <div class="text-xs opacity-70 mt-1">Welke lijn? Wanneer?</div>
  </div>
  <div class="p-3 bg-purple-50 rounded-lg">
    <div class="font-bold text-purple-900">T — Taak</div>
    <div class="text-xs opacity-70 mt-1">Wat was jouw rol?</div>
  </div>
  <div class="p-3 bg-orange-50 rounded-lg">
    <div class="font-bold text-orange-900">A — Actie</div>
    <div class="text-xs opacity-70 mt-1">Wat deed je?</div>
  </div>
  <div class="p-3 bg-green-50 rounded-lg">
    <div class="font-bold text-green-900">R — Resultaat</div>
    <div class="text-xs opacity-70 mt-1">Echt of vals?</div>
  </div>
  <div class="p-3 bg-red-50 rounded-lg">
    <div class="font-bold text-red-900">R — Reflectie</div>
    <div class="text-xs opacity-70 mt-1">Wat viel op?</div>
  </div>
  <div class="p-3 bg-yellow-50 rounded-lg">
    <div class="font-bold text-yellow-900">T — Transfer</div>
    <div class="text-xs opacity-70 mt-1">Volgende keer?</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-80 p-4 bg-slate-50 rounded-lg">
  <span class="font-bold">Eén zin per stap.</span> Geen opstel — alleen herkenning.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min individueel · 3 min buurman · wb-02
</div>

<!--
Zet timer op 8 min voor individueel invullen.
Loop rond. Help bij blokkades, vooral bij 'Taak' (abstract) en 'Reflectie' (zelfkritisch).
Normaliseer: "Je rol was misschien gewoon 'werk doorgaan' — dat mag."

Na 8 min: buurman-uitwisseling (3 min, 90 sec per persoon).
"Deel één ding: welke situatie en wat had je achteraf anders gedaan?"

Plenaire oogst (30 sec) — 1-2 vrijwilligers, één zin.
Tel innerlijk tot 7. Niet zelf invullen.

Verwijs naar draaiboek blok 2, instructie 3-5.
-->

---
layout: section
---

# Theoretiseren

## Waar komen die getallen vandaan?

<!--
Overgang naar blok 3 (theoretiseren).
"Jullie hebben nu zelf gerekend. Jullie hebben nu zelf teruggekeken.
Nu gaan we naar de theorie. En je zult zien: de theorie bevestigt vooral wat jullie al vermoedden."

Onthul het A3-diagram achter in de zaal (diagram-lo-spc-202.svg).
"Drie staafjes. Kaal, WECO, Nelson. Let op de verhouding."

Deel wb-03-handout uit. "Pak je markeerstift. Markeer wat voor jou nieuw is."

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---
layout: center
class: text-center
---

# De centrale zin

<div class="text-2xl mt-6 max-w-3xl mx-auto leading-relaxed font-bold">
  "Elke extra signaalregel maakt je regelkaart<br/>
  <span class="text-amber-700">gevoeliger</span> — maar ook vaker <span class="text-red-700">vals</span>."
</div>

<div v-click class="mt-10 text-xl max-w-2xl mx-auto leading-relaxed opacity-90">
  Te veel regels = <span class="font-bold">alarm-fatigue</span>.<br/>
  Operators gaan signalen negeren.
</div>

<div v-click class="mt-10 text-sm opacity-60 max-w-lg mx-auto">
  Deze zin is de hele sessie in twee regels.<br/>
  Schrijf hem over of markeer hem.
</div>

<!--
Lees hardop voor. Laat de zin staan.
Stilte — 3 sec.
"Deze zin is de hele sessie in twee regels. Schrijf hem over of markeer hem."

Dit is de kernslide. Niet snel doorklikken.

Verwijs naar draaiboek blok 3, instructie 3.
-->

---

# ARL-tabel — drie regelsets

| Configuratie | Wat let de kaart op? | ARL | Bij 96/dag |
|--------------|----------------------|-----|------------|
| **Kale Shewhart** | 1 punt buiten ±3σ | **~371** | ~1 per 4 dagen |
| **+ WECO (4 regels)** | Trends + zones | **~91,75** | ~1 per dag |
| **+ Volledige Nelson (8 regels)** | Diagnostisch volledig | **~40–60** | ~2 per dag |

<div v-click class="mt-6 p-4 bg-amber-50 rounded-lg text-sm">
  <span class="font-bold">Bronverantwoording:</span> Het getal <span class="font-mono font-bold">ARL ≈ 91,75</span> voor WECO komt uit
  <span class="font-bold">Champ &amp; Woodall (1987, Technometrics)</span> — niet uit NIST zoals vaak foutief wordt doorgegeven. Let op bij citeren.
</div>

<div v-click class="mt-4 text-xs opacity-60 text-center">
  Shewhart 1924 · WECO 1956 · Nelson 1984 · Champ &amp; Woodall 1987
</div>

<!--
Loop door:
- Kale Shewhart: klassieke Shewhart-regel (1924). Robuust.
- WECO: Western Electric Company, 1956. Vier extra regels. ARL = 91,75.
- Nelson: Lloyd Nelson (1984), JQT 16(4). 8 regels, strenger.

Bronverantwoording expliciet: "Het getal 91,75 — Champ & Woodall 1987, Technometrics. NIET NIST."
Een paar seconden langzaam spreken hier geeft gewicht — operators waarderen dat.

Verwijs naar draaiboek blok 3, instructie 4.
Let op valkuil vk-handout-diep-op-nelson en vk-cusum-ewma.
-->

---

# Drie redenen waarom 'meer' averechts werkt

<div class="grid grid-cols-1 gap-4 mt-6">

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">1. Alarm-fatigue</div>
  <div class="text-sm opacity-80 mt-1">Als het alarm vaker vals is dan echt, gaan mensen het niet meer checken. De échte verstoring mist zijn kans om opgemerkt te worden.</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">2. Verloren productietijd</div>
  <div class="text-sm opacity-80 mt-1">Elk alarm = lijn stil of operator ernaartoe. 2 valse alarmen per dag × 5 min × 20 dagen = 3+ uur productie per maand.</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
  <div class="font-bold text-red-800">3. Verloren vertrouwen in de kaart</div>
  <div class="text-sm opacity-80 mt-1">Als operators het systeem niet meer geloven, is de kaart als instrument kwijt. Een kapotte vertrouwensrelatie repareer je niet even.</div>
</div>

</div>

<div v-click class="mt-6 text-center text-sm italic opacity-70">
  "Liever drie regels die je begrijpt, dan acht die je negeert." — Minitab-stelregel
</div>

<!--
Loop snel door de drie redenen (2 min totaal).

KERNZIN: "Vals alarm is niet 'gratis ruis' — het is echt geld en echt vertrouwen."

Reken plenair even voor: 2 valse alarmen × 5 min × 20 dagen = 200 min = 3+ uur per maand. Tastbaar.

Sluit af met de Minitab-stelregel als bruggetje naar de gefaseerde aanpak.

Verwijs naar draaiboek blok 3, instructie 5.
-->

---

# De gefaseerde AIMM-aanpak

<div class="grid grid-cols-3 gap-4 mt-6">

<div class="p-4 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-sm font-bold text-green-900 mb-2">Module 1 — Gebruik</div>
  <div class="text-xs opacity-80 mb-2">Regels 1 + 2</div>
  <div class="text-xs opacity-70">Basisstabiliteit. Je leert de kaart lezen.</div>
</div>

<div class="p-4 bg-amber-50 rounded-xl border-2 border-amber-300 ring-2 ring-amber-400">
  <div class="text-sm font-bold text-amber-900 mb-2">Module 2 — Train <span class="text-xs">(nu)</span></div>
  <div class="text-xs opacity-80 mb-2">Regels 3–6</div>
  <div class="text-xs opacity-70">Trend- en mixsignalen. Je leert wat ze toevoegen én wat ze kosten.</div>
</div>

<div class="p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-sm font-bold text-blue-900 mb-2">Module 3 — Op Maat</div>
  <div class="text-xs opacity-80 mb-2">Regels 7 + 8</div>
  <div class="text-xs opacity-70">Diagnostische verdieping. Alleen bij begrip van subgroepering.</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Die volgorde is geen toeval — het voorkomt dat je te snel te veel tegelijk aan zet.
</div>

<!--
Loop door de drie modules.
"Module 1 — regels 1 en 2. Basisstabiliteit. Je leert de kaart lezen."
"Module 2 — deze module. Regels 3-6. Trend en mix."
"Module 3 — regels 7 en 8. Diagnostisch. Alleen bij subgroepering-begrip."

Benadruk: volgorde is bewust. Voorkomt overload.

Verwijs naar draaiboek blok 3, instructie 6.
-->

---

# Operator-implicatie

| Wat zie jij? | Wat doe je? |
|--------------|-------------|
| Meerdere alarmen per dag op dezelfde lijn | Vraag teamleider welke regelset actief is |
| Engineering stelt voor meer regels aan te zetten | Vraag om de afweging gevoeligheid vs vals alarm |
| Collega's negeren alarmen | Meld als productierisico — niet als mentaliteitsprobleem |
| Je weet niet welke regelset actief is | Vraag het na — als niemand het weet, is dat ook informatie |

<div v-click class="mt-6 p-4 bg-blue-50 rounded-lg text-center">
  Jij hoeft geen regelset <span class="font-bold">in te stellen</span>.<br/>
  Jij moet <span class="font-bold">begrijpen</span> waarom jouw lijn is ingesteld zoals die is.
</div>

<!--
Loop door de praktijktabel uit de handout.
Benadruk de laatste regel: jij als operator bent geen engineer, maar wel gespreksgesprekspartner.

Aha-oogst (1 min 30):
"Wie wil één aha-moment delen uit de handout? Iets wat je gemarkeerd hebt en waarom."
Vang 1-2 vrijwilligers. Bevestig kort. Niet uitdiepen.

Verwijs naar draaiboek blok 3, instructie 7-8.
-->

---
layout: center
class: text-center
---

# Transferopdracht — deze week

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Ga op je eigen lijn na<br/>
  welke <span class="font-bold">signaalregels</span> actief zijn.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-2xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Welke regels?</div>
    <div class="text-xs opacity-70 mt-1">kaal / WECO / Nelson / mix</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Hoeveel alarm?</div>
    <div class="text-xs opacity-70 mt-1">per dag ongeveer</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Past dit?</div>
    <div class="text-xs opacity-70 mt-1">bij wat je nu weet over ARL</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-70 max-w-lg mx-auto">
  Bonus: praat er deze week één keer over met je teamleider.<br/>
  <span class="text-sm opacity-80">"Waarom staat bij ons déze regelset en niet een andere?"</span>
</div>

<!--
Sluit af met de transferopdracht.
"Vraag teamleider, kijk in het dashboard, of vraag engineering.
Noteer in je werkschrift en neem mee naar volgende sessie."

"Volgende workshop vragen we kort rond: welke regelset staat op jouw lijn en hoe vaak krijg je alarm?"

Verwijs naar draaiboek blok 3, instructie 9.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">configuratiebesluit eigen lijn</span> —<br/>
  we bespreken welke regelsets bij welke lijnen passen.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 2 (Train) · Gevoeligheid vs vals alarm
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (configuratiebesluit eigen lijn).

Vergeet niet werkbladen in te nemen of foto's te maken voor learning analytics.

Notities voor jezelf na afloop:
- Welke regelsets hadden deelnemers op hun eigen lijn (of weten ze het niet)?
- Wie zat bij het vrijwillig delen — vrouw-rolmodel aanwezig?
- Is de rekensom bij iemand echt blijven hangen als drempel? Markeer voor volgende keer.

Verwijs naar draaiboek "Checklist na de sessie".
-->
