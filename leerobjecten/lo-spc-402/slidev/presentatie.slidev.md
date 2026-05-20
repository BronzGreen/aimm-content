---
theme: default
title: DMAIC — vijf-stappen verbeterroute
info: |
  ## SPC Module 3 — Op Maat
  Workshop-blok over DMAIC-skeleton voor eigen verbeterproject.
  Doelgroep: teamleiders HBO + MBO-4, 60 minuten, coachende stijl.
  v1.1 — minder slides voor blok 1 (max 5), meer ruimte voor canvas-werk
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# DMAIC

### Vijf-stappen verbeterroute voor bestaande processen

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Workshop-blok · 60 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Teamleiders HBO + MBO-4 · DMAIC-skeleton voor eigen project
</div>

<!--
SLIDE 1 — Cover. Open warm en direct.

"Welkom in module 3 — Op Maat. De afgelopen twee modules werkten jullie op voorbeelddata.
Vanaf nu werken we aan jullie eigen projecten, op jullie eigen lijn.

We beginnen met een denkkader op tafel te leggen — niet om jullie iets nieuws te leren,
maar om wat jullie al weten gestructureerd in te zetten. Ik ga jullie weinig vertellen vandaag — meestal vraag ik."

Houd de toon coachend, niet doceren. HBO-teamleiders kennen het denken al — laat ze dat voelen.

Verwijs naar draaiboek blok 1, instructie 1.
-->

---
layout: center
class: text-center
---

# Waarom DMAIC?

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-80">
  Zonder structuur vervalt verbetering in:
</div>

<div class="grid grid-cols-3 gap-4 mt-8 max-w-3xl mx-auto">
  <div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Snelle aannames</div>
    <div class="text-xs mt-2 opacity-70">"Het zal wel de operator zijn"</div>
  </div>
  <div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Symptoombestrijding</div>
    <div class="text-xs mt-2 opacity-70">Oplossen zonder oorzaak</div>
  </div>
  <div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Geen blijvend resultaat</div>
    <div class="text-xs mt-2 opacity-70">"We hadden het opgelost…"</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-80 max-w-xl mx-auto">
  DMAIC dwingt: <span class="font-bold">eerst meten, dan analyseren, dan veranderen, dan borgen.</span>
</div>

<!--
SLIDE 2 — Trigger-slide. Coachende vraag eerst, dan pas de drie patronen.

Stel coachende vraag aan de groep:
"Wat zijn de drie meest voorkomende manieren waarop verbeterprojecten op jullie werkvloer mislukken?"

Wacht. Tel innerlijk tot 7. Vang 2-3 antwoorden.

Dan pas de drie blokjes onthullen met v-click — bevestig wat je hoorde:
"Wat ik hoor: aannames in plaats van data, oplossingen in plaats van diagnoses, en winst die niet beklijft."

Niet meer. Geen lange uitleg.

Daarna: deel wb-01-handout-dmaic uit:
"Pak je markeerstift. Markeer wat je herkent uit projecten die wél werkten,
en wat je herkent uit projecten die niet werkten. Twee minuten — kort."

Zet timer op 2 min. Loop rustig rond, lees mee, stel geen vragen.

Verwijs naar draaiboek blok 1, instructie 2-3.
-->

---

# De DMAIC-cyclus

<div class="grid grid-cols-5 gap-3 mt-8">
  <div v-click class="text-center p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-3xl mb-2">🎯</div>
    <div class="font-bold text-blue-800">Define</div>
    <div class="text-xs opacity-70 mt-1">Wat is het probleem?</div>
  </div>
  <div v-click class="text-center p-4 bg-cyan-50 rounded-xl border-2 border-cyan-200">
    <div class="text-3xl mb-2">📊</div>
    <div class="font-bold text-cyan-800">Measure</div>
    <div class="text-xs opacity-70 mt-1">Wat is de baseline?</div>
  </div>
  <div v-click class="text-center p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-3xl mb-2">🔍</div>
    <div class="font-bold text-amber-800">Analyze</div>
    <div class="text-xs opacity-70 mt-1">Waardoor ontstaat het?</div>
  </div>
  <div v-click class="text-center p-4 bg-orange-50 rounded-xl border-2 border-orange-200">
    <div class="text-3xl mb-2">🛠️</div>
    <div class="font-bold text-orange-800">Improve</div>
    <div class="text-xs opacity-70 mt-1">Welke verandering?</div>
  </div>
  <div v-click class="text-center p-4 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-3xl mb-2">🔒</div>
    <div class="font-bold text-green-800">Control</div>
    <div class="text-xs opacity-70 mt-1">Hoe borgen we de winst?</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-sm opacity-70 max-w-xl mx-auto">
  Pijl van Control terug naar Define is geen versiersel — nieuwe afwijking = nieuw Define.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Diagram lo-spc-402 — DMAIC-cyclus
