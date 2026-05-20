---
theme: default
title: Van anomaliescore naar onderhoud — het verkeerslichtmodel
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over het vertalen van anomaliescores naar onderhoudsacties met
  het verkeerslichtmodel (groen/geel/oranje/rood) en het maken van een
  complete werkorder. Doelgroep: operators MBO-3, 30 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Van score naar onderhoud

### Het verkeerslichtmodel — wanneer grijp je in?

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 30 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · CNC / spuitgieten / draaibank
</div>

<!--
Welkom. Vorige sessies: sensordata lezen (LO-201) en drempelwaarden (LO-202).
Vandaag de laatste stap: wat doe je met die scores?

Trigger: "Wie heeft op zijn werkvloer wel eens een hoge score gezien op het dashboard?"
Vang 1-2 reacties. Geen oordeel. Doorpakken naar quiz.
-->

---
layout: section
---

# Ervaren

## Storingsquiz: 4 dashboardscenario's

<!--
Overgang naar blok 1.
"Per scenario: kies een kleur. Schrijf actie + termijn + waarom.
Geen kapstok nu — gebruik je gevoel."
-->

---
layout: center
class: text-center
---

# 4 dashboards — kies de kleur

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Per scenario:<br/>
  <span class="font-bold">welke kleur?</span><br/>
  <span class="font-bold">welke actie?</span><br/>
  <span class="font-bold">welke termijn?</span>
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Geen kapstok nu.<br/>
  Gebruik je gevoel en je kennis uit LO-201 en LO-202.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5.5 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01. Timer op 5 min 30.
Loop rustig rond. Niet voorzeggen.

Bij vastlopen: "Wat zou je doen als dit JOUW machine was?"
Bij snelle MBO-4: "Wat zou je willen weten dat NIET in dit dashboard staat?"

Verkeerslichtmodel-flap-over BLIJFT BEDEKT in deze fase.
-->

---
layout: section
---

# Reflecteren

## Vergelijk je keuzes met je buurman

<!--
Overgang naar blok 2. "Pak een buurman. Drie vragen op het werkblad."
-->

---
layout: center
class: text-center
---

# Bespreek in duo's

<div class="grid grid-cols-3 gap-6 mt-10">
  <div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-4xl mb-3">🎨</div>
    <div class="text-lg font-bold text-blue-700">Waar kozen jullie verschillend?</div>
  </div>
  <div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-4xl mb-3">⚖️</div>
    <div class="text-lg font-bold text-purple-700">Wanneer score, wanneer gevoel?</div>
  </div>
  <div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-4xl mb-3">🤔</div>
    <div class="text-lg font-bold text-green-700">Bij welk scenario twijfelde je?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Wat zou helpen om met meer zekerheid te kiezen?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min duo · 2.5 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Timer op 4 min.
Loop rond. Verzamel 2-3 sterke voorbeelden.

Plenair (2.5 min):
- "Bij welk scenario verschilden jullie het meest?"
- "Wanneer vertrouw je de score, wanneer je gevoel?"
- "Wat zou helpen?" — mik op antwoord: een kapstok / kader.

Aan eind: ONTHUL de verkeerslichtmodel-flap-over.
"Die kapstok krijgen we nu."
-->

---
layout: section
---

# Theoretiseren

## Verkeerslichtmodel + werkorder

<!--
Overgang naar blok 3. 5 minuten — strak.
"Dit is wat jullie in fase 1 gevoelsmatig al deden — nu met getallen."
-->

---

# Het verkeerslichtmodel

<div class="grid grid-cols-4 gap-4 mt-8">

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-300 text-center">
  <div class="text-4xl mb-2">🟢</div>
  <div class="text-lg font-bold text-green-700">0 - 30</div>
  <div class="text-sm opacity-80 mt-2">Geen actie</div>
  <div class="text-xs opacity-60 mt-1">—</div>
</div>

