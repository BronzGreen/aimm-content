---
theme: default
title: CNN — hoe een neuraal netwerk patronen leert herkennen
info: |
  ## AI Fundamentals — Module 2 (Train)
  Workshop-blok over CNN-architectuur: vier lagen, vier datavoorbeelden, eigen lijn-actieplan.
  Doelgroep: operators/teamleiders MBO-4, 50 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# CNN

### Hoe een neuraal netwerk patronen leert herkennen

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 2 (Train) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · vision-AI · vibration-PdM
</div>

<!--
Welkom. De komende 50 minuten kijken we onder de motorkap van een CNN.
De magie van vision-AI en trillingsanalyse.

Tegen het eind kun je per laag uitleggen wat hij doet, en kun je vier datavoorbeelden beoordelen op of CNN past.

Niet de wiskunde — wel het idee.
-->

---
layout: center
class: text-center
---

# Het werkt — maar wat doet het?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Vision-AI op je lijn.<br/>
  Trillingsanalyse op je lager.
</div>

<div v-click class="text-xl mt-8 opacity-70">
  Rood / groen / klasse-label.
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  En achter dat label?
</div>

<!--
Vraag: "Wie heeft op zijn lijn een vision-AI of trillingsanalyse-systeem zien werken?"
Vang 2-3 reacties. Vraag door: "Weet je hoe het werkt?"
Bevestig: "Precies — die magie gaan we vandaag opentrekken."
-->

---

# Vier lagen — één architectuur

<div class="grid grid-cols-5 gap-3 mt-10 text-center text-sm">

<div class="p-4 bg-gray-100 rounded-lg">
  <div class="text-3xl mb-2">📥</div>
  <div class="font-bold">Input</div>
  <div class="opacity-60 text-xs mt-1">Pixels of samples</div>
</div>

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">
  <div class="text-3xl mb-2">🔍</div>
  <div class="font-bold text-blue-700">Convolutie</div>
  <div class="opacity-60 text-xs mt-1">Patronen zoeken</div>
</div>

<div class="p-4 bg-purple-50 rounded-lg border-2 border-purple-200">
  <div class="text-3xl mb-2">🗜️</div>
  <div class="font-bold text-purple-700">Pooling</div>
  <div class="opacity-60 text-xs mt-1">Comprimeren</div>
</div>

<div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">
  <div class="text-3xl mb-2">🧠</div>
  <div class="font-bold text-green-700">Fully connected</div>
  <div class="opacity-60 text-xs mt-1">Eindoordeel</div>
</div>

<div class="p-4 bg-amber-100 rounded-lg">
  <div class="text-3xl mb-2">📤</div>
  <div class="font-bold">Output</div>
  <div class="opacity-60 text-xs mt-1">Klasse / score</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70 italic">
  Vier lagen. Elk doet één ding. Samen herkennen ze patronen.
</div>

<!--
Wijs op A3-diagram in zaal en op scherm.
Loop top-down af: input → conv → pool → fc → output.

"Vier lagen. Elk doet één ding. Samen herkennen ze patronen in beeld of tijdreeks."

Deel daarna wb-01 uit:
"Tijdens de vier lagen vul je dit lege architectuurdiagram in. Per laag: wat doet hij? Wat zou hij 'zien'?"
-->

---
layout: center
class: text-center
---

# Laag 1 · Input

<div class="text-xl mt-10 max-w-xl mx-auto opacity-80">
  Niets bijzonders.
</div>

<div v-click class="mt-6 text-lg opacity-70">
  Bij beeld → pixels (RGB)<br/>
  Bij tijdreeks → meetwaarden over tijd
</div>

<div v-click class="mt-8 text-base opacity-50">
  Geen patronen — alleen getallen.
</div>

<!--
Anderhalve minuut.
Niet uitweiden — input is geen werkpaard.

Brug naar laag 2: "Daar wordt het interessant."
-->

---
layout: two-cols-header
---

# Laag 2 · Convolutielaag

::left::

### De speurder met een vergrootglas

<v-clicks>

- Kernel = klein venster (bv. 3×3)
- Schuift over de hele input
- Vraagt op elke plek: zit hier een patroon?
- Resultaat: feature map

</v-clicks>

::right::

### Twee kernconcepten

<v-clicks>

- **Lokale connectiviteit**<br/>kijkt alleen naar lokaal venster
- **Shared weights**<br/>zelfde kernel werkt overal

</v-clicks>

<div v-click class="mt-6 p-3 bg-blue-50 rounded-lg text-sm">
  Dezelfde randdetector werkt linksboven en rechtsonder.
</div>

<!--
Pak het vergrootglas op. Beweeg het over een denkbeeldige foto.
Spreek hardop: "krasje hier — krasje daar — randje — randje."

Vier minuten. De kern van fase 1.

"Twee kernconcepten — schrijf ze op je werkblad:
- Lokale connectiviteit
- Shared weights"