</div>

<!--
SLIDE 3 — De DMAIC-cyclus. Centrale didactische slide voor blok 1.

Wijs naar de A3-print achter in de zaal. Toon dit overzicht.

Werkvorm: per fase niet zelf vertellen — vraag de groep.
Per fase ~90 sec:

1. Onthul de fase met v-click.
2. Vraag: "Wat is hier de centrale vraag — wie kan het in eigen woorden zeggen?"
   Wacht 5-7 sec. Vang één antwoord. Bevestig of scherp aan met één zin.
3. Vraag: "Welke valkuil zien jullie hier het vaakst?"
   Vang één antwoord. Bevestig met de valkuil uit de handout.
4. Bij Define: het spuitgiet-anchor in 3 zinnen — "afkeur 1,2 % naar < 0,3 %, in 3 mnd, €40k.
   Dat is de schaal. Niet om over te nemen — om als ijkpunt te gebruiken."

Niet zelf de tools opsommen — die staan in de handout.
"Welke tool zou je hier eerst pakken?" en bevestig wat past.

Bij tijdsdruk: koppel D+M samen, dan A+I+C.

Tempo: max 8 min totaal voor alle 5 fases. Stilte van 5-7 sec na elke fase (consistent met draaiboek + coaching-spiekbriefje).

Verwijs naar draaiboek blok 1, instructie 4.
Verwijst naar trainee-SVG: diagram-lo-spc-402.svg.
-->

---
layout: section
---

# Experimenteren

## DMAIC-canvas voor jouw lijn

<div class="text-base mt-8 opacity-80 max-w-2xl mx-auto">
  Tot zover de structuur. De rolverdeling tussen operator en teamleider staat in de handout — terug te lezen na de pauze.<br/>
  <span class="font-bold mt-4 block">Nu de echte vraag: jouw eigen project. Vanaf nu jij.</span>
</div>

<!--
SLIDE 4 — Overgang naar blok 2 (experimenteren).

"Tot zover de structuur. De rolverdeling tussen operator en teamleider — wie wat doet —
staat in de handout, terug te lezen na de pauze.
Nu de echte vraag: jullie eigen project. Vanaf nu jij."

Maak de pedagogische overgang expliciet: van "we lopen samen door" (blok 1, geleide coaching) naar
"jij doet, ik vraag" (blok 2, individueel coaching). Dat sluit naadloos aan op de toon van blok 1
en breekt de pedagogische lijn niet.

Deel wb-02-dmaic-canvas uit (A3, vijf kolommen).

"Vijf kolommen, één per fase. Per fase staat de centrale vraag al voorgedrukt.
Jouw werk: vul de fase met jouw project. Niet abstract — concreet.
Welke meetwaarde, welke operator, welke tool, welke datum."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Wat ga je nu doen?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het canvas
<v-clicks>

1. Schrijf bovenaan: **"Mijn project is..."**
2. Werk **top-down**: D → M → A → I → C
3. Per fase **één regel** is het minimum
4. **Concreet**: meetwaarde, operator, datum

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Welke afwijking ergerde je deze week?
- Welke operator zou hierin meewerken?
- Welke meting doe je nu al?
- Hoe toon je over 3 maanden de winst?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  12 min · individueel · A3-canvas · post-its in 5 kleuren
</div>

<!--
SLIDE 5 — Canvas-instructie. Toon de instructie. Zet timer op 12 min.

Belangrijke instructie aan jezelf als trainer:
- Pak het coaching-spiekbriefje (apart blad) erbij — leg het naast je laptop.
- Loop rond, buig je niet over schouders.
- Bij stagnatie: stel ÉÉN coaching-vraag uit het spiekbriefje per fase. Niet meer.
- GEEF GEEN VOORBEELDEN. Vervang elke neiging tot voorbeeld door een vraag.
- Bij blokkade: drie-zinnen-aanpak — vraag → wacht 5 sec → bevestig wat hij al heeft → stilte.

