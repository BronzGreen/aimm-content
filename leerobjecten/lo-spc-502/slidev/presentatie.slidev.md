---
theme: default
title: Welke kaart, welke bovengrens, welk signaal?
info: |
  ## SPC Module 2 — Train
  Workshop-blok over de c-kaart, UCL-berekening en Nelson-regel-1.
  Doelgroep: operators MBO-3/4 + teamleiders MBO-4, 45 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Welke kaart?

### Welke bovengrens? Welk signaal?

<div class="mt-12 text-sm opacity-60">
  SPC Module 2 (Train) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3/4 + teamleiders · c-kaart en escalatie
</div>

<!--
Open warm.
"Stel je voor: je staat om 7 uur 's ochtends op een assemblagelijn. Nieuwe materiaalbatch.
Eerste uur zie je 8 soldeerfouten op 50 boards. Normaal 2 of 3. Is dit toeval — of bel je nu?"

Wacht. Laat 1-2 mensen knikken. Geen lange verhalen.

Trigger: "Wie nu aan de bel trekt = schade beperkt tot ~150 boards.
Wie een uur afwacht = 500. Wie een shift afwacht = duizenden.
Dat is het verschil dat we vandaag maken."

Verwijs naar draaiboek blok 1, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Vandaag leer je

<v-clicks>

- Welke **kaart** past bij telgegevens (c / p / np / u)
- Hoe je de **UCL** berekent met c̄ + 3√c̄
- Wat **Nelson-regel-1** is — en waarom één punt al telt
- De **escalatieketen** van operator naar leverancier
- Waarom **traceerbaarheid** de voorwaarde is

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">🎯</div>
    <div class="text-xl font-mono font-bold text-red-600">8 fouten · t=0</div>
    <div class="text-sm opacity-60 mt-2">wat doe je nu?</div>
  </div>
</div>

<!--
Korte ophaal voorkennis (1 min).
"Snel rondje — wie kan in één zin zeggen wat 'één punt buiten UCL' betekende
in de sessie van gisteren?"
Verwijs naar lo-spc-201 (Nelson-regels generiek), lo-spc-108 (common vs special cause).

Vang 1-2 antwoorden, bevestig kort.
"Goed — Nelson-regel-1. Dat komt vandaag terug, specifiek op de c-kaart voor tellingen.
Maar eerst gaan jullie het zelf proberen."

Verwijs naar draaiboek blok 1, instructie 3.
-->

---
layout: center
class: text-center
---

# 🟢 Werkblad — c-kaart oefening

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Eén PCB-casus.<br/>
  Vier deelvragen.<br/>
  <span class="font-bold">Formule staat op het werkblad.</span>
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Kaart? · UCL? · Signaal? · Eerste stap?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  11 minuten · individueel · pen + rekenmachine
</div>

<!--
Deel wb-01-oefening uit (30 sec).
"Eén casus. Vier deelvragen. Op het werkblad staan alle getallen die je nodig hebt —
en de formule. Jouw taak: kies de kaart, reken de UCL, markeer het signaal,
schrijf op wat je als eerste zou doen. Bij twijfel: zet een vraagteken."

Zet timer op 11 min. Loop rond. Beantwoord praktische vragen, GEEN inhoudelijke.
"Is c de goede kaart?" → "Schrijf op wat jij denkt, ook als je twijfelt."

Na 11 min: buurman-check (1 min) — alleen verschillen noteren, niet uitleggen.
Verzamel-moment: "Bij welke deelvraag had je de meeste twijfel? Hand op bij kaartkeuze...
UCL... signaal... eerste stap." Tel, schrijf op flip-over.

NB: fictieve PCB-casus uit ko-spc-502 — bewust markeren als "fictief voorbeeld".

Verwijs naar draaiboek blok 1, instructie 4-7.
-->

---
layout: section
---

# Reflecteren

## Wanneer werd het bij jou pas laat gezien?

<!--
Overgang naar blok 2.
"Jullie hebben net geoefend op een fictieve casus — bewust simpel.
In de praktijk is het zelden zo helder. We halen nu één concreet moment terug
waarop een materiaal- of kwaliteitsprobleem op jouw lijn pas laat werd opgemerkt."

