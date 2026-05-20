---
theme: default
title: De acht Nelson-rules — patroonherkenning op de regelkaart
info: |
  ## SPC Module 2 — Train
  Workshop-blok over patroonherkenning met de Nelson-rules.
  Doelgroep: operators MBO-4 + teamleiders MBO-4, 60 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Patronen op de kaart

### Wat zegt jouw regelkaart écht?

<div class="mt-12 text-sm opacity-60">
  SPC Module 2 (Train) · Workshop-blok · 60 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-4 + teamleiders · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. In Module 1 leerden we het verschil tussen common en special cause.
Vandaag: hoe zie je dat verschil concreet op een regelkaart?

Open zin: "Eén punt buiten de grenzen is niet de enige manier waarop een proces je vertelt dat er iets verandert. Er zijn er meer."

Zie draaiboek blok 1 voor opening + trigger-vraag.
-->

---

# Recap — de regelkaart

<div class="grid grid-cols-[2fr_1fr] gap-8 mt-6">

<div>

<v-clicks>

- **Centrumlijn** = procesgemiddelde
- **UCL / LCL** = controlegrenzen op ±3σ
- **Zone A / B / C** = ±1σ, ±2σ, ±3σ vanaf centrumlijn
- Punten in tijd — patroon zegt méér dan losse waarde

</v-clicks>

</div>

<div class="flex items-center justify-center">
  <div class="text-center">
    <div class="text-5xl mb-2">📈</div>
    <div class="text-sm font-mono opacity-70">UCL ━━━━━━</div>
    <div class="text-xs opacity-50 my-1">+2σ ┄┄┄┄┄┄</div>
    <div class="text-xs opacity-50 my-1">+1σ ┄┄┄┄┄┄</div>
    <div class="text-sm font-bold my-1">━━━ centrum</div>
    <div class="text-xs opacity-50 my-1">−1σ ┄┄┄┄┄┄</div>
    <div class="text-xs opacity-50 my-1">−2σ ┄┄┄┄┄┄</div>
    <div class="text-sm font-mono opacity-70">LCL ━━━━━━</div>
  </div>
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  Bekend uit ko-spc-108
</div>

<!--
Korte recap (max 90 sec). Niet uitleggen, alleen activeren.

Trigger-vraag: "Wie heeft wel eens op een regelkaart iets verdacht gezien — zonder dat één punt buiten de grenzen zat?"
Vang 1-2 reacties. Reageer alleen met "herkenbaar".

Zie draaiboek blok 1, instructie 2.
-->

---
layout: center
class: text-center
---

# 🟢 Patroonquiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  8 fictieve regelkaarten.<br/>
  Per kaart: <span class="font-bold text-blue-600">welk patroon zie je?</span>
</div>

<div v-click class="mt-8 text-base opacity-70 max-w-md mx-auto">
  Schrijf in eigen woorden.<br/>
  Regelnummers krijg je straks.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 minuten · individueel · wb-01-patroonquiz
</div>

<!--
Deel wb-01-patroonquiz uit (1 min).

"In dit werkblad zitten 8 fictieve regelkaarten. Per kaart: één — zie je een patroon? Twee — wat zou je doen als operator? In eigen woorden. Tel de punten."

Zet timer op 10 min. Loop rond. GEEN inhoudelijke vragen beantwoorden — alleen praktische.

Bij kaart 2 (controlekaart): noteer wie 'patroon' invult. Dat is je vk-01-signaal voor de bespreking.

Zie draaiboek blok 1.
-->

---
layout: section
---

# Reflecteren

## Welke kaart was de lastigste?

<!--
Overgang naar blok 2 (reflecteren — 15 min).

"Pen neer. Welke kaart vond je het lastigst? Steek je hand op bij het nummer."
Tel hardop bij elk kaartnummer. Schrijf op flip-over.

Daarna: deel wb-02-reflectie uit. Loop naar de A3-kaarten aan de wand voor draai-de-kaart-bespreking.
-->

---

# Draai de kaart om

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Per kaart bespreken
<v-clicks>

- Wat zie je? (in eigen woorden)
- Wie ziet hetzelfde? Wie ziet iets anders?
- Wat zou je doen als operator?

