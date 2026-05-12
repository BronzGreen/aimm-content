# Regelkaart lezen: stabiel of onstabiel?
*Wat staat er op die grafiek bij mijn machine?*

**Naam:** ____________________  **Datum:** __________
**Module 1 — SPC Gebruik | Workshop: Regelkaart-fundament**

---

> **Over dit werkblad**
> Je krijgt drie korte regelkaart-fragmenten. Elk fragment laat een stuk van een lopend proces zien: de centrale lijn (CL), de bovengrens (UCL), de ondergrens (LCL) en de meetpunten in de volgorde waarin ze zijn gedaan. Jouw taak: aanvinken of het proces er **stabiel** (voorspelbaar) of **onstabiel** (onvoorspelbaar) uitziet. Bij twijfel: vraagteken zetten en kort noteren waarom.

---

## Snelle herinnering

| **Stabiel (voorspelbaar) =** | **Onstabiel (onvoorspelbaar) =** |
|------------------------------|----------------------------------|
| Punten schommelen willekeurig rond de centrale lijn | Eén of meer punten buiten UCL of LCL |
| Alles binnen UCL/LCL | Duidelijke trend (structureel omhoog of omlaag) |
| Geen lange reeks aan één kant | Cluster: 7 of meer op rij aan één kant |
| Geen rare patronen | Een onwaarschijnlijk patroon |

Volgens ASQ en ISO 7870-1/-2 is dit de kerntaak van een regelkaart: beoordelen of variatie consistent is of niet (bron: ASQ — Control Chart; ISO 7870-1, ISO 7870-2).

---

## 🔵 Fragment 1 — Spuitgietlijn, onderdeelgewicht

*Fictieve illustratie ter oefening. Meting: gemiddeld onderdeelgewicht per uur, in gram.*

```
      UCL ─────────────────────────── 100,3
             •
                 •     •
CL   ─────•─────────•─────•──────── 100,0
                •           •   •
                    •
      LCL ─────────────────────────── 99,7

      tijd →  1   2   3   4   5   6   7   8
```

**Wat zie je?** Punten schommelen rond de centrale lijn van 100,0 g. Geen punt komt boven 100,3 of onder 99,7. Geen duidelijke trend.

**Antwoord:**  ⚪ Stabiel   ⚪ Onstabiel   ⚪ Twijfel (?)

*Waarom? (1 zin):* _______________________________________________

_______________________________________________

---

## 🔵 Fragment 2 — CNC-frees, diameter-meting

*Fictieve illustratie ter oefening. Meting: gemiddelde diameter per meetronde, in mm.*

```
      UCL ─────────────────────────── 25,04
                                  •
                              •
                          •
CL   ─────────────────•───────────── 25,00
                  •
              •
          •
      LCL ─────────────────────────── 24,96

      tijd →  1   2   3   4   5   6   7   8
```

**Wat zie je?** De diameters kruipen van onderaan de centrale lijn structureel omhoog. Punt 8 zit dicht tegen UCL. Niet willekeurig — er is richting in.

**Antwoord:**  ⚪ Stabiel   ⚪ Onstabiel   ⚪ Twijfel (?)

*Waarom? (1 zin):* _______________________________________________

_______________________________________________

---

## 🔵 Fragment 3 — Verpakkingslijn, vulgewicht

*Fictieve illustratie ter oefening. Meting: vulgewicht per doos per uur, in gram.*

```
      UCL ─────────────────────────── 502
          •
              •       •
CL   ─────────────•───────•───•───── 500
                                  •
                                          •
                                              •×  (506)
      LCL ─────────────────────────── 498

      tijd →  1   2   3   4   5   6   7   8
```

**Wat zie je?** De eerste zes punten schommelen netjes rond de centrale lijn. Punt 8 springt naar 506 gram — ruim boven UCL van 502.

**Antwoord:**  ⚪ Stabiel   ⚪ Onstabiel   ⚪ Twijfel (?)

*Waarom? (1 zin):* _______________________________________________

_______________________________________________

---

## 🟢 Klaar?

Tel je antwoorden:
**Stabiel:** _____   **Onstabiel:** _____   **Twijfel (?):** _____

**Korte samenvattingsvraag:** Welk van de drie componenten op een regelkaart (centrale lijn, UCL/LCL, of punten in tijd) gebruikte jij het meest bij het beoordelen?

_______________________________________________

_______________________________________________

> **Volgende stap:** Vergelijk je antwoorden kort met je buurman. Daarna bespreken we plenair de fragmenten waar de groep verdeeld is. Niet erg als je nog twijfelt — we zijn dit net gaan leren.

---
*Bron: Shewhart, W.A. (1931); ASQ — Control Chart; ISO 7870-1, ISO 7870-2 | AIMM Module 1 — SPC Gebruik | v1.0*
