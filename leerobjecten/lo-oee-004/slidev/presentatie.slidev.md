---
theme: default
title: Kwaliteit — hoeveel is in een keer goed?
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over First Pass Yield, herbewerking en opstartverlies.
  Doelgroep: operators MBO-3, 42 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Kwaliteit

### Hoeveel producten zijn in een keer goed?

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok 4 · 42 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Dit is het derde deel van OEE.
Beschikbaarheid hadden we (draait hij?), prestatie (snel genoeg?), nu kwaliteit.

Maar kwaliteit in OEE is niet wat de meeste operators denken.
We gaan tellen — twee manieren, hetzelfde voorbeeld.
-->

---
layout: section
---

# Ervaren

## Twee manieren tellen

<!--
Overgang naar blok 1.
-->

---

# Eén voorbeeld — twee tellingen

<div class="mt-6">

### De cijfers
- 1000 stuks gemaakt
- 20 stuks afgekeurd
- 30 stuks herbewerkt (en daarna goed)

</div>

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">

### Manier A — eindstand
**(totaal − afkeur) / totaal**
<div class="mt-4 text-3xl font-mono font-bold text-blue-700 text-center">__ %</div>
</div>

<div class="p-6 bg-amber-50 rounded-xl border-2 border-amber-200">

### Manier B — in één keer
**(totaal − afkeur − herbewerkt) / totaal**
<div class="mt-4 text-3xl font-mono font-bold text-amber-700 text-center">__ %</div>
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · werkblad twee tellingen
</div>

<!--
IK DOE — laat de structuur zien op het whiteboard.
Reken NIET zelf — dat is de groep.

Zet timer op 5 min. Loop rond. Help bij blokkades:
- "Trek 20 af van 1000 — wat krijg je?"
- "Deel door 1000 — keer 100 voor het percentage."
-->

---
layout: center
class: text-center
---

# Vergelijk

<div class="grid grid-cols-2 gap-12 mt-10">
  <div>
    <div class="text-sm opacity-60 mb-2">Manier A</div>
    <div class="text-6xl font-mono font-bold text-blue-600">98%</div>
    <div class="text-sm opacity-60 mt-2">eindstand goedkeur</div>
  </div>
  <div>
    <div class="text-sm opacity-60 mb-2">Manier B</div>
    <div class="text-6xl font-mono font-bold text-amber-600">95%</div>
    <div class="text-sm opacity-60 mt-2">in één keer goed</div>
  </div>
</div>

<div v-click class="mt-12 text-xl opacity-80">
  Verschil: <span class="font-bold">3 procentpunten</span>
</div>

<div v-click class="mt-4 text-base opacity-60">
  Lijkt klein. Het is niet klein.
</div>

<!--
Vraag: "Manier A — wie heeft 98%?" Handen.
"Manier B — wie heeft 95%?" Handen.

"Verschil: 3 procentpunten. Lijkt klein. We gaan zien dat het niet klein is."
-->

---
layout: section
---

# Reflecteren

## Wat heeft die herbewerking jou gekost?

<!--
Overgang naar blok 2.
-->

---

# Verborgen kosten

<div class="mt-6">

### Bespreek met je buurman
- Wat moest je er extra voor doen?
- Wie deed het — jij, een collega?
- Hoe lang duurde het?
- Wat had de machine ondertussen kunnen doen?

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Schrijf minimaal drie kostenposten op.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · in tweetallen · werkblad verborgen kosten
</div>

<!--
Zet timer op 5 min. Loop rond.
Stel doorvragen, geen voorzeggen.

Verzamel mentaal 4-5 sterke voorbeelden voor plenaire ronde.
-->

---

# Vier kostenposten

<div class="grid grid-cols-2 gap-6 mt-8">

<div class="p-5 bg-red-50 rounded-lg">

### ⏱️ Extra machinetijd
<v-clicks>

- Machine had nieuwe producten kunnen maken
- Capaciteit weg

</v-clicks>

</div>

<div class="p-5 bg-orange-50 rounded-lg">

### 👤 Extra arbeid
<v-clicks>

- Iemand moet nabewerken
- Vaak buiten lijn-tempo

</v-clicks>

</div>

<div class="p-5 bg-yellow-50 rounded-lg">

### 📦 Extra materiaal
<v-clicks>

- Soms gaat materiaal verloren
- Bewerking kost grondstof

</v-clicks>

</div>

<div class="p-5 bg-purple-50 rounded-lg">

### ✅ Extra controle
<v-clicks>

- QC moet opnieuw beoordelen
- Risico op missen blijft

</v-clicks>

</div>

</div>

<!--
Vraag: "Wat heb je opgeschreven?"
Schrijf elke kostenpost op flap-over.

Verwacht en stuur: machinetijd, arbeid, materiaal, controle.
Als groep er twee noemt: schrijf de andere twee zelf erbij — "En vergeet ook niet..."

