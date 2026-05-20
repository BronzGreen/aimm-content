---
theme: default
title: AI + SPC — samenspel op jouw eigen machine
info: |
  ## SPC Module 3 — Op Maat (synthese-blok)
  Synthese van SPC-fundamenten (Shewhart, Nelson) met AI-ervaring uit Module 1+2.
  Doelgroep: MBO-4 operator of teamleider, 45 minuten, coachende stijl.
  Volgt op lo-spc-402 (DMAIC-skeleton) als afsluitende synthese van Module 3.
  v1.0
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# AI + SPC

### Samenspel op jouw eigen machine

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Synthese-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  MBO-4 operator &amp; teamleider · drie lagen, drie tijdperken, jouw werkvloer
</div>

<!--
SLIDE 1 — Cover. Open warm en direct.

"Welkom in het laatste werkblok van Module 3. In Module 1 hebben jullie gezien wat AI kan.
In Module 2 hebben jullie zelf een model getraind op voorbeelddata.
Vandaag brengen we het samen — niet op voorbeeldfabriek, maar op jullie eigen lijn.

Ik ga jullie vandaag niks nieuws leren. Ik help jullie alleen om te zien waar de stukjes bij elkaar passen op jullie werkvloer."

Houd de toon coachend. De groep is bewust bekwaam — ze doen het denkwerk, jij stelt vragen.

Verwijs naar draaiboek blok 1, instructie 1.
-->

---
layout: center
class: text-center
---

# De centrale zin

<div class="mt-8 max-w-3xl mx-auto">
  <div class="text-2xl leading-relaxed font-light text-gray-800 italic">
    &ldquo;Shewhart bedacht in <span class="font-bold not-italic text-blue-700">1924</span> het onderscheid tussen signaal en ruis.
  </div>
  <div v-click class="text-2xl leading-relaxed font-light text-gray-800 italic mt-4">
    Dat onderscheid is in het <span class="font-bold not-italic text-purple-700">AI-tijdperk</span> belangrijker dan ooit —
  </div>
  <div v-click class="text-2xl leading-relaxed font-light text-gray-800 italic mt-4">
    juist omdat sensoren <span class="font-bold not-italic">miljoenen punten per dag</span> leveren.&rdquo;
  </div>
</div>

<div v-click class="mt-10 text-sm opacity-60">
  Onthoud deze zin. Hij is de kern van vandaag.
</div>

<!--
SLIDE 2 — Centrale zin. Lees voor, één keer, rustig.

"Shewhart bedacht in 1924 het onderscheid tussen signaal en ruis. Dat onderscheid is in het AI-tijdperk
belangrijker dan ooit — juist omdat sensoren miljoenen punten per dag leveren."

Stilte van 3 seconden. Geen uitleg.

"Onthoud deze zin. Hij is de kern van vandaag."

Zet de toon: we komen niks nieuws brengen — we brengen samen wat al bestaat.

Verwijs naar draaiboek blok 1, instructie 2.
-->

---

# Drie lagen, drie tijdperken

<div class="grid grid-cols-4 gap-2 mt-4 text-xs">
  <div></div>
  <div class="text-center font-bold py-2 rounded bg-gray-200 text-gray-700">Klassiek</div>
  <div class="text-center font-bold py-2 rounded bg-blue-200 text-blue-900">Digitaal</div>
  <div class="text-center font-bold py-2 rounded bg-purple-200 text-purple-900">AI-aanvulling</div>

  <div v-click class="text-right font-bold py-3 pr-2 text-sky-800">1. Meten</div>
  <div v-click class="p-2 bg-gray-50 rounded border border-gray-200">Handmeting elke 2 uur</div>
  <div v-click class="p-2 bg-blue-50 rounded border border-blue-200">IoT-sensor continu</div>
  <div v-click class="p-2 bg-purple-50 rounded border border-purple-200">Gaten vullen, meetfouten herkennen</div>

  <div v-click class="text-right font-bold py-3 pr-2 text-amber-800">2. Signaal</div>
  <div v-click class="p-2 bg-gray-50 rounded border border-gray-200">Operator scant kaart, Nelson-regels</div>
  <div v-click class="p-2 bg-blue-50 rounded border border-blue-200">Auto-alarm op Nelson-regels</div>
  <div v-click class="p-2 bg-purple-50 rounded border border-purple-200">Combinatie-patronen — multivariaat</div>

  <div v-click class="text-right font-bold py-3 pr-2 text-purple-800">3. Beslissen</div>
  <div v-click class="p-2 bg-gray-50 rounded border border-gray-200">Operator beslist</div>
  <div v-click class="p-2 bg-blue-50 rounded border border-blue-200">Operator beslist (alarm helpt)</div>
  <div v-click class="p-2 bg-purple-100 rounded border-2 border-purple-500 font-semibold">AI adviseert — mens beslist</div>
