---
theme: default
title: Wat is een neuraal netwerk — patroonherkenning in lagen
info: |
  ## AI Fundamentals — Module 1 (Gebruik)
  Workshop-blok over neurale netwerken voor camera-inspectie en sensorsystemen.
  Doelgroep: operators/teamleiders MBO-4, 45 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Wat is een neuraal netwerk?

### Patroonherkenning in lagen — voor camera-inspectie

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 1 (Gebruik) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · camera-inspectie · sensorsystemen
</div>

<!--
Welkom.

"Op steeds meer werkplekken hangt een camera die zelf goedkeurt of afkeurt. Voor velen voelt dat als magie of een black box. Het is geen van beide — het is wiskunde. De komende 45 minuten zie je hoe dat op hoofdlijnen werkt."

Dit LO bouwt op lo-ai-fund-101 (wat is AI). Daar leerde je de twee kenmerken — leren van voorbeelden + zelf beslissen. Hier zien we het MECHANISME van kenmerk 1: hoe leert zo'n systeem eigenlijk?
-->

---
layout: center
class: text-center
---

# Een camera op de lopende band

<div class="text-xl mt-8 max-w-2xl mx-auto leading-relaxed opacity-80">
  Hij wijst aan: deze beugel heeft een kras.<br/>
  Die niet.
</div>

<div v-click class="mt-10 text-2xl font-bold text-blue-700">
  Hoe denk je dat hij dat doet?
</div>

<div v-click class="mt-6 text-base opacity-60 italic">
  Hoe ziet hij het verschil tussen goed en kras?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  2 min · individueel · geel briefje · twijfel mag
</div>

<!--
Toon foto of korte video van inspectiecamera boven lopende band met metalen beugels (sommige met kras van 2mm).

Deel gele briefjes uit.
"Schrijf één zin op het gele briefje: 'volgens mij ziet de camera het zo: ...'
Geen goede of foute antwoorden — je antwoord is een startpunt, geen toets."

IK DOE-voorbeeld hardop (30-45 sec):
"Ik kijk naar deze foto en denk: zou de camera de hele foto in één keer beoordelen?
Of zou hij eerst naar lijnen kijken, daarna naar vormen?
Ik weet het eigenlijk niet zeker — laat ik dat opschrijven."

Schrijf zelf demonstratief op een briefje. Daarna 2 min individueel.
Loop rond. Verzamel briefjes na 2-3 min.

Lees 3-4 voor zonder commentaar. Knik en zeg "mooi, ik hoor je".
-->

---
layout: center
class: text-center
---

# Buurman-check

<div class="text-xl mt-10 max-w-2xl mx-auto leading-relaxed">
  Vergelijk jullie briefjes.
</div>

<div v-click class="mt-6 text-base opacity-70">
  Wat heb je opgeschreven? Wat heeft je buurman opgeschreven?
</div>

<div v-click class="mt-8 text-sm opacity-60 italic">
  Op het werkblad: het meest verrassende voor mij was ...
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · duo · wb-01
</div>

<!--
Deel wb-01 uit.

"Tweetal met je buurman. Vergelijk jullie briefjes. Wat heb je opgeschreven? Wat heeft je buurman opgeschreven? Op het reflectiewerkblad schrijf je één zin: 'het meest verrassende voor mij was ...'"

Zet timer op 5 min. Loop rond, vang vastlopers binnen 2 min.
Bij stilte: "Wie begint? Lees voor wat je hebt opgeschreven."

Niet rondlopen-corrigeren — alleen luisteren en helpen.
-->

---

# In één keer of in stapjes?

<div class="grid grid-cols-2 gap-8 mt-10">

<div class="p-6 bg-purple-50 rounded-lg border-2 border-purple-200">

### Stem 1

<div class="mt-4 text-xl font-bold text-purple-700">
  In één keer
</div>

