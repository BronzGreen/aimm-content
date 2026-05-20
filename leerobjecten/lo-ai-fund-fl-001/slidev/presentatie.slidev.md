---
theme: default
title: Federated Learning — samen leren zonder data te delen
info: |
  ## AI Fundamentals — Module 2 (Train)
  Workshop-blok over federated learning: drie kenmerken, drie scenario's, eigen organisatie-actieplan.
  Doelgroep: operators/teamleiders MBO-4, 50 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Federated Learning

### Samen leren zonder data te delen

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 2 (Train) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · multi-fabriek PdM · OEM-leverancier
</div>

<!--
Welkom. De komende 50 minuten kijken we naar een ML-paradigma dat je naam gaat zien als jullie organisatie nadenkt over data-samenwerking: federated learning.

Tegen het eind kun je in eigen woorden uitleggen wat het is, en kun je drie scenario's beoordelen op of het past.

[Open warm op] Geen vragen vooraf — direct door naar de medische opening op slide 2.
-->

---
layout: center
class: text-center
---

# Een vraag om mee te beginnen

<div class="text-2xl mt-8 max-w-2xl mx-auto leading-relaxed opacity-80">
  Vijf ziekenhuizen willen samen<br/>
  een AI-model trainen voor tumordetectie.
</div>

<div v-click class="text-xl mt-8 opacity-70 max-w-xl mx-auto">
  Niemand mag patiëntbeelden uit het pand laten gaan.
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Hoe doen ze het dan?
</div>

<!--
Pauze 5 seconden na de vraag.
"Iemand een idee?" — vang 1-2 reacties.
Bevestig: "Dat is precies de denkrichting: niet de data delen, maar iets anders."

Brug naar slide 3 — het diagram.
-->

---

# Klassiek vs. federated

<div class="grid grid-cols-2 gap-8 mt-6">

<div class="p-6 bg-red-50 rounded-xl border-2 border-red-200">

### Klassieke ML

<v-clicks>

- Alle data → één centrale plek
- Centraal trainen
- Model komt terug naar gebruiker
- Vereist: data delen mag

</v-clicks>

</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">

### Federated Learning

<v-clicks>

- Model gaat **naar de data toe**
- Lokaal trainen op eigen data
- Alleen **parameters** terug
- Centrale server middelt
- Volgende ronde

</v-clicks>

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Ruwe data blijft thuis — alleen geleerde gewichten reizen.
</div>

<!--
Wijs op A3-diagram in de zaal en op het scherm.
Loop het verschil langzaam af. Klik per punt.
Eindig met de slogan: "ruwe data blijft thuis — alleen geleerde gewichten reizen."

Deel daarna wb-01 uit:
"Tijdens de drie kenmerken die ik nu uitleg vul je dit schema in. Per kenmerk: wat gebeurt er bij klassieke ML, wat gebeurt er bij FL? Markeer het verschil dat jou het meest verrast."
-->

---
layout: center
class: text-center
---

# Kenmerk 1

## Data blijft lokaal

<div class="text-xl mt-10 max-w-xl mx-auto opacity-80">
  Sensorlogs, camerabeelden, ERP-rijen<br/>
  verlaten de fabriek niet.
</div>

<div v-click class="mt-10 text-base opacity-60">
  GDPR · IP-bescherming · klantvertrouwen
</div>

<!--
Twee minuten max.
"Welke implicatie heeft dat voor privacy?" — vang 1 antwoord.
Bevestig: GDPR-compliance, IP-bescherming, klantvertrouwen.

Niet ingaan op differential privacy of gradient leakage.
Houd het bij: data blijft thuis.
-->

---
layout: center
class: text-center
---

# Kenmerk 2

## Alleen modelparameters reizen

<div class="text-3xl mt-10 font-mono">
  <span class="opacity-60">parameters</span>
  <span class="text-xl mx-2 opacity-40">&lt;&lt;</span>
  <span class="text-red-500">ruwe data</span>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Geleerde gewichten — niet de patiëntfoto, niet de productformule.
</div>

<div v-click class="mt-6 text-sm opacity-50">
  Veel kleiner. Veel minder reconstrueerbaar.
</div>

<!--
Twee minuten.
Schrijf op flip-over: 'modelparameters << ruwe data'.

"Dat is heel andere data dan ruwe sensorlogs.
Veel kleiner, en je kunt er geen patiëntfoto of productformule uit reconstrueren — al zijn er geavanceerde aanvallen, daarover later meer."