</v-clicks>

</div>

<div>

### Vijf woorden, vijf patronen
<v-clicks>

- **Sprong**
- **Trend**
- **Verschuiving**
- **Zigzag**
- **Cluster**

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  12 min · plenair · A3-kaarten aan de wand
</div>

<!--
Werk de 8 kaarten door — prioriteer de 'lastige' uit de stemming.

KERNCASUSSEN om extra tijd aan te besteden:
- Kaart 2 (controlekaart): vraag expliciet "Wie zag patroon, wie zag géén patroon?" — vk-01.
- Kaart 3 (trend): "Stel je verkoopt wat hier wordt gemaakt en je krijgt over twee uur klacht..." — vk-02.
- Kaart 8 (combinatie regel 3 + regel 1): "Wie kaart 3 had herkend, had kaart 8 niet meegemaakt." Dit is dé kaart van de sessie.

Stem zelf NOOIT mee. Tel innerlijk tot 7 bij stilte.
Zie draaiboek blok 2 voor antwoordmodel.
-->

---
layout: section
---

# Theoretiseren

## Lloyd Nelson — 1984

<!--
Overgang naar blok 3 (theoretiseren — 15 min).

"Vijf woorden, vijf patronen. Mooi: jullie hebben ze zelf ontdekt.
Nu gaan we kijken hoe Lloyd Nelson — een Amerikaan, 1984 — diezelfde patronen formuleerde als regels met getallen erbij."

Deel wb-03-handout-zes-regels uit. "Pak je markeerstift."
-->

---
layout: two-cols
layoutClass: gap-8
---

# 8 regels — wij doen er 6

### Vandaag (regels 1-6)
<v-clicks>

- Regel 1 — punt buiten grenzen
- Regel 2 — 9 aan één kant
- Regel 3 — 6 stijgend of dalend
- Regel 4 — 14 afwisselend
- Regel 5 — 2 van 3 voorbij ±2σ
- Regel 6 — 4 van 5 voorbij ±1σ

</v-clicks>

::right::

### Module 3 (regels 7-8)
<v-clicks>

- Regel 7 — verdacht weinig variatie
- Regel 8 — mengvorm / mixture

</v-clicks>

<div v-click class="mt-6 p-3 bg-amber-50 rounded-lg text-sm">
  Vereisen begrip subgroepering — eigen data nodig.
</div>

<!--
Eerst kader: waarom 6 vandaag, 2 in module 3.

"Regels 7 en 8 vereisen begrip van steekproefstrategie en het verschil tussen 'gewenste lage variatie' (procesbekwaamheid) en 'verdacht lage variatie' (stratificatie). Hoort bij eigen data — module 3."

Wijs naar de parkeerlijst op flip-over. Zie vk-04 in draaiboek.
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 1 — Punt buiten ±3σ

::left::

<div class="mt-4">

**Patroon**
- 1 punt buiten UCL of LCL

**Operator-actie**
<v-clicks>

- Meetfout uitsluiten
- Output veiligstellen
- Teamleider informeren

</v-clicks>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <line x1="10" y1="100" x2="190" y2="100" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <text x="195" y="22" font-size="7" fill="#dc2626">UCL</text>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <text x="195" y="102" font-size="7" fill="#dc2626">LCL</text>
    <circle cx="25" cy="58" r="2.5" fill="#1e40af"/>
    <circle cx="45" cy="63" r="2.5" fill="#1e40af"/>
    <circle cx="65" cy="55" r="2.5" fill="#1e40af"/>
    <circle cx="85" cy="62" r="2.5" fill="#1e40af"/>
    <circle cx="105" cy="58" r="2.5" fill="#1e40af"/>
    <circle cx="125" cy="65" r="2.5" fill="#1e40af"/>
    <circle cx="145" cy="60" r="2.5" fill="#1e40af"/>
    <circle cx="165" cy="10" r="4" fill="#dc2626" stroke="#7f1d1d" stroke-width="1"/>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 1 · bekend uit module 1
</div>

<!--
1 minuut. Kort, want bekend uit ko-spc-104.

"Eén punt buiten ±3σ. Kennen jullie. Quizkaart 1 — 100,7 g buiten UCL."

