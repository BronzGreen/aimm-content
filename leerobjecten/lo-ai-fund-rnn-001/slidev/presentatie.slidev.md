---
theme: default
title: RNN, LSTM en BiLSTM — neurale netwerken met geheugen
info: |
  ## AI Fundamentals — Module 2 (Train)
  Workshop-blok over RNN, LSTM en BiLSTM voor tijdreeksen.
  Doelgroep: operators/teamleiders MBO-4, 50 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# RNN, LSTM, BiLSTM

### Neurale netwerken met geheugen

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 2 (Train) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · vibration · temperatuur · druk · akoestiek
</div>

<!--
Welkom. De komende 50 minuten kijken we naar drie verwante AI-architecturen voor tijdreeks-data.

Tegen het eind kun je per variant uitleggen wat hij doet, en kun je drie scenario's beoordelen op welke variant past.

Niet de wiskunde — wel het idee.
-->

---
layout: center
class: text-center
---

# Een venster van 200 samples

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  PdM-systemen kijken zelden naar één meting.<br/>
  Vaak naar een tijdreeks.
</div>

<div v-click class="text-xl mt-8 opacity-70">
  Waarom?
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Trends · patronen · context.
</div>

<!--
"Wie heeft op zijn lijn een PdM-systeem dat een venster bekijkt voordat het alarmeert?"
Vang 1-2 reacties. "Waarom een venster en niet één meetwaarde?"
Antwoord: trends, patronen.

"Voor tijdreeksen heb je een ander type AI nodig — met geheugen.
Drie geheugen-architecturen vandaag."
-->

---
layout: center
class: text-center
---

# Variant 1 · Vanilla RNN

<div class="text-xl mt-8 opacity-80">
  Recurrent Neural Network
</div>

<div class="mt-10 max-w-xl mx-auto text-base">
  <span class="font-bold">Idee:</span> output van vorige timestep<br/>
  is input voor volgende timestep
</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg max-w-md mx-auto text-sm">
  <span class="font-bold">In schrifttermen:</span><br/>
  ik schrijf alleen op wat er net gebeurde
</div>

<div v-click class="mt-6 text-base text-red-600">
  Probleem: long-term dependency<br/>
  <span class="opacity-70 text-sm">vergeet snel wat ver geleden gebeurde</span>
</div>

<!--
Vier minuten.
Pak fysiek het schrift erbij.

"Stel: dit is mijn aantekeningen-schrift. Elke pagina = één timestep.
Wat ik schrijf, wat ik onthoud — daar gaan de drie varianten over."

"RNN: ik schrijf alleen op wat er net gebeurde. Wat 50 pagina's geleden gebeurde? Vergeten."

Probleem: long-term dependency.
Voorbeeld: trillingspiek nu door wrijving 100 samples geleden — RNN heeft die wrijving allang vergeten.

Schrijf op flip-over: 'RNN: kort geheugen — vergeet snel'.
-->

---

# Variant 2 · LSTM

<div class="text-base opacity-70 mt-2">Long Short-Term Memory · 1997</div>

<div class="grid grid-cols-3 gap-4 mt-8">

<div class="p-5 bg-red-50 rounded-xl border-2 border-red-200 text-center">
  <div class="text-3xl mb-2">🚫</div>
  <div class="font-bold text-red-700">Forget gate</div>
  <div class="mt-2 text-xs opacity-70">Wat vergeten we?</div>
  <div class="mt-1 text-xs italic">doorstrepen</div>
</div>

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-200 text-center">
  <div class="text-3xl mb-2">➕</div>
  <div class="font-bold text-green-700">Input gate</div>
  <div class="mt-2 text-xs opacity-70">Wat voegen we toe?</div>
  <div class="mt-1 text-xs italic">bijschrijven</div>
</div>

<div class="p-5 bg-yellow-50 rounded-xl border-2 border-yellow-200 text-center">
  <div class="text-3xl mb-2">📤</div>
  <div class="font-bold text-yellow-700">Output gate</div>
  <div class="mt-2 text-xs opacity-70">Wat geven we door?</div>
  <div class="mt-1 text-xs italic">voorlezen</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Drie gates · cell-state als rode draad · geheugen overleeft over lange afstand.
