# Werkblad: Confusion matrix van jouw model

**Leerobject:** Resultaten interpreteren en het model verbeteren
**Kolb-fase:** Experimenteren (1e ronde)
**Type:** Scoringsformulier
**Tijd:** 10 minuten

---

## Jouw confusion matrix

Vul de confusion matrix in op basis van de resultaten van jouw model (de drempelwaarde die je in de vorige activiteit koos).

**Drempelwaarde die jullie kozen:** _____

|  | Model: GOED | Model: DEFECT | Totaal |
|---|---|---|---|
| **Werkelijk GOED** | _____ | _____ | _____ |
| **Werkelijk DEFECT** | _____ | _____ | _____ |
| **Totaal** | _____ | _____ | _____ |

---

## De vier vakken in gewone taal

Vul de aantallen in en lees de uitleg:

| Vak | Aantal | Wat betekent het? |
|---|---|---|
| **Terecht goed** | _____ | Het product is goed en het model zegt goed. Prima! |
| **Vals alarm** | _____ | Het product is goed, maar het model zegt defect. Vervelend! |
| **Gemist defect** | _____ | Het product is defect, maar het model zegt goed. Gevaarlijk! |
| **Terecht defect** | _____ | Het product is defect en het model zegt defect. Prima! |

---

## Precision berekenen

**"Als het model alarm slaat, hoe vaak is het dan echt raak?"**

Precision = terecht defect / (terecht defect + vals alarm)

Precision = _____ / (_____ + _____) = _____ %

---

## Recall berekenen

**"Van alle echte defecten, hoeveel vindt het model er?"**

Recall = terecht defect / (terecht defect + gemist defect)

Recall = _____ / (_____ + _____) = _____ %

---

## Eerste indruk

| Vraag | Jouw antwoord |
|---|---|
| Ben je tevreden met de precision? | Ja / Nee, want: |
| Ben je tevreden met de recall? | Ja / Nee, want: |
| Wat is het grootste probleem: valse alarmen of gemiste defecten? | |

---

*AIMM Pipeline | ko-smart-mfg-513 | Werkblad confusion matrix*
