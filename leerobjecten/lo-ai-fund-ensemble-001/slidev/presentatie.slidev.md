---
theme: default
title: Ensemble learning — meerdere modellen die samen sterker zijn
info: |
  ## AI Fundamentals — Module 2 (Train)
  Workshop-blok over ensembles: diagnose-spel, bagging vs. boosting, eigen PdM-actieplan.
  Doelgroep: operators/teamleiders MBO-4, 48 minuten.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Ensemble Learning

### Meerdere modellen die samen sterker zijn

<div class="mt-12 text-sm opacity-60">
  AI Fundamentals · Module 2 (Train) · Workshop-blok · 48 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators / teamleiders MBO-4 · PdM · RUL · failure prediction
</div>

<!--
Welkom. De komende 48 minuten kijken we naar een ML-paradigma dat in PdM-onderzoek consequent betere voorspellingen geeft.

We beginnen niet met theorie — we beginnen met een spel.
-->

---
layout: center
class: text-center
---

# Drie experts. Eén machine.

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Je laat een kapotte machine zien<br/>
  aan drie collega-monteurs.
</div>

<div v-click class="text-xl mt-8 opacity-70">
  Soms zijn ze het eens.<br/>
  Soms niet.
</div>

<div v-click class="text-2xl mt-10 font-bold text-blue-700">
  Wat doe jij?
</div>

<!--
"Stel: drie collega's stellen elk een diagnose. Wat doe jij — alleen luisteren naar de meest senior? Of alle drie?"

Pauze. "Je gaat het zo zelf ervaren — vijf mystery cases."

Deel daarna wb-01 uit:
"Per case: wat doe je met alleen expert A? En met alle drie?"
-->

---

# Het spel

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Per case
<v-clicks>

- Een korte machinebeschrijving
- Sensorwaarden
- Drie 'expert'-diagnoses (A / B / C)

</v-clicks>

</div>

<div>

### Twee vragen
<v-clicks>

- Wat doe je met **alleen A**?
- Wat doe je met **alle drie samen**?

</v-clicks>

<div v-click class="mt-4 p-3 bg-amber-50 rounded-lg text-sm">
  Verandert je antwoord?
</div>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  IK DOE eerst — case 1
</div>

<!--
IK DOE eerst — case 1 hardop voorlezen:
- Spuitgietpers, lichte cyclustijd-stijging
- Sensoren: temp normaal, druk verhoogd, trilling normaal
- A: lichte plunjer-slijtage
- B: drukvariatie hydrauliek
- C: drukvariatie hydrauliek

"Met alleen A: monitoren plunjer.
Met alle drie: 2 op 3 zegt drukvariatie. Mijn antwoord verandert.
Win voor het ensemble."

Plak op flip-over: case 1 = 1 win.
-->

---
layout: center
class: text-center
---

# Doe cases 2-5 zelf

<div class="text-xl mt-10 opacity-80">
  Per case: telt of het ensemble wint
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Bij hoeveel cases verandert je antwoord<br/>
  als je alle drie meeneemt?
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · individueel · wb-01 <span class="opacity-60">of tablet · model-ensemble-stemming</span>
</div>

<!--
Zet timer op 6 min.
Loop rond. Stel verdiepende vragen:
- Waar veranderde je antwoord?
- Als alle drie hetzelfde — wat voegt het ensemble toe?
- Als ze elkaar tegenspreken — hoe kies je?

Geen antwoorden geven. Alleen vragen.
-->

---

# Wins per case — tellen we plenair

<div class="mt-10 max-w-xl mx-auto">

| Case | Wint het ensemble? |
|------|-------------------|
| 1 | _________ |
| 2 | _________ |
| 3 | _________ |
| 4 | _________ |
| 5 | _________ |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Bij hoeveel cases werkte het ensemble gemiddeld?
</div>

<!--
Eerst tweetallen vergelijken (5 min).
Daarna plenair tellen — schrijf op flip-over.

Tel innerlijk tot 7 na elke vraag.
Bij stilte: 'wie van jullie veranderde van mening op case 3?'
-->

---
layout: center
class: text-center
---