Benadruk: geen eigen incident? Iets wat een collega vertelde telt ook.
Alleen de T (Transfer) mag straks vrijwillig plenair gedeeld worden.

Verwijs naar draaiboek blok 2, instructie 1-2.
-->

---

# STARRT — zes stappen

<div class="grid grid-cols-3 gap-3 mt-6">
  <div class="text-center p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-2xl mb-1">🔵</div>
    <div class="text-sm font-bold text-blue-800">S — Situatie</div>
    <div class="text-xs opacity-70 mt-1">Welk moment, welke lijn?</div>
  </div>
  <div class="text-center p-4 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-2xl mb-1">🟣</div>
    <div class="text-sm font-bold text-purple-800">T — Taak</div>
    <div class="text-xs opacity-70 mt-1">Wat was jouw rol?</div>
  </div>
  <div class="text-center p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-2xl mb-1">🟢</div>
    <div class="text-sm font-bold text-green-800">A — Actie</div>
    <div class="text-xs opacity-70 mt-1">Wat deed je, wie werd geïnformeerd?</div>
  </div>
  <div class="text-center p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-2xl mb-1">🟠</div>
    <div class="text-sm font-bold text-amber-800">R — Resultaat</div>
    <div class="text-xs opacity-70 mt-1">Hoeveel uren/stuks ertussen?</div>
  </div>
  <div class="text-center p-4 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-2xl mb-1">🔴</div>
    <div class="text-sm font-bold text-red-800">R — Reflectie</div>
    <div class="text-xs opacity-70 mt-1">Met c-kaart: wanneer eerder?</div>
  </div>
  <div class="text-center p-4 bg-yellow-50 rounded-xl border-2 border-yellow-300">
    <div class="text-2xl mb-1">🟡</div>
    <div class="text-sm font-bold text-yellow-800">T — Transfer</div>
    <div class="text-xs opacity-70 mt-1">Welke stap deze week?</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  De eerste vijf blijven van jou. De laatste T mag je vrijwillig plenair delen.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min individueel · wb-02-reflectie
</div>

<!--
Deel wb-02 uit. "STARRT — zes korte stapjes. Alleen de Transfer mag je straks
vrijwillig plenair delen. Als niemand wil delen, ook prima."

Zet timer op 10 min. Blijf op afstand, buig je niet over schouders.
Stilte verdragen — sommige deelnemers hebben 3 min nodig om een moment op te halen.

Bij blokkade zachte hints:
- "Welk moment komt als eerste in je op bij 'pas na een hele shift werd het opgepakt'?"
- "Geen eigen incident? Iets wat een collega je vertelde mag ook."
- "De R van Reflectie: als er die dag een c-kaart had gehangen — wanneer had je kunnen handelen?"

Bij emotionele reacties (iemand bij een echte miskleun): "Je hoeft het niet op te
schrijven. De reflectie is voor jezelf."

Verwijs naar draaiboek blok 2, instructie 3.
-->

---
layout: center
class: text-center
---

# Transfer — wat neem je mee?

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Eén zin per persoon.<br/>
  Welke <span class="font-bold">concrete stap</span> neem jij deze week<br/>
  op jouw eigen lijn?
</div>

<div v-click class="mt-8 inline-block px-6 py-3 bg-amber-100 text-amber-900 rounded-lg text-base">
  Vrijwillig · 3-4 deelnemers · max 45 sec per persoon
</div>

<div v-click class="mt-6 text-sm opacity-70 max-w-lg mx-auto">
  Geen vraag naar de Situatie — dat was privé.<br/>
  Alleen: "Wat ga je maandag anders doen?"
</div>

<!--
4 min plenair. "Wie wil in één zin de Transfer delen?"
3-4 deelnemers max 45 sec. Bevestig kort: "Concreet — dat helpt."
of "Goed dat je aan de teamleider-kant begint."

NIET doorvragen op de Situatie. NIET zelf een anekdote delen.
NIET hun Transfers op de flip-over schrijven — die stappen zijn van hen.

Valkuil: reflectie wordt klaagronde. Bij "wij doen het altijd fout":
"Voor de reflectie: wat had jíj toen kunnen doen, wat ga je deze week doen?"
Verplaats altijd naar eigen actie.

Verwijs naar draaiboek blok 2, instructie 4-5.
-->

