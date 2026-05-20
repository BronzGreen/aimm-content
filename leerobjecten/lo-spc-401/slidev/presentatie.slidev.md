---
theme: default
title: Six Sigma — wat het is en hoe het zich verhoudt tot SPC
info: |
  ## SPC Module 3 — Op Maat
  Workshop-blok over Six Sigma-positionering ten opzichte van SPC.
  Doelgroep: operators MBO-4 en teamleiders MBO-4 die met SPC werken. 45 minuten, coachende stijl.
  v1.0 — handout + STARRT + eigen-vraagstuk-positionering met maandag-actie.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Six Sigma

### Wat het is — en waar jouw SPC ophoudt

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-4 + teamleiders · Positionering SPC binnen DMAIC
</div>

<!--
SLIDE 1 — Cover. Open warm en direct.

"Welkom. Je werkt al met regelkaarten en Cpk. Vandaag leggen we daar één puzzelstuk naast: Six Sigma.
Niet om iets nieuws te leren, maar om te zien waar SPC ophoudt en waar een breder verbeterproject begint.
Aan het eind van dit uur heb jij één lopend vraagstuk van jouw lijn gepositioneerd — met een maandag-actie."

Houd de toon coachend. De doelgroep is bewust bekwaam — ze kennen SPC al in de praktijk.

Verwijs naar draaiboek blok 1, instructie 1.
-->

---
layout: center
class: text-center
---

# Waarom dit onderwerp?

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-80">
  Je kent de zinnen al:
</div>

<div class="grid grid-cols-3 gap-4 mt-8 max-w-3xl mx-auto">
  <div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
    <div class="font-bold text-amber-900">"Hier moet DMAIC op"</div>
    <div class="text-xs mt-2 opacity-70">maar waar begin je?</div>
  </div>
  <div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
    <div class="font-bold text-amber-900">"Dit is een Six Sigma-project"</div>
    <div class="text-xs mt-2 opacity-70">en jouw kaart?</div>
  </div>
  <div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
    <div class="font-bold text-amber-900">"Sigma-niveau 4"</div>
    <div class="text-xs mt-2 opacity-70">is dat jouw Cpk?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-80 max-w-xl mx-auto">
  Vandaag maken we scherp: <span class="font-bold">waar eindigt SPC, waar begint Six Sigma.</span>
</div>

<!--
SLIDE 2 — Trigger-slide. Coachende vraag eerst, dan de drie zinnen onthullen.

Stel coachende vraag:
"Wanneer heeft een collega of kwaliteitscoördinator voor het laatst tegen jou gezegd:
'we moeten er een Six Sigma-project van maken' of 'laten we DMAIC erop zetten'? Wat voelde je toen — snapte je wat ze bedoelden?"

Wacht. Tel innerlijk tot 7. Vang 2-3 antwoorden.

Dan pas de drie blokjes onthullen met v-click — bevestig wat je hoorde:
"Wat ik hoor is herkenning — je weet dat het bestaat, maar de exacte grens met SPC blijft schimmig. Precies dat maken we scherp."

Daarna: deel wb-03-handout uit:
"Pak je markeerstift. Scan de handout kort. Markeer wat je al wist en wat nieuw is. Twee minuten."
Zet timer op 2 min. Loop rustig rond, lees mee, stel geen vragen.

Verwijs naar draaiboek blok 1, instructie 2-3.
-->

---

# SPC binnen DMAIC