NIET LANG BIJ HANGEN. Zie vk-05 in draaiboek. Door naar regel 2.
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 2 — 9 aan één kant

::left::

<div class="mt-4">

**Patroon**
- 9 opeenvolgende punten boven óf onder centrumlijn
- Allemaal binnen UCL/LCL

**Operator-actie**
<v-clicks>

- Check set-up, gereedschap, offset
- Nieuwe grondstofbatch?
- Matrijstemperatuur veranderd?

</v-clicks>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <line x1="10" y1="100" x2="190" y2="100" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <text x="195" y="22" font-size="7" fill="#dc2626">UCL</text>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <circle cx="20" cy="62" r="2.5" fill="#1e40af"/>
    <circle cx="40" cy="58" r="2.5" fill="#1e40af"/>
    <circle cx="60" cy="42" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="78" cy="38" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="96" cy="45" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="114" cy="40" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="132" cy="48" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="150" cy="42" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="168" cy="38" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="186" cy="44" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <text x="120" y="115" font-size="6" fill="#92400e" font-weight="bold">9 punten boven centrumlijn</text>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 4 · gemiddelde verschoven
</div>

<!--
2 minuten.

"9 punten aan één kant van de centrumlijn. Quizkaart 4 — allemaal binnen UCL maar consistent boven het gemiddelde. Het proces is verschoven."

Tel hardop op de slide tot 9. Visueel laten zien dat dit echt 9 punten zijn — geen 5, geen 7.

Mogelijke oorzaken: nieuwe set-up, ander gereedschap, andere grondstofbatch, andere matrijstemperatuur.
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 3 — 6 stijgend of dalend

::left::

<div class="mt-4">

**Patroon**
- 6 opeenvolgende punten omhoog of omlaag
- Trend — vaak slijtage of opwarming

**Operator-actie**
<v-clicks>

- Controleer drift
- Gereedschapsslijtage?
- Opwarming, drukverlies?
- Slijpsteen, koeling?

</v-clicks>

<div v-click class="mt-3 text-sm font-bold text-amber-700">
  Wie regel 3 ziet, voorkomt regel 1.
</div>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <line x1="10" y1="100" x2="190" y2="100" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <text x="195" y="22" font-size="7" fill="#dc2626">UCL</text>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <circle cx="20" cy="65" r="2.5" fill="#1e40af"/>
    <circle cx="40" cy="62" r="2.5" fill="#1e40af"/>
    <circle cx="65" cy="68" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="85" cy="60" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="105" cy="52" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="125" cy="44" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="145" cy="36" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="165" cy="28" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <path d="M 65 68 L 165 28" stroke="#f59e0b" stroke-width="0.5" stroke-dasharray="2 1" opacity="0.6"/>
    <text x="100" y="115" font-size="6" fill="#92400e" font-weight="bold">6 punten stijgend</text>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 3 · spuitgieten matrijskoeling
</div>

<!--
2 minuten — DE regel van vandaag.

"6 punten stijgend of dalend. Quizkaart 3 — gewicht kroop omhoog van 99,80 naar 100,05. Patroon: drift. Oorzaak: matrijskoeling deels verstopt — de pers werd warmer."

Tel hardop tot 6.

Klap-zin: "Wie regel 3 herkent, voorkomt regel 1 — dat is precies wat we op kaart 8 zagen."
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 4 — 14 afwisselend

::left::

<div class="mt-4">

**Patroon**
- 14 punten afwisselend op-neer-op-neer
- Zigzag — geen ruis maar ritme

**Operator-actie**
<v-clicks>

- Twee oorzaken die elkaar afwisselen:
  - Twee operators die om en om meten
  - Twee caviteiten met andere temperatuur
  - Pulserende regeling die overcompenseert

