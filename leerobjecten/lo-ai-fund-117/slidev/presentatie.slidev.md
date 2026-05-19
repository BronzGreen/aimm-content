---
theme: default
title: Drie vormen van machine learning — Module 1B Sanne op Lijn B
info: |
  ## AI Fundamentals — Module 1B (Gebruik)
  Workshop-blok over drie basisvormen van machine learning.
  Doelgroep: operators/teamleiders MBO-4, 42 minuten.
  Casus: Sanne op Lijn B bij Van Daalen Plastics — InspectAI (Joyce, kwaliteit) + CycleAdvise (Karim, onderhoud)
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Hoe leert AI?

### Twee systemen op Lijn B, één leerprincipe

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 1B (Gebruik) · Workshop-blok · 42 min<br/>
  Sanne op Lijn B · Joyce (InspectAI) · Karim (CycleAdvise)
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · drie vormen ML · contrastleren
</div>

<!--
Welkom.

"Sanne werkt op Lijn B bij Van Daalen Plastics. Sinds vorig jaar hangen er twee AI-systemen aan haar lijn: InspectAI op het inspectiestation en CycleAdvise op het dashboard. Vandaag laat Joyce van kwaliteit haar zien hoe InspectAI heeft leren kijken. En Karim van onderhoud laat zien hoe CycleAdvise heeft leren adviseren. Wij kijken mee."

Verwijs kort: "In 1A leerde je dat AI leert van voorbeelden. Hier zien we: er zijn drie manieren — en dezelfde manier werkt bij heel verschillende data."
-->

---

# Vier scenario's

<div class="grid grid-cols-2 gap-3 mt-4 text-xs">

<div class="p-3 bg-blue-50 rounded-lg border-2 border-blue-300">

### Case 1A · InspectAI op Lijn B
- **4.000 foto's** van zijpanelen
- **Joyce** (kwaliteit) heeft gelabeld: GOED / TWIJFEL / AFGEKEURD
- Systeem leert nieuwe foto te beoordelen

<div class="mt-2 text-xs opacity-60">Welke vorm?</div>

</div>

<div class="p-3 bg-blue-50 rounded-lg border-2 border-blue-300">

### Case 1B · CycleAdvise op Lijn B
- **4.000 tabel-rijen** (temperatuur, druk, cyclustijd, uitval)
- **Karim** (onderhoud) heeft gelabeld: BIJSTELLEN / NIET BIJSTELLEN
- Systeem leert advies te geven

<div class="mt-2 text-xs opacity-60">Zelfde vorm als 1A?</div>

</div>

<div class="p-3 bg-purple-50 rounded-lg border-2 border-purple-200">

### Case 2 · Lasrobot (ander bedrijf)
- **50.000 lasnaden** in zes maanden
- **Geen administratie** over goed/fout
- Welke dagen lopen anders?

<div class="mt-2 text-xs opacity-60">Welke vorm?</div>

</div>

<div class="p-3 bg-green-50 rounded-lg border-2 border-green-200">

### Case 3 · Verpakkingsrobot (ander bedrijf)
- Mag zelf grijpkracht aanpassen
- Score per poging: **+1** of **-1**
- Leert beste strategie

<div class="mt-2 text-xs opacity-60">Welke vorm?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-01 · twijfel mag
</div>

<!--
Deel wb-01 uit.

Vier scenario's: twee van Sanne's eigen lijn (1A InspectAI / 1B CycleAdvise) + twee externe (lasrobot / verpakkingsrobot).

IK DOE op case 1A zo direct. Daarna contrast-bridge naar 1B.
-->

---
layout: center
class: text-center
---

# IK DOE — case 1A · InspectAI

<div class="text-lg mt-8 max-w-3xl mx-auto leading-relaxed">

"Joyce heeft bij elke foto <span class="font-bold">een antwoord</span> gezet.<br/>
Dat is leren met voorbeelden — <span class="font-bold text-blue-700">supervised learning</span>."

</div>

<div v-click class="mt-8 text-base opacity-80">
  Argument: 4.000 foto's, allemaal gelabeld.
