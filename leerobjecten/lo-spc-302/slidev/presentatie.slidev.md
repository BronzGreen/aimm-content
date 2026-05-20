---
theme: default
title: Pp en Ppk — langetermijn-bekwaamheid
info: |
  ## SPC Module 3 — Op Maat
  Workshop-blok over Cpk-vs-Ppk-gap-diagnose voor de eigen lijn.
  Doelgroep: MBO-4 operators + teamleiders, 45 minuten, coachende stijl.
  v1.0 — 4 slides voor blok 1 (max 4), veel ruimte voor eigen-analyse.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Pp en Ppk

### Wat ervaart je klant écht?

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  MBO-4 operator + teamleider · gap-diagnose voor eigen lijn
</div>

<!--
SLIDE 1 — Cover. Open warm en direct.

"Welkom in module 3 — Op Maat. In het vorige blok keken we naar Cpk — wat je proces kan.
Nu kijken we naar Ppk — wat je klant ervaart.

Soms zijn die twee getallen hetzelfde. Vaak niet. En het verschil tussen die twee is zelf
een signaal. Ik ga jullie weinig vertellen vandaag — meestal vraag ik."

Houd de toon coachend, niet doceren. De MBO-4-doelgroep kent Cpk — laat ze dat voelen.

Verwijs naar draaiboek blok 1, instructie 1.
-->

---
layout: center
class: text-center
---

# Cpk vs Ppk

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-80">
  Twee getallen over hetzelfde proces —<br/>
  maar ze meten iets anders.
</div>

<div class="grid grid-cols-2 gap-6 mt-10 max-w-3xl mx-auto">
  <div v-click class="p-5 bg-blue-50 rounded-xl border-l-4 border-blue-500">
    <div class="font-bold text-blue-900 text-lg">Cpk</div>
    <div class="text-sm mt-2 opacity-80">Kortetermijn · binnen-subgroep</div>
    <div class="text-sm mt-2 font-bold">Wat je proces <span class="underline">kan</span></div>
  </div>
  <div v-click class="p-5 bg-red-50 rounded-xl border-l-4 border-red-500">
    <div class="font-bold text-red-900 text-lg">Ppk</div>
    <div class="text-sm mt-2 opacity-80">Langetermijn · totale spreiding</div>
    <div class="text-sm mt-2 font-bold">Wat je klant <span class="underline">ervaart</span></div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-80 max-w-xl mx-auto">
  Bijna altijd: <span class="font-bold">Cpk ≥ Ppk</span>. Het verschil noemen we de <span class="font-bold">gap</span>.
</div>

<!--
SLIDE 2 — Trigger. Coachende vraag eerst, dan pas de twee blokjes.

Stel coachende vraag aan de groep:
"Wie van jullie heeft weleens meegemaakt dat de Cpk netjes boven 1,33 stond en de klant tóch klaagde?
Hand op."

Wacht. Tel innerlijk tot 5. Vang 2-3 herkenningen.

Dan pas de twee blokjes onthullen met v-click — bevestig wat je hoorde:
"Precies dat is waar Ppk over gaat — wat de klant ervaart over weken, niet wat de machine
laat zien binnen één shift."

Dan de derde v-click: "Cpk groter of gelijk aan Ppk, bijna altijd. Het verschil is de gap."

Daarna: deel wb-03-handout uit:
"Pak je markeerstift. Markeer twee dingen: de Ford-drempel van 1,67, en de vier typische
oorzaken van tussen-subgroep-variatie. Twee minuten — kort."

Zet timer op 2 min. Loop rustig rond, lees mee, stel geen vragen.

Verwijs naar draaiboek blok 1, instructie 2-3.
-->

---

# De gap als diagnose