---
layout: section
---

# Theoretiseren

## Welke kaart, welke formule, welke regel?

<!--
Overgang naar blok 3.
"Jullie hebben net zelf ervaren dat tussen 'iets voelt niet goed' en
'er wordt actie ondernomen' soms uren zitten.

We gaan nu precies uittekenen: wélke kaart, wélke formule, wélke regel.
En hoe de escalatieketen eruit ziet zodat uren minuten worden."

Onthul het A3-diagram achter in de zaal.
Deel wb-03-handout uit. "Pak je markeerstift. Markeer één aha-moment."

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---

# Het centrale diagram

<div class="mt-6 text-center">
  <img src="../../trainee/lo-spc-502/diagram-lo-spc-502.svg" class="max-h-100 mx-auto rounded-lg shadow-lg" alt="c-kaart PCB — Nelson-regel-1 na materiaalwissel" />
</div>

<div v-click class="mt-4 text-center text-sm opacity-70">
  Regelkaart · keuzehulp · escalatieketen — alles op één plaat
</div>

<div class="abs-br m-6 text-xs opacity-40">
  diagram-lo-spc-502.svg · ook A3 achter in de zaal
</div>

<!--
"Drie dingen op één plaat.
- Links: de regelkaart die jullie net hebben uitgerekend. c̄ = 2,4, UCL op 7,1,
  meetreeks 8/6/9. De rode stip op t=0 is Nelson-regel-1.
- Rechts: de keuzehulp c/p/np/u.
- Onder: de escalatieketen in vijf stappen.

Dit diagram neem je straks mee — het is je naslagwerk voor op je lijn."

Stilte van 3 sec. Laat de hele plaat landen.

Verwijs naar draaiboek blok 3, instructie 1.
-->

---
layout: two-cols
layoutClass: gap-6
---

# Kaart kiezen — twee vragen

<div class="mt-6 text-sm">

**Vraag 1:** Tel je...
<v-clicks>

- **defecten** (een item kan er meerdere hebben)?
- of **defecte stuks** (elk telt 1×)?

</v-clicks>

</div>

<div v-click class="mt-6 text-sm">

**Vraag 2:** Is je eenheid...
- **constant** (altijd 50 boards)?
- of **variabel** (soms 30, soms 80)?

</div>

::right::

<div class="mt-4 text-xs">

| Je telt… | Eenheid | **Kaart** |
|----------|---------|:---------:|
| Defecten | constant | **c** |
| Defecten | variabel | u |
| Stuks | constant | np |
| Fractie (%) | variabel | p |

</div>

<div v-click class="mt-6 p-3 bg-green-50 rounded-lg border-l-4 border-green-400 text-sm">
  <span class="font-bold text-green-800">Onze casus:</span>
  fouten (meerdere per board) · vaste eenheid (50 boards) →
  <span class="font-bold">c-kaart</span>
</div>

<!--
Verwijs terug naar oefening. "Wie koos c? Wie iets anders?" Vang stemming.
Als 70%+ c koos: "Mooi. Laten we vastleggen waarom."
Als < 50% c: "Dat is juist het vakmanschap. Kijk mee."

Schrijf op flip-over:
- Defecten + constant = c
- Defecten + variabel = u
- Stuks + constant = np
- Fractie + variabel = p

Koppel terug: "In onze casus telden jullie soldeerfouten (een board kan er meerdere
hebben) per vaste eenheid (50 boards). Dat is c. Niet np — np telt defecte boards,
en dan had één board met vier fouten één defect opgeleverd, niet vier."

Benoem: "De keuze is het vakmanschap — niet de formule."

Valkuil vk-01: deelnemers willen p of u formules. "Goede vraag voor module 3.
Vandaag blijven we bij c."

Verwijs naar draaiboek blok 3, instructie 3.
-->

---
layout: two-cols
layoutClass: gap-6
---

# De c-kaart formule

<div class="text-2xl font-mono mt-4 mb-6 text-red-700">
  UCL = c̄ + 3√c̄
</div>

<v-clicks>

- **c̄** = historisch gemiddelde aantal fouten per eenheid
- **3√c̄** = drie keer wortel van c̄ (Poisson-aanname)
- **LCL** = c̄ − 3√c̄ — als negatief: afkappen op **0**

