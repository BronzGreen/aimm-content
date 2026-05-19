---
theme: default
title: Beschikbaarheid — hoeveel van de geplande tijd draait de machine?
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over beschikbaarheid en de vier stilstandstypen.
  Doelgroep: operators MBO-3, 42 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Beschikbaarheid

### Hoeveel van de geplande tijd draait de machine?

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok 2 · 42 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. In LO-001 zagen we de drie OEE-componenten.
We pakken er nu één: beschikbaarheid.

Hoeveel van de geplande tijd draait de machine echt?
Eerst gaan we sorteren — daarna rekenen — daarna jouw eigen dienst.
-->

---
layout: center
class: text-center
---

# Sorteer de kaartjes

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  12 situaties uit de werkvloer.<br/>
  Per kaartje: <span class="font-bold text-green-600">telt mee</span> of <span class="font-bold text-red-600">telt niet mee</span>?
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Twijfel? Maak een derde stapeltje. Die bespreken we straks.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · in tweetallen · 12 kaartjes
</div>

<!--
IK DOE eerst — pak een kaartje, lees voor "lunchpauze 30 min", denk hardop:
- "Telt dit mee als stilstand voor OEE?"
- "Lunchpauze staat in de planning. De machine zou tijdens lunch sowieso niet draaien."
- "Dus: stapel NEE."

Schrijf op flap-over (afgedekt!): "Stilstand = niet draaien tijdens GEPLANDE productietijd"
Dek toe — laat de groep zelf herontdekken.

Zet timer op 6 min. Loop rond. Stel alleen vragen, geen antwoorden.
Onderbreek discussie niet — dat is leerstof.
-->

---
layout: section
---

# Reflecteren

## Wat hebben de stapels gemeen?

<!--
Overgang naar blok 2.
We gaan plenair stemmen per kaartje en daarna de regel zoeken.
-->

---

# Plenair stemmen

<div class="grid grid-cols-2 gap-8 mt-6">
  <div class="text-center p-8 bg-green-50 rounded-xl border-2 border-green-200">
    <div class="text-6xl mb-3">🟢</div>
    <div class="text-2xl font-bold text-green-700">Telt mee</div>
    <div class="text-sm opacity-70 mt-2">Stilstand binnen geplande tijd</div>
  </div>
  <div class="text-center p-8 bg-red-50 rounded-xl border-2 border-red-200">
    <div class="text-6xl mb-3">🔴</div>
    <div class="text-2xl font-bold text-red-700">Telt niet mee</div>
    <div class="text-sm opacity-70 mt-2">Buiten geplande tijd</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Bij twijfel: <span class="font-bold">beide kaartjes omhoog.</span>
</div>

<!--
Werk de 12 kaartjes door.

Eensgezindheid (k01, k02, k04, k12): kort bevestigen, max 15 sec.
Verdeeldheid (k08, k09, k06): laat één deelnemer per kant uitleggen, schrijf op whiteboard.

KERNCASUSSEN:
- k08 (sensor reset 90 sec): TWIJFEL toegestaan. Telt voor prestatie (LO-003), niet beschikbaarheid.
  "Korte stop blijft onder de radar; we behandelen het in LO-003."
- k09 (WC 5 min): JA — wachten. Niet moralistisch worden.
- k11 (eerste stuks afkeur): NEE voor stilstand — kwaliteitsverlies (LO-004).

Stem zelf NOOIT mee. Tel innerlijk tot 7 bij stilte.
-->

---
layout: center
class: text-center
---

# De regel

<div class="text-2xl mt-10 max-w-2xl mx-auto leading-relaxed">
  Stilstand = <span class="font-bold">niet draaien</span><br/>
  tijdens <span class="text-amber-600 font-bold">GEPLANDE productietijd</span>
</div>

<div v-click class="mt-12 text-base opacity-70 max-w-xl mx-auto">
  Pauzes en weekenden zitten <span class="italic">niet</span> in de geplande productietijd.<br/>
  Dus ook niet in de berekening.
</div>

<!--
Vraag eerst: "Wat hebben alle JA-kaartjes gemeen?"
Wacht 5 sec. Laat een deelnemer de regel verwoorden.
Schrijf op het whiteboard met DIENS woorden.

Onthul daarna jouw flap-over uit fase 1:
"Dit is wat de boeken zeggen — komt overeen."

Maak overgang: "Twijfel rond k08 (sensor reset) komt terug in LO-003 — daar valt het onder prestatie.
k11 (eerste stuks afkeur) komt terug in LO-004 — kwaliteit.
Voor nu: vier soorten stilstand voor beschikbaarheid."
-->

---
layout: section
---

# Theoretiseren

## Formule en vier stilstandstypen

<!--
Overgang naar blok 3.
"De vier categorieën uit jullie sortering krijgen nu een naam."
-->

---
layout: center
class: text-center
---

# De formule

<div class="text-3xl mt-10 font-mono">
  <span class="text-blue-600 font-bold">Beschikbaarheid</span>
  <span class="opacity-60 mx-3">=</span>
  <span class="text-green-600 font-bold">Draaitijd</span>
</div>

<div class="text-3xl font-mono">
  <span class="opacity-30">— — — — — — — — — — — — — — —</span>
</div>

<div class="text-3xl font-mono">
  <span class="text-amber-600 font-bold">Geplande productietijd</span>
</div>

<div v-click class="mt-12 text-base opacity-70 max-w-xl mx-auto">
  Geplande productietijd = totale tijd MINUS de geplande pauzes.<br/>
  Draaitijd = geplande productietijd MINUS de stilstand.
</div>