</v-clicks>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <line x1="10" y1="100" x2="190" y2="100" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <circle cx="15" cy="48" r="2.5" fill="#f59e0b"/>
    <circle cx="28" cy="72" r="2.5" fill="#f59e0b"/>
    <circle cx="41" cy="46" r="2.5" fill="#f59e0b"/>
    <circle cx="54" cy="74" r="2.5" fill="#f59e0b"/>
    <circle cx="67" cy="48" r="2.5" fill="#f59e0b"/>
    <circle cx="80" cy="72" r="2.5" fill="#f59e0b"/>
    <circle cx="93" cy="46" r="2.5" fill="#f59e0b"/>
    <circle cx="106" cy="74" r="2.5" fill="#f59e0b"/>
    <circle cx="119" cy="48" r="2.5" fill="#f59e0b"/>
    <circle cx="132" cy="72" r="2.5" fill="#f59e0b"/>
    <circle cx="145" cy="46" r="2.5" fill="#f59e0b"/>
    <circle cx="158" cy="74" r="2.5" fill="#f59e0b"/>
    <circle cx="171" cy="48" r="2.5" fill="#f59e0b"/>
    <circle cx="184" cy="72" r="2.5" fill="#f59e0b"/>
    <path d="M 15 48 L 28 72 L 41 46 L 54 74 L 67 48 L 80 72 L 93 46 L 106 74 L 119 48 L 132 72 L 145 46 L 158 74 L 171 48 L 184 72" stroke="#f59e0b" stroke-width="0.5" fill="none" opacity="0.5"/>
    <text x="80" y="115" font-size="6" fill="#92400e" font-weight="bold">14 punten op-neer-op-neer</text>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 5 · zigzag
</div>

<!--
2 minuten.

"14 punten afwisselend op-neer. Quizkaart 5 — zigzag. Twee oorzaken die elkaar afwisselen: twee operators die om en om meten, twee caviteiten met andere temperatuur, pulserende regeling."

Tel hardop tot 14. Laat zien dat dit véél punten zijn — Nelson is hard.

Boodschap: niet één probleem, maar twee — denk in paren.
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 5 — 2 van 3 voorbij ±2σ

::left::

<div class="mt-4">

**Patroon**
- 2 van 3 opeenvolgende punten voorbij +2σ of −2σ
- Aan dezelfde kant
- Subtieler dan regel 1, eerder dan regel 2

**Operator-actie**
<v-clicks>

- Vroege waarschuwing
- Controleer of proces wegdrijft
- Vóór er echte overschrijdingen komen

</v-clicks>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="33" x2="190" y2="33" stroke="#f59e0b" stroke-width="1" stroke-dasharray="3 2" opacity="0.6"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <line x1="10" y1="100" x2="190" y2="100" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <text x="195" y="22" font-size="7" fill="#dc2626">UCL</text>
    <text x="195" y="35" font-size="7" fill="#f59e0b">+2σ</text>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <rect x="0" y="20" width="200" height="13" fill="#fee2e2" opacity="0.4"/>
    <text x="100" y="30" font-size="5" fill="#991b1b" text-anchor="middle">zone A</text>
    <circle cx="20" cy="65" r="2.5" fill="#1e40af"/>
    <circle cx="40" cy="58" r="2.5" fill="#1e40af"/>
    <circle cx="60" cy="62" r="2.5" fill="#1e40af"/>
    <circle cx="80" cy="55" r="2.5" fill="#1e40af"/>
    <circle cx="100" cy="50" r="2.5" fill="#1e40af"/>
    <circle cx="125" cy="28" r="3.5" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="145" cy="40" r="2.5" fill="#1e40af"/>
    <circle cx="165" cy="25" r="3.5" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <text x="135" y="115" font-size="6" fill="#92400e" font-weight="bold">2 van 3 in zone A</text>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 6 · subtiele shift
</div>

<!--
2 minuten.

"2 van 3 opeenvolgende punten voorbij +2σ aan dezelfde kant. Quizkaart 6 — subtieler dan regel 1, eerder dan regel 2."

Verwijs naar zone-indeling (Western Electric: zone A = ±2σ tot ±3σ).
"Vroege waarschuwing dat het proces wegdrijft."

Differentiatie teamleider: voeg na regel 5 of 6 de discussievraag in (zie draaiboek): "Welke regel schakel jij eerst in op een nieuwe lijn?"
-->

---
layout: two-cols-header
layoutClass: gap-6
---

# Regel 6 — 4 van 5 voorbij ±1σ

::left::

<div class="mt-4">