"Drie procent verschil — dat zijn 30 stuks die jou geld en tijd kosten,
maar de klant niet ziet. Dat is het verschil tussen eindstand en FPY."
-->

---
layout: section
---

# Theoretiseren

## FPY en drie verliestypen

<!--
Overgang naar blok 3.
-->

---
layout: center
class: text-center
---

# First Pass Yield

<div class="text-3xl mt-10 font-mono">
  <span class="text-amber-600 font-bold">FPY</span>
  <span class="opacity-60 mx-3">=</span>
  <span class="text-green-600 font-bold">Goed in één keer</span>
</div>

<div class="text-3xl font-mono">
  <span class="opacity-30">— — — — — — — — — — — —</span>
</div>

<div class="text-3xl font-mono">
  <span class="text-blue-600 font-bold">Totaal geproduceerd</span>
</div>

<div v-click class="mt-12 text-base opacity-70 max-w-xl mx-auto">
  In OEE is kwaliteit altijd FPY.<br/>
  Herbewerking telt als verlies — ook als het uiteindelijk goedkomt.
</div>

<!--
"First Pass Yield — Engels voor 'goed in eerste poging'.
Strenger dan eindstand goedkeur."

Schrijf op flap-over: FPY = goed-1e-keer / totaal.
-->

---

# Drie kwaliteitsverliestypen

<div class="mt-6">

| Type | Wat het is | Voorbeeld |
|---|---|---|
| **🔴 Afkeur** | Niet te redden | Scheur, verkeerde maat, breuk |
| **🟡 Herbewerking** | Moet opnieuw bewerkt | Nabramen, opnieuw lassen |
| **🟢 Opstartverlies** | Eerste stuks niet goed | Spuitgietmachine moet eerst op temp |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Wie herkent welke op zijn lijn?
</div>

<!--
Behandel elk type — vang per type 1 voorbeeld uit groep.
"Wie herkent afkeur?" "Wie herkent herbewerking?" "Wie herkent opstartverlies?"
-->

---
layout: quote
---

# 3900 stuks per jaar

<div class="text-xl mt-6 opacity-80">
  Spuitgieten — 15 stuks opstartverlies per dag<br/>
  × 5 dagen × 52 weken
</div>

<div v-click class="mt-8 text-base opacity-70">
  <span class="font-bold">Per lijn.</span> Vind een truc — voorverwarmen,<br/>
  eerste stuks apart — en je wint <span class="font-bold">800 stuks per jaar</span>.
</div>

<div v-click class="mt-8 text-sm opacity-50">
  Zonder dat de klant er iets van merkt.
</div>

<!--
Stilte 3 sec na 3900.
Maak het uitdaging, geen schuldgevoel.
"Hier zit ruimte voor jou als operator om iets te WINNEN."
-->

---
layout: section
---

# Experimenteren

## Jouw eigen FPY

<!--
Overgang naar blok 4.
-->

---

# Stappenplan voor je eigen lijn

<div class="mt-6">

<v-clicks>

1. **Hoeveel stuks** heb je vorige week ongeveer gemaakt?
2. **Afkeur** — een paar stuks of een paar procent?
3. **Herbewerkt** — schat ruim
4. **Opstartverlies** — eerste stuks per dag × 5
5. **Trek alle drie af, deel door totaal** = FPY

</v-clicks>

<div v-click class="mt-8 text-center text-base opacity-70">
  Schat in tientallen. Bewustwording, geen precisie.
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · werkblad eigen FPY
</div>

<!--
Zet timer op 8 min.

Help bij blokkades:
- "Hoeveel per dag × 5 dagen?"
- "Afkeur in stuks of in procenten?"
- "Hoeveel opstartverlies?"

Bevestig: bewustwording, geen precisie.
-->

---
layout: center
class: text-center
---

# Welk verliestype was bij jou het grootst?

<div class="text-2xl mt-10 max-w-xl mx-auto leading-relaxed opacity-80">
  Afkeur, herbewerking of opstart?<br/>
  En welke actie zou je willen proberen?
</div>

<!--
Korte deel-ronde — 1 min 30.
3-4 deelnemers, max 30 sec per persoon.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Houd één dienst bij
<v-clicks>

- Totaal aantal
- Afkeur
- Herbewerkt
- Opstartverlies
- Reken FPY uit

</v-clicks>

</div>

<div>

### Vergelijk + vraag
<v-clicks>

- Vergelijk met het kwaliteitsbord
- Staat herbewerking daar?
- Vraag een collega van een andere lijn
- "Hoe gaan jullie om met opstartverlies?"

</v-clicks>

</div>

</div>

<!--
Sluit af.
Volgende workshop: LO-005 — alles samen, OEE berekenen stap voor stap.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">OEE berekenen — stap voor stap met een echt voorbeeld</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Notitie:
- Welke verliesposten kwamen het meest voor? (input voor LO-005)
- Hoeveel sceptici waren er over herbewerking?
- Welke deelnemers waren het meest gemotiveerd na 3900-getal?
-->