Schrijf op flip-over.
-->

---
layout: center
class: text-center
---

# Laag 3 · Pooling

<div class="text-xl mt-8 opacity-80">
  Comprimeren · robuust maken
</div>

<div class="mt-10 grid grid-cols-2 gap-8 max-w-2xl mx-auto">

<div class="p-4 bg-gray-100 rounded-lg">

### Voor pooling
4×4 feature map<br/>
detail per pixel

</div>

<div class="p-4 bg-purple-100 rounded-lg">

### Na pooling
2×2 feature map<br/>
samengevat per blokje

</div>

</div>

<div v-click class="mt-10 text-base opacity-70 italic">
  Krasje een halve millimeter naar links?<br/>
  Dezelfde feature.
</div>

<!--
Tweeënhalve minuut.
Onderscheid scherp: convolutie ZOEKT, pooling COMPRIMEERT.
Eén zoekt, één vat samen. Twee verschillende werkstappen.

Schrijf op flip-over: 'conv = zoeken, pool = comprimeren'.
-->

---
layout: center
class: text-center
---

# Laag 4 · Fully connected + output

<div class="text-xl mt-8 opacity-80">
  Het eindoordeel
</div>

<div v-click class="mt-8 max-w-xl mx-auto text-base">
  Geen lokaal venster meer.<br/>
  Élk neuron kijkt naar álle features.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-4 text-sm">
  <div class="p-3 bg-green-50 rounded-lg">
    <div class="font-bold">Kras</div>
    <div class="opacity-60">88%</div>
  </div>
  <div class="p-3 bg-red-50 rounded-lg">
    <div class="font-bold">Geen kras</div>
    <div class="opacity-60">10%</div>
  </div>
  <div class="p-3 bg-yellow-50 rounded-lg">
    <div class="font-bold">Onzeker</div>
    <div class="opacity-60">2%</div>
  </div>
</div>

<!--
Drie minuten.
Klassiek vraag: waarom heet die laag 'fully connected'?
Antwoord: élk neuron kijkt naar álle features uit de vorige laag.

"Hier wordt de uiteindelijke beslissing gemaakt: kras of geen kras, klasse A of B, RUL is 30 cycli."

Output = probabiliteit per klasse of numerieke voorspelling.
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
  Het kernel-vergrootglas glijdt over een lasergravure-beeld.<br/>
  De feature map vult zich live.
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
Optionele inzet — alleen als je in tempo zit (fase 1 in 14 min i.p.v. 17).
Toon de 90s video na laag 4. Geen bespreking achteraf — laat het bezinken.

Voor wie het visueel wil zien: scene 2 (25s) laat letterlijk zien hoe de
3x3 kernel over het beeld glijdt en per stap de feature-map vult.
Scene 5 (20s) brengt de 4 datavoorbeelden uit fase 2 al even in beeld.
-->

---
layout: center
class: text-center
---

# Wanneer past CNN?

<div class="grid grid-cols-2 gap-8 mt-10 max-w-3xl mx-auto">

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">

### Past sterk
- Beelddata (vision)
- 1D-tijdreeksen (vibration, akoestiek)
- Lokale ruimtelijke / volgordelijke structuur

</div>

<div class="p-6 bg-red-50 rounded-xl border-2 border-red-200">

### Past niet
- Tabular data (ERP, klantprofielen)
- Geen lokale structuur
- Volgorde willekeurig

</div>

</div>

<div v-click class="mt-10 text-base opacity-70 italic">
  Voor tabular: random forest of boosting (zie volgende LO).
</div>

<!--
Brug naar fase 2.
"Vier lagen samen. Werkt fantastisch op data met lokale structuur. Werkt slecht op data zonder."
"Dat gaan jullie nu zelf beoordelen."

Slide 9 - vier voorbeelden.
-->

---

# Vier voorbeelden

<div class="grid grid-cols-2 gap-4 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### A · Lasergravure-beeld
- Metalen plaat
- Krassen detecteren
- 2D-beeld, RGB

<div class="mt-3 text-xs opacity-60">CNN ja / nee?</div>

</div>

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### B · Oppervlaktefoto
- Gespoten plaat
- Vlekken, krimpscheuren
- 2D-beeld

<div class="mt-3 text-xs opacity-60">CNN ja / nee?</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg border-2 border-purple-200">

### C · Vibration-signaal
- Lager-trilling
- 200 samples
- 1D-tijdreeks

<div class="mt-3 text-xs opacity-60">CNN ja / nee?</div>

</div>

<div class="p-4 bg-amber-50 rounded-lg border-2 border-amber-200">

### D · ERP-tabel
- Onderdeelnummer
- Leverdatum
- Tabulair

<div class="mt-3 text-xs opacity-60">CNN ja / nee?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-02 <span class="opacity-60">of tablet · model-cnn-past-hier</span>
</div>