Niet uitweiden. Door naar kenmerk 3.
-->

---
layout: center
class: text-center
---

# Kenmerk 3

## Centrale server aggregeert

<div class="grid grid-cols-3 gap-4 mt-10 text-sm">
  <div class="p-3 bg-blue-50 rounded-lg">Node A<br/>traint lokaal</div>
  <div class="p-3 bg-blue-50 rounded-lg">Node B<br/>traint lokaal</div>
  <div class="p-3 bg-blue-50 rounded-lg">Node C<br/>traint lokaal</div>
</div>

<div class="mt-4 text-2xl">↓</div>

<div class="mt-2 p-3 bg-amber-100 rounded-lg max-w-xs mx-auto font-bold">
  Centrale aggregator
</div>

<div v-click class="mt-6 text-base opacity-70">
  Middelt parameters · stuurt globaal model terug · volgende ronde
</div>

<div v-click class="mt-6 text-sm text-red-600">
  Beperking: single point of failure
</div>

<!--
Drie minuten.
"Wie ziet hier al een beperking?" — wacht.
Antwoord: single point of failure.

Bevestig: "Klopt — als de aggregator plat ligt, ligt de hele trainingsronde stil. Vanilla FL is niet decentraal — er bestaan decentrale varianten, maar die laten we vandaag links liggen."

Indien iemand naar FedAvg of differential privacy vraagt: parkeren op flip-over.
-->

---

# Waar zit FL al?

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-purple-50 rounded-lg">

### Telecom & mobile
- Google Keyboard (2017)
- Voorspellingsmodellen op je telefoon
- Niet typtekst uploaden

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Medisch
- Multi-ziekenhuis diagnose
- Geen patiëntdata delen
- Model leert van iedereen

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Maakindustrie (nu)
- Multi-fabriek PdM
- OEM-leverancier ketens
- Sectorconsortia

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Drie golven · zelfde paradigma.
</div>

<!--
Anderhalve minuut.
Kort de drie golven afgaan.

Maak de brug: "Nu we weten wat FL is, gaan we kijken: past het in jouw situatie?"
Naar slide 8 — sectie ervaren.
-->

---
layout: center
class: text-center
---

# Wil je het zien gebeuren?

<div class="text-xl mt-10 max-w-xl mx-auto opacity-80">
  91 seconden video
</div>

<div v-click class="mt-8 text-lg opacity-70">
  Drie fabrieken, data blijft thuis, alleen parameters reizen,<br/>
  samen leren pomp-anomalieën herkennen.
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion · <code>FederatedLearningVideo</code>)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
Optionele inzet — aan einde van fase 1 (theoretiseren), na de drie kenmerken.
Scene 4 (parameter-aggregatie) is dé visuele anker voor 'alleen modelparameters reizen'.
-->

---
layout: section
---

# Drie scenario's

## Past FL hier wel of niet?

<!--
Overgang naar blok 2 (ervaren).
Zeg: "Per scenario kies je: past FL hier, en welk van de drie kenmerken is doorslaggevend."

Deel wb-02 uit.
-->

---

# Drie scenario's

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-amber-50 rounded-lg border-2 border-amber-200">

### A · Zusterfabrieken
- Drie fabrieken concern
- Zelfde lager-types
- Samen PdM-model trainen

<div class="mt-3 text-xs opacity-60">FL wel of niet?</div>

</div>

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### B · Edge-device
- Mobiele kraan
- 4G — beperkte bandbreedte
- Realtime trillingsanalyse

<div class="mt-3 text-xs opacity-60">FL wel of niet?</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg border-2 border-purple-200">

### C · Lasrobot
- Productiedata concurrentiegevoelig
- Klant: data blijft van ons
- OEM wil model blijven verbeteren

<div class="mt-3 text-xs opacity-60">FL wel of niet?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-02
</div>

<!--
IK DOE eerst — scenario A voor:
"Zusterfabrieken — als ze al volledig vertrouwen, simpeler centraal.
Maar als verschillende GDPR-regimes of concurrerende plant managers — dan wordt FL relevant.
A is bewust grijs — 'het hangt ervan af'."

Daarna: "Pak je werkblad. Doe B en C zelf. Zes minuten."

Loop rond. Stel verdiepende vragen.
-->

---
layout: center
class: text-center
---

# Stem mee

