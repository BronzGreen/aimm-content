---
theme: default
title: Operator-respons bij een out-of-control signaal — vier stappen
info: |
  ## SPC Module 1 — Gebruik
  Workshop-blok over de vier-stappen-volgorde bij een signaal op de regelkaart.
  Doelgroep: operators MBO-3, 50 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Signaal — wat nu?

### De vier stappen bij een out-of-control punt

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom terug na de pauze.
"In het vorige blok hebben we geleerd om een special cause te herkennen op de regelkaart.
In de komende 50 minuten leren we wat je dán doet.
Want herkennen is niet genoeg — je staat met een signaal en je moet handelen.
De vraag is: wat doe je als eerste, wat doe je als tweede, en wat doe je vooral niet?"

Brug naar vorig blok: "Wie weet nog wat tampering was?" Vang 1-2 antwoorden.
"Precies — bijstellen op een signaal dat eigenlijk geen signaal is.
Vandaag gaan we de andere kant op: wat als het wél een signaal is — wat dan?"
-->

---
layout: two-cols
layoutClass: gap-8
---

# Karim, donderdag 14:20

Spuitgietlijn 4 — onderdeelgewicht.

<v-clicks>

- **Normaal bereik:** 99,8 – 100,2 g · UCL = 100,5
- **Vandaag gemeten:** 100,7 g — boven UCL
- **Vorige 25 metingen:** netjes binnen grenzen
- **Om 14:00:** nieuwe materiaalbatch HDPE-B geladen
- **Wat doet Karim?**

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">⚠️</div>
    <div class="text-2xl font-mono font-bold text-red-600">100,7 g</div>
    <div class="text-sm opacity-60 mt-2">boven UCL</div>
    <div class="text-xs opacity-50 mt-4">spuitgietlijn 4 · do 14:20</div>
  </div>
</div>

<!--
Slide 2 — introductie casus.

"We gaan kijken naar Karim, operator op spuitgietlijn 4. Donderdagmiddag, 14:20.
Hij ziet iets op zijn regelkaart. Pak je werkblad."

Deel wb-01-signaalcasus uit.
"Lees de casus eerst rustig door. Daarna schrijf je in eigen woorden op:
'Als ik Karim was, zou ik nu het volgende doen — in deze volgorde.'
Geen lijstje van regels — gewoon wat jij feitelijk zou doen. 7 minuten."

Zet timer op 7 min. Loop rond. Beantwoord praktische vragen, GEEN inhoudelijke.
Daarna 3 min buurman-check: "Vergelijk 60 sec — verschillen jullie?"

NIET vooraf de vier stappen noemen. Dat is de leerstof.
-->

---
layout: section
---

# Reflecteren

## Wat was jouw eerste reflex?

<!--
Overgang naar blok 2 (reflecteren).
We gaan eerst STARRT individueel, dan plenair turven welke eerste actie iedereen koos.
-->

---
layout: two-cols-header
---

# STARRT — over jezelf

::left::

### Wat vul je in?
<v-clicks>

- **S**ituatie — wat zag je op de kaart?
- **T**aak — wat moest jij beslissen?
- **A**ctie — wat zou je als eerste doen?
- **R**esultaat — wat verwacht je dat er gebeurt?
- **R**eflectie — was die eerste stap juist?
- **T**ransfer — wat neem je mee?

</v-clicks>

::right::

### Hoe vul je in?
<v-clicks>

- Over **jezelf**, niet over Karim
- In jouw eigen woorden
- Eerlijk — geen "juiste antwoord"
- Twijfel mag

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · wb-02-starrt-reflectie
</div>

<!--
Deel wb-02 uit.
"Dit werkblad volgt de STARRT-structuur. Je vult het in over jezelf — niet over Karim.
Wat zou JIJ doen, en waarom?"

Zet timer op 5 min. Loop rond.
Help bij blokkades op 'Reflectie' met: "Wat denk je achteraf — was die eerste stap inderdaad de juiste?"
-->

---

# Wat schreef jij als eerste actie?

<div class="mt-8 grid grid-cols-2 gap-6 text-base">

<div class="p-4 bg-blue-50 rounded-lg">
  <div class="font-bold text-blue-700">📞 "Ik bel teamleider"</div>
  <div class="text-xs opacity-60 mt-1">turfje</div>
</div>

<div class="p-4 bg-green-50 rounded-lg">
  <div class="font-bold text-green-700">📏 "Ik meet opnieuw"</div>
  <div class="text-xs opacity-60 mt-1">turfje</div>
</div>

<div class="p-4 bg-amber-50 rounded-lg">
  <div class="font-bold text-amber-700">🔍 "Ik kijk wat net is veranderd"</div>
  <div class="text-xs opacity-60 mt-1">turfje</div>
</div>