<!--
IK DOE eerst — voorbeeld A:
"Lasergravure-beeld, krassen detecteren. Een kras is een lokaal patroon — een streepje, ergens.
Het kernel uit de convolutielaag is precies daarvoor gemaakt. Shared weights helpen: dezelfde kras-detector werkt overal.
CNN past sterk. Doorslaggevend: lokale ruimtelijke structuur."

Daarna: "Pak je werkblad. Doe B, C en D zelf. Zes minuten."
Loop rond. Stel verdiepende vragen.
-->

---
layout: center
class: text-center
---

# Stem mee

<div class="grid grid-cols-4 gap-4 mt-10 text-base">
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-700">A · Beeld</div>
    <div class="mt-2 text-sm">CNN?</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="font-bold text-blue-700">B · Foto</div>
    <div class="mt-2 text-sm">CNN?</div>
  </div>
  <div class="p-4 bg-purple-50 rounded-lg">
    <div class="font-bold text-purple-700">C · Vibration</div>
    <div class="mt-2 text-sm">CNN?</div>
  </div>
  <div class="p-4 bg-amber-50 rounded-lg">
    <div class="font-bold text-amber-700">D · ERP</div>
    <div class="mt-2 text-sm">CNN?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Hand omhoog per voorbeeld — tellen we plenair.
</div>

<!--
Eerst tweetallen (5 min).
Daarna plenair stemmen — schrijf uitslag op flip-over.

Tel innerlijk tot 7. Veroordeel geen antwoord.
-->

---

# Het antwoord

<div class="grid grid-cols-4 gap-3 mt-6 text-xs">

<div class="p-3 bg-blue-50 rounded-lg">

### A · CNN past sterk
- Krassen = lokaal patroon
- Shared weights helpen
- Ruimtelijke structuur

</div>

<div class="p-3 bg-blue-50 rounded-lg">

### B · CNN past
- Vlekken = lokale textuur
- 2D-ordening
- Past sterk

</div>

<div class="p-3 bg-purple-50 rounded-lg">

### C · CNN past (1D)
- Frequentiebanden
- Volgordelijk in tijd
- 1D-CNN bestaat

</div>

<div class="p-3 bg-red-50 rounded-lg">

### D · CNN past niet
- Geen lokale structuur
- Kolommen verwisselbaar
- Beter: random forest

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  De truc: zit er lokale structuur in mijn data?<br/>
  Zo nee → kies iets anders.
</div>

<!--
A en B unaniem — kort bevestigen.
C is de nuance: 1D-CNN bestaat. Vibration past wél.
D is het contrast — kerncase.

"Verwissel de kolommen — verandert er iets? Nee. Geen ruimtelijke of volgordelijke structuur. Voor tabular: random forest of gradient boosting."

Verwijs kort naar volgende LO over ensembles.
-->

---
layout: section
---

# Experimenteren

## Waar past CNN op jouw lijn?

<!--
Overgang naar blok 4.
"Laatste 11 minuten — eigen lijn-scan.
Welke plek waar visuele inspectie of trillingsmeting plaatsvindt?"
-->

---

# Eigen lijn-scan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier velden in te vullen
<v-clicks>

- Welk type **data** — beeld of tijdreeks?
- Welk **patroon** herken je nu zelf?
- Op welke **plek** zit het — overal of specifiek?
- Welke **laag** doet het werk?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Kras / vlek / kleur / vorm?
- Trilling met patroon, of constant?
- Convolutie = lokaal zoeken
- Pooling = robuust maken
- FC = eindoordeel

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6,5 min · individueel · wb-04
</div>

<!--
Eerst inventarisatie-vraag (1 min): "Bij wie speelt vision of vibration — CNC, spuitgieten, verpakking, lakken?"
Vang 4-5 antwoorden, niet bespreken.

Zet timer op 6 min 30.
Help één concrete koppeling: patroon ↔ laag.
Hypothetisch mag — als het maar concreet is.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bevraag de leverancier
<v-clicks>

- Gebruikt het systeem een CNN?
- Wat is de input — beeld of tijdreeks?
- Welk type defect herkent het — en welk niet?
- Noteer en koppel aan de architectuur

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Zoek op YouTube:<br/>"CNN feature map visualization"
- Je ziet letterlijk wat de convolutielaag oppikt
- 60-90 seconden — maakt het tastbaar

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat zegt de leverancier?
</div>

<!--
Sluit af met de transferopdracht.
"Volgende sessie: kort delen — wat zegt de leverancier of IT?
Daarna door naar de volgende paradigma-LO over RNN/LSTM."

Bonus tip alleen noemen als er tijd over is.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">RNN, LSTM en BiLSTM — neurale netwerken met geheugen</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Stemming per voorbeeld (verdeling = indicatie groepsbegrip)
- Welke transfer-acties? (input voor volgende sessie)
- Welke vragen op parkeerlijst? (verdiepingsmateriaal)
-->
