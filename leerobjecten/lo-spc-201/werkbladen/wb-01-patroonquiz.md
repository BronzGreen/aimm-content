# Patroonquiz: Zie jij het signaal op de kaart?
*Nelson-rules — Lloyd S. Nelson (1984)*

**Naam:** ____________________  **Datum:** __________  
**Module 2 — SPC Train | Workshop: Patroonherkenning op de regelkaart**

---

> **Over dit werkblad**  
> Je krijgt 6 regelkaarten te zien — fictief, maar gebaseerd op echte spuitgiet- en CNC-lijnen. Per kaart vraag je jezelf af: *Zie ik een patroon? Welk patroon precies? Wat zou ik doen?* Je hoeft de officiële Nelson-regelnummers nog niet te weten — beschrijf het patroon in je eigen woorden. Bij twijfel zet je een vraagteken; die kaart bespreken we straks samen.

---

## Hoe lees je de mini-kaarten?

Elke kaart toont een tijdreeks van 12 metingen, met centrumlijn (CL) en de grenzen ±1σ, ±2σ, ±3σ.

```
     +3σ ─────────────────────────  ← UCL (bovengrens)
     +2σ ·························
     +1σ ·························
      CL ─────────────────────────  ← centrumlijn (gemiddelde)
     −1σ ·························
     −2σ ·························
     −3σ ─────────────────────────  ← LCL (ondergrens)
```

Een `●` is een meetwaarde. De positie laat zien op welke hoogte de meting valt.

---

## 🔵 Kaart 1 — Spuitgieten | onderdeelgewicht (g) — IK DOE (voorbeeld)

> *De trainer doet deze kaart voor. Je hoeft hier niets in te vullen — luister mee hoe de trainer hardop denkt.*

```
     +3σ ─────────────────────────────────────────●─  ← punt buiten grens!
     +2σ ······································●·····
     +1σ ····························●···············
      CL ───●────●────●────────────────────────────
     −1σ ········●·····●··············
     −2σ ········································
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

**Trainer-uitleg:**  
*"Ik zie eerst 5 punten netjes rond de centrumlijn — ziet er normaal uit. Maar dan: punt 9 al boven +1σ, punt 10 boven +2σ, en punt 11 vliegt boven +3σ. Dat laatste punt is een **regel 1**: één punt buiten de bovengrens. Eerste actie: meetfout uitsluiten, kijken of er net een matrijswissel of batchwissel was, en het verdachte product apart leggen."*

---

## 🔵 Kaart 2 — Spuitgieten | onderdeelgewicht (g)

```
     +3σ ─────────────────────────────────────────────
     +2σ ························●·····●·············
     +1σ ───●────●────●────●────●────────●────●────●─
      CL ─────────────────────────────────────────────
     −1σ ·············································
     −2σ ·············································
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

*Geen punt valt buiten de grenzen. Maar kijk naar de positie van de punten ten opzichte van de centrumlijn.*

**Zie je een patroon? Beschrijf in eigen woorden:**

_______________________________________________

_______________________________________________

**Wat zou je als eerste doen?**

_______________________________________________

**Antwoord:**  ⚪ Ik zie een patroon   ⚪ Niets opvallends   ⚪ Twijfel (?)

---

## 🔵 Kaart 3 — Spuitgieten | onderdeelgewicht (g)

```
     +3σ ─────────────────────────────────────────────
     +2σ ················································●
     +1σ ··················································
      CL ───●────●────●────●─────────────────────────
     −1σ ··········●·······●··············
     −2σ ········································●·····
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

*Hint: kijk naar de richting van de punten 6 t/m 12.*

```
   waarden:    99,8 → 99,85 → 99,9 → 99,95 → 100,0 → 100,05 → 100,1
                 ↑      ↑      ↑       ↑       ↑       ↑        ↑
              meting 6  7      8       9      10      11       12
```

**Zie je een patroon? Beschrijf in eigen woorden:**

_______________________________________________

_______________________________________________

**Wat zou je als eerste doen?**

_______________________________________________

**Antwoord:**  ⚪ Ik zie een patroon   ⚪ Niets opvallends   ⚪ Twijfel (?)

---

## 🔵 Kaart 4 — CNC-frees | diameter (mm)

```
     +3σ ─────────────────────────────────────────────
     +2σ ─────●────────●────────●────────●────────●──
     +1σ ·············································
      CL ─────────────────────────────────────────────
     −1σ ·············································
     −2σ ──────────●────────●────────●────────●──────
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

*De punten staan afwisselend hoog–laag–hoog–laag. Tussen +2σ en −2σ wisselen ze elkaar af.*

**Zie je een patroon? Beschrijf in eigen woorden:**

_______________________________________________

_______________________________________________

**Wat zou je als eerste doen?**

_______________________________________________

**Antwoord:**  ⚪ Ik zie een patroon   ⚪ Niets opvallends   ⚪ Twijfel (?)

---

## 🔵 Kaart 5 — CNC-frees | diameter (mm)

```
     +3σ ─────────────────────────────────────────────
     +2σ ······························●····●·········
     +1σ ····················●···········●··········●
      CL ───●────●────●────●─────────────────────────
     −1σ ········●·····●·······························
     −2σ ·············································
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

*Hint: 2 van de 3 metingen 7-8-9 vallen voorbij +2σ aan dezelfde kant. Dat is geen toeval.*

**Zie je een patroon? Beschrijf in eigen woorden:**

_______________________________________________

_______________________________________________

**Wat zou je als eerste doen?**

_______________________________________________

**Antwoord:**  ⚪ Ik zie een patroon   ⚪ Niets opvallends   ⚪ Twijfel (?)

---

## 🔵 Kaart 6 — Spuitgieten | onderdeelgewicht (g)

```
     +3σ ─────────────────────────────────────────────
     +2σ ·············································
     +1σ ·······················●····●····●·····●·····
      CL ───●────●────●────●─────────────────────────
     −1σ ········●·····●·······························
     −2σ ·············································
     −3σ ─────────────────────────────────────────────
         1    2    3    4    5    6    7    8    9   10   11   12
```

*Hint: 4 van de laatste 5 metingen (8 t/m 12) vallen voorbij +1σ aan dezelfde kant. Subtieler dan kaart 2 — maar hetzelfde type signaal.*

**Zie je een patroon? Beschrijf in eigen woorden:**

_______________________________________________

_______________________________________________

**Wat zou je als eerste doen?**

_______________________________________________

**Antwoord:**  ⚪ Ik zie een patroon   ⚪ Niets opvallends   ⚪ Twijfel (?)

---

## 🟢 Klaar?

Tel je antwoorden:  
**Patroon gezien:** _____   **Niets opvallends:** _____   **Twijfel (?):** _____

**Welke kaart vond je het lastigst?** Kaart nummer: _____

**Welke kaart vond je het makkelijkst?** Kaart nummer: _____

> **Volgende stap:** Vergelijk je antwoorden met je buurman (5 minuten). Daarna bespreken we plenair de kaarten waar de groep verdeeld was. *Daarna* pakken we de Nelson-handout erbij en koppelen we elke kaart aan een regelnummer. Je hoeft het nu nog niet allemaal goed te hebben — twijfel is leerstof.

---
*Bron: Nelson, L.S. (1984) ‘The Shewhart Control Chart — Tests for Special Causes’, Journal of Quality Technology | NIST/SEMATECH Handbook | AIMM Module 2 — SPC Train | v1.0*