# Twee patronen

<div class="grid grid-cols-2 gap-8 mt-10 max-w-3xl mx-auto">

<div class="p-5 bg-red-50 rounded-xl border-2 border-red-200 text-left">

### Drie experts eensgezind
- Ensemble voegt niets toe
- Verspilde rekenkracht

</div>

<div class="p-5 bg-green-50 rounded-xl border-2 border-green-200 text-left">

### Drie experts uiteenlopend
- Ensemble wint vaak
- Verschillende fouten

</div>

</div>

<div v-click class="mt-10 text-base font-bold text-blue-700">
  Diversiteit is voorwaarde.
</div>

<div v-click class="mt-3 text-sm opacity-60">
  Drie identieke modellen ≠ ensemble.
</div>

<!--
Anderhalve minuut.
"Diversiteit is voorwaarde — herhaal dit steekwoord.
Drie identieke modellen voegen niets toe. Ensembles werken alleen als modellen verschillende fouten maken."

Brug naar fase 3:
"Wat jullie deden — drie meningen middelen — was een vorm van bagging.
Maar dat is niet de enige manier."
-->

---
layout: section
---

# Theoretiseren

## Twee families: bagging en boosting

<!--
Overgang naar blok 3.
Deel wb-03 uit. Pak markeerstift erbij.
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
  Eén expert op 75% → vijf modellen die stemmen (bagging)<br/>
  → ketting van correcties (boosting) → naast elkaar gezet
</div>

<div v-click class="mt-10 inline-block p-4 bg-blue-50 rounded-lg text-sm border border-blue-200">
  <code>video/composition.tsx</code> (Remotion · <code>EnsembleVideo</code>)<br/>
  Pre-render naar MP4 of <code>npx remotion preview</code>
</div>

<!--
Optionele inzet — als brug van fase 2 naar fase 3, vóór de handout.
Toon de 90s video. Geen bespreking achteraf — direct door naar bagging-uitleg.
-->

---

# Bagging

<div class="text-base opacity-70 mt-2">Bootstrap Aggregating · 2001</div>

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

### Hoe werkt het?
<v-clicks>

- Train modellen **onafhankelijk**
- Elk model: random subset data + features
- Middel hun voorspellingen
- Parallel uitvoerbaar

</v-clicks>

</div>

<div>

### Wat verlaagt het?
<v-clicks>

- **Variance** — instabiliteit
- Eén model wankel? Ensemble stabiel.

</v-clicks>

<div v-click class="mt-4 p-3 bg-blue-50 rounded-lg text-center">
  <span class="font-bold">Random Forest</span><br/>
  een 'bos' van decision trees
</div>

</div>

</div>

<!--
Vier minuten.
Schrijf op flip-over: 'bagging = parallel + variance + Random Forest'.

"Wat jullie deden in het diagnose-spel — meningen middelen — was bagging-achtig.
Random Forest is het beroemdste voorbeeld."

Niet uitweiden over bootstrap-sampling tenzij iemand vraagt.
-->

---

# Boosting

<div class="text-base opacity-70 mt-2">Sequentiele correctie · 1990 / 2001</div>

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

### Hoe werkt het?
<v-clicks>

- Eerste model traint op data
- Tweede model traint op **fouten** van eerste
- Derde focust op fouten van tweede
- **Sequentieel** — niet parallel

</v-clicks>

</div>

<div>

### Wat verlaagt het?
<v-clicks>

- **Bias** — systematische fouten
- Elke iteratie corrigeert

</v-clicks>

<div v-click class="mt-4 p-3 bg-purple-50 rounded-lg text-center">
  <span class="font-bold">Gradient Boosting</span><br/>
  XGBoost · LightGBM
</div>

</div>

</div>

<!--
Vier minuten.
Schrijf op flip-over: 'boosting = sequentieel + bias + Gradient Boosting'.

"Tweede model corrigeert eerste. Derde corrigeert tweede.
Gradient Boosting (XGBoost, LightGBM) wint heel veel Kaggle-competities."

Maak op flip-over scherp tegenover bagging — twee aparte rijen.
-->

---

# Drie PdM-cases