**Patroon**
- 4 van 5 opeenvolgende punten voorbij +1σ of −1σ
- Aan dezelfde kant
- Nog subtieler dan regel 5

**Operator-actie**
<v-clicks>

- Monitoring intensiveren
- Achtergrondoorzaak zoeken
- Vóór regel 5 of 1 triggert

</v-clicks>

</div>

::right::

<div class="flex items-center justify-center h-full">
  <svg viewBox="0 0 200 120" class="w-full max-w-xs">
    <line x1="10" y1="20" x2="190" y2="20" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="4 2"/>
    <line x1="10" y1="46" x2="190" y2="46" stroke="#f59e0b" stroke-width="1" stroke-dasharray="3 2" opacity="0.6"/>
    <line x1="10" y1="60" x2="190" y2="60" stroke="#64748b" stroke-width="1"/>
    <text x="195" y="22" font-size="7" fill="#dc2626">UCL</text>
    <text x="195" y="48" font-size="7" fill="#f59e0b">+1σ</text>
    <text x="195" y="62" font-size="7" fill="#64748b">x̄</text>
    <rect x="0" y="20" width="200" height="26" fill="#fef3c7" opacity="0.4"/>
    <text x="100" y="38" font-size="5" fill="#92400e" text-anchor="middle">zone A + B</text>
    <circle cx="20" cy="62" r="2.5" fill="#1e40af"/>
    <circle cx="45" cy="58" r="2.5" fill="#1e40af"/>
    <circle cx="70" cy="65" r="2.5" fill="#1e40af"/>
    <circle cx="95" cy="40" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="115" cy="55" r="2.5" fill="#1e40af"/>
    <circle cx="135" cy="38" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="155" cy="42" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <circle cx="175" cy="36" r="3" fill="#f59e0b" stroke="#92400e" stroke-width="0.5"/>
    <text x="115" y="115" font-size="6" fill="#92400e" font-weight="bold">4 van 5 voorbij +1σ</text>
  </svg>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Quizkaart 7 · vroegste waarschuwing
</div>

<!--
2 minuten.

"4 van 5 opeenvolgende punten voorbij +1σ. Quizkaart 7 — nóg subtieler. Operator-actie: monitoring intensiveren, achtergrondoorzaak zoeken voordat regel 5 of 1 triggert."

Bij uitloop: dit blok is in te korten — regels 5 en 6 herken je in de praktijk vanzelf als je 2, 3 en 4 beheerst. Zie vk-05 in draaiboek.
-->

---
layout: default
---

# Wat doe je bij dit patroon?

<div class="grid grid-cols-2 gap-x-8 gap-y-3 mt-6 text-sm">

<div v-click class="p-3 bg-red-50 rounded-lg border-l-4 border-red-500">
  <div class="font-bold text-red-700">Regel 1 — punt buiten</div>
  <div class="opacity-80 mt-1">Stoppen, output veiligstellen, teamleider</div>
</div>

<div v-click class="p-3 bg-blue-50 rounded-lg border-l-4 border-blue-500">
  <div class="font-bold text-blue-700">Regel 2 — verschuiving</div>
  <div class="opacity-80 mt-1">Set-up checken, batch, offset</div>
</div>

<div v-click class="p-3 bg-amber-50 rounded-lg border-l-4 border-amber-500">
  <div class="font-bold text-amber-700">Regel 3 — trend</div>
  <div class="opacity-80 mt-1">Drift opsporen — slijtage, opwarming</div>
</div>

<div v-click class="p-3 bg-purple-50 rounded-lg border-l-4 border-purple-500">
  <div class="font-bold text-purple-700">Regel 4 — zigzag</div>
  <div class="opacity-80 mt-1">Twee bronnen zoeken — operators, caviteiten</div>
</div>

<div v-click class="p-3 bg-orange-50 rounded-lg border-l-4 border-orange-500">
  <div class="font-bold text-orange-700">Regel 5 — 2 van 3 in ±2σ</div>
  <div class="opacity-80 mt-1">Vroege waarschuwing — monitor</div>
</div>

