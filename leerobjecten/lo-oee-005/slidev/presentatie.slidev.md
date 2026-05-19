---
theme: default
title: OEE berekenen — stap voor stap met een echt voorbeeld
info: |
  ## OEE Module 1 — Gebruik
  Workshop-blok over de volledige OEE-berekening (B × P × K).
  Doelgroep: operators MBO-3, 45 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# OEE berekenen

### Stap voor stap met een echt voorbeeld

<div class="mt-12 text-sm opacity-60">
  OEE Module 1 (Gebruik) · Workshop-blok 5 · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. In de afgelopen vier sessies hadden we de drie componenten apart.
Nu gaan we ze samenbrengen.

Eerst doe IK een voorbeeld voor — jij schrijft mee.
Daarna jij met een buurman op een variant.
Daarna jij alleen op je eigen lijn.

Drie rondes. IK DOE → WIJ DOEN → JIJ DOET.
-->

---

# CNC-freesmachine — situatie

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

### Tijd
- Dienst: **480 min** (8 uur)
- Geplande pauze: **30 min**
- Storing: **25 min** (hydrauliekleak)
- Omstellen: **20 min**

</div>

<div>

### Productie
- Ideale cyclustijd: **2 min/stuk**
- Geproduceerd: **180 stuks**
- Afgekeurd: **5 stuks**
- Herbewerkt: **4 stuks**

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  Schrijf de cijfers bovenaan je werkblad.
</div>

<!--
Lees voor — rustig.
"CNC-freesmachine. Dienst: 8 uur = 480 minuten."
"Geplande pauze: 30 minuten."
"Storing vandaag: 25 minuten — hydraulieklek."
Etc.

"Schrijf deze cijfers bovenaan je werkblad. Even de tijd nemen."
-->

---

# Stap 1 — Beschikbaarheid

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Rekenstap
<v-clicks>

- Geplande tijd = 480 - 30 = **450 min**
- Stilstand = 25 + 20 = **45 min**
- Draaitijd = 450 - 45 = **405 min**
- B = 405 / 450

</v-clicks>

</div>

<div class="flex items-center justify-center">
  <div v-click class="p-6 bg-blue-100 text-blue-900 rounded-xl text-center">
    <div class="text-5xl font-mono font-bold">90,0%</div>
    <div class="text-sm opacity-70 mt-2">Beschikbaarheid</div>
  </div>
</div>

</div>

<!--
Schrijf elke stap op het whiteboard.
Reken-tempo is denk-tempo.

"Geplande productietijd. We trekken de pauze eraf — 480 minus 30 = 450 minuten."
"Stilstand. Storing 25 + omstellen 20 = 45 minuten."
"Draaitijd. 450 minus 45 = 405 minuten."
"Beschikbaarheid = draaitijd gedeeld door geplande tijd. 405 / 450 = 90,0%."
-->

---

# Stap 2 — Prestatie

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Rekenstap
<v-clicks>

- Theoretisch mogelijk = 405 / 2 = **202,5 stuks**
- Werkelijk = **180 stuks**
- Verschil = 22,5 stuks "verdwenen"
- P = 180 / 202,5

</v-clicks>

</div>

<div class="flex items-center justify-center">
  <div v-click class="p-6 bg-purple-100 text-purple-900 rounded-xl text-center">
    <div class="text-5xl font-mono font-bold">88,9%</div>
    <div class="text-sm opacity-70 mt-2">Prestatie</div>
  </div>
</div>

</div>

<div v-click class="mt-6 text-center text-sm opacity-70 italic">
  22,5 stuks verloren door korte stops of langzamer draaien — verborgen fabriek.
</div>

<!--
"Hier komt het anders. We kijken: wat KON de machine maken in 405 min draaitijd?"
"Ideale cyclustijd is 2 min/stuk. 405 / 2 = 202,5 stuks — dat had hij theoretisch kunnen maken."
"Werkelijk: 180 stuks."
"Prestatie = 180 / 202,5 = 88,9%."

Verwijs terug naar LO-003 (verborgen fabriek).
-->

---

# Stap 3 — Kwaliteit

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Rekenstap
<v-clicks>

- Goed in één keer = 180 - 5 - 4 = **171 stuks**
- Totaal geproduceerd = **180 stuks**
- K = 171 / 180

</v-clicks>

</div>