<!--
Spreek elk woord langzaam uit.
Schrijf op flap-over: B = D / GPT.

"Geplande productietijd = de tijd die je had ingepland — dus zonder lunch, zonder weekend.
Draaitijd = de tijd dat hij echt draaide — geplande tijd minus de stilstand."
-->

---

# De vier stilstandstypen

<div class="grid grid-cols-2 gap-6 mt-6">

<div class="p-5 bg-red-50 rounded-lg border-2 border-red-200">

### 🔴 Storing
- Hydraulieklek
- Gereedschapsbreuk
- Elektronische storing
- Motordefect

<div class="text-xs opacity-60 mt-3">k02, k10</div>
</div>

<div class="p-5 bg-amber-50 rounded-lg border-2 border-amber-200">

### 🟡 Omstellen
- Matrijswissel
- Productwissel
- Kleurwissel
- Kalibratie na wissel

<div class="text-xs opacity-60 mt-3">k03</div>
</div>

<div class="p-5 bg-blue-50 rounded-lg border-2 border-blue-200">

### 🔵 Wachten
- Op materiaal / heftruck
- Op gereedschap
- Op operator
- Op TD'er

<div class="text-xs opacity-60 mt-3">k05, k09</div>
</div>

<div class="p-5 bg-purple-50 rounded-lg border-2 border-purple-200">

### 🟣 Opstarten
- Opwarmtijd
- Kalibratie koude start
- Eerste run-in

<div class="text-xs opacity-60 mt-3">k07</div>
</div>

</div>

<!--
Behandel met voorbeelden uit de zojuist gesorteerde kaartjes.
Vraag bij elk type: "Welk kaartje uit jullie sortering hoort hier?"

Verschil omstellen vs opstarten: omstellen = ánder product. Opstarten = zelfde product na koud begin.

MBO-4: SMED (Shingo 1985) verkort omstellen.
-->

---

# Voorbeeld: ponsmachine

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### De situatie
- Dienst: 480 min (8 uur)
- Pauzes: 60 min
- Stilstand: 20 min (afstellen)

</div>

<div>

### De berekening
<v-clicks>

- Geplande tijd: 480 - 60 = **420 min**
- Draaitijd: 420 - 20 = **400 min**
- B = 400 / 420

</v-clicks>

<div v-click class="mt-4 p-3 bg-amber-100 text-amber-900 rounded-lg text-center font-bold text-2xl">
  = 95,2%
</div>

</div>

</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Eén soort stilstand. Eén berekening. Verder niks magisch.
</div>

<!--
Reken hardop voor.
"Ploeg van 8 uur = 480 minuten.
Geplande pauzes 60 minuten — geplande productietijd = 420 minuten.
Stilstand vandaag: 20 minuten afstellen 's ochtends.
Draaitijd = 400 minuten.
Beschikbaarheid = 400 / 420 = 95,2%."

Stilte 3 sec.
-->

---
layout: section
---

# Experimenteren

## Jouw eigen dienst

<!--
Overgang naar blok 4.
Deel werkblad uit.
-->

---

# Stappenplan voor je eigen dienst

<div class="mt-6">

<v-clicks>

1. **Hoe lang was je dienst?** (in minuten)
2. **Trek vaste pauzes eraf** = geplande productietijd
3. **Tel stilstand op per type** (storing / omstellen / wachten / opstarten)
4. **Trek af van geplande tijd** = draaitijd
5. **Deel draaitijd door geplande tijd** = beschikbaarheid

</v-clicks>

<div v-click class="mt-8 text-center text-base opacity-70">
  Schat in blokken van 5 minuten. Preciezer hoeft niet.
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · werkblad eigen dienst
</div>

<!--
Zet timer op 8 min.

Help met aanknooppunten:
- "Hoe lang is je dienst? 8 uur. Wat zijn de vaste pauzes? 60 min. Geplande tijd = 420 min."
- "Hoeveel stilstand schat je? Een kwartier? Een uur?"
- "Welk type was het grootst?"

Bevestig: blokken van 5 min is genoeg.
-->

---
layout: center
class: text-center
---

# Welk type was bij jou het grootst?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Storing, omstellen, wachten of opstarten?<br/>
  En hoeveel minuten ongeveer?
</div>

<div v-click class="mt-12 text-base opacity-60 max-w-md mx-auto">
  Eén zin. Drie tot vier deelnemers.
</div>

<!--
Korte deel-ronde — 2 min.
"Wie wil in één zin vertellen welk type stilstand bij jou het grootst was?"
3-4 deelnemers, max 30 sec per persoon.

Niet alle uitkomsten bespreken — verzamel patronen.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Houd één dienst bij
<v-clicks>

- Per stilstand: starttijd + eindtijd
- Plus type (storing/omstellen/wachten/opstarten)
- Reken aan het eind je beschikbaarheid uit
- Neem het briefje mee

</v-clicks>

</div>

<div>

### Vergelijk
<v-clicks>

- Vraag aan je teamleider:<br/>"is er stilstandsregistratie op de lijn?"
- Vergelijk wat erin staat met wat jij hebt gemeten
- Vaak ontbreken de korte stops
- Daar gaan we volgende workshop op in

</v-clicks>

</div>

</div>

<!--
Sluit af met de transferopdracht.
Volgende workshop: LO-003 over prestatie en korte stops — daar gaan we dieper in op k08-achtige verschijnselen.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">Prestatie — draait hij wel op volle snelheid?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Werkbladen + kaartjes innemen.

Notitie:
- Welke kaartjes leverden meeste discussie? (input voor LO-003)
- Gemiddelde beschikbaarheid van de groep
- Welke twijfelgevallen kwamen vaak terug
-->