</div>

<div v-click class="mt-6 text-center text-sm opacity-70 max-w-2xl mx-auto">
  Shewhart-principe blijft — alleen de uitvoering verschuift.
  <span class="font-bold">De beslis-laag blijft altijd bij de mens.</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Diagram lo-spc-601 — drie-lagen-matrix
</div>

<!--
SLIDE 3 — Drie-lagen-matrix. Centrale didactische slide.

Wijs naar de A3-print achter in de zaal. Per rij één coachende vraag aan de groep:

1. LAAG METEN: "Wie meet handmatig, wie continu, wie heeft meet-assistentie?"
   Vang antwoorden. Bevestig: "Drie tijdperken staan naast elkaar in deze groep — dat is normaal."

2. LAAG SIGNAAL: "Wie scant zelf de kaart, wie heeft auto-alarmen, wie ziet al combinatie-signalen?"
   Bevestig: "Nelson blijft correct — ze zien één variabele tegelijk. Dat is het gat waar AI in stapt."

3. LAAG BESLISSEN: "Wie beslist er op jouw lijn als er een alarm afgaat?"
   Vang antwoorden. Bevestig: "In alle drie de tijdperken blijft de beslis-laag bij de mens.
   Dat is geen technische beperking — dat is een ontwerpkeuze." Wijs naar de paars-omrande cel rechtsonder.

Niet zelf de tools of voorbeelden opsommen. De cellen tonen het — de groep verwoordt het.
Stilte van 5 sec na elke vraag.

Verwijs naar draaiboek blok 1, instructie 4.
Verwijst naar trainee-SVG: diagram-lo-spc-601.svg.
-->

---
layout: two-cols-header
---

# Fictieve referentiecasus — chemische reactor

<div class="text-sm opacity-70 italic mb-4">
  Markeer elke keer: dit is fictief. Gebruik als ijkpunt voor schaal, niet als sjabloon.
</div>

::left::

### Klassiek / digitaal

<v-clicks>

- Druk, temperatuur, debiet — elk een eigen controlekaart
- Nelson-regels op elke variabele apart
- Auto-alarm bij overschrijding van een grens
- Elke variabele **op zich** binnen de tolerantie → geen alarm

</v-clicks>

::right::

### + AI-aanvulling

<v-clicks>

- Model getraind op historische batches
- Herkent **combinatie**: temp iets hoog + debiet iets laag + druk normaal
- Geeft waarschuwing **40 min eerder** dan Nelson zou piepen
- Operator beslist · Nelson blijft als tweede net

</v-clicks>

<!--
SLIDE 4 — Fictieve reactor-casus. Drie zinnen, niet meer.

"Eén voorbeeld ter illustratie — fictief, markeer dat.
Een chemische reactor meet druk, temperatuur en debiet. Nelson-regels op elke variabele apart werken prima.

Wat AI toevoegt: een model herkent dat temperatuur iets hoog + debiet iets laag + druk normaal vaak
voorafgaat aan een off-spec batch — 40 minuten eerder dan een Nelson-regel zou piepen.
Het model geeft vroege waarschuwing. De operator beslist. Nelson-regels blijven actief als tweede net."