</v-clicks>

::right::

<div class="mt-4 p-4 bg-amber-50 rounded-xl border-2 border-amber-200">

### Uitgewerkt · c̄ = 2,4
<div class="font-mono text-sm mt-2 space-y-1">
  <div>√2,4 ≈ 1,549</div>
  <div>3 × 1,549 ≈ 4,65</div>
  <div class="text-base font-bold text-amber-700 pt-2">UCL = 2,4 + 4,65 ≈ 7,1</div>
  <div class="text-sm text-gray-600">LCL = 2,4 − 4,65 = −2,25 → 0</div>
</div>

</div>

<div v-click class="mt-4 text-xs text-center opacity-70">
  Een punt ≥ 8 fouten ligt dus boven UCL
</div>

<!--
Schrijf op flip-over: UCL = c̄ + 3√c̄.

"De formule is ongemakkelijk eenvoudig. Bewust — de c-kaart gaat uit van een
Poisson-verdeling, en daarin is de standaardafwijking gewoon de wortel van het gemiddelde."

Werk de getallen uit op het bord — exact zoals op slide.
"c̄ = 2,4. √2,4 ≈ 1,549. Drie keer is 4,65. UCL = 2,4 + 4,65 ≈ 7,1."

LCL: "2,4 − 4,65 = −2,25 — wordt 0. Telling kan niet negatief zijn."

Valkuil vk-02: "waarom precies 3σ?"
"3σ is de gangbare keuze bij Shewhart-kaarten — volgt AIAG, NIST, Nelson (1984).
Statistische onderbouwing komt in module 3 of vraag je kwaliteitsdienst."

Verwijs naar draaiboek blok 3, instructie 4.
-->

---
layout: center
class: text-center
---

# Nelson-regel-1

<div class="text-2xl mt-6 max-w-2xl mx-auto leading-relaxed">
  Eén punt buiten de ±3σ-grenzen<br/>
  = <span class="font-bold text-red-700">signaal van special cause</span>
</div>

<div v-click class="mt-8 inline-block px-6 py-3 bg-red-100 text-red-900 rounded-lg text-base">
  Kans op toeval bij stabiel Poisson-proces: ≈ 0,3%
</div>

<div v-click class="mt-6 text-base opacity-80 max-w-xl mx-auto">
  Als je het tóch ziet, is de kans dat er écht iets bijzonders gebeurt<br/>
  <span class="font-bold">vele malen groter</span> dan de kans op pech.
</div>

<div v-click class="mt-6 p-3 bg-amber-50 rounded-lg text-sm max-w-md mx-auto">
  <span class="font-bold">Daarom is één punt genoeg</span> —<br/>
  je hoeft niet te wachten op bevestiging.
</div>

<div v-click class="mt-6 text-xs opacity-60 max-w-lg mx-auto">
  Bron: Nelson, L.S. (1984). "The Shewhart Control Chart — Tests for Special Causes."<br/>
  Journal of Quality Technology, 16(4), 237-239.
</div>

<!--
"Eén punt buiten ±3σ-grenzen. Bij stabiel Poisson-proces is de kans op toeval ≈ 0,3%.
Als je het tóch ziet, is er vele malen waarschijnlijker iets bijzonders aan de hand.

Dat is waarom één punt genoeg is om te handelen — je hoeft niet te wachten op
een tweede bevestiging."

Verwijs naar bron: "Dit is regel 1 van acht in Nelson's artikel uit 1984.
De andere zeven gaan over patronen over meerdere punten. Regel 1 is de krachtigste
én de makkelijkste — vandaag houden we het bij deze."

Verwijs naar draaiboek blok 3, instructie 4.
-->

---

# De meetreeks — wat zie je?

<div class="mt-4">

| Uur | Fouten | Boven UCL (7,1)? | Betekenis |
|-----|:------:|:----------------:|-----------|
| t=0 | **8** | <span class="text-red-700 font-bold">Ja</span> | **Nelson-regel-1 — eerste signaal. Escaleren NU.** |
| t=1 | 6 | Nee | Hoog, maar binnen UCL — op zichzelf geen signaal |
| t=2 | **9** | <span class="text-red-700 font-bold">Ja</span> | **Bevestiging — patroon is echt** |