<div class="grid grid-cols-3 gap-4 mt-8">
  <div v-click class="text-center p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-2xl mb-2 font-bold text-blue-900">&lt; 0,10</div>
    <div class="font-bold text-blue-800">Klein</div>
    <div class="text-xs opacity-70 mt-2">Stabiel proces</div>
    <div class="text-xs opacity-80 mt-3 font-bold">Actie (als Cpk laag):<br/>op het proces zelf</div>
  </div>
  <div v-click class="text-center p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-2xl mb-2 font-bold text-amber-900">0,10 – 0,20</div>
    <div class="font-bold text-amber-800">Middel</div>
    <div class="text-xs opacity-70 mt-2">Tussen-subgroep merkbaar</div>
    <div class="text-xs opacity-80 mt-3 font-bold">Kijk naar:<br/>batches, shifts, setups</div>
  </div>
  <div v-click class="text-center p-5 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-2xl mb-2 font-bold text-red-900">&gt; 0,20</div>
    <div class="font-bold text-red-800">Groot</div>
    <div class="text-xs opacity-70 mt-2">Systeem rondom onrustig</div>
    <div class="text-xs opacity-80 mt-3 font-bold">Actie op:<br/>het systeem rondom</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-sm opacity-80 max-w-2xl mx-auto p-4 bg-slate-50 rounded-lg">
  Een grote gap los je <span class="font-bold">niet</span> op door de machine strakker te zetten.<br/>
  Je lost hem op door wat <span class="font-bold">erbuiten</span> gebeurt onder controle te krijgen.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Diagram lo-spc-302 · Ford PPAP ≥ 1,67 · AIAG SPC · NIST/SEMATECH
</div>

<!--
SLIDE 3 — De gap als diagnose. Centrale didactische slide voor blok 1.

Wijs naar de A3-print voor in de zaal. Toon dit overzicht.

Werkvorm: per categorie niet zelf vertellen — vraag de groep.
Per categorie ~80 sec:

1. Onthul de categorie met v-click (< 0,10, 0,10-0,20, > 0,20).
2. Vraag bij de eerste: "Wat zit er in Ppk dat NIET in Cpk zit?" Wacht 5-7 sec. Vang één antwoord.
   Bevestig: "Alles wat tussen subgroepen gebeurt — shift-wissels, batch-verschillen, setup-afwijkingen, temperatuur."
3. Vraag: "Waarom geldt bijna altijd Cpk >= Ppk?" Wacht. Vang.
   Bevestig: "Omdat tussen-subgroep-variatie boven op binnen-subgroep komt — nooit eronder."
4. Vraag: "Wat betekent het als ze heel dicht bij elkaar liggen?" Vang.
   Bevestig: "Stabiel proces — weinig ruis tussen shifts en batches."

Spuitgiet-anchor (drie zinnen, fictieve referentiecase):
"In de fictieve referentiecase: Cpk 1,42, Ppk 1,05, gap 0,37. Groot gat.
Onderzoek: ploeg B stelde 0,15 mm hoger in dan ploeg A.
Dat is de schaal — concreet, meetbaar, terug te voeren op het systeem rondom. Niet om over te
nemen — om als ijkpunt te gebruiken."

BENOEM expliciet: "Fictieve case, gebaseerd op veldervaring — als illustratie."

Noem bronnen inline: Ford PPAP 4e editie (Ppk ≥ 1,67), AIAG SPC Reference Manual, NIST/SEMATECH e-Handbook.

Tempo: max 5 min voor drie categorieën + spuitgiet. Stiltes van 5-7 sec na elke vraag.

Verwijs naar draaiboek blok 1, instructie 4.
Verwijst naar trainee-SVG: diagram-lo-spc-302.svg.
-->

---
layout: section
---

# Experimenteren

## Jouw Cpk/Ppk-gap — voor jouw lijn

<div class="text-base mt-8 opacity-80 max-w-2xl mx-auto">
  Tot zover het kader. De formules en oorzakenlijst staan op de handout — terug te lezen als referentie.<br/>
  <span class="font-bold mt-4 block">Nu de echte vraag: jouw cijfers op jouw lijn. Vanaf nu jij.</span>
</div>

<!--
SLIDE 4 — Overgang naar blok 2 (experimenteren).

"Tot zover het kader. De formules en oorzakenlijst staan op de handout —
terug te lezen als referentie.
Nu de echte vraag: jouw cijfers op jouw lijn. Vanaf nu jij."

