---
theme: default
title: Tampering — waarom ingrijpen op common cause variatie het proces slechter maakt
info: |
  ## SPC Module 1 — Gebruik
  Workshop-blok over tampering en het funnel-experiment van Deming.
  Doelgroep: operators MBO-3, 35 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Niet aan de knop draaien

### Tampering en het funnel-experiment van Deming

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 35 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom.
"Vorig blok leerden we dat common cause variatie gewoon bij het proces hoort.
Vandaag: wat gebeurt er als je daarop reageert — ook al is er niets aan de hand?"

"Deze les heeft een bijnaam: 'niet aan de knop draaien'. En dat is veel moeilijker dan het klinkt."

Brug naar vorig blok: "Wie weet nog wat common cause was?" Vang 1-2 antwoorden.
Bevestig: "De normale schommeling die er altijd zit. Vandaag: wat gebeurt er als je toch reageert?"
-->

---
layout: two-cols
layoutClass: gap-8
---

# De meetcasus

Jij bent operator op een verpakkingslijn.

<v-clicks>

- **Doseerpomp** vult dozen met product
- **Specs:** 500 ± 5 gram (495 – 505 g)
- Je krijgt zo **6 metingen**
- Per meting kies je: **wel — niet — twijfel**
- Één zin **waarom**

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">⚖️</div>
    <div class="text-2xl font-mono font-bold text-blue-700">500 ± 5 g</div>
    <div class="text-sm opacity-60 mt-2">specs</div>
    <div class="text-xs opacity-50 mt-4">verpakkingslijn · 08:00</div>
  </div>
</div>

<!--
Slide 2 — introductie casus.

"Je bent operator op een verpakkingslijn. De doseerpomp vult dozen.
Specs: 500 gram, plus of min 5. Dus alles tussen 495 en 505 is goed.
Je krijgt zo 6 metingen. Per meting kies je: wel ingrijpen, niet ingrijpen, of twijfel.
Pak je werkblad."

Deel wb-01-meetcasus-vulgewicht uit.
-->

---
layout: center
class: text-center
---

# IK DOE — meting 1

<div class="text-6xl font-mono font-bold text-blue-700 my-8">502 g</div>

<div class="max-w-2xl mx-auto text-left text-base bg-blue-50 p-5 rounded-lg">

*"Ik meet 502 gram. Specs: 500 ± 5. Dus 502 zit ruim binnen marge."*

*"Ik doe niets. Ik noteer alleen."*

*"Op het werkblad: 'niet ingrijpen'. Waarom? Binnen specs, één meting zegt nog niks."*

</div>

<div v-click class="mt-8 text-sm opacity-80">
  Nu jij — meting 2 tot en met 6 zelf. 7 minuten. Twijfel mag.
</div>

<!--
IK DOE-moment. Lees hardop voor en wijs op het werkblad.
"Meting 1 — 08:10 — 502 gram. Binnen specs. Ik doe niets, noteer alleen.
Op het werkblad omcirkel ik 'niet ingrijpen' en schrijf erbij: 'binnen specs, één meting zegt nog niks'."

Zeg: "Zo doe jij de andere 5. Omcirkelen, één zin waarom. Geen goed of fout — twijfel mag."

Zet timer op 7 min. Loop rond.
Beantwoord praktische vragen, GEEN inhoudelijke.

NIET uitleggen wat tampering is — dat komt in blok 3.

Na 7 min: "Pen neer. Tel onderaan hoeveel keer je 'wel' 'niet' 'twijfel' koos.
Onthoud je eigen getallen."
-->

---
layout: section
---

# Reflecteren

## Heb jij ooit gecorrigeerd — en werd het erger?

<!--
Overgang naar blok 2.
"Even weg uit de casus, terug naar jezelf. De rest van deze les gaat over hoe
tampering eruitziet op JOUW werkvloer."
-->

---
layout: two-cols-header
---

# STARRT — over jezelf

::left::

### Wat vul je in?
<v-clicks>

- **S**ituatie — wat zag je op je lijn?
- **T**aak — wat dacht je dat je moest doen?
- **A**ctie — wat heb je gedaan?
- **R**esultaat — wat gebeurde er?
- **R**eflectie — wat denk je er nu van?
- **T**ransfer — wat ga je NIET meer doen?

</v-clicks>

::right::

### Hoe vul je in?
<v-clicks>

- Over een moment op **jouw eigen lijn**
- Eerlijk — dit overkomt **iedereen**
- Geen schaamte, geen "juiste antwoord"
- Twijfel mag

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  5 min individueel + 5 min in tweetallen · wb-02-reflectie
</div>

<!--
Deel wb-02-reflectie uit.

Normaliseer vooraf:
"Dit overkomt iedereen. Echt iedereen. Ook teamleiders. Ook mij.
Het is geen schaamtemoment — het is een valkuil in hoe wij als mensen op variatie reageren."

Zet timer op 5 min voor individueel.
Loop rond. Help bij 'Reflectie': "Wat voelde je toen het erger werd?"
Bij 'Transfer': "Wat had je willen weten op dat moment?"

