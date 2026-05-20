# Werkblad: Model configureren — drempelwaarde instellen

**Leerobject:** Trainingsdata labelen en een model configureren
**Kolb-fase:** Experimenteren (2e ronde)
**Type:** Simulatie-werkblad
**Tijd:** 15 minuten

---

## Situatie

Jullie model is getraind op 160 foto's en getest op 40 foto's. De testset bevat 24 goede producten en 16 defecte producten. Hieronder staan de resultaten bij drie verschillende drempelwaarden.

---

## Resultaten bij drempelwaarde 0.3 (streng)

|  | Model: GOED | Model: DEFECT | Totaal |
|---|---|---|---|
| **Werkelijk GOED** | 15 | 9 | 24 |
| **Werkelijk DEFECT** | 1 | 15 | 16 |
| **Totaal** | 16 | 24 | 40 |

- Defecten gevonden: **15 van 16** (recall = ____%)
- Valse alarmen: **9** (precision = ____%)
- Gemiste defecten: **1**

---

## Resultaten bij drempelwaarde 0.5 (gebalanceerd)

|  | Model: GOED | Model: DEFECT | Totaal |
|---|---|---|---|
| **Werkelijk GOED** | 21 | 3 | 24 |
| **Werkelijk DEFECT** | 3 | 13 | 16 |
| **Totaal** | 24 | 16 | 40 |

- Defecten gevonden: **13 van 16** (recall = ____%)
- Valse alarmen: **3** (precision = ____%)
- Gemiste defecten: **3**

---

## Resultaten bij drempelwaarde 0.7 (soepel)

|  | Model: GOED | Model: DEFECT | Totaal |
|---|---|---|---|
| **Werkelijk GOED** | 23 | 1 | 24 |
| **Werkelijk DEFECT** | 6 | 10 | 16 |
| **Totaal** | 29 | 11 | 40 |

- Defecten gevonden: **10 van 16** (recall = ____%)
- Valse alarmen: **1** (precision = ____%)
- Gemiste defecten: **6**

---

## Jullie keuze

Vul in met je duo:

| Vraag | Jullie antwoord |
|---|---|
| Welke drempelwaarde kiezen jullie? | 0.3 / 0.5 / 0.7 |
| Waarom? | |
| Hoeveel defecten vindt het model dan? | _____ van 16 |
| Hoeveel valse alarmen geeft het dan? | _____ |
| Is dat acceptabel voor jullie product? | Ja / Nee, want: |

---

## Bedenk: wat voor product is het?

| Als je product is... | Dan kies je... | Omdat... |
|---|---|---|
| Een veiligheidsonderdeel | Drempel _____ | |
| Een cosmetisch onderdeel | Drempel _____ | |
| Een duur onderdeel | Drempel _____ | |

---

## Pitch voorbereiding (1 minuut)

Bereid samen een korte pitch voor:

1. "Ons product is: _________________________________"
2. "Wij kozen drempelwaarde: _____"
3. "Dat betekent: _____ defecten gevonden, _____ valse alarmen"
4. "Wij vinden dit acceptabel / niet acceptabel omdat: _______________"

---

*AIMM Pipeline | ko-smart-mfg-512 | Werkblad model-configuratie*