Zeg: "Niet om over te nemen — als ijkpunt voor de schaal van waar AI waarde toevoegt."

BELANGRIJK: de reactor-casus is je ENIGE toegestane illustratie. Geen eigen voorbeelden uit 'mijn praktijk'.
De deelnemer vergelijkt zich met de reactor-casus, niet met de trainer.

Verwijs naar draaiboek blok 1, instructie 5.
-->

---
layout: section
---

# Experimenteren

## Jouw machine, jouw drie lagen

<div class="text-base mt-8 opacity-80 max-w-2xl mx-auto">
  Tot zover het kader. Nu de echte vraag:<br/>
  <span class="font-bold mt-4 block">hoe ziet dit eruit op jouw lijn? Vanaf nu jij.</span>
</div>

<!--
SLIDE 5 — Overgang naar blok 2.

"Tot zover het kader. Nu de echte vraag: hoe ziet dit eruit op jouw lijn? Vanaf nu jij."

Maak de pedagogische overgang expliciet: van "we lopen samen door" (blok 1)
naar "jij doet, ik vraag" (blok 2).

Deel wb-01-synthese-opdracht uit (A4):
"Drie lagen, zelfde volgorde als op de handout. Per laag: wat meet je / hoe detecteer je / wie beslist —
en zou AI hier iets toevoegen of niet? Eindig met één kans en één zorg."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Wat ga je nu doen?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het werkblad

<v-clicks>

1. Kies **één** machine of lijn
2. Per laag: klassiek / digitaal / AI?
3. Wat weet je niet? Markeer **"uitzoeken met..."**
4. Sluit af met **één kans** en **één zorg**

</v-clicks>

</div>

<div>

### Hulpvragen per laag

<v-clicks>

- **Meten** — elke seconde of elke shift?
- **Signaal** — wanneer zou je 30 min eerder willen weten?
- **Beslissen** — wat weet jij dat een model niet weet?
- **Kans/zorg** — welke afwijking miste Nelson deze week?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  16 min · individueel · A4-werkblad · pen
</div>

<!--
SLIDE 6 — Werkblad-instructie. Toon. Zet timer op 16 min.

Belangrijke instructie aan jezelf als trainer:
- Loop rond. Buig je niet over schouders.
- Bij stagnatie: één coaching-vraag per bezoek uit de tabel in het draaiboek. Niet meer.
- GEEF GEEN VOORBEELDEN. Vervang elke neiging tot voorbeeld door een vraag.
- Bij blokkade: drie-zinnen-aanpak — vraag → wacht 5 sec → bevestig wat hij al heeft → stilte → loop weg.

PLAN-B (zie draaiboek blok 2, gele box):
Bij 10 min visuele check. Als > 50 % nog vastzit in laag 1:
"Even bijschakelen. Maak laag 1 en 2 af in deze sessie. Laag 3 + kans/zorg neem je mee naar je team-overleg.
Liever scherp op 2 lagen dan dun op 3."

Halverwege (8 min): zachte tafelklap.
"Halverwege. Heb je álle drie de lagen aangeraakt? Als laag 3 nog leeg is, ga er nu naartoe."

Eindsignaal:
"Pen neer. Leg je werkblad waar je het zo kunt teruglezen voor de reflectie.
Het werkblad hoeft niet af — minimaal 2 lagen is genoeg."

Verwijs naar draaiboek blok 2, volledige instructie.
-->

---
layout: section
---

# Reflecteren

## STARRT op jouw werkvloer

<!--
SLIDE 7 — Overgang naar blok 3 (reflectie + plenair rondje).

Deel wb-02-reflectie uit:
"STARRT — zes stappen. Niet lang — kort en eerlijk. Situatie, Taak, Actie, Resultaat, Reflectie, Transfer.
De kern zit in de twee R's. Daar vraag je jezelf: wat heb ik geleerd over mijn eigen werkvloer,
en wat ga ik daar maandag mee doen?"

Eerst 7 min individueel schrijven. Dan plenair rondje: één zin per persoon.