<div class="p-5 bg-yellow-50 rounded-xl border-2 border-yellow-300 text-center">
  <div class="text-4xl mb-2">🟡</div>
  <div class="text-lg font-bold text-yellow-700">30 - 50</div>
  <div class="text-sm opacity-80 mt-2">Verhoogde monitoring</div>
  <div class="text-xs opacity-60 mt-1">Dagelijks checken</div>
</div>

<div class="p-5 bg-orange-50 rounded-xl border-2 border-orange-300 text-center">
  <div class="text-4xl mb-2">🟠</div>
  <div class="text-lg font-bold text-orange-700">50 - 70</div>
  <div class="text-sm opacity-80 mt-2">Plan onderhoud</div>
  <div class="text-xs opacity-60 mt-1">Binnen 2 weken</div>
</div>

<div class="p-5 bg-red-50 rounded-xl border-2 border-red-300 text-center">
  <div class="text-4xl mb-2">🔴</div>
  <div class="text-lg font-bold text-red-700">70 +</div>
  <div class="text-sm opacity-80 mt-2">Plan inspectie</div>
  <div class="text-xs opacity-60 mt-1">Binnen 48 uur</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Vier kleuren = vier acties. Niet ingewikkelder.
</div>

<!--
Loop de vier kleuren één voor één langs.
Wijs naar de flap-over.
"Score 45 in fase 1 — wat koos je? Geel? Klopt."

Bij vraag over grenzen-precisie (49 vs 51):
"Richtgrenzen, geen wetten. Trend telt mee."
-->

---

# Eén sensor of meerdere?

<div class="grid grid-cols-3 gap-4 mt-8">

<div class="p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-3xl mb-2">📍</div>
  <div class="text-base font-bold text-blue-700 mb-2">Eén sensor hoog</div>
  <div class="text-sm opacity-80">Lokaal probleem of sensorstoring.<br/>Check die ene component.</div>
</div>

<div class="p-5 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-3xl mb-2">🌐</div>
  <div class="text-base font-bold text-purple-700 mb-2">Meerdere matig verhoogd</div>
  <div class="text-sm opacity-80">Systeembreed probleem.<br/>Check koeling, smering, voeding.</div>
</div>

<div class="p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-3xl mb-2">🔗</div>
  <div class="text-base font-bold text-amber-700 mb-2">Hoog + laag samen</div>
  <div class="text-sm opacity-80">Combinatie. Bijv. temperatuur hoog + koeldruk laag = koelprobleem.</div>
</div>

</div>

<!--
Drie vuistregels. Concreet voorbeeld bij elke regel.

"Twee sensoren temperatuur hoog + koelmiddeldruk laag = koelprobleem."
-->

---

# Werkorder in 5 stappen

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="space-y-3">

<div class="p-3 bg-blue-50 rounded-lg">
  <span class="font-bold text-blue-700">1. Welke machine</span><br/>
  <span class="text-sm opacity-80">Specifiek — niet 'machine 2' maar 'CNC-2 in cel B'.</span>
</div>

<div class="p-3 bg-purple-50 rounded-lg">
  <span class="font-bold text-purple-700">2. Welke sensoren</span><br/>
  <span class="text-sm opacity-80">Wat wees de SHAP-analyse aan? (LO-108)</span>
</div>

<div class="p-3 bg-amber-50 rounded-lg">
  <span class="font-bold text-amber-700">3. Urgentie</span><br/>
  <span class="text-sm opacity-80">Welke kleurzone uit het verkeerslicht?</span>
</div>

</div>

<div class="space-y-3">

<div class="p-3 bg-green-50 rounded-lg">
  <span class="font-bold text-green-700">4. Voorgestelde actie</span><br/>
  <span class="text-sm opacity-80">Inspectie · preventief onderhoud · vervanging</span>
</div>

<div class="p-3 bg-red-50 rounded-lg">
  <span class="font-bold text-red-700">5. Deadline</span><br/>
  <span class="text-sm opacity-80">Uit het verkeerslichtmodel.</span>
</div>

<div v-click class="p-4 bg-slate-50 rounded-lg mt-2">

### Voorbeeld Marjan
Machine 2 · hydraulisch systeem · oranje · inspectie · binnen 2 weken · SHAP-grafiek als bijlage.