<div class="mt-3 text-sm opacity-70">
  De camera beoordeelt het hele beeld direct.
</div>

</div>

<div class="p-6 bg-blue-50 rounded-lg border-2 border-blue-200">

### Stem 2

<div class="mt-4 text-xl font-bold text-blue-700">
  In stapjes
</div>

<div class="mt-3 text-sm opacity-70">
  Eerst lijnen → daarna vormen → daarna patronen.
</div>

</div>

</div>

<div v-click class="mt-10 text-center text-base font-bold opacity-80">
  Wat dachten jullie?
</div>

<!--
Plenair stemmen met handen omhoog.
"Wie dacht dat de camera in één keer naar het hele beeld kijkt? Steek je hand op." Tel hardop.
"Wie dacht in stapjes — eerst lijnen, dan vormen?" Tel hardop.

Flipover-verzameling (2 min):
"Bijna iedereen denkt aan 'in stapjes'. Welke stapjes zou de camera dan kunnen maken? Wat als eerste?"
Verzamel op flipover: 'lijnen', 'vormen', 'kleuren', 'krassen' — letterlijk wat de groep zegt.

Brug: "Bijna iedereen denkt aan in stapjes kijken — en dat klopt. Dat is precies wat een neuraal netwerk doet. Nu zien we hoe dat eruitziet."

NIET 'in één keer' bestempelen als fout — het is ook een logische gedachte.
-->

---
layout: section
---

# Theoretiseren

## Drie blokken — input, lagen, output

<!--
Brug naar blok 3.

Deel wb-02 uit. Wijs het A3-diagram aan.
"Pak je markeerstift. Wat we straks gaan zien heeft een naam: een neuraal netwerk. Drie blokken op het diagram."
-->

---

# Een neuraal netwerk in drie blokken

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### Input

- Wat erin gaat
- Een foto, meting of geluid
- Omgezet in pixels of getallen

<div class="mt-3 text-xs opacity-60 italic">
  Voorbeeld: foto van metalen beugel
</div>

</div>

<div class="p-4 bg-amber-50 rounded-lg border-2 border-amber-200">

### Lagen

- Hier zit het rekenwerk
- Kleine eenheden: **neuronen**
- Eerste laag: lijnen, randen
- Volgende laag: vormen
- Laatste lagen: complete patronen

<div class="mt-3 text-xs opacity-60 italic">
  In stapjes — zoals jullie zeiden
</div>

</div>

<div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">

### Output

- Het antwoord
- Goed of kras op positie 3
- Geen tussenvragen

<div class="mt-3 text-xs opacity-60 italic">
  Voorbeeld: 'kras op beugel 47'
</div>

</div>

</div>

<div v-click class="mt-8 text-center text-base font-bold text-blue-700">
  Drie woorden om te onthouden: input → lagen → output.
</div>

<!--
Loop drie blokken door — wijs telkens aan op het A3-diagram.

INPUT (2 min):
"Dit is wat erin gaat — een foto van de metalen beugel op de lopende band. De camera maakt een foto en die wordt omgezet in pixels — getallen die het netwerk begrijpt."

LAGEN (4 min):
"Dit zijn de tussenlagen — hier zit het rekenwerk. Veel kleine eenheden — neuronen — kijken elk naar een stukje. EERSTE laag herkent lijnen en randen. VOLGENDE laag herkent vormen — een rond, een hoek. LAATSTE lagen herkennen complete patronen — een kras, een deuk, een ontbrekende schroef. Daarom dachten jullie net al aan 'in stapjes' — dat is precies wat hier gebeurt."

OUTPUT (2 min):
"Het antwoord komt eraan — goed of kras op positie 3. Geen tussenvragen."

Verbind expliciet terug: "Jullie 'lijnen' en 'vormen' zijn precies wat de eerste lagen herkennen. Jullie hadden gelijk."

NIET activatiefuncties, backpropagation, gewichten-wiskunde uitleggen.
-->