</div>

<div v-click class="mt-10 text-base font-bold">
  Op dezelfde lijn werkt nog een AI — kijk naar 1B.
</div>

<!--
Doe hardop voor:
"Joyce heeft bij elke foto een antwoord gezet. Dat is leren met voorbeelden — supervised learning. Schrijf op: 1A = supervised."

Schrijf demonstratief op een werkblad.

Doe IK DOE kort — 1 min. Daarna 30 sec contrast-bridge naar 1B.
-->

---

# Case 1B en case 2-3 — jouw beurt

<div class="grid grid-cols-3 gap-3 mt-4 text-xs">

<div class="p-3 bg-blue-50 rounded-lg border-2 border-blue-400">

### Case 1B · CycleAdvise
- 4.000 tabel-rijen
- Karim heeft gelabeld
- Zelfde lijn als InspectAI

<div class="mt-3 text-xs italic opacity-70">Zelfde vorm als 1A — of anders?</div>

</div>

<div class="p-3 bg-purple-50 rounded-lg border-2 border-purple-300">

### Case 2 · Lasrobot
- 50.000 lasnaden
- **Geen** administratie
- Welke dagen anders?

<div class="mt-3 text-xs italic opacity-70">Staat er bij elke lasnaad een antwoord?</div>

</div>

<div class="p-3 bg-green-50 rounded-lg border-2 border-green-300">

### Case 3 · Verpakkingsrobot
- Probeert grijpkracht
- Score per poging
- Past aanpak aan

<div class="mt-3 text-xs italic opacity-70">Krijgt hij feedback per actie?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · twijfel mag
</div>

<!--
"Case 2: lasrobot maakt al zes maanden 50.000 lasnaden. Er is geen administratie over welke lasnaden goed of fout waren. Toch wil de productieleider weten of bepaalde dagen anders lopen.

Case 3: verpakkingsrobot mag zelf zijn grijpkracht uitproberen voor verschillende producten. Hij probeert een instelling, kijkt naar het resultaat (heel of beschadigd) en past zijn aanpak aan voor de volgende poging."

Zet timer op 6 min. Loop rond na 2 min.
Stel vragen: "Zijn er labels?" "Krijgt het systeem feedback na elke poging?"
Geef GEEN antwoord. Stop bij niemand langer dan 30 sec.

Schrijf voor jezelf op welke keuzes de groep maakt — voor de plenaire stemming.
-->

---
layout: center
class: text-center
---

# Buurman-check

<div class="text-xl mt-10 max-w-2xl mx-auto leading-relaxed">
  Vergelijk je keuzes op alle vier de cases.
</div>

<div v-click class="mt-6 text-base opacity-70">
  Extra: wat zei je over het contrast tussen 1A en 1B?
</div>

<div v-click class="mt-8 text-lg font-bold text-blue-700">
  Welk woord uit de scenario-tekst was doorslaggevend?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · duo · wb-02
</div>

<!--
Deel wb-02 uit.

"Tweetal met je buurman. Vergelijk je keuzes op alle vier de cases. Extra: wat zei je over het contrast tussen 1A InspectAI en 1B CycleAdvise — zelfde vorm of anders? Welk woord was doorslaggevend?"

Zet timer op 5 min. Loop rond, luister mee.

Verzamel terwijl je rondloopt: welke woorden noemt de groep als signaal? ('Joyce labelt', 'Karim labelt', 'geen administratie', 'score per poging')

Tel innerlijk tot 7 na een vraag.
-->

---

# De antwoorden — let op het signaalwoord

<div class="grid grid-cols-2 gap-3 mt-4 text-xs">

<div class="p-3 bg-blue-50 rounded-lg">

### Case 1A — Supervised
<div class="text-sm italic">Joyce HEEFT GELABELD — 4.000 foto's</div>
<div class="mt-2 text-xs opacity-60">Met labels → supervised</div>

</div>

<div class="p-3 bg-blue-50 rounded-lg">

### Case 1B — Supervised
<div class="text-sm italic">Karim HEEFT GELABELD — 4.000 tabel-rijen</div>
<div class="mt-2 text-xs opacity-60">Óók supervised — andere data, zelfde principe</div>