<div class="p-4 bg-red-50 rounded-lg">
  <div class="font-bold text-red-700">📦 "Ik zet stukken apart"</div>
  <div class="text-xs opacity-60 mt-1">turfje</div>
</div>

<div class="p-4 bg-orange-100 rounded-lg border-2 border-orange-300">
  <div class="font-bold text-orange-800">🎛️ "Ik draai de instelling bij"</div>
  <div class="text-xs opacity-70 mt-1">→ PARKEER</div>
</div>

<div class="p-4 bg-gray-50 rounded-lg">
  <div class="font-bold text-gray-700">❓ "Anders, namelijk..."</div>
  <div class="text-xs opacity-60 mt-1">turfje</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Vijf operators in één ruimte. <span class="font-bold">Vijf verschillende eerste acties.</span>
</div>

<!--
Plenaire inventarisatie: ga rond, in één zin per persoon de eerste actie.
Schrijf op flip-over een streepje per categorie.

NIET nu beoordelen welk antwoord 'goed' is. Alleen verzamelen.

Na de ronde: laat de cijfers zien.
"Kijk eens. Vijf verschillende eerste acties. Vijf operators in één fabriek zouden dus
vijf verschillende dingen doen bij hetzelfde signaal. Wat is jouw vraag op dit moment?"

Vang 1-2 vragen. Niet beantwoorden — alleen erkennen: "Goede vraag, daar gaan we nu naartoe."
-->

---
layout: section
---

# Theoretiseren

## De vier stappen — in deze volgorde

<!--
Overgang naar blok 3.
"Twijfel is brandstof. We gaan nu kijken hoe je deze situatie volgens het AIAG SPC Reference Manual
moet aanpakken — en je gaat zien dat de volgorde uitmaakt."

Onthul het A3-diagram achter in de zaal.
-->

---
layout: image-right
image: ./diagram-lo-spc-203.svg
backgroundSize: contain
---

# Vier stappen, vaste volgorde

<v-clicks>

1. **Meetfout uitsluiten** — meet ik wel goed?
2. **Recente wijziging checken** — wat is er net veranderd?
3. **Verdachte output veiligstellen** — apart zetten + etiket
4. **Teamleider informeren** — bel + meld in 30 sec

</v-clicks>

<div v-click class="mt-8 text-sm opacity-70">
  Niet je gevoel. Niet je ervaring. <span class="font-bold">Deze volgorde — elke keer.</span>
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: AIAG SPC Reference Manual; Ford PPAP Reaction Plan
</div>

<!--
Slide 8 — vier-stappen-cyclus visueel.

"Hier is de volgorde. Vier stappen, in deze volgorde.
Niet je gevoel, niet je ervaring, niet wat de buurman doet — déze volgorde, elke keer."

Deel wb-03-handout uit.
"Pak je markeerstift. Markeer onderweg wat anders is dan jouw eerste-actie-antwoord."

We gaan nu stap voor stap door — slides 9-12.
-->

---
layout: two-cols
layoutClass: gap-6
---

# Stap 1 — Meetfout uitsluiten

### Eerste vraag
<v-clicks>

- Is het instrument gecalibreerd?
- Volgens procedure gemeten?
- Tweede meting met ander apparaat?
- Referentiestuk?

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">📏</div>
    <div class="text-base opacity-70">"Meet ik het wel goed?"</div>
  </div>

  <div v-click class="p-4 bg-green-50 rounded-lg text-sm">
    <div class="font-bold text-green-800 mb-1">Karim:</div>
    Tweede meting met back-up-weegschaal → óók 100,7 g. Calibratie vanmorgen 06:00 ploegwissel. <span class="font-bold">Meetfout uitgesloten.</span>
  </div>
</div>

<!--
Stap 1 (2 min).

"Een signaal is alleen geldig als de meting klopt. Eerste vraag: is mijn meting wel correct?"

Wijs naar de turfjes-flip-over: "Hoeveel van jullie hadden DIT als eerste actie?"
Tel hardop. Vaak: 0-2 turfjes. Maak het zichtbaar.

"In de literatuur (AIAG MSA) is naar schatting 20-30% van de signalen feitelijk een meetfout.
Als je daarop gaat ingrijpen, maak je het proces alleen maar slechter."

Schrijf op flip-over kolom STAP 1: "Meet ik het wel goed?"
-->

---
layout: two-cols
layoutClass: gap-6
---

# Stap 2 — Recente wijziging checken

### Wat is er **recent** veranderd?
<v-clicks>

