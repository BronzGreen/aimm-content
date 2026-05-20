---
theme: default
title: AI als aanvulling op SPC — wanneer klassieke regels tekortschieten
info: |
  ## SPC Module 3 — Op Maat
  Workshop-blok over wanneer welke aanpak past — klassieke SPC of AI — en waarom XAI voorwaarde is.
  Doelgroep: teamleider HBO + teamleider MBO-4, 25 minuten, ontwerp-oefening.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# AI als aanvulling op SPC

### Wanneer klassieke regels tekortschieten

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Workshop-blok · 25 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Teamleiders HBO + MBO-4 · ontwerp-oefening eigen lijn
</div>

<!--
Open warm.
"Wie van jullie heeft al een AI-systeem op zijn lijn? Welke vraag beantwoordt het?"

Wacht. Als iemand opsteekt: "Even kort — welke vraag?" Vang max 90 sec, schrijf op flip-over rechts.
Als niemand opsteekt: "Goed — dan is dit blok geen evaluatie, maar een ontwerp-oefening."

In de komende 25 minuten ontwerpen we voor jouw lijn de combinatie van klassieke SPC en AI.
We leren niet rekenen met SHAP. We leren wanneer welke aanpak past — en waarom XAI voorwaarde is.

Verwijs naar draaiboek blok 1, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Vandaag leer je

<v-clicks>

- Welke **vraag** klassieke SPC beantwoordt
- Welke **vraag** AI beantwoordt
- Wanneer klassiek **tekortschiet** (4 redenen)
- Waarom **XAI voorwaarde** is, geen luxe
- Hoe je **jouw eigen lijn** screent

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-7xl mb-4">🤖</div>
    <div class="text-xl font-mono font-bold text-amber-600">AI ≠ vervanger</div>
    <div class="text-sm opacity-60 mt-2">AI = aanvulling — mits XAI</div>
  </div>
</div>

<!--
Korte trigger (45 sec).
"In 25 minuten ontwerpen we voor jouw lijn. Geen wiskunde — wel scherpe vragen.
Aan het eind heb je één eigen lijn-screen ingevuld met procesvraag, aanpak-categorie en XAI-eis."

HBO-doelgroep wil weten waar het naartoe gaat. Toon het einddoel.

Verwijs naar draaiboek blok 1, instructie 2.
-->

---
layout: section
---

# Theoretiseren

## Welke vraag beantwoordt jouw SPC nu?

<!--
Overgang naar de centrale onderscheid-slide.
"Voordat we naar AI kijken: welke vraag beantwoordt jouw huidige SPC nu wél?
En welke vraag KAN het niet beantwoorden — maar zou je wel willen?"

Dit is je vangrail bij elke discussie vandaag. Verwijs er voortdurend naar.

Verwijs naar draaiboek blok 1, instructie 3.
-->

---
layout: two-cols-header
---

# Het centrale onderscheid

::left::

### 📊 Klassieke SPC vraagt:
<div class="mt-4 p-5 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-xl font-bold text-blue-900 leading-snug">
    "Is het proces NU<br/>anders dan normaal?"
  </div>
  <div class="text-sm opacity-70 mt-3">
    Shewhart · Nelson-rules<br/>
    Univariate · vaste limieten
  </div>
</div>

::right::

### 🤖 AI vraagt:
<div class="mt-4 p-5 bg-amber-50 rounded-xl border-2 border-amber-200">
  <div class="text-xl font-bold text-amber-900 leading-snug">
    "Welk PATROON leidt<br/>naar verstoring?"
  </div>
  <div class="text-sm opacity-70 mt-3">
    Predictive monitoring<br/>
    Multivariate · adaptief
  </div>
</div>

<div v-click class="mt-8 text-center text-base p-3 bg-purple-50 text-purple-900 rounded-lg max-w-2xl mx-auto">
  En XAI vraagt: <span class="font-bold">"Welke SIGNALEN dragen het meest bij?"</span> — SHAP, LIME
</div>

<!--
KERNSLIDE — niet doorhaasten.

"Drie verschillende vragen. Geen vervangt de andere."
Stilte van 3 sec.

Belangrijk en expliciet:
"Nelson-rules zijn NIET verouderd. Ze beantwoorden een ándere vraag dan AI."

Wijs naar de twee koppen op de flip-over (zelfde tekst).

Verwijs naar draaiboek blok 1, instructie 3 + valkuil vk-02 (Nelson afschaffen).
-->