<div class="grid grid-cols-3 gap-6 mt-10 text-base">
  <div class="p-4 bg-amber-50 rounded-lg">
    <div class="font-bold text-amber-700">A · Zusterfabrieken</div>
    <div class="mt-2 text-sm">FL ja / nee / twijfel?</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-700">B · Edge-device</div>
    <div class="mt-2 text-sm">FL ja / nee / twijfel?</div>
  </div>
  <div class="p-4 bg-purple-50 rounded-lg">
    <div class="font-bold text-purple-700">C · Lasrobot</div>
    <div class="mt-2 text-sm">FL ja / nee / twijfel?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Hand omhoog per stelling — tellen we plenair.
</div>

<!--
Eerst tweetallen vergelijken (5 min).
Daarna plenair stemmen — schrijf uitslag op flip-over.

Tel innerlijk tot 7 na elke vraag.
Veroordeel geen antwoord.
-->

---

# Het antwoord

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-amber-50 rounded-lg">

### A · Grijs

- Hangt af van vertrouwen
- Eén concern + datalake → centraal simpeler
- Verschillende GDPR-regimes → FL relevant

<div class="mt-3 text-xs italic">data lokaal — als nodig</div>

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### B · FL past sterk

- 4G-bandbreedte beperkt
- Parameters &lt;&lt; ruwe data
- Lokaal trainen rendabel

<div class="mt-3 text-xs italic">bandbreedte-kenmerk</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### C · FL past sterk

- Productie-IP gevoelig
- Klant: data blijft van ons
- OEM krijgt verbeterd model

<div class="mt-3 text-xs italic">IP-bescherming</div>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  FL is een antwoord op een echt obstakel — niet altijd-toepassen.
</div>

<!--
B en C zijn unaniem — kort bevestigen.
A is bewust grijs. Vraag een ja-stemmer en een nee/twijfel-stemmer.

Bevestig: "FL past als de data tussen zusterfabrieken niet zomaar gedeeld mag worden — bijvoorbeeld door GDPR of concurrentie tussen plant managers. Maar als ze al delen via een datalake, voegt FL alleen overhead toe."
-->

---
layout: section
---

# Experimenteren

## Waar speelt FL bij ons?

<!--
Overgang naar blok 4.
"Laatste 13 minuten — eigen organisatie-scan.
Welke data wordt nu níet centraal verzameld vanwege privacy, IP of bandbreedte?"
-->

---

# Eigen organisatie-scan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier velden in te vullen
<v-clicks>

- Welke **data** betreft het?
- Met **wie** zou je samen willen leren?
- Welk **modeldoel** — vision, vibration, kwaliteit, RUL?
- Welk **kenmerk** weegt het zwaarst?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Welke data krijg je nu niet uit de zusterfabriek?
- Heeft jouw klant ooit gezegd: deze data blijft binnen?
- Met welke leverancier zou je willen co-trainen?
- Hypothetisch mag — als het maar concreet is.

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-04
</div>

<!--
Eerst inventarisatie-vraag (1 min): "Bij wie speelt dit type vraag — multi-fabriek, OEM, klant?"
Vang 4-5 antwoorden, niet bespreken.

Zet timer op 8 min.
Loop rond. Help één concrete trio invullen: data-type / partner / modeldoel.

Een specifiek hypothetisch voorbeeld werkt beter dan een vaag generiek antwoord.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Open een gesprek
<v-clicks>

- Praat met IT of data-collega
- Open met: "Ik leerde over federated learning"
- Vraag: "Kennen jullie het concept?"
- Vraag: "Past het in onze data-strategie?"

</v-clicks>

</div>

<div>

### Wat je gaat horen
<v-clicks>

- Soms: "ja — staat al op de roadmap"
- Soms: "nee — niet relevant voor ons"
- Soms: "interessant — vertel meer"
- Allemaal nuttig — je krijgt zicht op de stand

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat heb je gehoord?
</div>

<!--
Sluit af met de transferopdracht.
"Volgende sessie bespreken we kort: wat heb je gehoord van IT?
Daarna gaan we door naar de volgende paradigma-LO."

Geef niet te veel weg — laat de nieuwsgierigheid open.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">CNN-architectuur, RNN/LSTM, Ensemble learning</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Stemming per scenario (verdeling A/B/C)
- Welke transfer-acties zijn aangekondigd? (input voor volgende sessie)
- Welke vragen zijn op de parkeerlijst beland? (verdiepingsmateriaal)
-->