<div class="grid grid-cols-5 gap-3 mt-8">
  <div v-click class="text-center p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-3xl mb-2">🎯</div>
    <div class="font-bold text-blue-800">Define</div>
    <div class="text-xs opacity-70 mt-1">Wat is het probleem?</div>
    <div class="text-[10px] mt-2 opacity-50">SIPOC · charter</div>
  </div>
  <div v-click class="text-center p-4 bg-orange-50 rounded-xl border-2 border-orange-300 ring-2 ring-orange-400 ring-offset-1">
    <div class="text-3xl mb-2">📊</div>
    <div class="font-bold text-orange-800">Measure</div>
    <div class="text-xs opacity-70 mt-1">Baseline?</div>
    <div class="text-[10px] mt-2 font-bold text-orange-700">SPC baseline · Gage R&amp;R</div>
  </div>
  <div v-click class="text-center p-4 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-3xl mb-2">🔍</div>
    <div class="font-bold text-purple-800">Analyze</div>
    <div class="text-xs opacity-70 mt-1">Oorzaak?</div>
    <div class="text-[10px] mt-2 opacity-50">visgraat · 5-Why</div>
  </div>
  <div v-click class="text-center p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-3xl mb-2">🛠️</div>
    <div class="font-bold text-green-800">Improve</div>
    <div class="text-xs opacity-70 mt-1">Verandering?</div>
    <div class="text-[10px] mt-2 opacity-50">pilot · DOE</div>
  </div>
  <div v-click class="text-center p-4 bg-red-50 rounded-xl border-2 border-red-300 ring-4 ring-red-400 ring-offset-1">
    <div class="text-3xl mb-2">🔒</div>
    <div class="font-bold text-red-800">Control</div>
    <div class="text-xs opacity-70 mt-1">Borging?</div>
    <div class="text-[10px] mt-2 font-bold text-red-700">SPC kernrol · audit</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-sm opacity-80 max-w-2xl mx-auto">
  SPC staat <span class="font-bold">vooral in Control</span> (borging) en <span class="font-bold">Measure</span> (baseline).<br/>
  <span class="text-xs opacity-70">In Analyze hooguit als data-bron — oorzaken vindt SPC niet.</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  diagram-lo-spc-401.svg — A3-print achter in zaal
</div>

<!--
SLIDE 3 — Centrale didactische slide. DMAIC met SPC-accentring rond Measure (dun) en Control (dik).

Wijs naar de A3-print achter in de zaal. Toon dit overzicht.

Werkvorm: loop de vier ankerpunten af. Niet alle 9 handout-secties behandelen.

Ankerpunt (a) — Definitie + historie (90 sec):
"Wie kan in eigen woorden zeggen wat Six Sigma is?" — vang één antwoord. Scherp aan:
"Data-gedreven verbeterbenadering, doel 3,4 DPMO, ontstaan Motorola 1986 (Bill Smith), opgeschaald GE onder Welch jaren '90." Eén zin.

Ankerpunt (b) — Het 1,5σ-shift-detail (2 min). Kritiek punt.
"De 3,4 DPMO hoort bij een 1,5σ-shift-aanname. 'Zes sigma' in Six Sigma-taal is niet hetzelfde als de zuiver kortetermijnkans
van een perfect gecentreerde normaalverdeling. Wees voorzichtig met terminologie."
GEEN wiskundige uitleg — wel correct benoemen.

Ankerpunt (c) — Sigma-niveau vs Cpk (90 sec).
Vraag: "Stel je kwaliteitscoördinator zegt 'we zitten op sigma-niveau 4' — is dat hetzelfde als Cpk 1,33?"
Wacht 5-7 sec. Vang antwoord. Scherp aan:
"Nee. Sigma-niveau is managementmaat voor defectkans, inclusief 1,5σ-shift. Cpk is capability-index uit SPC-data. Niet verwisselen."

Ankerpunt (d) — DMAIC-tabel, waar zit SPC (3 min).
Onthul de vijf fases met v-click. Wijs de twee accent-ringen aan (Measure dunne ring, Control dikke ring).
Vraag: "In welke DMAIC-fase zit jouw regelkaart meestal?" Vang antwoorden.
Bevestig: "Vooral Control — daar borgt hij. En als baseline-bron in Measure. In Analyze levert SPC hooguit data, geen oorzaken."

Verwijs naar draaiboek blok 1, instructie 4.
Verwijst naar SVG: diagram-lo-spc-401.svg.
-->

---
layout: center
class: text-center
---

# De kernboodschap

<div class="mt-12 max-w-3xl mx-auto">

<div class="text-3xl leading-relaxed font-semibold text-slate-800 italic">
  "Een regelkaart is niet het hele verbeterproces,<br/>
  maar wel het instrument waarmee je ziet<br/>
  of een verbetering werkelijk blijft staan."
</div>

<div v-click class="mt-12 grid grid-cols-3 gap-4">
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-900 text-sm">Vóór het project</div>
    <div class="text-xs mt-1 opacity-75">SPC = baseline (Measure)</div>
  </div>
  <div class="p-4 bg-green-50 rounded-lg">
    <div class="font-bold text-green-900 text-sm">Tijdens het project</div>
    <div class="text-xs mt-1 opacity-75">SPC = pilot-monitoring (Improve)</div>
  </div>
  <div class="p-4 bg-red-50 rounded-lg">
    <div class="font-bold text-red-900 text-sm">Ná het project</div>
    <div class="text-xs mt-1 opacity-75">SPC = borging (Control)</div>
  </div>