</div>

<div v-click class="mt-8 p-4 bg-red-50 rounded-lg text-center border-l-4 border-red-400 max-w-xl mx-auto">
  <span class="font-bold text-red-800">De operatorles</span><br/>
  <span class="text-sm">Niet wachten op bevestiging.</span><br/>
  <span class="text-sm">Bij t=0 is de materiaalbatch verdacht.<br/>Bij t=2 is het zeker.</span>
</div>

<!--
Loop door de tabel.
"t=0: 8 fouten boven UCL van 7,1. Nelson-regel-1 is compleet op dit ene punt.
Wie nu escaleert, beperkt de impact tot ~150 boards."

"t=1: 6 fouten. Onder UCL — op zichzelf geen signaal. Het valt mee."

"t=2: 9 fouten. Wéér boven UCL. Dit is de bevestiging — maar je had de escalatie
al 2 uur eerder moeten starten."

KERNZIN: "Niet wachten op bevestiging. Bij t=0 is de materiaalbatch verdacht;
bij t=2 is het zeker. Het verschil tussen die twee momenten = 100 boards."

Verwijs naar draaiboek blok 3, instructie 4 (slot).
-->

---

# De escalatieketen — 5 stappen

<div class="mt-4 text-sm">

| # | Stap | Door wie? | Wanneer? |
|---|------|-----------|----------|
| 1 | Operator informeert **teamleider** | operator | direct · t=0 |
| 2 | Boards van verdachte uren **apart zetten** | operator + ploeg | binnen 15 min |
| 3 | Escalatie naar **kwaliteit + engineering** | teamleider | binnen 30 min |
| 4 | Materiaalbatch in **quarantaine** | engineering / magazijn | binnen 1 uur |
| 5 | **Leverancier** informeren — batch terugroepen | inkoop / kwaliteit | binnen 2 uur |
| 6 | Productie hervatten met **vorige batch** | operator + teamleider | zodra bevestigd OK |

</div>

<div v-click class="mt-6 grid grid-cols-2 gap-4">
  <div class="p-3 bg-green-50 rounded-lg text-center border-l-4 border-green-400">
    <div class="font-bold text-green-800">Escalatie binnen 2 uur</div>
    <div class="text-sm opacity-80">impact ≈ <span class="font-bold">150 boards</span> (3 uur × 50)</div>
  </div>
  <div class="p-3 bg-red-50 rounded-lg text-center border-l-4 border-red-400">
    <div class="font-bold text-red-800">Escalatie na shift</div>
    <div class="text-sm opacity-80">impact = <span class="font-bold">duizenden boards</span></div>
  </div>
</div>

<!--
Wijs op onderste deel A3-diagram. "Vijf stappen, elk met een tijdsdoel.
Dit is geen theorie — dit is de reden dat we vandaag hier staan."

Loop de stappen door — exact zoals draaiboek blok 3 instructie 5:
- Stap 1: teamleider direct (t=0). Niet bij koffiepauze. Direct.
- Stap 2: boards apart (< 15 min). Op de werkvloer, niet in het kantoor.
- Stap 3: kwaliteit + quarantaine (< 1 uur). Teamleider regelt, materiaal fysiek apart.
- Stap 4: leverancier / terugroepen (< 2 uur). Inkoop of kwaliteit. Signaal begon bij jou.
- Stap 5/6: hervatten met vorige batch (zodra OK). Niet doorgaan met verdacht materiaal.

Schrijf op flip-over: "2 uur = ~150 boards. Hele shift = duizenden."

Valkuil vk-03: "wij kunnen niet zomaar de leverancier bellen."
Niet uitpraten. "Wie kan dat op jouw lijn wel? Noteer die naam op wb-03 onder stap 4."

Verwijs naar draaiboek blok 3, instructie 5.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Voorwaarde: traceerbaarheid

<v-clicks>

- Welke **batch** is wanneer op welke **lijn** gegaan?
- In welke **boards** verwerkt?
- Staat dat in het **MES**, op **papier**, of **nergens**?

</v-clicks>

<div v-click class="mt-6 p-3 bg-amber-50 rounded-lg text-sm">
  Zonder registratie: Nelson-regel-1 zie je nog steeds —<br/>
  <span class="font-bold">maar terugroepen lukt niet.</span>