- Nieuwe materiaalbatch
- Setup-wissel
- Andere ploeg
- Onderhoud uitgevoerd
- Nieuwe of bijgeslepen tools
- Veranderde omgeving (temp, vocht)

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">🔍</div>
    <div class="text-base opacity-70">"Wat is er net veranderd?"</div>
  </div>

  <div v-click class="p-4 bg-amber-50 rounded-lg text-sm">
    <div class="font-bold text-amber-800 mb-1">Karim:</div>
    Setup-board: <span class="font-mono">14:00 nieuwe batch HDPE leverancier B</span>. Geen matrijswissel, geen onderhoud, ploeg sinds 06:00 dezelfde. <span class="font-bold">Wijziging gevonden.</span>
  </div>
</div>

<!--
Stap 2 (2 min).

"Wat is er recent veranderd? Recent betekent: laatste uur, laatste shift.
Niet vorige maand. Niet 'ik weet het niet meer'."

Karim ziet: 14:00 nieuwe batch. Logische kandidaat-oorzaak — densiteit kan
verschillen tussen leveranciers.

Schrijf op flip-over kolom STAP 2: "Wat is er net veranderd?"

[MBO-4 differentiatie]: voeg toe: "En welke regel ging hier af? Punt buiten grenzen.
Maar als het een trend was, of een run rule (Western Electric), zou stap 2 nóg zwaarder wegen."
-->

---
layout: two-cols
layoutClass: gap-6
---

# Stap 3 — Verdachte output veiligstellen

### Niet één stuk — alle stukken sinds de wijziging
<v-clicks>

- Sinds laatste in-control punt
- Apart zetten in rode bak
- Etiket: lijn, tijd, signaal, vermoeden
- **Niet** doorvoeren naar volgende stap

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">📦</div>
    <div class="text-base opacity-70">"Apart zetten + etiket"</div>
  </div>

  <div v-click class="p-4 bg-red-50 rounded-lg text-sm">
    <div class="font-bold text-red-800 mb-1">Karim:</div>
    Alle stukken sinds 14:00 in de rode bak. Etiket: <span class="font-mono">"lijn 4, 14:00-14:20, batch HDPE-B, gewicht-OOC"</span>.
  </div>
</div>

<!--
Stap 3 (2 min).

PAK DE RODE BAK van de tafel. Hou hem omhoog tijdens deze slide.

"Producten gemaakt sinds het laatste in-control punt zijn verdacht.
Niet één stuk — ALLE stukken sinds de wijziging.
Bij Karim: het signaal kwam om 14:20, maar de batch wisselde om 14:00.
Dus alles tussen 14:00 en 14:20 is verdacht."

"Dit is geen vies woord — dit is bescherming.
Voor de klant, voor jou, voor de fabriek."

Schrijf op flip-over kolom STAP 3: "Apart zetten + etiket."
-->

---
layout: two-cols
layoutClass: gap-6
---

# Stap 4 — Teamleider informeren

### Geen zelf-correctie — teamleider beslist
<v-clicks>

- Doorgaan na verificatie?
- Lijn stilleggen?
- Engineering inschakelen?
- 100% inspectie van rode bak?

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-6xl mb-2">📞</div>
    <div class="text-base opacity-70">"Bel + meld in 30 sec"</div>
  </div>

  <div v-click class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-800 mb-1">Karim belt Yasmin:</div>
    <span class="italic">"Lijn 4, één punt boven UCL gewicht, meting bevestigd, nieuwe batch HDPE-B sinds 14:00, output sinds 14:00 in rode bak."</span> 30 seconden.
  </div>
</div>

<!--
Stap 4 (2 min).

"Geen zelf-correctie zonder consultatie. Stap 4 is GEEN escalatie als laatste redmiddel —
het is onderdeel van de standaard reactie."

Optioneel: pak telefoon-prop. Doe de melding voor: "Yasmin, met Karim, lijn 4..."
30 seconden. Concreet. Compleet. Geen excuses, geen interpretatie — feiten.

"Yasmin beslist over wat er daarna gebeurt. Dat beschermt jou als operator:
bij een latere klacht is duidelijk wie wat besloot."

Schrijf op flip-over kolom STAP 4: "Bel + meld in 30 sec."
-->

---
layout: center
class: text-center
---

# Wat doe je vooral NIET

<div class="mt-6 grid grid-cols-2 gap-4 max-w-2xl mx-auto text-left text-sm">

<div v-click class="p-3 bg-red-50 rounded-lg">
  <span class="font-bold text-red-700">❌ "Terugduwen" naar gemiddelde</span><br/>
  <span class="opacity-70 text-xs">= tampering (ko-spc-105)</span>
</div>

<div v-click class="p-3 bg-red-50 rounded-lg">
  <span class="font-bold text-red-700">❌ Negeren — "komt wel goed"</span><br/>
  <span class="opacity-70 text-xs">audit / klantklacht later</span>
</div>