PLAN-B (zie draaiboek blok 2, gele box):
Bij 6 min visuele check. Als > 50 % nog bij D+M hangt:
"Even bijschakelen. Maak D en M af in deze sessie. A, I, C krijg je als huiswerk
vóór blok 3 — peer-review werkt dan op D+M en op de schets van AIC die je thuis maakt."

Halverwege (6 min): zachte tafelklap.
"Halverwege. Heb je álle vijf fases aangeraakt? Als Control nog leeg is, ga er nu naartoe.
Zonder Control valt elke verbetering in." (overslaan bij plan-B)

Eindsignaal:
"Pen neer. Leg je canvas waar je collega het zo kan lezen. Het hoeft niet af —
op alle vijf fases één regel is genoeg. (of: D+M scherp + AIC-schets, bij plan-B)"

Verwijs naar draaiboek blok 2, volledige instructie.
-->

---
layout: section
---

# Reflecteren

## Peer-review met je collega

<!--
SLIDE 6 — Overgang naar blok 3 (peer-review).

Deel wb-03-peer-review uit:
"Dit werkblad helpt je om coach te zijn — niet om beoordelaar te zijn.
Op het werkblad staan per fase 2-3 coaching-vragen die je kunt stellen.
Gebruik ze, of bedenk je eigen — zolang het maar vragen zijn, geen oplossingen."

Vorm duo's: bij voorkeur iemand uit andere context (ander bedrijf, andere lijn).
Andere context = scherpere vragen.

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---

# Peer-review — vragen, geen oplossingen

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-5 bg-purple-50 rounded-xl">

### 👤 Auteur
<v-clicks>

- Lees hardop één fase voor
- Begin bij de **dunste** fase
- Schrijf de meest rakende vraag in de marge
- Maximaal **3 fases in 6 min**

</v-clicks>

</div>

<div class="p-5 bg-amber-50 rounded-xl">

### 🤝 Coach
<v-clicks>

- Stel **minstens 2 vragen** per fase
- Gebruik het werkblad als spiek
- **Geen oplossingen** — alleen vragen
- Bevestig wat sterk is

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base p-4 bg-blue-50 text-blue-900 rounded-lg max-w-xl mx-auto">
  Na 6 min: <span class="font-bold">wisselen</span>. <br/>
  <span class="text-sm opacity-80">Slotvraag samen: "Wat heb ik vandaag van jouw canvas geleerd?"</span>
</div>

<!--
SLIDE 7 — Peer-review-instructie.

Eerste ronde — 6 min. Zet timer.
"A is auteur, B is coach. Auteur leest hardop één fase voor — bij voorkeur de fase die nog het minst stevig is.
Coach stelt minstens twee vragen uit het werkblad. Auteur schrijft de meest rakende vraag in de marge.
Maximaal 3 fases in 6 minuten."

Wisseling met bel/gong. B is auteur, A is coach. Zelfde aanpak.

Wat je doet als trainer:
- Loop tussen duo's, luister mee.
- GRIJP NIET IN. Bij stilte: lees één regel hardop voor van het canvas, vraag de luisteraar:
  "Wat is de coaching-vraag die hier op zijn plaats is?" Modelleer geen vraag — vraag erom.
- Bij oplossings-gedrag: zachtjes "Vraag, geen oplossing — wat zou je willen weten?"

Slot-1-min: laatste vraag in elk duo:
"Wat heb ik vandaag van jouw canvas geleerd dat ik in mijn eigen denken ga gebruiken?" Twee zinnen elk.

Verwijs naar draaiboek blok 3, volledige instructie.
-->

---
layout: section
---

# Ervaren

## Plenaire deel-ronde — 1 minuut per persoon

<!--
SLIDE 8 — Overgang naar blok 4 (deel-ronde + transfer).

Deel wb-04-deelronde-format uit (1 pagina A4):
"Eén minuut per persoon. Drie zinnen — niet meer.
Eerste zin: 'Mijn project is...'
Tweede zin: 'De fase die ik het stevigst heb staan is X, omdat...'
Derde zin: 'De fase waar ik het minste vertrouwen in heb is Y, omdat...'
Geen vragen aan elkaar — die noteren we voor de volgende sessie. Ik tel hard."

Verwijs naar draaiboek blok 4, instructie 1.
-->

---
layout: center
class: text-center
---

# Drie zinnen — exact

<div class="space-y-4 mt-8 max-w-2xl mx-auto text-left">

