---
theme: default
title: Het patroon van elk AI-camerasysteem
info: |
  AIMM × BronzGreen — Module 1: Gebruik
  Leerobject lo-smart-mfg-602-trainee
  Voor MBO-3 operators
  Vervolgt op lo-smart-mfg-601
highlighter: shiki
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Het patroon van elk AI-camerasysteem

*Vier vakjes die je overal herkent*

<div class="mt-12 text-sm opacity-70">
Module 1: Gebruik &middot; 40 minuten &middot; Na `lo-601 data-bottleneck`
</div>

---

# Wat leerden we vorige keer?

<div class="mt-12 text-3xl font-bold text-red-500">
Het model is niet het probleem.
</div>

<div class="mt-4 text-3xl font-bold">
Jouw data is het probleem.
</div>

<div class="mt-16 text-xl opacity-70">
Vandaag: hoe herken je de rest van het systeem?
</div>

---
layout: center
class: text-center
---

# Het patroon

<div class="mt-8 text-3xl font-mono">
CAMERA → BEELD → MODEL → BESLISSING
</div>

<div class="mt-16 text-lg opacity-60">
Vier zichtbare stappen. Plus één die je niet ziet.
</div>

<!--
Teken dit op de flipover terwijl je de slide laat zien. Schrijvend
uitleggen werkt beter dan projecteren.
-->

---

# En dan dit — onzichtbaar maar cruciaal

<div class="grid grid-cols-2 gap-8 mt-8">

<div>

```
CAMERA → BEELD → MODEL → BESLISSING
                    ▲
                    │
           TRAININGSDATA
          (gelabelde foto's)
```

</div>

<div class="text-lg pt-8">

**Eenmalig** vóór het systeem live ging.

**Maar:** als die stap niet goed was, zie je dat **elke dag** terug.

</div>

</div>

---

# Vijf vakjes, vijf faalpunten

| Vakje | Wat kan stuk? | Vraag |
|-------|---------------|-------|
| Camera | Vuil, licht, trillingen | *Wanneer schoongemaakt?* |
| Beeld | Resolutie, uitsnede | *Zien we hetzelfde als 't model?* |
| Model | Niet bijgetraind | *Wanneer laatste update?* |
| Beslissing | Drempel scheef | *Wat doet 't bij twijfel?* |
| Trainingsdata | Te klein of oud | *Welke foto's en wie labelde?* |

---

# Case A — samen

<div class="mt-12 text-2xl leading-relaxed">

De inspectiecamera boven lopende band 3
keurt sinds vanochtend <span class="font-bold text-red-500">3× zoveel</span> producten af.

Ze zien er voor het oog goed uit.

</div>

<div class="mt-16 text-xl italic opacity-70">
Waar check je als eerste?
</div>

<!--
Start plenair. Noteer antwoorden op flipover bij het juiste vakje.
-->

---

# Case B — in duo's

<div class="mt-8 text-xl leading-relaxed">

Klachten uit de keten: <span class="font-bold">krassen bij de klant</span>
die de camera doorlaat.

De camera keurt de normale afkeuringen netjes af.

Deze specifieke krassen glippen erdoorheen.

</div>

<div class="mt-12 text-lg opacity-70">
Gebruik werkblad 2. Zeven minuten.
</div>

---

# Case C — in duo's

<div class="mt-8 text-xl leading-relaxed">

Nieuwe leverancier van plastic kapjes sinds gisteren.
Kapjes zijn functioneel gelijk, maar een
<span class="font-bold">tint donkerder</span>.

De camera keurt sindsdien veel meer af.

</div>

<div class="mt-12 text-lg opacity-70">
Kies: B of C. Zeven minuten.
</div>

---
transition: fade
---

# Reflectie

<div class="mt-16 text-3xl">
Welk vakje was het lastigst?
</div>

<div class="mt-6 text-3xl">
Waar twijfelden jullie het meest?
</div>

<div class="mt-16 text-xl opacity-70 italic">
Vaak is het saaiste vakje het belangrijkste in de praktijk.
</div>

---

# Jouw werkvloer — vijf vragen

<div class="mt-8 text-2xl">

Kies **één** systeem dat je kent.

Formuleer **vijf vragen** — één per vakje.

</div>

<div class="mt-12 text-lg">

> Niet: *"werkt dit goed?"*

> Wel: *"wanneer is de lens voor het laatst schoongemaakt?"*

</div>

<div class="mt-12 text-lg text-red-600 font-semibold">
Werkblad 4. Vijf minuten. Daarna één vraag delen.
</div>

---
layout: center
class: text-center
---

# Vier vakjes + één onzichtbaar + vijf vragen

<div class="mt-16 text-2xl">
Dat is alles.
</div>

<div class="mt-16 text-lg opacity-60">
Volgende keer: Module 2 — Train.<br/>
Daar maak je zelf een systeem dat dit patroon heeft.
</div>