Maak de pedagogische overgang expliciet: van "we lopen samen door" (blok 1, geleide coaching)
naar "jij doet, ik vraag" (blok 2, individueel coaching). Dat sluit naadloos aan op de toon
van blok 1 en breekt de pedagogische lijn niet.

Deel wb-01-eigen-analyse uit (A3 of A4 dubbelzijdig, zes blokken).

"Zes blokken. Scope, cijfers, gap-diagnose, oorzaakhypothesen, actie-beslissing, open vragen.
Per blok: concreet werken. Welke lijn, welke maat, welk getal, welke ploeg. Niet abstract."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Wat ga je nu doen?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het werkblad
<v-clicks>

1. Schrijf bovenaan: **"Mijn lijn is..."** + kritische maat
2. Werk **top-down**: scope → cijfers → gap → hypothese → actie
3. Per blok **één regel** is het minimum
4. **Concreet**: getal, ploeg, batch, datum

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Welke maat geeft klantklachten of scope-uitval?
- Welke getallen heb je uit week 14 (of realistisch schatten)?
- Over hoeveel shifts ging de data?
- Wat is de kleinste observatie die je maandag kunt doen?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  16 min · individueel · A3-werkblad · eigen data of schatting
</div>

<!--
SLIDE 5 — Eigen-analyse-instructie. Toon de instructie. Zet timer op 16 min.

Belangrijke instructie aan jezelf als trainer:
- Loop rond, buig je niet over schouders.
- Bij stagnatie: stel ÉÉN coaching-vraag uit de tabel in het draaiboek per blok van het werkblad. Niet meer.
- GEEF GEEN VOORBEELDEN. Vervang elke neiging tot voorbeeld door een vraag.
- Bij blokkade: drie-zinnen-aanpak — vraag → wacht 5 sec → bevestig wat hij al heeft → stilte.
- Het spuitgiet-anchor mag als ijkpunt (schaal), niet als sjabloon om over te nemen.

PLAN-B (zie draaiboek blok 2, gele box):
Bij 8 min visuele check. Als > 50 % nog bij blok 1-2 (scope + cijfers) hangt:
"Even bijschakelen. Maak scope en cijfers af in deze sessie. Oorzaak-hypothese en maandag-actie
doen we in blok 3, daarna peer-check. Liever scherp tot de gap-diagnose dan dun op alle zes."

Halverwege (8 min): zachte tafelklap.
"Halverwege. Heb je blok 1 (scope) en blok 2 (cijfers) gevuld? Ga door naar de cijfers —
daar leren we het meeste van."

Eindsignaal:
"Pen neer. Leg je werkblad waar je collega het zo kan lezen. Het moet een getal hebben bij
Cpk én Ppk, een gap-classificatie, en één hoofdhypothese."

Verwijs naar draaiboek blok 2, volledige instructie.
-->

---
layout: section
---

# Reflecteren

## STARRT + peer-check in tweetal

<!--
SLIDE 6 — Overgang naar blok 3 (reflecteren).

Deel wb-02-reflectie uit:
"Dit werkblad is de STARRT-reflectie op je eigen analyse: Situatie, Taak, Actie, Resultaat,
Reflectie, Transfer.

Eerst 8 min individueel. Daarna wissel je met een collega voor 7 min peer-check.
Afsluiten met je definitieve maandag-actie onderaan."

Verwijs naar draaiboek blok 3, instructie 1.
-->

---

# STARRT + peer-check

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-5 bg-purple-50 rounded-xl">

### 📝 STARRT — individueel
<v-clicks>

- **S** — Situatie: welke lijn, welke maat?
- **T** — Taak: wat wilde je leren?
- **A** — Actie: hoe heb je gerekend/geschat?
- **R** — Resultaat: gap + Ford-toets
- **R** — Reflectie: welke hypothese + wat verraste?
- **T** — Transfer: maandag-actie

</v-clicks>

<div v-click class="text-xs mt-4 opacity-70">8 min · stil werk · eerlijk invullen</div>

</div>

<div class="p-5 bg-amber-50 rounded-xl">

### 🤝 Peer-check — in tweetal
<v-clicks>