<div v-click class="p-4 bg-blue-50 rounded-lg flex gap-4 items-start">
  <div class="text-2xl">1️⃣</div>
  <div>
    <div class="font-bold text-blue-900">Mijn project is...</div>
    <div class="text-sm opacity-70 mt-1">Eén zin. Concrete meetwaarde + lijn.</div>
  </div>
</div>

<div v-click class="p-4 bg-green-50 rounded-lg flex gap-4 items-start">
  <div class="text-2xl">2️⃣</div>
  <div>
    <div class="font-bold text-green-900">Stevigste fase is X, omdat...</div>
    <div class="text-sm opacity-70 mt-1">Waar je vertrouwen voelt.</div>
  </div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-lg flex gap-4 items-start">
  <div class="text-2xl">3️⃣</div>
  <div>
    <div class="font-bold text-amber-900">Minste vertrouwen in fase Y, omdat...</div>
    <div class="text-sm opacity-70 mt-1">Waar de werkelijke leervraag zit.</div>
  </div>
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  60 sec per persoon · timer hard · geen vervolgvragen
</div>

<!--
SLIDE 9 — Drie zinnen format. Strakke timing.
De waarde zit in exposure + commitment, niet in feedback.

Per persoon:
- Knik. "Begin."
- Bij 60 sec: zacht handgebaar of gong. "Dank je."
- Geen vervolgvraag, geen reactie. Knik naar de volgende. "Begin."

Bij twijfelaar: "Wie volgt vrijwillig?" — niet aanwijzen.

VALKUIL: deel-ronde wordt feedback-ronde of coachings-marathon.
"Dank je — vervolgvraag noteren we voor de volgende sessie. We willen iedereen horen."

Voor ervaren green-belt-achtig: vraag deze deelnemer als laatste — zet de norm hoog.
Voor onzeker / nieuw: bevestig vooraf dat de derde zin (minste vertrouwen) juist de waardevolle is.

Verwijs naar draaiboek blok 4, instructie 2-3.
-->

---
layout: center
class: text-center
---

# Transferopdracht — maandag 9:00

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Wat doe je <span class="font-bold">maandagochtend</span> als eerste?
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-3xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag bel ik de kwaliteitsdienst voor de baseline-data van lijn 3."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag vraag ik mijn operator naar zijn drie ergste afwijkingen."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag schrijf ik mijn charter af in 30 min en stuur ik het ter reactie."</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-80 max-w-xl mx-auto">
  Niet 'ik ga nadenken' — <span class="font-bold">één concrete actie</span>.<br/>
  <span class="text-sm opacity-70">Schrijf onderaan je deelronde-format (wb-04). Foto maken voor jezelf.</span>
</div>

<!--
SLIDE 10 — Transferopdracht.

"Tot zover de skeleton. Nu de echte vraag: wat doe je maandagochtend om 9:00 als eerste?
Niet over een week — maandag. Niet 'ik ga nadenken' — maandag concreet.
Een actie waar je vandaag al ja op zegt."

Twee minuten schrijftijd:
"Schrijf je maandag-actie onderaan wb-04 — duidelijk, één zin. Foto maken voor jezelf is goed."

Bij blokkade ('ik weet het nog niet'):
"Wat is de kleinste stap die je morgen nog kunt zetten? Niet de mooiste — de kleinste."

Afsluitings-rondje (3 min):
"Laatste rondje. Eén woord per persoon: wat neem je mee uit dit uur?"
Loop het rondje af. Eindig zelf — ook één woord.

Verwijs naar draaiboek blok 4, instructie 4-6.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende blok in module 3: <span class="font-bold">Six Sigma belt-rollen</span> (ko-spc-403)<br/>
  <span class="text-sm opacity-60">Wie heb je nodig in je team — en wanneer roep je een green of black belt erbij?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · DMAIC · v1.1
</div>

<!--
SLIDE 11 — Afsluiter. Bedank de groep. Kondig het volgende blok aan (Six Sigma belt-rollen, ko-spc-403).

"Goed werk vandaag. Pak je canvas mee — dat is je werkdocument voor de komende drie maanden."

Notities voor jezelf na afloop:
- Foto's gemaakt van alle canvasvellen?
- Welke fases waren bij velen 'minste vertrouwen' (input voor follow-up)?
- Welke maandag-acties zijn opgeschreven (input voor opvolg-coaching)?
- Welke vragen op parkeerflip overgedragen aan trainer ko-spc-403?
- Bij ervaren green-belt-achtige deelnemers: warm overdragen naar belt-rollen-blok.

Verwijs naar draaiboek "Checklist na de sessie".
-->