<div v-click class="p-3 bg-yellow-50 rounded-lg border-l-4 border-yellow-500">
  <div class="font-bold text-yellow-700">Regel 6 — 4 van 5 in ±1σ</div>
  <div class="opacity-80 mt-1">Subtiel — onderzoek achtergrond</div>
</div>

</div>

<div v-click class="mt-6 text-center text-sm opacity-70">
  Concrete reaction plans → <span class="font-bold">lo-spc-203</span>
</div>

<!--
1 minuut. Synthese.

"Zes regels, zes operator-acties. Allemaal komen ze erop neer: zien dat het proces verandert vóórdat het buiten de grenzen valt. Daar zit de winst."

Verwijs naar lo-spc-203 (reaction plans per regel) als post-workshop LO.
-->

---
layout: center
class: text-center
---

# En de regels 7 en 8?

<div class="text-lg mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Regel 7: <span class="font-bold">verdacht weinig variatie</span><br/>
  Regel 8: <span class="font-bold">mengvorm — twee bronnen door elkaar</span>
</div>

<div v-click class="mt-8 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-sm">
  Vereisen begrip van subgroepering en steekproefstrategie.<br/>
  <span class="font-bold">→ Module 3: op je eigen data</span>
</div>

<!--
30 seconden. Niet uitleggen, alleen benoemen.

"Voor de volledigheid: regels 7 en 8 bestaan ook. 'Te weinig spreiding' en 'mengvorm'. Vereisen begrip van steekproefstrategie — komt in module 3."

Wijs naar de parkeerlijst op flip-over.

Niet doorvragen. Door naar blok 4. Zie vk-04 in draaiboek.
-->

---
layout: section
---

# Experimenteren

## Jouw lijn, jouw kaart

<!--
Overgang naar blok 4 (experimenteren — 15 min).

Deel wb-04-eigen-kaart-analyse uit.
"De afgelopen 45 minuten waren oefenen op fictieve kaarten. Nu het echte werk: jouw lijn."
-->

---

# Bouw je eigen kaart deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Stappen op werkblad
<v-clicks>

1. Welke meetwaarde kies je?
2. Wat is je centrumlijn?
3. Welke 2 regels schakel je eerst in?
4. Wat doe je als die regel triggert?

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Welke meting doe je sowieso al?
- Welk patroon zou jij eerst willen zien?
- Bij welk patroon écht direct ingrijpen?
- Wanneer eerst monitoren?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · individueel · wb-04-eigen-kaart-analyse
</div>

<!--
Zet timer op 10 min.

Inventarisatie-vraag (1 min): "Welke meting doe je dagelijks waar je twijfels bij had?"
Vang 4-5 voorbeelden. Niet bespreken — alleen verzamelen.

Loop rond. Help met de hulpvragen.
NIET zelf meedenken over welke regels 'het beste' zijn — autonomie is de werkende component.

Bij iemand die alle 6 wil: "Twee deze week is al een prestatie. Volgende week kun je uitbreiden."
-->

---
layout: center
class: text-center
---

# Volgende sessie

<div class="text-xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Neem je eigen regelkaart mee.<br/>
  We bespreken per deelnemer kort:<br/>
  <span class="font-bold">welke regels heb je gekozen, en waarom?</span>
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-base">
  Bonus: praat er deze week één keer met een collega over.<br/>
  <span class="text-sm opacity-70">"Welke patronen herken jij eerst op je kaart?"</span>
</div>

<!--
Korte deel-ronde (3 min): "Wie wil in één zin vertellen welke meetwaarde, en welke 2 regels?"
4-5 deelnemers, max 30 sec.

Sluit af met de transferopdracht en de bonus-collega-vraag.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">van patroon herkennen naar reaction plan bouwen</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 2 (Train) · Nelson-rules
</div>

<!--
Bedank de groep. Kondig vervolg aan (lo-spc-203 — reaction plans).

Vergeet niet:
- Werkbladen ophalen of foto's maken (learning analytics)
- "Patronen we zagen"-flip-over fotograferen
- "Parkeerlijst regel 7+8" fotograferen — meenemen naar module 3 voorbereiding

Notitie voor jezelf:
- Welke kaarten waren voor déze groep het lastigst?
- Welke meetwaardes hebben deelnemers gekozen voor wb-04?
-->