<div class="flex items-center justify-center">
  <div v-click class="p-6 bg-green-100 text-green-900 rounded-xl text-center">
    <div class="text-5xl font-mono font-bold">95,0%</div>
    <div class="text-sm opacity-70 mt-2">Kwaliteit (FPY)</div>
  </div>
</div>

</div>

<!--
"Goed in één keer = 180 - 5 afkeur - 4 herbewerkt = 171 stuks."
"Kwaliteit = 171 / 180 = 95,0%."
-->

---

# Stap 4 — OEE

<div class="grid grid-cols-3 gap-4 mt-8">
  <div class="p-4 bg-blue-100 rounded-lg text-center">
    <div class="text-3xl font-mono font-bold text-blue-700">90,0%</div>
    <div class="text-xs opacity-70">B</div>
  </div>
  <div class="p-4 bg-purple-100 rounded-lg text-center">
    <div class="text-3xl font-mono font-bold text-purple-700">88,9%</div>
    <div class="text-xs opacity-70">P</div>
  </div>
  <div class="p-4 bg-green-100 rounded-lg text-center">
    <div class="text-3xl font-mono font-bold text-green-700">95,0%</div>
    <div class="text-xs opacity-70">K</div>
  </div>
</div>

<div class="text-center mt-8 text-2xl font-mono">
  0,90 × 0,889 × 0,95 = ?
</div>

<div v-click class="mt-8 flex justify-center">
  <div class="p-6 bg-amber-100 text-amber-900 rounded-xl text-center">
    <div class="text-6xl font-mono font-bold">76,0%</div>
    <div class="text-sm opacity-70 mt-2">OEE</div>
  </div>
</div>

<div v-click class="mt-6 text-center text-base opacity-70 italic">
  Drie cijfers boven 88% — samen 76%. Multiplicatie-effect.
</div>

<!--
Wijs naar flap-over: ÷100 → × → × → ×100.
"Drie percentages. Vermenigvuldigen — als decimaal."
"0,90 × 0,889 = 0,800. Keer 0,95 = 0,76. Keer 100 = 76,0%."

Stilte 3 sec na 76%.
"Eén zwakke schakel trekt het hele getal omlaag."
-->

---
layout: section
---

# Reflecteren

## Variant in tweetallen

<!--
Overgang naar blok 2 — WIJ DOEN.
-->

---

# Variant — spuitgietmachine

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

### Tijd
- Dienst: **480 min**
- Pauze: **60 min**
- Storing: **35 min** (matrijswissel)

</div>

<div>

### Productie
- Cyclustijd: **1 min/stuk**
- Output: **350 stuks**
- Afkeur: **8** · Herbewerkt: **12**

</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Vier stappen — zelfde structuur. Reken samen, leg elke stap aan elkaar uit.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  6 min · in tweetallen · werkblad variant
</div>

<!--
Zet timer op 6 min. Loop rond.

Hints (geen voorzeggen):
- Stap 1: "Trek pauze van dienst af."
- Stap 2: "Hoeveel KON hij maken in 385 min draaitijd?"
- Stap 4: wijs naar flap-over decimaal-procent.

Verzamel veelvoorkomende fouten.
-->

---

# Vergelijk met buurpaar

<div class="mt-6">

| Stap | Verwachte uitkomst |
|------|---------------------|
| 1 Beschikbaarheid | **91,7%** |
| 2 Prestatie | **90,9%** |
| 3 Kwaliteit | **94,3%** |
| 4 **OEE** | **78,6%** |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Klopt? Verschil? Loop samen door waar het verschil ontstaat.
</div>

<!--
Plenaire check — 1 min.
Vraag uitkomsten. Schrijf op het bord.
Veelvoorkomende fouten:
- Stilstand niet bij elkaar
- Stap 2 vergelijkt output met geplande tijd
- Stap 4 vermenigvuldigt zonder ÷100
-->

---
layout: section
---

# Theoretiseren

## Waar zit het verbeterpotentieel?

<!--
Overgang naar blok 3.
"We pakken het CNC-voorbeeld weer. Stel: één ding verbeteren — wat doet dat met OEE?"
-->

---

# Scenario-tabel — CNC-voorbeeld

<div class="mt-6">