---

# Wanneer schiet klassiek tekort?

<div class="grid grid-cols-2 gap-4 mt-4">

<div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
  <div class="font-bold text-amber-900">1. Hoge dimensionaliteit</div>
  <div class="text-sm opacity-80 mt-1">10 sensoren tegelijk — Shewhart kijkt per stuk; mist multivariate samenhang.</div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
  <div class="font-bold text-amber-900">2. Niet-lineaire interacties</div>
  <div class="text-sm opacity-80 mt-1">Druk × temperatuur × debiet — patronen die geen lineair model vangt.</div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
  <div class="font-bold text-amber-900">3. Autocorrelatie</div>
  <div class="text-sm opacity-80 mt-1">Opvolgende metingen niet onafhankelijk — Shewhart-aanname schendt.</div>
</div>

<div v-click class="p-4 bg-amber-50 rounded-lg border-l-4 border-amber-400">
  <div class="font-bold text-amber-900">4. Dynamische baseline</div>
  <div class="text-sm opacity-80 mt-1">Sensor-drift, materiaal-batch-variatie — vaste limieten lopen achter.</div>
</div>

</div>

<div v-click class="mt-6 text-center text-sm opacity-70">
  Vier aannames van klassieke SPC die in moderne lijnen zwakker zijn.
</div>

<!--
Klik per reden langs.
1. Hoge dimensionaliteit — anker voor voorbeeld 1 (chemische reactor).
2. Niet-lineaire interacties — wat klassieke SPC structureel niet ziet.
3. Autocorrelatie — opvolgende metingen niet onafhankelijk.
4. Dynamische baseline — anker voor voorbeeld 2 (drift).

NIET dieper op de wiskunde. Dit zijn de aannames; volgende slide laat zien wat AI toevoegt.

Verwijs naar draaiboek blok 1, instructie 5-6.
-->

---
layout: two-cols
layoutClass: gap-6
---

# Voorbeeld 1 — chemische reactor

Tien sensoren op een reactor.

<v-clicks>

- Alle individueel **binnen ±3σ**
- **Geen Nelson-regel** triggert
- Combinatie: T+1σ, P+0,5σ, Q-0,8σ
- In 78% van de gevallen vóór katalysator-degradatie

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-6xl mb-4">⚗️</div>
    <div class="text-base opacity-70 max-w-xs mx-auto">
      Klassieke SPC ziet niets.<br/>
      Multivariate AI ziet het patroon.
    </div>
  </div>
</div>

<!--
Dit is HET ankervoorbeeld uit het KO. Gebruik volledig.

"Tien sensoren op een chemische reactor. Alle individueel binnen ±3σ. Geen Nelson-regel triggert.
Maar de combinatie temperatuur +1σ, druk +0,5σ, debiet -0,8σ ging in 78% van de gevallen vooraf
aan katalysator-degradatie. Wie ziet wat hier de tekortkoming is van klassieke SPC?"

Wacht. Iemand zegt 'multivariaat' of 'samenhang'. Bevestig.

"Klassieke SPC beoordeelt elk signaal apart. Multivariate AI — kernel methods, autoencoders —
leert het collectieve patroon."

Verwijs naar draaiboek blok 1, instructie 5.
-->

---

# AI-toevoegingen

| Tekort klassieke SPC | AI-aanpak |
|----------------------|-----------|
| Multivariate samenhang | **Autoencoders, one-class classifiers** |
| Niet-lineaire interacties | **Kernel methods, deep learning** |
| Autocorrelatie | **Tijdreeksmodellen, RNN's** |
| Dynamische baseline | **Drift-aware modellen, online learning** |
| High-mix-low-volume | **Transfer learning over runs** |

<div v-click class="mt-6 text-center text-sm opacity-70 max-w-xl mx-auto">
  Concept-niveau — geen wiskunde vandaag.<br/>
  <span class="text-xs opacity-60">Verdieping: Technometrics review 2024 · Lundberg & Lee (2017)</span>
</div>

<!--
Loop snel langs.
"AI-aanpakken op concept-niveau. Vandaag geen wiskunde — alleen weten dat ze bestaan
en welk type vraag ze beantwoorden."

Voor data-savvy teamleider: noem kort kernel-methods en autoencoders.
Voor minder technische: focus op de tweede kolom = aanpak-categorieën.

NIET de Shapley-formule, NIET autoencoder-architectuur. Eén zin per term volstaat.