"Helemaal onderaan wb-02 één zin: je belangrijkste inzicht. Die deel je straks hardop."

Trainer tijdens schrijven: loop rond, kijk op afstand, grijp niet in. Reflectie is solitair werk.

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---
layout: center
class: text-center
---

# Eén zin — de hele groep

<div class="mt-8 max-w-3xl mx-auto">
  <div class="text-xl opacity-80">
    Onderaan wb-02 schreef je één zin.<br/>
    <span class="font-bold">Jouw belangrijkste inzicht over SPC + AI op jouw werkvloer.</span>
  </div>

  <div v-click class="mt-10 p-6 bg-slate-50 rounded-xl">
    <div class="text-sm uppercase tracking-wide text-slate-500 mb-3">Zo doen we het</div>
    <div class="text-base text-slate-700 space-y-2">
      <div>🗣 Eén zin per persoon · ca. 45 sec</div>
      <div>✍ Trainer schrijft kernwoord op flipover</div>
      <div>🤫 Geen vervolgvragen · alleen luisteren en vangen</div>
    </div>
  </div>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · plenair · flipover met kernwoorden
</div>

<!--
SLIDE 8 — Plenair één-zin-rondje.

"Laatste deel. Iedereen zegt één zin — niet meer. Die ene zin onder aan je wb-02.
Ik schrijf de kernwoorden op de flipover. Geen vervolgvraag, geen reactie van de groep.
Alleen luisteren en vangen."

Per persoon:
- Knik. "Begin."
- Luister. Vang kernwoord of kernzin. Schrijf op flipover.
- Bij ~45 sec: "Dank je." Geen vervolgvraag.
- Knik volgende. "Jij."
- Bij twijfelaar: "Wie volgt vrijwillig?" — niet aanwijzen.
- Sluit af met jouw eigen zin. Modelleert gelijkheid en openheid.

VALKUIL: rondje wordt discussie. Beheers tijd hard.
"Interessant — dat pakken we op in het team-overleg. Nu willen we iedereen horen."

Verwijs naar draaiboek blok 3, instructie 3-4.
-->

---
layout: end
---

# Dit was jullie synthese

<div class="mt-8 text-base opacity-70 max-w-2xl mx-auto">
  Neem je <span class="font-bold">wb-01</span> en <span class="font-bold">wb-02</span> mee — die zijn je werkdocument.<br/>
  <span class="text-sm mt-2 block">Binnen twee weken: bespreken met leidinggevende · kans + zorg agenderen in team-overleg.</span>
</div>

<div v-click class="mt-10 text-sm opacity-80 italic max-w-xl mx-auto">
  &ldquo;Shewhart bedacht in 1924 het onderscheid tussen signaal en ruis.<br/>
  Dat onderscheid is in het AI-tijdperk belangrijker dan ooit.&rdquo;
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · lo-spc-601 · v1.0
</div>

<!--
SLIDE 9 (end) — Afsluiter + transfer-herinnering.

Wijs naar de flipover met kernwoorden uit het rondje:
"Dit is wat jullie vandaag hebben gevonden. Niet uit een boek — van jullie eigen lijn."

"Eén ding nog: op wb-02 staat een transferopdracht. Binnen twee weken: bespreek je synthese met je
leidinggevende of kwaliteitscoördinator. Vraag na welke AI-toepassing op jouw lijn gepland staat.
Agendeer één kans en één zorg in je team-overleg. Neem je werkbladen mee — dat zijn je werkdocumenten."

Onthul de centrale zin nog één keer met v-click — sluit de cirkel van slide 2.

Notities voor jezelf na afloop:
- Foto's gemaakt van alle werkbladen?
- Kernwoorden-flipover gefotografeerd (input voor volgende sessie)?
- Welke deelnemers zitten op AI-lijnen, welke nog volledig klassiek?
- Parkeerflip-vragen overgedragen aan module-eigenaar?
- xAPI-statements verstuurd: experienced + completed + attempted (transfer).

Verwijs naar draaiboek "Checklist na de sessie".
-->