</div>

<!--
Zes minuten — kern van fase 1.

Pak de drie post-its in kleuren.
Houd elke omhoog terwijl je hem benoemt:

- Rood (forget): "Wat vergeten we uit het langetermijngeheugen?"
- Groen (input): "Wat voegen we toe?"
- Geel (output): "Wat geven we door naar de volgende laag?"

"Drie gates, drie acties: doorstrepen, bijschrijven, voorlezen.
Plus cell-state — een rode draad door alle timesteps.
LSTM is het werkpaard van realtime PdM."

Schrijf op flip-over: 'LSTM: lang geheugen — drie gates'.
-->

---

# Variant 3 · BiLSTM

<div class="text-base opacity-70 mt-2">Bidirectional LSTM</div>

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-4 bg-blue-50 rounded-lg">

### LSTM 1
- Leest van **begin** naar **eind**
- Verleden → nu

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### LSTM 2
- Leest van **eind** naar **begin**
- Toekomst → nu

</div>

</div>

<div v-click class="mt-8 p-4 bg-amber-100 rounded-lg max-w-xl mx-auto text-center">
  Beide outputs samengevoegd<br/>
  voor elke timestep wordt zowel verleden als toekomst gebruikt
</div>

<div v-click class="mt-6 text-center text-base text-red-600">
  Catch: alleen offline · je hebt de hele reeks vooraf nodig
</div>

<!--
Vier minuten.
"BiLSTM: twee LSTM's. Eén leest tijdreeks van begin naar eind, één omgekeerd."

Pauze: "Wat lost dit op?" — Antwoord: toekomst-context.
Bij offline batch-analyse heb je de hele reeks. BiLSTM gebruikt zowel verleden als toekomst.

Pauze 5 sec: "Wat is de catch?"
Antwoord: nooit online — je kunt geen alarm geven op iets wat over 50 samples gebeurt.

Bevestig. Schrijf op flip-over: 'BiLSTM: geheugen + toekomst — alleen offline'.
-->

---

# Drie varianten — één keuzecriterium

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-amber-50 rounded-lg">

### RNN
- Kort geheugen
- Lichte modellen
- Korte sequenties
- Online of offline

</div>

<div class="p-4 bg-green-50 rounded-lg">

### LSTM
- Lang geheugen
- Drie gates
- Realtime PdM
- Online of offline

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### BiLSTM
- Geheugen + toekomst
- Hoogste accuracy
- Offline batch / RUL
- **Alleen offline**

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  De vraag: heb je geheugen nodig? Heb je de toekomst beschikbaar?
</div>

<!--
Anderhalve minuut.
Brug naar fase 2.

"Drie varianten. Eén keuzecriterium: heb je geheugen nodig? Heb je toekomst beschikbaar?
Of is je context kort? Op basis daarvan kies je."

"Dat gaan jullie nu zelf doen."
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
  Sensorsignaal over tijd → RNN unrolled met geheugen-puls →<br/>
  LSTM-gates als sluizen → BiLSTM bidirectioneel → pomp-anomalie.
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion · <code>RnnLstmVideo</code>)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
Optionele inzet — aan einde van fase 1 (theoretiseren).
Tijds-animatie maakt het geheugen-mechanisme tastbaar.
Scene 4 (LSTM-gates als sluizen) is dé visuele anker voor 'wat onthouden, wat vergeten, wat doorgeven'.
-->

---

# Drie scenario's

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-amber-50 rounded-lg border-2 border-amber-200">

### A · Online vibration
- Actieve machine
- 50 samples context
- Alarm binnen seconden

<div class="mt-3 text-xs opacity-60">Welke variant?</div>

</div>

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### B · Offline batch RUL
- 24 uur opgenomen
- RUL-schatting achteraf
- Accuracy belangrijk

<div class="mt-3 text-xs opacity-60">Welke variant?</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg border-2 border-purple-200">

### C · Korte signaalclassificatie
- 20-sample window
- Geen lange context
- Snel oordeel

<div class="mt-3 text-xs opacity-60">Welke variant?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-02
</div>