</div>

</div>

</div>

<!--
Loop de 5 stappen langs.
Voorbeeld Marjan kort: machine 2, oranje, hydrauliekslang.

Marjan-volledig: 2 dagen later score 73 — rood, deadline naar 48 uur.
Technicus vond lekkende hydrauliekslang. 30 min reparatie.
Zonder framework had ze moeten gokken.
-->

---
layout: quote
---

# Score = advies, geen bevel

<div class="text-xl mt-6 opacity-80">
  Jij kent je machine.
</div>

<div v-click class="mt-8 text-base opacity-70">
  Als score zegt <span class="font-bold">45</span> maar jij hoort iets raars,<br/>
  plan dan toch een inspectie.
</div>

<div v-click class="mt-8 text-sm opacity-60">
  AI ondersteunt jouw vakkennis — het vervangt het niet.
</div>

<!--
Belangrijk moment. Maak expliciet:
- Score is advies
- Operator vergelijkt met machine
- Bij conflict: operator wint

Wijs naar tweede flap-over: SCORE = ADVIES, GEEN BEVEL.

Voorkomt blind vertrouwen + voorkomt afwijzing van het systeem.
-->

---
layout: section
---

# Experimenteren

## Schrijf je eigen werkorder

<!--
Overgang naar blok 4. 10 min. Coachen, niet voorzeggen.
-->

---

# Jouw werkorder

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Kies en bedenk
<v-clicks>

- Eén machine waar je vaak op werkt
- Bedenk een scenario
- Welke sensoren wijken af?
- Welke kleur op het dashboard?

</v-clicks>

</div>

<div>

### Schrijf de 5 stappen
<v-clicks>

- Machine · sensoren
- Urgentie · actie · deadline
- Schrijf alsof de technicus niets weet
- Hij leest het — moet hij het snappen?

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-amber-50 rounded-lg text-center">

### Anker
De technicus die jouw werkorder leest, weet niet wat jij weet. Schrijf alsof hij niets weet.

</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min individueel · 2 min plenair · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Timer op 6 min.
Coach-modus: niet voorzeggen.

"Welke machine? Wees specifiek."
"Welke sensoren? Hoe weet je dat?"
"Welke kleurzone? Klopt met je drempelwaarden uit LO-202?"

Bij vage werkorder ('kijken'): "Wat moet de technicus DOEN?"

Plenair (2 min): vraag 2 deelnemers werkorder voor te lezen.
-->

---

# Deze week — jouw transferopdracht

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Morgen
<v-clicks>

- Check het dashboard van **jouw** machine
- Bepaal de kleurzone
- Beslis of actie nodig is

</v-clicks>

</div>

<div>

### Deze week — 1 week lang
<v-clicks>

- Elke ochtend: dashboard checken
- Kleur bepalen, actie noteren
- Bespreek met teamleider in werkoverleg
- Drie observaties in groepsapp

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-4 bg-blue-50 rounded-lg text-center">

### En vraag een collega
Lees jouw werkorder van vandaag. Klopt het? Snapt hij het zonder uitleg?

</div>

<!--
Loop rond, check dat het ingevuld is.
LO-205 is het sluitstuk van module 2.

Bij geen toegang dashboard: alternatief = dagelijks de drie kritische sensoren
uit LO-201/202 checken. Verkeerslichtmodel werkt op drempel-overschrijdingen.

Volgende module 3: eigen PdM-business case.
-->

---
layout: end
---

# Module 2 afgerond

<div class="mt-8 text-base opacity-70">
  Volgende module: <span class="font-bold">PdM op maat — jouw eigen business case (Module 3)</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie voor jezelf:
- Welke werkorders gemaakt? (input voor module 3)
- Wie schreef sterke werkorder? Kandidaat voor module 3 case-presentatie.
- Wie was sceptisch? (1-op-1 in module 3)
- Bron: Sesana et al. (2024). Artificial Intelligence in Manufacturing, pp. 474-475.
-->