</div>

<div class="p-3 bg-purple-50 rounded-lg">

### Case 2 — Unsupervised
<div class="text-sm italic">"geen administratie" — welke dagen anders</div>
<div class="mt-2 text-xs opacity-60">Geen labels → patronen vinden</div>

</div>

<div class="p-3 bg-green-50 rounded-lg">

### Case 3 — Reinforcement
<div class="text-sm italic">"score per poging" — +1 / -1</div>
<div class="mt-2 text-xs opacity-60">Feedback per actie → leren door proberen</div>

</div>

</div>

<div v-click class="mt-6 text-center text-base font-bold text-blue-700">
  Kerninzicht: leerprincipe ≠ data-vorm.
</div>

<div v-click class="mt-2 text-center text-sm opacity-80 italic">
  1A foto's, 1B tabel — beide supervised.
</div>

<!--
Per case stemmen:

1A InspectAI: handen omhoog. Tel. "1A = supervised. Joyce heeft 4.000 keer gelabeld."
1B CycleAdvise: handen omhoog "zelfde of anders dan 1A?" Tel. "Óók supervised. Karim heeft 4.000 tabel-rijen gelabeld."

KERNINZICHT EXPLICIET UITSPREKEN: "Twee verschillende data-vormen — foto's en tabel — maar zelfde leerprincipe. Leerprincipe ≠ data-vorm."

Case 2 Lasrobot: handen omhoog. Tel. "Case 2 = unsupervised. Signaalwoord: GEEN ADMINISTRATIE."
Case 3 Verpakkingsrobot: handen omhoog. Tel. "Case 3 = reinforcement. Signaalwoord: SCORE PER POGING."

Maak expliciet: "In de praktijk komen jullie als operator vooral supervised en unsupervised tegen."

Behoud evenwicht — niet reinforcement als 'belangrijker' positioneren.
-->

---
layout: section
---

# Theoretiseren

## Drie vormen op één bladzijde

<!--
Brug naar blok 3.
Deel wb-03 uit. Pak markeerstift erbij.

"Drie vormen op één bladzijde. Per vorm: kerngedachte, type data, maakindustrie-voorbeeld."
-->

---

# Supervised — leren met voorbeelden

<div class="grid grid-cols-2 gap-6 mt-8">

<div>

### Kerngedachte
- **Gelabelde data**: mens heeft antwoord gezet
- Computer leert verschil
- Voorspelt klasse of getal

### Wanneer past het?
- Veel gelabelde data — foto's, tabel, álle data-vormen
- Duidelijk doel: voorspel klasse of getal

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Twee voorbeelden op Lijn B
- **InspectAI** — 4.000 foto's, Joyce labelt
- **CycleAdvise** — 4.000 tabel-rijen, Karim labelt

### Anker
- 1A en 1B — beide supervised — leerprincipe ≠ data-vorm

</div>

</div>

<!--
2 min op deze slide.

"Gelabelde data — een mens heeft goed of fout aangegeven. Voorspelt klasse of getal."

NOEM ALTIJD BEIDE Lijn-B-systemen:
- InspectAI — 4.000 foto's, Joyce van kwaliteit labelt
- CycleAdvise — 4.000 tabel-rijen, Karim van onderhoud labelt

"Twee verschillende data-vormen — foto's en tabel — maar zelfde leerprincipe. Dat is de kern: leerprincipe ≠ data-vorm."

Andere voorbeelden: camera-inspectie met voorbeeldfoto's per klasse, voorspellen wanneer onderdeel slijt.

Vermijd algoritmen (k-means, deep learning) — niveau is leervorm.
-->

---

# Unsupervised — patronen zonder labels

<div class="grid grid-cols-2 gap-6 mt-8">

<div>

### Kerngedachte
- **Geen labels**: niemand heeft aangegeven
- Computer zoekt zelf patronen of groepen
- Vindt afwijkingen of clusters