</div>

</div>

<!--
SLIDE 4 — Kernboodschap. Lees voor.

"Dat is het zinnetje dat je vasthoudt. De rest is context."

Optioneel v-click: de drie rollen van SPC in een verbeterproject (baseline, monitoring, borging).

Niet uitweiden — de volgende slide is de overgang naar blok 2.

Verwijs naar draaiboek blok 1, instructie 5.
-->

---
layout: section
---

# Reflecteren

## STARRT — toen SPC alleen niet volstond

<div class="text-base mt-8 opacity-80 max-w-2xl mx-auto">
  Eén moment uit jouw praktijk.<br/>
  <span class="font-bold mt-4 block">Een terugkerende uitval, een drift, een signaal waar je niet uit kwam.</span>
</div>

<!--
SLIDE 5 — Overgang naar blok 2 (reflecteren).

"Tot zover de theorie. Nu naar een moment uit je eigen praktijk waar dit precies zo speelde."

Deel wb-02-reflectie uit.
"Dit werkblad loopt via STARRT. Vijf echte letters plus één voor Transfer.
Je gaat één concrete situatie ophalen waar je regelkaart een probleem liet zien dat met SPC alleen niet op te lossen was —
een drift, een terugkerend patroon, een signaal waar je nog niet uit kwam."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# STARRT — in 11 minuten

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Snel doorlopen
<v-clicks>

- **S**ituatie — welke kaart, welk signaal?
- **T**aak — wat moest je doen?
- **A**ctie — wat heb je gezet?
- **R**esultaat — is het opgelost?

</v-clicks>

</div>

<div>

### Hier zit de waarde
<v-clicks>

- **R**eflectie — welke vraag kon de kaart níét?
- **T**ransfer — wat doe je nu anders?
- **Bonus** — sigma-niveau versus Cpk

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center p-4 bg-amber-50 rounded-lg max-w-xl mx-auto">
  <span class="font-bold text-amber-900">S, T, A, R:</span> steekwoorden zijn prima.<br/>
  <span class="font-bold text-amber-900">R (reflectie) + T (transfer):</span> iets meer pen.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  11 min · individueel · stil · trainer coacht met vragen
</div>

<!--
SLIDE 6 — STARRT-overzicht. Zet timer op 11 min.

Instructie aan jezelf als trainer:
- Loop rond, buig je niet over schouders.
- Bij stagnatie: stel één coaching-vraag uit draaiboek blok 2 per STARRT-stap. Niet meer.
- GEEF GEEN VOORBEELDEN. Vervang elke neiging tot voorbeeld door een vraag.
- Stilte is welkom — reflectie heeft rust nodig.

Halverwege (6 min): zachte tafelklap.
"Halverwege. Check: zit je al bij R — de reflectie? Daar zit de waarde."

Eindsignaal:
"Pen neer. De terminologie-check onderaan hoeft niet af — die is bonus."

Verwijs naar draaiboek blok 2, volledige instructie.
-->

---
layout: section
---

# Experimenteren

## Jouw vraagstuk in DMAIC

<!--
SLIDE 7 — Overgang naar blok 3 (eigen vraagstuk + maandag-actie).

Deel wb-01-eigen-analyse uit.
"Dit is het werkblad dat je meeneemt. Acht korte vragen. Eindigt met één concrete maandag-actie —
een zin, maximaal twee."

Kies-moment:
"Eerste vraag — welk vraagstuk? Iets wat nu loopt op jouw lijn. Niet hypothetisch.
Als je bij blok 2 al een situatie hebt gevonden die nog steeds speelt — gebruik die."

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---

# Wat ga je nu doen?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het werkblad (10 min)
<v-clicks>

1. Eén zin: **wat is je vraagstuk?**
2. In welke DMAIC-**fase** zit je?
3. Welke SPC-tools **draaien al?**
4. Welke Six Sigma-tool is **het volgende stapje?**
5. Wie **trekt** de bredere verbetering?
6. SPC- of Six Sigma-vraagstuk?
7. **Maandag-actie — kritiek**
8. Voor de 2-weeks check-in

</v-clicks>

</div>

<div>

### Hulpvragen (wb-03 erbij)
<v-clicks>

