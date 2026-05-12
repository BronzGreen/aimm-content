---
theme: default
title: Vier ML-leerklassen — welke past bij welk PdM-probleem?
info: |
  ## AI Fundamentals — Module 2 (Train)
  Workshop-blok over de vier ML-leerklassen: scenario's, framework, eigen organisatie-actieplan.
  Doelgroep: operators/teamleiders MBO-4, 50 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Vier ML-leerklassen

### Welke past bij welk PdM-probleem?

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 2 (Train) · Workshop-blok · 50 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · PdM · datasituatie → AI-keuze
</div>

<!--
Welkom. De komende 50 minuten kijken we naar het belangrijkste keuzemodel uit ML.

Niet één AI — vier soorten. Tegen het eind weet je welke past bij welke data en welk type PdM-probleem.

Dit is een foundational LO — het kader waar alle andere paradigma-LOs (FL, CNN, RNN, Ensemble) zich aan ophangen.
-->

---
layout: center
class: text-center
---

# Een leveranciersgesprek

<div class="text-2xl mt-10 max-w-2xl mx-auto leading-relaxed opacity-80">
  Leverancier 1: <span class="italic">"wij doen supervised regression — geef ons jullie failure-data"</span>
</div>

<div v-click class="text-2xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-80">
  Leverancier 2: <span class="italic">"wij doen unsupervised clustering — jullie hoeven geen labels te leveren"</span>
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Wat zegt dat over wat jij in huis hebt?
</div>

<!--
"Tegen het eind van deze sessie kun je dat gesprek leiden in plaats van ondergaan."

Brug naar fase 1 — vier scenario-kaarten.
Deel wb-01 uit. "Twijfel mag — vraagteken zetten is welkom."
-->

---

# Vier scenario's — kies een leerklasse

<div class="grid grid-cols-2 gap-4 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">

### A · Rijke uitvalhistorie
- 5 jaar uitvalhistorie
- Duidelijke failure-labels
- RUL voorspellen

<div class="mt-3 text-xs opacity-60">Welke leerklasse?</div>

</div>

<div class="p-4 bg-purple-50 rounded-lg border-2 border-purple-200">

### B · Geen labels
- Geen uitvalhistorie
- Veel sensordata
- Afwijkende patronen vinden

<div class="mt-3 text-xs opacity-60">Welke leerklasse?</div>

</div>

<div class="p-4 bg-amber-50 rounded-lg border-2 border-amber-200">

### C · Beetje labels
- 50 gelabelde failures
- 5000 ongelabelde cycli
- Classificatie

<div class="mt-3 text-xs opacity-60">Welke leerklasse?</div>

</div>

<div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">

### D · Beslissingen
- Continue beslissingen
- Onderhoud uitstellen / doen / vervangen
- Beste strategie?

<div class="mt-3 text-xs opacity-60">Welke leerklasse?</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  7 min · individueel · wb-01 · twijfel mag
</div>

<!--
IK DOE eerst — scenario A:
"5 jaar uitvalhistorie + RUL voorspellen.
Gelabelde data → supervised mogelijk.
Voorspelling van GETAL → regression.
Combinatie: supervised regression."

Daarna: "Doe B, C en D zelf. Zeven minuten. Twijfel mag."
Loop rond. Stel vragen. Geef geen antwoorden.
-->

---
layout: center
class: text-center
---

# Stem mee — vier kleuren

<div class="grid grid-cols-4 gap-4 mt-10 text-sm">
  <div class="p-4 bg-red-50 rounded-lg border-2 border-red-200">
    <div class="font-bold text-red-700">Rood</div>
    <div class="mt-2">Supervised</div>
  </div>
  <div class="p-4 bg-blue-50 rounded-lg border-2 border-blue-200">
    <div class="font-bold text-blue-700">Blauw</div>
    <div class="mt-2">Unsupervised</div>
  </div>
  <div class="p-4 bg-yellow-50 rounded-lg border-2 border-yellow-200">
    <div class="font-bold text-yellow-700">Geel</div>
    <div class="mt-2">Semi-supervised</div>
  </div>
  <div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">
    <div class="font-bold text-green-700">Groen</div>
    <div class="mt-2">Reinforcement</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-70">
  Per scenario steek je een kleur omhoog.
</div>

<!--
Eerst tweetallen vergelijken (5 min).
Daarna stemmen met kleurkaartjes — schrijf uitslag op flip-over.

Tel innerlijk tot 7. Veroordeel geen antwoord.
Bij stilte: noem zelf de eerste 'hand omhoog' om ijs te breken.
-->

---

# Het antwoord

<div class="grid grid-cols-2 gap-3 mt-6 text-xs">

<div class="p-3 bg-red-50 rounded-lg">

### A · Supervised regression
- Gelabelde data + RUL
- Voorspelling van een getal
- Standaard PdM-keuze

</div>

<div class="p-3 bg-blue-50 rounded-lg">

### B · Unsupervised clustering
- Geen labels
- Zoek groepen / afwijkingen
- Anomaliedetectie

</div>

<div class="p-3 bg-yellow-50 rounded-lg">

### C · Semi-supervised
- Combinatie 50 + 5000
- Recent populair in PdM
- Vaak gemist!

</div>

<div class="p-3 bg-green-50 rounded-lg">

### D · Reinforcement
- Leren van beslissingen
- Adaptief onderhoud
- Niet alleen voor robots

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  C en D zijn de tricky ones — meeste mensen missen ze.
</div>

<!--
A en B zijn meestal goed.
C en D — maak expliciet:

"C: semi-supervised gebruikt BEIDE — klein gelabeld + groot ongelabeld. Niet alleen labels, niet alleen ongelabeld. Combinatie."

"D: reinforcement = leren van beslissingen met feedback. Bij onderhoud: uitstellen vs. preventief — elke beslissing heeft kosten/baten. Reinforcement learnt optimaliseren."

Brug naar fase 3.
-->

---
layout: section
---

# Theoretiseren

## Vier leerklassen × drie PdM-probleemtypen

<!--
Overgang naar blok 3.
Deel wb-03 uit. Pak markeerstift erbij.
-->

---

# Vier leerklassen

<div class="grid grid-cols-2 gap-4 mt-6 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### Supervised
- **Met labels** — input → bekende output
- Veel gelabelde failure-cases
- Classification of regression
- Voorbeeld: RUL met 5 jaar historie

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Unsupervised
- **Zonder labels** — zoekt structuur
- Geen failure-history nodig
- Clustering / anomaliedetectie
- Voorbeeld: afwijkende vibration-patronen

</div>

<div class="p-4 bg-yellow-50 rounded-lg">

### Semi-supervised
- **Beetje labels** + veel ongelabeld
- Recent populair (labelen is duur)
- Pseudo-labeling
- Voorbeeld: 50 + 5000 cycli

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Reinforcement
- **Leren van beslissingen** + feedback
- Online, adaptief
- Niet veel in deployment, vaak academisch
- Voorbeeld: adaptief onderhoudsbeleid

</div>

</div>

<!--
Vijf minuten.
Loop af, koppel elke leerklasse aan het scenario uit fase 1.

Schrijf op flip-over: vier leerklassen onder elkaar met steekwoord per stuk.
Vermijd k-means, t-SNE, Q-learning. Op leerklasse-niveau.
-->

---

# Drie PdM-probleemtypen

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Classification
- **Welke klasse?**
- Bv. uitvalmode A / B / C
- Past supervised
- Of semi-supervised

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Regression
- **Hoeveel?**
- Bv. RUL = 23 cycli
- Bv. kosten = 12.000 €
- Past supervised

</div>

<div class="p-4 bg-green-50 rounded-lg">

### Clustering
- **Welke groep?**
- Bv. machines die similar gedragen
- Past unsupervised

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  PROBLEEM × LEERKLASSE — beide moet je matchen.
</div>

<!--
Drie en een halve minuut.
Maak op flip-over: PROBLEEM × LEERKLASSE.

Loop drie types af. Verbindt aan scenario A (regression+supervised) en B (clustering+unsupervised).
-->

---

# Praktische realiteit in PdM

<div class="grid grid-cols-3 gap-4 mt-8 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### 80% van fabrieken
- Geen systematische failure-data
- → unsupervised of semi-supervised meest realistisch

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### Logboeken
- Vrije tekst, vaak waardevol
- Labelen = verborgen werk
- → potentieel voor semi-supervised

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### Reinforcement
- Zeldzaam in deployment
- Vaak academisch
- Cloud-platformen experimenteren

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Leerklasse moet aansluiten op DATA-realiteit, niet op een ideaal.
</div>

<!--
Twee minuten.
Belangrijk inzicht — herhaal: DATA-REALITEIT, niet ideaal.

Brug naar fase 4: "Nu jouw eigen organisatie."
-->

---
layout: section
---

# Experimenteren

## Welke leerklasse past bij ons?

<!--
Overgang naar blok 4.
"Laatste 12 minuten — eigen organisatie-actieplan."
-->

---

# Eigen actieplan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen
<v-clicks>

- Heb je **gelabelde uitvalhistorie**?
- Wat wil je **voorspellen** — getal, klasse, patroon, beslissing?
- Welke **leerklasse** past?
- Welke **vraag** stel je aan IT?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Hoe vaak houden jullie systematisch uitval bij?
- Heeft ERP een uitval-categorie-veld?
- 'Weet ik niet' = waardevolle uitkomst
- Dat is precies de eerste IT-vraag

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-04
</div>

<!--
Inventarisatie-vraag (1 min): "Bij wie speelt PdM of monitoring — spuitgieten, CNC, verpakking?"
Vang 4-5 antwoorden, niet bespreken.

Zet timer op 8 min.
'Weet ik niet' is een GELDIGE uitkomst.
Help formuleren als 3 concrete IT-vragen.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Drie IT-vragen
<v-clicks>

- Registreren we systematisch failures?
- Hoeveel cases over afgelopen 1-3 jaar?
- Zijn oorzaken gecategoriseerd (uitvalmode)?

</v-clicks>

</div>

<div>

### Bonus-praatje
<v-clicks>

- Vraag een onderhoudscollega:<br/>"houden wij eigenlijk systematisch bij waarom een machine stuk gaat?"
- Vaak: informatie zit in logboeken
- Maar niet bruikbaar gestructureerd
- Dat ontdekken = waardevol voor elk AI-project

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat heb je gevonden?
</div>

<!--
Sluit af met de transferopdracht.
"Volgende sessie kort delen.
Daarna door naar de paradigma-LOs (FL, CNN, RNN, Ensemble) die op deze foundation bouwen."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Federated Learning · CNN · RNN/LSTM · Ensemble</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Stemming per scenario (verdeling = groepsbegrip)
- Hoe scoorde groep op C en D? (vaak gemist = leerwinst)
- Welke IT-vragen aangekondigd?
- Welke vragen op parkeerlijst?
-->