| Scenario | B | P | K | OEE |
|---|---|---|---|---|
| **Huidig** | 90,0% | 88,9% | 95,0% | **76,0%** |
| Storing halveren | 92,8% | 88,9% | 95,0% | **77,9%** |
| Prestatie naar 95% | 90,0% | **95,0%** | 95,0% | **81,2%** |
| Alles +5pp | 92,8% | 95,0% | 97,5% | **85,8%** |

</div>

<div v-click class="mt-8 text-center text-base opacity-70">
  Welke verbetering geeft de grootste sprong? Waarom?
</div>

<!--
Behandel rij voor rij. Bij elke rij: "Welke verbetering geeft het meeste? Waarom?"

Operator: "storing is gewoon pech."
Daag uit: "Stel het IS aan te pakken — preventief onderhoud. Hoeveel stijgt OEE?"
-->

---
layout: quote
---

# 73% → 86%

<div class="text-xl mt-6 opacity-80">
  Drie keer 90% = <span class="font-bold">73%</span><br/>
  Drie keer 95% = <span class="font-bold">86%</span>
</div>

<div v-click class="mt-8 text-base opacity-70">
  5 procentpunten per component → <span class="font-bold">13 punten op de OEE</span>
</div>

<div v-click class="mt-8 text-sm opacity-50">
  Het zwakste onderdeel domineert het totaal — daar zit per definitie de grootste winst.
</div>

<!--
Hét leerpunt van fase 3.
Stilte. Laat het verschil staan.

"Op je handout: markeer met een ster welk scenario de grootste sprong geeft.
Schrijf in eigen woorden waarom."
-->

---
layout: section
---

# Experimenteren

## JIJ DOET — eigen lijn

<!--
Overgang naar blok 4.
Belangrijkste deel van de sessie.
-->

---

# Jouw eigen OEE

<div class="mt-6">

### Zes getallen voor je laatste dienst
<v-clicks>

1. Geplande productietijd (na pauzes)
2. Totale stilstand
3. Ideale cyclustijd (min/stuk)
4. Output (aantal stuks)
5. Afkeur (aantal)
6. Herbewerkt (aantal)

</v-clicks>

<div v-click class="mt-6 text-center text-base opacity-70">
  Vier stappen → B, P, K, OEE.
</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · individueel · werkblad eigen OEE
</div>

<!--
Zet timer op 10 min. Loop rond.

Help bij blokkades:
- "Hoe lang was je dienst? Trek pauzes eraf."
- "Hoeveel stilstand totaal — schat ruim."
- "Wat is de cyclustijd volgens specificatie?"
- "Hoeveel output - afkeur - herbewerkt?"

Coach 2-3 deelnemers expliciet door alle vier stappen.
-->

---

# STARRT — kort

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

### Vragen
<v-clicks>

- Welke stap was het lastigst?
- Klopte je uitkomst met buurman?
- Welke component is bij jou de zwakste?
- Wat ga je deze week doen om hem 1 procentpunt beter te maken?

</v-clicks>

</div>

<div>

### Tellen
<v-clicks>

- Handen omhoog: B is zwakste
- Handen omhoog: P is zwakste
- Handen omhoog: K is zwakste
- Patroon van de groep zien

</v-clicks>

</div>

</div>

<!--
Plenair, kort — 2 min.
Tel de zwakste-component-handen mee — patroon zien.
Veel B = beschikbaarheidsfocus voor module 2.
Veel P = de verborgen fabriek.
Veel K = kwaliteitsverbetering.
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Werkelijke meting
<v-clicks>

- Volgende dienst: meet werkelijke getallen
- Reken B, P, K, OEE
- Markeer zwakste component
- Bedenk één concrete actie

</v-clicks>

</div>

<div>

### Bonus
<v-clicks>

- Vergelijk met collega op vergelijkbare lijn
- Zelfde getallen?
- Verschillende zwakste componenten?
- Spreek erover

</v-clicks>

</div>

</div>

<!--
Sluit af.
Volgende workshop: LO-006 — alle verliezen, gestructureerd. Zes grote verliezen + Pareto van eigen lijn.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">De zes grote verliezen — waar verlies je productietijd?</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · OEE Module 1 (Gebruik)
</div>

<!--
Bedank de groep.
Notitie:
- Hoeveel deelnemers wezen B / P / K aan als zwakste?
- Welke deelnemers hadden onrealistisch hoge OEE (95%+)?
- Welke deelnemers hadden moeite met stap 2?
-->