<div v-click class="p-3 bg-red-50 rounded-lg">
  <span class="font-bold text-red-700">❌ Wachten op meer signalen</span><br/>
  <span class="opacity-70 text-xs">één geldig signaal is genoeg</span>
</div>

<div v-click class="p-3 bg-red-50 rounded-lg">
  <span class="font-bold text-red-700">❌ Meetwaarde aanpassen in systeem</span><br/>
  <span class="opacity-70 text-xs">= fraude · reden voor ontslag</span>
</div>

</div>

<!--
De anti-regel-slide (1 min).

"Wat doe je vooral NIET?"

Loop kort de vier verboden langs.
Bij de eerste: "Niet zomaar terugduwen — dat is tampering, ko-spc-105 van vorig blok.
Daar hebben we al uitgebreid naar gekeken."

Bij de laatste: "Meetwaarde aanpassen klinkt onschuldig, maar dat is data-vervalsing.
Bij elke audit valt dit op en is het reden voor ontslag. Geen grijs gebied."

Korte vraagronde: "Welke stap had je niet zelf bedacht?
Of welke staat op een andere plek dan jij dacht?"
2-3 mensen kort delen.
-->

---
layout: section
---

# Experimenteren

## Eén signaal van jouw lijn

<!--
Overgang naar blok 4.
"Karim is klaar. Nu jij. We gaan de vier stappen toepassen op jouw lijn."

Deel wb-04-eigen-reactieplan uit.
"De afgelopen 37 minuten ging over Karim. De komende 13 minuten gaan over jou.
Je vult een reactieplan in voor één signaal-type op jouw lijn —
geen abstracte oefening, maar iets dat morgen op je werkplek hangt."
-->

---

# Jouw reactieplan — concreet

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Welk signaal kies je?
<v-clicks>

- Eén meetwaarde van jouw lijn
- Welk signaal-type? (punt buiten grenzen, trend, cluster)
- Bij voorkeur dezelfde meetwaarde als in vorig blok

</v-clicks>

</div>

<div>

### Vul in per stap
<v-clicks>

- Stap 1: welk back-up-instrument?
- Stap 2: waar staat het setup-board?
- Stap 3: waar staat de rode bak?
- Stap 4: telefoonnummer teamleider

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  9 min · individueel · wb-04-eigen-reactieplan
</div>

<!--
Inventarisatie-vraag (1 min): "Even rondkijken: noem in één zin welk signaal je
op JOUW lijn zou kunnen tegenkomen."
Vang 4-5 voorbeelden op (gewicht boven UCL, temperatuur trend, diameter buiten tolerantie).
Niet bespreken — alleen verzamelen. Helpt deelnemers die niet weten wat ze moeten kiezen.

Zet timer op 9 min. Loop rond.
Help bij blokkades met:
- "Welke meting doe je sowieso al? (= dezelfde als in lo-spc-104)"
- "Welk instrument heb je voor de tweede meting?"
- "Wie is jouw teamleider? Heb je het nummer paraat?"
- "Waar staat jouw rode bak? Zo niet — kun je er een regelen?"

Bevestig dat klein beginnen prima is — één signaal-type, niet alle.
NIET zelf meedenken over instellingen — autonomie is de werkende component.
-->

---
layout: center
class: text-center
---

# Deze week op de werkvloer

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Hang je reactieplan <span class="font-bold">zichtbaar bij je machine.</span><br/>
  Als zich het signaal voordoet — ook als 'vals alarm' —<br/>
  loop je <span class="font-bold">de vier stappen door.</span>
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-base">
  Bonus: laat je reactieplan zien aan je teamleider.<br/>
  <span class="text-sm opacity-70">"Klopt het telefoonnummer? Klopt de procedure?"</span>
</div>

<!--
Korte deel-ronde (2 min): "Wie wil in één zin vertellen welk signaal je gaat plannen,
en wat voor jou de moeilijkste stap wordt?"
3-4 deelnemers, max 30 sec per persoon.

Sluit af met de transferopdracht en de bonus-vraag aan teamleider.
"Daarmee maak je samen het reactieplan eigenaarschap."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop-blok: <span class="font-bold">groepsreflectie en transfer naar eigen lijn</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik)
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (groepsreflectie + transfer, 35 min).
Vergeet niet werkbladen 1-2-3 in te nemen of foto's te maken voor learning analytics.
Werkblad 4 (eigen reactieplan) gaat MEE naar de werkvloer — niet innemen.

Notitie voor jezelf na afloop:
- Welke "eerste actie" had de meeste turfjes? (= reflex die de groep moet afleren)
- Bij welke stap was de meeste discussie?
- Welke valkuil viel het meeste op (vk-01 tampering / vk-02 stap-1-overslaan / vk-03 negeren / vk-04 zelf-correctie)?
- Welke signaal-types hebben deelnemers gekozen voor het reactieplan?
-->