</div>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-6xl mb-4">🔗</div>
    <div class="text-base opacity-70 max-w-xs mx-auto">
      Batch-ID ↔ uur-inspectie<br/>
      Batch-ID ↔ boards
    </div>
  </div>
</div>

<!--
"De hele keten werkt alleen als materiaal-traceerbaarheid is geregeld:
welke batch is wanneer op welke lijn gegaan, in welke boards verwerkt.

Zonder die registratie: Nelson-regel-1 zie je nog steeds, boards apart zetten werkt —
maar terugroepen lukt niet, en de leverancier kan niet gericht onderzoeken."

Praktische check: "Wordt op jouw lijn de batch-ID gekoppeld aan de uur-inspectie?
Staat dat in het MES, op papier, of nergens? Vraag dit deze week aan je teamleider —
dat is de bonus-transferopdracht."

Differentiatie teamleider: parkeer "wie is stap 3, wie is stap 4 op jouw lijn?"
voor de groepsreflectie die volgt in module 2.

Verwijs naar draaiboek blok 3, instructie 6.
-->

---
layout: center
class: text-center
---

# Transferopdracht — deze week

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Zoek op jouw eigen lijn <span class="font-bold">één kwaliteitsgrootheid</span><br/>
  die je per <span class="font-bold">vaste eenheid</span> telt.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-2xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Wat tel je?</div>
    <div class="text-xs opacity-70 mt-1">soldeerfouten · krassen · labels</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Per welke eenheid?</div>
    <div class="text-xs opacity-70 mt-1">50 boards · 100 stuks · 1 pallet</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Wat is c̄?</div>
    <div class="text-xs opacity-70 mt-1">vraag teamleider · kijk in rapport</div>
  </div>
</div>

<div v-click class="mt-6 text-base opacity-80">
  Reken zelf de <span class="font-bold">UCL uit</span> met c̄ + 3√c̄.
</div>

<div v-click class="mt-4 text-sm opacity-70 max-w-lg mx-auto">
  <span class="font-bold">Bonus:</span> vraag of de leverancierscode / batch-ID<br/>
  op jouw lijn aan de telgegevens gekoppeld wordt.
</div>

<!--
Slide 10. "Eén opdracht voor deze week.

Zoek op jouw eigen lijn één kwaliteitsgrootheid die je per vaste eenheid telt —
soldeerfouten per 50 boards, krassen per 100 stuks, foute labels per pallet.

Vraag je teamleider naar het gemiddelde over de laatste weken. Reken zelf de UCL uit
met c̄ + 3√c̄. Neem dit mee naar de volgende sessie — we bespreken per persoon
of je UCL realistisch is.

Bonus: vraag of de batch-ID aan de uur-inspectie gekoppeld wordt.
Zo niet — dan is Nelson-regel-1 nog wel te zien, maar terugroepen wordt lastig."

Verwijs naar draaiboek blok 3, instructie 7.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende blok in module 2: <span class="font-bold">groepsreflectie traceerbaarheid + escalatie-verantwoordelijkheid</span>
</div>

<div class="mt-4 text-xs opacity-50 max-w-lg mx-auto">
  Bronnen: AIAG SPC Reference Manual · NIST/SEMATECH sectie 6.3.3 ·<br/>
  Nelson (1984) Journal of Quality Technology 16(4) · ko-spc-502 (fictief voorbeeld)
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 2 (Train) · c-kaart + Nelson-regel-1
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (groepsreflectie traceerbaarheid
en escalatie-verantwoordelijkheid).

Vergeet niet wb-01 en wb-03 in te nemen of foto's te maken voor learning analytics.
wb-02 blijft bij de deelnemer (privé-reflectie).

Notities voor jezelf na afloop:
- Bij welke deelvraag was de meeste twijfel? (kaart / UCL / signaal / eerste stap)
- Welke kwaliteitsgrootheden hebben deelnemers gekozen voor de eigen UCL?
- Bij teamleider-deelnemers: warm overdragen naar groepsreflectie traceerbaarheid.
- Bij emotionele momenten in blok 2: informeel napraten met deelnemer.

Verwijs naar draaiboek "Checklist na de sessie".
-->
