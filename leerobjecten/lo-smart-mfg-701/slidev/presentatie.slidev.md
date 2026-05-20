---
theme: default
title: Drempel-simulatie — wanneer vertrouw je het AI-oordeel?
info: |
  AIMM × BronzGreen — Module 2: Train, sessie 1
  Leerobject lo-smart-mfg-701-trainee
  Bouwt voort op Module 1 (KO-601, 602, 603)
highlighter: shiki
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Drempel-simulatie

*Wanneer vertrouw je het AI-oordeel?*

<div class="mt-12 text-sm opacity-70">
Module 2: Train &middot; Sessie 1 van 2 &middot; 45 minuten
</div>

---

# Waar stonden we in Module 1?

<div class="mt-8 grid grid-cols-3 gap-4">

<div class="p-4 bg-yellow-50 rounded text-center">
  <div class="font-bold">KO-601</div>
  <div class="text-sm mt-2">Data is de bottleneck</div>
</div>

<div class="p-4 bg-green-50 rounded text-center">
  <div class="font-bold">KO-602</div>
  <div class="text-sm mt-2">5 vakjes + trainingsdata</div>
</div>

<div class="p-4 bg-blue-50 rounded text-center">
  <div class="font-bold">KO-603</div>
  <div class="text-sm mt-2">Synthetische data als antwoord</div>
</div>

</div>

<div class="mt-12 text-center text-xl">
Vandaag: het vakje <strong>"beslissing"</strong> — wat doet het systeem bij twijfel?
</div>

---
layout: center
class: text-center
---

# Nu zelf doen

<div class="mt-8 text-2xl">
50 inspectie-resultaten
</div>

<div class="mt-4 text-2xl">
Kies een drempel
</div>

<div class="mt-4 text-2xl">
Tel wat er gebeurt
</div>

<div class="mt-16 text-lg opacity-70 italic">
Geen theorie eerst. Gewoon beginnen.
</div>

---

# Ronde 1 — intuïtief

<div class="mt-8 text-lg">

**Werkblad 1 erbij.**

Voor elk van de 50 foto's weet je:

- Wat het model zegt *(goed of afkeur)*
- Hoe zeker *(0-100%)*
- Wat de werkelijkheid is *(goed of defect)*

</div>

<div class="mt-12 text-xl">

**Kies:** bij welke confidence-drempel stuur je naar jezelf?

**Tel:** hoeveel vals alarm? Hoeveel gemist defect?

</div>

<div class="mt-8 text-center text-lg text-red-600">
⏱ 15 minuten — individueel
</div>

---
transition: fade
---

# Hoe ging het?

<div class="mt-16 text-2xl">
Welke drempel koos jij? Welke je buurman?
</div>

<div class="mt-8 text-xl opacity-70">
Verschillen zijn niet fouten — ze zijn het bewijs dat drempel-keuze context-gevoelig is.
</div>

<!--
Blok 2 duo-vergelijking. Geen slide-content nodig — flipover doet het werk.
Laat deze slide staan tijdens duo-gesprek.
-->

---

# De logica — twee curves

<div class="flex justify-center mt-4">

```
     100% ┤        Gemist defect ↓                Vals alarm ↑
          │  ▓
          │     ▓▓
Aantal    │        ▓▓
 fouten   │           ▓▓     ●           ░
 per week │              ▓▓░░  ░░░░░░
          │           ░░░░░░░░
          │   ░░░░░░░░
        0 ┼──────────────────────────────
          soepel       drempel         streng
                        ●
              Waar kruist? Bij product X anders dan bij product Y.
```

</div>

<div class="mt-8 text-center text-lg font-bold">
Er is geen universele drempel.
</div>

---

# Ronde 2 — Medicatie

<div class="mt-12 text-xl">

**Context:** pil-blisters op ontbrekende tabletten.

- Gemist defect = patiënt-risico (**catastrofaal**)
- Vals alarm = €2 materiaal + 1 min controle

</div>

<div class="mt-12 text-2xl font-semibold">
Welke drempel kies jij?
</div>

<div class="mt-4 text-lg opacity-70">
Werkblad 1, ronde 2. Zelfde dataset.
</div>

---

# Ronde 3 — Verpakkingspapier

<div class="mt-12 text-xl">

**Context:** rollen cadeaupapier op kleurafwijkingen.

- Gemist defect = lichte afwijking bij klant (klachten zeldzaam)
- Vals alarm = rol van €25 weg

</div>

<div class="mt-12 text-2xl font-semibold">
En nu?
</div>

<div class="mt-4 text-lg opacity-70">
Werkblad 1, ronde 3. Zelfde dataset.
</div>

---

# Samenvatting

<div class="mt-8 text-xl leading-relaxed">

- Drie contexten, drie verschillende drempels
- Zelfde model, zelfde dataset
- **De keuze hangt af van wat elke fout kost**

</div>

<div class="mt-12 text-lg opacity-80">
Module 2 sessie 2 (LO-702): hoe reken je die kosten uit?
</div>

---
layout: center
class: text-center
---

# Voor deze week

<div class="mt-16 text-2xl">
Vraag aan iemand in jullie organisatie:
</div>

<div class="mt-6 text-xl italic">
"Wat is onze drempel-waarde op het AI-inspectiesysteem?"
</div>

<div class="mt-6 text-xl italic">
"Hoe is die gekozen?"
</div>

<div class="mt-16 text-base opacity-60">
Verwacht antwoord: "weet niet" of "standaard". Dat is oké.<br/>
Volgende sessie bouwen we daar op voort.
</div>

---
layout: center
class: text-center
---

# STARRT-reflectie

<div class="mt-12 text-xl">
Werkblad 1 onderaan — individueel afronden.
</div>

<div class="mt-8 text-base opacity-70">
Situatie · Taak · Actie · Resultaat · Reflectie · Transfer
</div>

<div class="mt-16 text-sm opacity-50 italic">
ko-smart-mfg-701 · Module 2: Train · sessie 1 van 2
</div>