---

# Twee misverstanden

<div class="grid grid-cols-2 gap-6 mt-10">

<div class="p-5 bg-red-50 rounded-lg border-2 border-red-200">

### Het is geen magie

- Mensen hebben het gebouwd
- Getraind en getest
- Elk antwoord komt uit rekenwerk
- Niet stap-voor-stap zoals Excel — maar wel wiskunde

</div>

<div class="p-5 bg-red-50 rounded-lg border-2 border-red-200">

### Het werkt niet zoals een brein

- Naam komt van hersencellen
- Vergelijking is INSPIRATIE, geen werkelijkheid
- Geen begrip, geen bewustzijn
- Alleen patroonherkenning

</div>

</div>

<div v-click class="mt-10 text-center text-lg font-bold text-blue-700">
  Wiskunde met laagsgewijze patroonherkenning.
</div>

<!--
Houd kort en bondig.

EÉN: "Het is geen magie. Iemand heeft het gebouwd, getraind en getest. Elk antwoord komt uit rekenwerk."

TWEE: "Het werkt niet precies zoals een brein. De naam komt van hersencellen — neuronen — maar de overeenkomst is oppervlakkig. Het is een rekenmodel, geen biologie."

Bij "dus de camera DENKT?" — bevestig de naam, maar verschil scherp: rekenmodel, geen biologie, geen begrip, geen humor.
-->

---

# Een concreet voorbeeld

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### De fabriek
- Kunststof brandstoftanks
- Cameracontrole bij eindcontrole

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### De data
- **1.300** synthetische foto's
- **295** echte foto's
- Goed én fout

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Het resultaat
- **70%** nauwkeurigheid
- Real-time tijdens productie

</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-80 italic">
  70 van 100 defecten vangt de camera meteen.<br/>
  De rest blijft mensenwerk.<br/>
  Het model neemt niet over — het helpt.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Bron: Soldatos (2024), Artificial Intelligence in Manufacturing, Ch. 17-18
</div>

<!--
Citeer de cijfers letterlijk — niet zelf inschatten of afronden.

"Een producent van kunststof brandstoftanks gebruikte zo'n model voor inspectie. Het model leerde van 1.300 synthetische foto's en 295 echte foto's. Daarna herkende het 70% van de defecten correct, in real-time. Bron: Soldatos 2024."

"70% klinkt niet zo hoog — maar het betekent: de camera vangt 70 van de 100 defecten meteen. De rest blijft mensenwerk. Het model neemt niet over — het helpt."

Bevestig dat 70% genoeg is om waarde toe te voegen.
NIET: 'AI vervangt jouw werk' — dat is hier feitelijk onjuist.

Brug: "Drie blokken — input, lagen, output. Hetzelfde patroon zit overal waar een camera of sensor meekijkt. Nu jouw lijn: waar staat dit ding bij jullie?"
-->

---
layout: center
class: text-center
---

# Wil je het zien gebeuren?

<div class="text-xl mt-10 max-w-xl mx-auto opacity-80">
  90 seconden video
</div>

<div v-click class="mt-8 text-lg opacity-70">
  Van tandwiel naar lijnen naar vormen naar 'kras' of 'goed'.<br/>
  En een heat-map die laat zien WAAR het netwerk kijkt.
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion · <code>NeuraalNetwerkVideo</code>)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
Optionele inzet — alleen als je in tempo zit (fase 3 in 13 min i.p.v. 15).
Toon de 90s video na de drie blokken en vóór de twee misconcepties.
-->

---
layout: section
---

# Experimenteren

## Vier vragen over jouw eigen lijn

<!--
Brug naar blok 4.

"Drie blokken — input, lagen, output. Hetzelfde patroon zit overal waar een camera of sensor meekijkt. Nu jouw lijn: waar staat dit ding bij jullie?"
-->

---

# Vier vragen

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Voor jouw eigen lijn
<v-clicks>