- Ruil wb-01 + wb-02
- Stel **één** scherpe vraag
- *"Klopt de hypothese met wat je écht ziet?"*
- *"Is de maandag-actie klein genoeg?"*
- Pas één ding aan op wb-01
- Schrijf vraag op wb-02

</v-clicks>

<div v-click class="text-xs mt-4 opacity-70">6 min · geen oordeel · doorvragend</div>

</div>

</div>

<div v-click class="mt-6 text-center text-base p-3 bg-blue-50 text-blue-900 rounded-lg max-w-xl mx-auto">
  Sluit af: <span class="font-bold">"Maandag ga ik..."</span> — één zin onderaan wb-02.
</div>

<!--
SLIDE 7 — STARRT + peer-check instructie.

STARRT individueel (8 min). Zet timer.
"Pen op papier. Zes STARRT-blokken, ga door. Eerlijk invullen — ook de lastige vragen
('wat voelde moeilijk?'). Als iets verraste tijdens het invullen, schrijf het op.
Dit is geen test — dit is je denken ordenen."
Loop stil rond, grijp niet in.

Duo's vormen (30 sec):
"Zoek een collega. Bij voorkeur iemand uit een ander type lijn of bedrijf — andere context
= scherpere vragen. Je ruilt wb-01 én wb-02."
Bij oneven aantal: trio met rotatie elke 2 min.

Peer-check (6 min totaal):
"Eerste ronde 3 min: A leest B's werkbladen, B leest A's.
Stel elk minstens één scherpe vraag — niet oordelend, wel doorvragend.
Gebruik de voorbeelden op wb-02. Schrijf de vraag die je krijgt op wb-02, en pas één ding
aan op je wb-01."

Wat je doet als trainer:
- Luister mee, grijp NIET in om te coachen.
- Bij stilte: lees één regel hardop voor van het werkblad, vraag de luisteraar:
  "Wat is de vraag die hier op zijn plaats is?" Modelleer geen vraag — vraag erom.
- Bij oplossings-gedrag: zachtjes "Vraag, geen oplossing — wat wil je weten?"

Plenair slot (2 min): deel 2-3 maandag-acties hardop. Bij aarzeling:
"Wat is de kleinste stap die je maandag nog kunt zetten? Niet de mooiste — de kleinste."

Verwijs naar draaiboek blok 3, volledige instructie.
-->

---
layout: end
---

# Dank

<div class="mt-8 text-base opacity-70">
  Volgend blok in module 3: <span class="font-bold">DMAIC — vijf-stappen verbeterroute</span> (lo-spc-402)<br/>
  <span class="text-sm opacity-60">Als je gap &gt; 0,20 is én Ford-eis niet gehaald — daar zetten we de volgende stap.</span>
</div>

<div class="mt-6 text-sm opacity-60 max-w-xl mx-auto">
  Foto van wb-01 + wb-02 maken. Check-in over 2 weken.<br/>
  <span class="italic opacity-70">Bronnen: Ford PPAP 4th ed. · AIAG SPC · NIST/SEMATECH · spuitgiet = fictieve referentiecase</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · Pp/Ppk · v1.0
</div>

<!--
SLIDE 8 — Afsluiter.

"Dank. Eén woord per persoon — wat neem je mee?"
Kort rondje, jij eindigt ook één woord.

"Foto van wb-01 + wb-02 maken voor jezelf. Check-in over 2 weken.
Volgend blok in module 3: DMAIC (lo-spc-402) — hoe zet je een gap > 0,20 + Ppk onder de
klant-eis om in een verbeterproject."

Notities voor jezelf na afloop:
- Foto's van alle wb-01-werkbladen gemaakt?
- Maandag-acties genoteerd per deelnemer (input voor check-in)?
- Welke deelnemers Ford-eis Ppk ≥ 1,67 niet haalden (DMAIC-prioriteit)?
- Welke deelnemers hadden geen eigen data (nabellen voor check-in)?
- Parkeerflip-vragen: DMAIC-vragen overdragen aan trainer lo-spc-402, formule-details naar lo-spc-301.

Verwijs naar draaiboek "Checklist na de sessie".
-->