<div class="grid grid-cols-3 gap-4 mt-6 text-sm">

<div class="p-4 bg-blue-50 rounded-lg">

### Tool wear (Wu)
- Random Forest
- Bagging-stijl
- Sensor-heterogeniteit
- Diversiteit ontstaat vanzelf

</div>

<div class="p-4 bg-purple-50 rounded-lg">

### Pipe failure
- Boosted decision tree
- Boosting-stijl
- Onevenwichtige data
- Focus op zeldzame failures

</div>

<div class="p-4 bg-amber-50 rounded-lg">

### RUL aircraft (Li)
- Combinatie ensemble
- 2026 onderzoek
- Beter dan losse modellen
- PdM-standaard

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  In PdM-onderzoek winnen ensembles consequent.
</div>

<!--
Drieënhalve minuut.
Loop drie cases af. Houd Wu, Li kort — namen zijn niet de inhoud.

"Random Forest werkt op tool wear omdat verschillende sensors verschillende patronen oppikken.
Boosted trees werken op pipe failure omdat ze zich focussen op zeldzame failures.
Li toont dat ensembles bij PdM consequent winnen."
-->

---
layout: center
class: text-center
---

# Drie redenen voor ensemble in PdM

<div class="grid grid-cols-3 gap-4 mt-10 text-sm">

<div class="p-4 bg-red-50 rounded-lg">

### 1 · Onevenwichtige data
Weinig failures, veel normaal — ensembles compenseren

</div>

<div class="p-4 bg-blue-50 rounded-lg">

### 2 · Sensor-heterogeniteit
Verschillende sensors, verschillende patronen

</div>

<div class="p-4 bg-green-50 rounded-lg">

### 3 · Robuustheid
Uitvalmodi variëren — ensemble blijft stabiel

</div>

</div>

<div v-click class="mt-10 text-base opacity-70 italic">
  Nu naar je eigen situatie.
</div>

<!--
Eén minuut.
Brug naar fase 4.
"Drie redenen waarom ensembles bij PdM zo vaak passen. Nu jouw eigen situatie."
-->

---
layout: section
---

# Experimenteren

## Zou een ensemble onze PdM verbeteren?

<!--
Overgang naar blok 4.
"Laatste 12 minuten — eigen PdM-actieplan."
-->

---

# Eigen PdM-actieplan

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vier vragen
<v-clicks>

- Hoeveel **failure-cases** beschikbaar?
- Is de data **heterogeen** (meerdere sensors)?
- Zou een **ensemble** passen?
- Welke **familie** — bagging of boosting?

</v-clicks>

</div>

<div>

### Hulp bij twijfel
<v-clicks>

- Hoe vaak per jaar gaat machine stuk?
- Hoeveel sensors meten mee?
- Gelijke uitvalmodi of wisselend?
- Weinig failures = ARGUMENT, geen blokker

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-04
</div>

<!--
Inventarisatie-vraag (1 min): "Bij wie loopt PdM op de lijn?"
Vang 4-5 antwoorden, niet bespreken.

Zet timer op 8 min.
Stel concretiserende vragen.
Bij 'we hebben weinig data': bevestig — JUIST argument voor ensemble.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Bevraag IT of leverancier
<v-clicks>

- Gebruikt het systeem een ensemble?
- Bagging-stijl (random forest)?
- Of boosting-stijl (gradient boosting)?
- Hoeveel failure-cases voor training?

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Zoek op YouTube:<br/>"random forest explained simple"
- Je ziet meerdere bomen samen stemmen
- 60 seconden — maakt het tastbaar

</v-clicks>

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Volgende sessie: kort delen — wat zegt IT?
</div>

<!--
Sluit af met de transferopdracht.
"Volgende sessie kort delen.
Daarna door naar volgende paradigma-LO over de vier ML-leerklassen."

Bonus alleen noemen als er tijd over is.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend in AI Fundamentals: <span class="font-bold">Vier ML-leerklassen — welke past bij welk PdM-probleem?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · AI Fundamentals Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Gemiddelde wins per case
- Welke transfer-acties?
- Welke vragen op parkeerlijst?
-->