Verwijs naar draaiboek blok 1, instructie 6 + valkuil vk-05 (te diep op SHAP/LIME).
-->

---
layout: center
class: text-center
---

# ⚠️ Nelson-rules zijn NIET verouderd

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Klassieke SPC en AI beantwoorden <span class="font-bold">verschillende vragen</span>.<br/>
  Beide blijven relevant.
</div>

<div v-click class="mt-8 inline-block px-6 py-3 bg-red-100 text-red-900 rounded-lg font-bold">
  AI vervangt Nelson niet — AI vult aan waar Nelson niets ziet.
</div>

<div v-click class="mt-6 text-base opacity-80 max-w-lg mx-auto">
  10 sensoren binnen ±3σ — geen Nelson-regel triggert.<br/>
  <span class="text-sm opacity-70">Maar het collectieve patroon is wel relevant.</span>
</div>

<!--
WAARSCHUWINGSSLIDE — niet doorhaasten.

Dit is dé valkuil bij teamleiders: "AI doet het wel, dus weg met Nelson."
Het KO is hierover ondubbelzinnig: NIET verouderd.

Stilte. Tel innerlijk tot 5.

"Operators die de Nelson-routine kwijtraken, raken hun referentiekader kwijt.
AI vult aan, vervangt niet. Beide blijven."

Verwijs naar draaiboek blok 1, instructie 3 + valkuil vk-02.
-->

---
layout: center
class: text-center
---

# 🔍 XAI is voorwaarde — geen luxe

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Black-box-systemen <span class="font-bold">ondermijnen vertrouwen</span>.<br/>
  Zonder uitlegbaarheid: alarm fatigue of paniek.
</div>

<div v-click class="mt-8 grid grid-cols-2 gap-4 max-w-2xl mx-auto">
  <div class="p-4 bg-red-50 rounded-lg">
    <div class="font-bold text-red-900">Zonder XAI</div>
    <div class="text-sm opacity-80 mt-2">Operator negeert het alarm,<br/>óf stopt de lijn op vermoeden.</div>
  </div>
  <div class="p-4 bg-green-50 rounded-lg">
    <div class="font-bold text-green-900">Met SHAP</div>
    <div class="text-sm opacity-80 mt-2">"Druk 45%, T 30%, Q 25%" —<br/>operator weet wáár te kijken.</div>
  </div>
</div>

<div v-click class="mt-6 text-sm opacity-60 max-w-md mx-auto">
  SHAP · LIME · hybride interpretabele modellen
</div>

<!--
KERNZIN — herhaal expliciet:
"XAI is geen luxe, het is de voorwaarde voor operator-vertrouwen.
Zonder uitlegbaarheid ondermijn je je eigen investering."

Het reactor-voorbeeld:
"Operator krijgt SHAP-uitleg: druk hoofdcontributor 45%, temperatuur 30%, debiet 25%.
Operator begrijpt waarom, doet drukvalcheck, voorkomt 6-uur productiestop.
Dat is het verschil tussen een AI-investering die rendeert en een die in de la verdwijnt."

Verwijs naar draaiboek blok 1, instructie 7 + valkuil vk-03 (XAI overslaan).
-->

---

# Implicatie voor de operator-rol

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-5 bg-blue-50 rounded-xl">
  <div class="text-sm opacity-70 mb-2">Was:</div>
  <v-clicks>

  - **Detector** (zelf signalen scannen)
  - **Regelvolger** (Nelson-rules toepassen)

  </v-clicks>
</div>

<div class="p-5 bg-green-50 rounded-xl">
  <div class="text-sm opacity-70 mb-2">Wordt:</div>
  <v-clicks>

  - **Interpreteerder** (alarm beoordelen)
  - **Systeem-bewaker** (alarmen rationaliseren)

  </v-clicks>
</div>

</div>

<div v-click class="mt-6 text-center text-base p-3 bg-amber-50 text-amber-900 rounded-lg max-w-xl mx-auto">
  Data Literacy is <span class="font-bold">voorwaarde</span> — wie traint dat bij jou?
</div>

<!--
Korte slide — 30-45 sec.
"AI vervangt operators niet. Het verandert hun rol.
Data Literacy wordt voorwaarde — zonder dat geen zinvolle interpretatie."

Vraag plenair: "Wie traint dat bij jou — eigen lijn of via Module 1?"
Vang 1-2 reacties, niet uitdiepen — alleen aanstippen.

Verwijs naar draaiboek blok 3, instructie 4.
-->