Daarna 5 min in tweetallen delen.
"Elk 2 minuten. Luisteraar stelt alleen verhelderende vragen, geen advies."

Plenair: 2-3 mensen delen één regel. Bedank elke bijdrage expliciet.
-->

---
layout: section
---

# Theoretiseren

## Signalen vs ruis — het funnel-experiment

<!--
Overgang naar blok 3.
"We gaan nu ordenen wat jullie net ervaarden.
Deming heeft hier een experiment van gemaakt dat beroemd is geworden."

Onthul het A3-diagram achter in de zaal.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Demings funnel-experiment

Trechter boven tafel. Kogel op doel.

<v-clicks>

- **Vier strategieën** getest
- Welke geeft de **strakste spreiding**?
- Antwoord verrast bijna iedereen

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-8xl mb-4">🎯</div>
    <div class="text-sm opacity-60">trechter · kogel · doel</div>
    <div class="text-xs opacity-50 mt-4">Deming, 1986</div>
  </div>
</div>

<!--
Slide 8 — introductie funnel.

"Dit heet het funnel-experiment. Deming heeft dit in de jaren '80 beroemd gemaakt.
Hij zette een trechter boven een tafel, liet er een kogel doorheen vallen,
en probeerde die op een doel te krijgen."

"Hij testte vier strategieën. Op de volgende slide zie je ze alle vier met het resultaat."

Deel wb-03-handout-signalen-vs-ruis uit.
"Pak je markeerstift. Markeer onderweg wat een aha-moment voor je is."

OPTIONEEL: Als je appendix A doet (live demo met trechter en knikkers),
doe je die nu — in plaats van alleen de volgende slide.
-->

---
layout: image-right
image: ./diagram-lo-spc-105.svg
backgroundSize: contain
---

# Vier strategieën — één winnaar

<v-clicks>

1. **Niets doen** — laagste spreiding
2. **Compenseren naar doel** — spreiding verdubbelt
3. **Compenseren naar laatste punt** — drijft af
4. **Compenseren naar laatste meting** — chaos

</v-clicks>

<div v-click class="mt-8 p-3 bg-green-50 rounded-lg text-sm">
  <span class="font-bold text-green-800">Strategie 1 wint altijd</span> — zolang het proces stabiel is (alleen common cause)
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: Deming 1986 · Deming Institute
</div>

<!--
Slide 9 — het funnel-diagram.

Loop de vier strategieën langs. Per strategie 30-45 seconden.

Strategie 1 — NIETS DOEN: "Trechter staat stil. Laat de kogel vallen waar hij valt.
Resultaat: strak cluster rond het doel. Laagste spreiding. De winnaar."

Strategie 2 — COMPENSEREN NAAR DOEL: "Kogel valt 3 cm rechts.
Trechter 3 cm links, om de volgende recht te krijgen. Logisch, toch? Fout.
Spreiding verdubbelt. Je voegt zelf variatie toe."

KOPPEL TERUG NAAR DE MEETCASUS:
"Dit is precies wat er gebeurt als de operator bij 502 gram 0,2 terugdraait.
Volgende meting 498 — draait er 0,4 bij. Spreiding verdubbeld."

Strategie 3 + 4: Korter. Kernboodschap: "Nog erger. En nóg erger."
(Voor MBO-4 differentiatie: wiskundige onderbouwing — variantie telt op.)
-->

---
layout: center
class: text-center
---

# Joiner's regel

<div class="text-2xl font-bold italic text-slate-700 my-10 max-w-3xl mx-auto leading-relaxed">
  "Overreageren verhoogt<br/>
  <span class="text-red-600">variatie</span> én <span class="text-red-600">kosten</span>."
</div>

<div v-click class="mt-8 text-sm opacity-70">
  Joiner, B.L. (1994) — <em>Fourth Generation Management</em>
</div>

<div v-click class="mt-12 text-base">
  Twee dingen tegelijk: <span class="font-bold">meer schommeling + meer geld weg</span>
</div>

<!--
Slide 10 — Joiner's kernzin.

Laat deze letterlijk zien. Lees hem op.
"Overreageren verhoogt variatie én kosten. Twee dingen tegelijk —
meer schommeling én meer geld weg. Dat is hoe tampering werkt."

Wijs naar de parkeer-flipover:
"Hoeveel van jullie hadden in de meetcasus minstens één keer 'wel ingrijpen' gekozen?"
Vang handen.

"Geen schaamte — dat is wat iedereen doet. Nu weet je wat het heet en waarom het niet werkt."
-->

---

# Ruis vs signaal — samen invullen

<div class="mt-6 grid grid-cols-2 gap-6">

<div class="p-5 bg-red-50 rounded-lg border-2 border-red-200">
  <div class="text-lg font-bold text-red-700 mb-3">RUIS — niet ingrijpen</div>
  <ul class="text-sm space-y-2">
    <li v-click>Eén meting binnen specs</li>
    <li v-click>Schommeling zonder patroon</li>
    <li v-click>Onderbuikgevoel zonder data</li>
    <li v-click>Variatie binnen bandbreedte</li>
  </ul>
</div>