- Waar werkt een camera of sensor mee — of zou dat kunnen?
- Wat is de **input** (foto, meting, geluid)?
- Wat is de **output** (goed/fout, klasse, getal)?
- Hoeveel **voorbeelden** zijn er — 100 of 1.000?

</v-clicks>

</div>

<div>

### Vangnet
<v-clicks>

- Antwoordmodel staat achterop het werkblad
- 'Weet ik niet zeker' is een geldig antwoord
- Dat is precies de eerste IT-vraag
- Geen camera op je lijn? Vraag een collega-lijn

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-03 <span class="opacity-60">of tablet · model-lagen-verkennen</span>
</div>

<!--
Deel wb-03 uit.

"Vier vragen over jouw eigen lijn.
(1) Op welke lijn of plek bij jou werkt een camera of sensor mee — of zou dat kunnen?
(2) Wat is daar de input — een foto, een meting, een geluid?
(3) Wat is daar de output — een goed/fout antwoord, een klasse, een getal?
(4) Heeft jouw bedrijf voorbeelden om mee te trainen — denk je 100 of 1.000?

Antwoordmodel staat achterop — kijk daar pas in als je echt vastloopt."

"'Weet ik niet zeker' is een geldig antwoord. Dat is precies de vraag voor IT."

Zet timer op 6 min. Loop rond na 2 min.
Doorvragen: "Welke camera bedoel je? Boven welke band?" "Wie weet hoe vaak er een foto wordt opgeslagen?"

Bij vastlopers: bied antwoordmodel aan of geef lijn-suggestie (spuitgieten, lasrobot, eindcontrole).
Bevestig 'ik weet het niet zeker' uitdrukkelijk — waardevolle eerste vraag.
-->

---

# Drie deelnemers

<div class="mt-12 text-center text-xl">
  Eén zin op vraag 1:
</div>

<div class="mt-4 text-center text-lg opacity-70 italic">
  Waar staat jouw camera of sensor?
</div>

<!--
"Drie deelnemers — kort, één zin op vraag 1: waar staat jouw camera of sensor?"
Vang precies 3 voorbeelden. NIET bespreken.

Maximum 3 — geen 5. Anders mist de transferopdracht zijn doel.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Drie dingen noteren
<v-clicks>

- Waar hangt de camera precies (boven welke band, bij welke machine)?
- Wat is de output (goed/fout, klasse, getal)?
- Waar komen de trainingsfoto's vandaan — wie maakt of beoordeelt die?

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Geen camera op je lijn? Vraag een collega-lijn.
- Praat één keer met een kwaliteitscollega:<br/><kbd>"Wie bepaalt eigenlijk wat de camera ziet als goed of fout?"</kbd>
- Die keuze is ooit gemaakt — vaak niet door iemand die nu nog op de lijn werkt.
- Waardevol voor elk AI-traject.

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Notities mee naar de volgende sessie.
</div>

<!--
Sluit af met de transferopdracht.

"Deze week loop je één keer langs de inspectiecamera of het sensorsysteem op jouw lijn. Drie dingen noteren:
(1) waar hangt de camera precies — boven welke band, bij welke machine?
(2) wat is de output — goed/fout, klasse, of getal?
(3) waar komen de trainingsfoto's vandaan — wie maakt of beoordeelt die?

Geen camera op je lijn? Vraag een collega van een andere lijn.

Bonus: praat één keer met een kwaliteitscollega — 'wie bepaalt eigenlijk wat de camera ziet als goed of fout?'

Neem je notities mee naar de volgende sessie."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Drie vormen ML · CNN · Vier ML-leerklassen voor PdM</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Welke voorbeelden plenair gedeeld? (input voor volgende sessie)
- Welke vragen op de parkeerlijst? (voor lo-ai-fund-117 of vervolg)
- Mentaal model van de groep — foto van flipover 'in stapjes'
-->