---
layout: section
---

# Experimenteren

## Eén lijn die jij goed kent

<!--
Overgang naar blok 2.
"Nu is het kader klaar. Tijd om het op je eigen lijn los te laten — strenge realiteitscheck inclusief."

Deel wb-02-eigen-lijn-screen uit.
"Kies één lijn die jij goed kent. Niet de moeilijkste — de meest representatieve."

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Jouw eigen lijn-screen

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier secties
<v-clicks>

1. **Procesvraag** — wat wil je beantwoorden?
2. **Data-check** — historie + storingen + drift
3. **Aanpak-categorie** — klassiek / drift-aware / multivariaat / transfer
4. **XAI-eis** — hoe leg je het uit aan operators?

</v-clicks>

</div>

<div>

### Coaching-vragen
<v-clicks>

- Welke vraag beantwoordt je SPC nu wél?
- Hoeveel labelled historie inclusief storingen?
- Past univariaat of multivariaat?
- Wat doet je operator bij alarm zonder uitleg?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  4 min individueel + 3 min sparring · wb-02-eigen-lijn-screen
</div>

<!--
Zet timer op 4 min individueel + 3 min 30 sparring (totaal 9 min met inventarisatie + verzameling).

Inventarisatie-vraag (45 sec): "Even rondkijken: noem in één zin welke lijn je kiest."
Vang 4-6 voorbeelden. Niet bespreken — alleen verzamelen.

Loop rond. Stel vragen, geef GEEN antwoorden. HBO-doelgroep komt voor sparring.
Coach met:
- "Welke vraag beantwoordt je huidige SPC nu wél?"
- "Hoeveel maanden labelled historie inclusief storingen?"
- "Wat doet je operator als hij alarm krijgt zonder uitleg?"

Tussentijds belletje na 4 min voor sparring-fase.

Verwijs naar draaiboek blok 2, instructie 2-4 + valkuilen vk-04 (geen historie) en vk-06 (doceren ipv coachen).
-->

---
layout: center
class: text-center
---

# Transferopdracht — komende 2 weken

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Voer <span class="font-bold">één concrete actie</span> uit op je eigen lijn-screen.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-3xl mx-auto">
  <div class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900 mb-2">A · Data-check</div>
    <div class="text-xs opacity-70">Hoeveel labelled historie heb je echt? Hoeveel dekt storingen?</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900 mb-2">B · Operator-gesprek</div>
    <div class="text-xs opacity-70">Wat zouden zij willen vragen — en hoe uitgelegd krijgen?</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900 mb-2">C · Leverancier-pitch</div>
    <div class="text-xs opacity-70">Vroeg die om XAI? Zo nee — wat ontbrak?</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-70 max-w-lg mx-auto">
  Schrijf je actie in één zin op wb-03.<br/>
  <span class="text-sm opacity-80">Volgende sessie bespreken we de uitkomsten.</span>
</div>

<!--
Bewaak je tijd — 8 min voor blok 3 gaat snel.

Na 2 plenaire cases (5 min) en centrale terugkoppeling (1 min 30):
toon deze slide voor de transferopdracht (45 sec).

Drie opties — laat de teamleider kiezen op basis van eigen rol en context.
Optie A is voor wie nog moet starten; B voor wie operators wil meenemen;
C voor wie een lopende leveranciersrelatie heeft.

Zonder deadline geen actie — benadruk "komende 2 weken" en "volgende sessie bespreken".

Verwijs naar draaiboek blok 3, instructie 5.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Direct hierna: <span class="font-bold">lo-spc-603 — alarmrationalisatie</span>
</div>

<div class="mt-4 text-sm opacity-60">
  Wat moet er met al die alarmen gebeuren als ze afgaan?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · AI + SPC
</div>

<!--
Bedank de groep. Kondig direct lo-spc-603 aan — geen pauze, doorlopende sessie.

"Alarmen zijn nu het thema. We gaan zo door met alarmrationalisatie —
wat moet er met al die alarmen gebeuren als ze afgaan?"

Vergeet niet werkbladen in te nemen of foto's te maken voor learning analytics.

Notities voor jezelf na afloop:
- Welke aanpak-categorieën kozen deelnemers het vaakst?
- Welke lijnen hebben deelnemers gekozen voor de eigen-lijn-screen?
- Bij data-savvy teamleider: warm overdragen naar Module 3 verdiepingsstap.

Verwijs naar draaiboek "Checklist na de sessie".
-->