### Wanneer past het?
- Geen labels beschikbaar
- Wel veel data
- Vraag: zijn er groepen of afwijkingen?

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Maakindustrie-voorbeelden
- Afwijkende sensorpatronen op CNC-frees ontdekken
- Productiedagen groeperen op gedrag

### Anker
- Case 2 — 50.000 ongelabelde lasnaden (extern voorbeeld)

</div>

</div>

<!--
2 min op deze slide.

"Geen labels. Computer zoekt zelf patronen of groepen."

Typische voorbeelden:
- Afwijkende sensorpatronen op CNC-frees
- Productiedagen groeperen

"Case 2 — 50.000 ongelabelde lasnaden — past hier."

Maak expliciet: 'Geen labels = geen supervised — maar wel veel AI-mogelijkheden via unsupervised.'
Voorkomt verkeerde conclusie dat AI bij hen niet kan starten.
-->

---

# Reinforcement — leren door proberen

<div class="grid grid-cols-2 gap-6 mt-8">

<div>

### Kerngedachte
- **Score per actie**: beloning of straf
- Leren door duizenden pogingen
- Optimaliseert beste strategie

### Wanneer past het?
- Sequentiële acties
- Meetbare uitkomst (kosten/baten)
- Onderhoud, robot-tuning

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Maakindustrie-voorbeelden
- Lasersnijder die snijsnelheid optimaliseert
- Robot die instellingen aanpast op type product

### Anker
- Case 3 — verpakkingsrobot met score per poging (extern voorbeeld)

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-80 italic">
  Vuistregel: zeldzaam in praktijk. Vaak alleen bij geavanceerde robots.
</div>

<!--
2 min op deze slide.

"Beloning per actie. Leren door proberen."

Typische voorbeelden:
- Lasersnijder die zelf snijsnelheid optimaliseert
- Robot die instellingen aanpast

"Case 3 — verpakkingsrobot met score per poging — past hier."

Voeg toe: "Vuistregel: in de praktijk kom je als operator vooral supervised en unsupervised tegen. Reinforcement is bijzonder. Te valideren per bedrijf."

NIET als 'belangrijker' positioneren.
-->

---

# Hoe herken je welke vorm past?

<div class="mt-8 text-lg">

Drie vragen over de data op je lijn:

</div>

<div class="mt-6 space-y-3">

<div class="p-4 bg-blue-50 rounded-lg border-l-4 border-blue-500">

**1. Staat er bij elk voorbeeld een antwoord?**

<div v-click class="mt-2 text-sm">
  → Ja: <span class="font-bold">supervised</span> (zoals Joyce en Karim). Nee: ga naar 2.
</div>

</div>

<div class="p-4 bg-green-50 rounded-lg border-l-4 border-green-500">

**2. Krijgt het systeem een score na elke poging?**

<div v-click class="mt-2 text-sm">
  → Ja: <span class="font-bold">reinforcement</span>. Nee: ga naar 3.
</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg border-l-4 border-purple-500">

**3. Zoeken we patronen of groepen?**

<div v-click class="mt-2 text-sm">
  → Ja: <span class="font-bold">unsupervised</span>.
</div>

</div>

</div>

<!--
Drie stappen — duidelijk gemaakt.

"Hoe herken je welke vorm past? Stel deze drie vragen over de data op je lijn:
(1) heeft iemand goed of fout aangegeven? Ja → supervised. Nee → vraag 2.
(2) Krijgt het systeem feedback na elke poging? Ja → reinforcement. Nee → vraag 3.
(3) Zoeken we naar patronen of groepen? Ja → unsupervised."

Houd de drie stappen scherp — geen subtypen toevoegen.
Bij vraag naar semi-supervised: parkeer naar lo-ai-fund-ml-001.

"Onthoud deze drie vragen. Nu jouw lijn — welke vorm past?"
-->

---
layout: section
---

# Experimenteren

## Welke vorm past bij jouw lijn?

<!--
Brug naar blok 4.
"Laatste 10 minuten — eigen lijn-verkenning."
-->

---

# Eigen lijn — vier vragen + contrast

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen
<v-clicks>