- Heb je een baseline? → Measure
- Ken je de oorzaak? → Analyze
- Twijfel je aan de meting? → Gage R&amp;R
- Is dit bewaking of verbetering?
- Wat is de **kleinste** stap voor maandag?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min werkblad · 3 min plenair rondje · maandag-actie is de slot
</div>

<!--
SLIDE 8 — Werkblad-instructie. Zet timer op 10 min.

Wat je doet als trainer (kerntaak van dit blok):
- Loop rond, stel één coaching-vraag per bezoek.
- Bij "in welke fase?"-blokkade: "Heb je een baseline? Zo nee, je bent in Measure."
- Bij "welke tool?"-blokkade: verwijs naar wb-03-handout sectie 6.
- Bij "wie trekt?"-blokkade: "Welke collega heeft hier een rol in — ook als het niet jij bent?"
- Bij te brede scope: "Welke ene meetwaarde wil je over drie maanden vergeleken hebben?"

PLAN-B bij tijdsdruk (draaiboek gele box):
- Skip vraag 4-5 in sessie, maak die huiswerk voor 2-weeks check-in.
- SKIP NOOIT vraag 7 (maandag-actie) — dat is de transferslot.

Halverwege (5 min): "Halverwege. Check: heb je al iets bij vraag 7 — de maandag-actie?
Zo niet, spring nu naar vraag 7 en vul die eerst in."

Eindsignaal:
"Pen neer. Maandag-actie scherp? Vouw het werkblad bij je."

Verwijs naar draaiboek blok 3, volledige instructie.
-->

---
layout: center
class: text-center
---

# Maandag-actie — hardop

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Wat doe je <span class="font-bold">maandagochtend 9:00</span> — of deze week?
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-3xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag vraag ik de kwaliteitscoördinator of we visgraat doen op de drift van lijn 2."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag noteer ik de baseline-Cpk van afkeur — als uitgangspunt."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag stel ik mijn teamleider voor een Gage R&amp;R op de nieuwe meter."</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-80 max-w-xl mx-auto">
  Geen 'ik ga nadenken' — <span class="font-bold">één concrete actie</span>.<br/>
  <span class="text-sm opacity-70">Eén zin per persoon. Ik tel — 15-20 sec.</span>
</div>

<!--
SLIDE 9 — Transferopdracht + plenair rondje.

Plenair rondje (3 min) — strakke timing. Per persoon:
- Knik. "Begin."
- 15-20 sec per persoon.
- Geen vervolgvraag — geen reactie. Knik naar de volgende.

Bij twijfelaar: "Wie volgt vrijwillig?" — niet aanwijzen.
Bij te ambitieuze actie ("maandag start ik een Six Sigma-project"):
"Wat is de kleinste stap die daar nu voor nodig is? Een gesprek, een meting, één telefoontje?"

Trainer eindigt zelf met een één-woord-afsluiter of één zin over wat hem/haar opviel.

Modelleert de openheid.

VALKUIL: rondje wordt feedback-ronde of coachings-marathon.
"Dank je — vervolgvraag noteren we voor de 2-weeks check-in. We willen iedereen horen."

Verwijs naar draaiboek blok 3, instructie 6.
-->

---
layout: end
---

# Bedankt

<div class="mt-8 text-base opacity-70">
  Volgende blok in module 3: <span class="font-bold">DMAIC-skeleton voor eigen verbeterproject</span> (lo-spc-402)<br/>
  Daarna: <span class="font-bold">Six Sigma belt-rollen</span> (ko-spc-403)<br/>
  <span class="text-sm opacity-60">Maandag-actie scherp? Dan heeft dit uur gewerkt.</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · Six Sigma-positionering · v1.0
</div>

<!--
SLIDE 10 — Afsluiter.

"Goed werk. Neem je werkbladen mee — wb-01 is je gesprekspunt met je kwaliteitscoördinator deze week."

Notities voor jezelf na afloop:
- Foto's gemaakt van de werkbladen (met toestemming)?
- Welke deelnemers verwarden sigma-niveau met Cpk (follow-up in 2-weeks check-in)?
- Welke maandag-acties zijn opgeschreven (input voor opvolg-coaching)?
- Welke vragen op parkeerflip overgedragen aan trainer lo-spc-402 / ko-spc-403?
- Welke deelnemers hebben een Six Sigma-waardig vraagstuk (warm overdragen aan lo-spc-402)?

Verwijs naar draaiboek "Checklist na de sessie".
-->