<!--
IK DOE eerst — scenario A:
"Online vibration, 50 samples, alarm binnen seconden.
- Online → BiLSTM valt af.
- 50 samples → niet kort, niet super lang.
- Long-term dependency kan optreden.
- Vanilla RNN risicovol.
- Mijn keuze: LSTM."

Daarna: "Doe B en C zelf. Zes minuten."
Loop rond. Stel verdiepende vragen.
-->

---
layout: center
class: text-center
---

# Stem mee

<div class="grid grid-cols-3 gap-6 mt-10 text-base">
  <div class="p-4 bg-amber-50 rounded-lg">
    <div class="font-bold text-amber-700">A · Online vibration</div>
    <div class="mt-2 text-xs">RNN / LSTM / BiLSTM?</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-700">B · Offline RUL</div>
    <div class="mt-2 text-xs">RNN / LSTM / BiLSTM?</div>
  </div>
  <div class="p-4 bg-purple-50 rounded-lg">
    <div class="font-bold text-purple-700">C · Korte classificatie</div>
    <div class="mt-2 text-xs">RNN / LSTM / BiLSTM?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Drie stemrondes per scenario.
</div>

<!--
Eerst tweetallen vergelijken (5 min).
Daarna plenair stemmen — schrijf uitslag op flip-over.

Tel innerlijk tot 7. Veroordeel geen antwoord.
-->

---

# Het antwoord

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-amber-50 rounded-lg">

### A · LSTM
- Online → geen toekomst
- Middellange context
- Long-term dependency speelt
- Vanilla RNN is risico

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### B · BiLSTM
- Offline → toekomst beschikbaar
- Lange sequentie
- Accuracy belangrijk
- Kerncase voor BiLSTM

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### C · Vanilla RNN
- 20 samples → kort
- Long-term dependency speelt nauwelijks
- LSTM mag, vaak overkill

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  In PdM-onderzoek (Li 2026) is BiLSTM precies daarom de keuze<br/>
  voor RUL-prognose op vibration-data.
</div>

<!--
A is meestal LSTM — bevestigen.
C is vaak vanilla RNN — kort uitleggen waarom LSTM overkill is.
B is de kerncase — daar zit het inzicht: offline + accuracy = BiLSTM.

"In PdM-onderzoek (Li 2026) is BiLSTM kern-keuze voor RUL-prognose."

Bij vragen over autoencoder of Isolation Forest: parkeer.
Verwijs naar lo-smart-mfg-092 (autoencoder) en lo-smart-mfg-107 (Isolation Forest) voor self-study.
-->

---
layout: section
---

# Experimenteren

## Welke variant past bij jouw tijdreeks?

<!--
Overgang naar blok 4.
"Laatste 10 minuten — eigen tijdreeks-scan."
-->

---

# Eigen tijdreeks-scan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier velden in te vullen
<v-clicks>

- Welke **meting** — vibration, temperatuur, druk?
- **Online** of offline?
- Hoe lang **context-venster**?
- Welke **variant** past?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Realtime alarm of achteraf?
- Aantal samples per beslissing?
- Spelen trends die zich opbouwen?
- Weet ik niet → vraag voor IT

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-04
</div>

<!--
Inventarisatie-vraag (1 min): "Bij wie speelt vibration, temperatuur, druk, akoestiek, stroom?"
Vang 4-5 antwoorden, niet bespreken.

Zet timer op 6 min.
Help één concrete trio: meting / venster / online-of-offline.
'Weet ik niet' is óók waardevol — dat is de eerste vraag aan IT.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bevraag IT of leverancier
<v-clicks>

- Hoe lang is het context-venster?
- Online of offline analyse?
- Welke modelfamilie — RNN, LSTM, BiLSTM?
- Noteer en koppel aan vergelijkingstabel

</v-clicks>

</div>

<div>

### Verdieping (optioneel)
<v-clicks>

- Olah (2015): Understanding LSTM Networks
- Visuele uitleg, sterk aanbevolen
- 15 minuten lezen
- Maakt de drie gates concreet

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat zegt IT?
</div>

<!--
Sluit af met de transferopdracht.
"Volgende sessie kort delen.
Daarna door naar volgende paradigma-LO over ensembles."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Ensemble learning — meerdere modellen samen</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Stemming per scenario
- Welke transfer-acties?
- Welke vragen op parkeerlijst?
-->