- Welk soort **data** hebben we — gelabeld of ongelabeld?
- Is er **feedback per actie** of meten we achteraf?
- Welke **vorm** past — supervised, unsupervised of reinforcement?
- Wat is dan de eerste **vraag** aan IT, kwaliteit of leverancier?

</v-clicks>

<div class="mt-4 text-sm font-bold text-blue-700">
  Plus: lijkt het meer op InspectAI (foto's) of CycleAdvise (tabel)?
</div>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Wie zou bij jullie de Joyce- of Karim-rol spelen?
- Wie bepaalt op jouw lijn wat een afkeur is?
- Wordt er feedback per actie verzameld?
- 'Weet ik niet' = waardevolle eerste IT-vraag

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-04
</div>

<!--
Deel wb-04 uit.

"Laatste 10 minuten. Eén AI-toepassing of monitoring-vraag op je eigen lijn of in je organisatie.
Vier vragen:
(1) welk soort data hebben we — gelabeld door een mens of ongelabeld?
(2) is er feedback per actie of meten we achteraf?
(3) welke vorm zou hierbij passen?
(4) wat is dan de eerste vraag aan onze IT-afdeling of leverancier?"

Gebruik de drie-stappen-vraag uit vorige slide.
'Weet ik niet' is geldig — dat is precies de IT-vraag.

Zet timer op 6 min. Loop rond na 2 min.
Bij vastlopers, geef lijn-suggestie (inspectiecamera, CNC-frees, robot).
Niet bij één persoon te lang blijven — max 60 sec.
-->

---

# Eén-zin-rondje

<div class="mt-12 text-center text-xl">
  Welke vorm past bij jouw lijn — en lijkt het meer op InspectAI of CycleAdvise?
</div>

<div class="mt-6 text-center text-base opacity-70 italic">
  Eén zin per deelnemer. Geen discussie.
</div>

<!--
"Elk om de beurt, één zin: welke vorm past bij jouw lijn — en waarom?"
Loop rond, elke deelnemer noemt vorm + één signaalwoord.
NIET bespreken.

Maximaal 1 min per persoon. Verzamel alle deelnemers.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Drie dingen + contrast
<v-clicks>

- Welke data verzamelen we daar nu al — foto's, tabel, iets anders?
- Heeft iemand goed of fout aangegeven (labels)?
- Welke vorm past — supervised, unsupervised of reinforcement?
- **Plus**: lijkt het meer op InspectAI of CycleAdvise?

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Praat met collega van kwaliteit of onderhoud:<br/><kbd>"Houden wij ergens vast wanneer er iets misgaat?"</kbd>
- Info zit vaak in logboeken
- Maar niet bruikbaar gestructureerd
- Waardevolle ontdekking voor elk AI-project

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Wil je verder met PdM en vier leerklassen?<br/>
  → lo-ai-fund-ml-001 (Module 2 Train)
</div>

<!--
Sluit af met de transferopdracht.

"Deze week: kies één machine of werkstation op je eigen lijn waar je AI-ondersteuning nuttig zou vinden — inspectiecamera, CNC-frees, verpakkingsrobot.
Drie dingen noteren:
(1) welke data verzamelen we daar nu al?
(2) heeft iemand goed of fout aangegeven in die data?
(3) welke vorm past — supervised, unsupervised of reinforcement?

Bonus: praat met een onderhoudscollega — 'houden wij eigenlijk ergens vast wanneer er iets misgaat met deze machine, en hoe?'

Wil je verder met PdM en vier leerklassen (incl. semi-supervised)? Kijk naar lo-ai-fund-ml-001 in Module 2 Train."

Eindig op tijd. Vermeld de bridge naar lo-ai-fund-ml-001.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">CNN · RNN/LSTM · Vier ML-leerklassen voor PdM</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 1B (Gebruik) · Sanne op Lijn B
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Flipover met signaalwoorden gefotografeerd?
- Welke vorm-keuzes plenair gedeeld? (input voor ml-001)
- Welke vragen op parkeerlijst? (algoritmes → CNN/RNN/ensemble; semi-supervised → ml-001)
-->