<div class="p-5 bg-green-50 rounded-lg border-2 border-green-200">
  <div class="text-lg font-bold text-green-700 mb-3">SIGNAAL — wel ingrijpen</div>
  <ul class="text-sm space-y-2">
    <li v-click>Punt buiten UCL / LCL</li>
    <li v-click>Trend over meerdere metingen</li>
    <li v-click>Nelson-patroon / run rule</li>
    <li v-click>Sprong of cluster na wijziging</li>
  </ul>
</div>

</div>

<div v-click class="mt-6 text-center text-sm opacity-70 italic">
  Wacht op een signaal voordat je draait
</div>

<!--
Slide 11 — ruis vs signaal.

Pak de flip-over met de twee kolommen.
Vraag plenair: "Wanneer is het ruis en doe je niets? Roep maar."
Schrijf mee, samen invullen. De slide biedt backup als de groep vastzit.

"En wanneer wel? Wat is een echt signaal?"
Samen invullen: UCL/LCL, trend, Nelson-patroon, sprong.

"Ken je die Nelson-patronen niet? Die komen in lo-spc-201 — dat is de volgende workshop."
-->

---
layout: two-cols
layoutClass: gap-8
---

# En als je tóch zorgen hebt?

<v-clicks>

- Metingen **binnen specs**, maar klanten klagen?
- Uitval loopt **op**?
- Dan is het **systeem**, niet de meting.

</v-clicks>

<div v-click class="mt-6 p-4 bg-amber-50 rounded-lg text-sm">
  <span class="font-bold">Regel:</span> systeemvariatie verbeter je <span class="font-bold">niet</span> met een operator-knopje.
</div>

::right::

### Escaleren — niet zelf draaien
<v-clicks>

1. **Patroon vastleggen** (10-20 metingen met datum/tijd)
2. Melden bij **teamleider**
3. **Engineering** bij matrijs, sensor, materiaal, machine
4. Blijf **zelf meten** zoals je gewend bent

</v-clicks>

<div v-click class="mt-6 text-xs opacity-70 italic">
  Operator lost operator-problemen op.<br/>
  Systeem lost systeemproblemen op.
</div>

<!--
Slide 12 — escalatieroute.

"Laatste punt. Soms is de common cause zelf te groot. Binnen specs, maar niet goed genoeg.
Klanten klagen, uitval loopt op. Wat dan?"

"Niet zelf aan de knop. Escaleren naar teamleider of engineering."

"Dit is geen probleem doorschuiven. Een operator lost operator-problemen op.
Een systeem lost systeemproblemen op."

Verwijs naar de handout: het hele blok "Wat als je tóch zorgen hebt?" staat uitgewerkt.
-->

---
layout: center
class: text-center
---

# Morgen op de werkvloer

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Één meting die je normaal <span class="font-bold">"even zou bijstellen"</span>.<br/>
  Noteer:
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-4 max-w-3xl mx-auto text-left text-sm">

<div class="p-4 bg-blue-50 rounded-lg">
  <div class="font-bold text-blue-800 mb-1">Welke meting?</div>
  <div class="text-xs opacity-70">Machine, waarde, tijd</div>
</div>

<div class="p-4 bg-blue-50 rounded-lg">
  <div class="font-bold text-blue-800 mb-1">Wat ga je NIET doen?</div>
  <div class="text-xs opacity-70">En waarom?</div>
</div>

<div class="p-4 bg-blue-50 rounded-lg">
  <div class="font-bold text-blue-800 mb-1">Escaleren?</div>
  <div class="text-xs opacity-70">Na 5 metingen patroon → teamleider</div>
</div>

</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-green-50 text-green-900 rounded-lg text-base">
  Bonus: bespreek het met een collega-operator.<br/>
  <span class="text-sm opacity-70">"Heb jij weleens iets bijgesteld en werd het erger?"</span>
</div>

<!--
Slide 13 — transferopdracht.

"Deze week: één meting op je lijn die je normaal zou bijstellen.
Je schrijft op: welke meting, wat je NIET gaat doen, waarom.
Als je na 5 metingen écht een patroon ziet — trend, sprong, cluster —
ga je naar je teamleider. Niet zelf draaien."

"Bonus: praat erover met een collega. 'Heb jij weleens iets bijgesteld
en werd het erger?' Je ontdekt dat het iedereen overkomt —
en erover praten maakt het minder stiekem."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop-blok: <span class="font-bold">reactieplan bij een out-of-control signaal</span> (lo-spc-203)
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik) · ko-spc-105
</div>

<!--
Bedank de groep. Kondig het volgende blok aan:
"In het volgende blok gaan we kijken wat je DOET als het een echt signaal is.
Vier stappen — in vaste volgorde."

Vergeet niet:
- Werkbladen 1 en 2 innemen of foto's maken (learning analytics)
- Werkblad 3 (handout) gaat MEE naar de werkvloer — niet innemen
- Parkeer-flipover fotograferen (welke tampering-reflexen waren sterkst?)

Notitie voor jezelf na afloop:
- Wie ontkende tampering nog? (vk-01)
- Bij welke strategie haakten mensen af? (vk-04)
- Welke eigen verhalen kwamen er? (gebruik in lo-spc-203)
-->
