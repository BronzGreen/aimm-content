# Handout: Gevoeligheid van een vision-model
*Vision-model configureren — AI Vision voor Kwaliteitscontrole*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train: Zelf configureren**

---

> **Over deze handout**
> Dit is een samenvatting van de theorie. Bewaar dit blad. Je kunt het later gebruiken als je zelf een model instelt.

---

## Wat is een drempelwaarde?

Een drempelwaarde (ook: threshold) is een getal tussen 0 en 1. Het bepaalt hoe streng het vision-model kijkt naar producten.

- **Lage drempelwaarde (bijv. 0.3)** = het model is streng. Het keurt snel af. Gevolg: veel valse alarmen, weinig gemiste fouten.
- **Hoge drempelwaarde (bijv. 0.7)** = het model is soepel. Het laat meer door. Gevolg: weinig valse alarmen, meer gemiste fouten.

---

## Twee soorten fouten

| Fout | Wat gebeurt er | Ander woord | Gevolg |
|------|---------------|-------------|--------|
| **Vals alarm** | Een goed product wordt afgekeurd | False positive | Verspilling, stilstand |
| **Gemist defect** | Een slecht product gaat door | False negative | Klacht, terugroep, schade |

---

## De afweging

Er is geen "perfecte" instelling. Je moet altijd kiezen:

| Strenger (lage drempel) | Soepeler (hoge drempel) |
|:-----------------------:|:-----------------------:|
| Meer valse alarmen | Minder valse alarmen |
| Minder gemiste defecten | Meer gemiste defecten |
| Meer stilstand | Minder stilstand |
| Hogere kwaliteit | Lagere kosten |

---

## Voorbeeld uit de praktijk

*Fictief rekenvoorbeeld — plausibele drempelwaarde-tradeoffs voor een camera-inspectie op kunststof, niet een specifieke casus.*

Een fabriek maakt plastic onderdelen. Ze gebruiken een camera om krassen te vinden.

| Drempelwaarde | Recall (gevonden defecten) | Valse alarmen |
|:-------------:|:--------------------------:|:-------------:|
| 0.3 | 95% | 40% |
| 0.5 | 85% | 10% |
| 0.7 | 70% | 0% |

De fabriek kiest 0.5. Reden: 85% van de fouten wordt gevonden. En ze hebben niet te veel stilstand door valse alarmen.

---

## Drie begrippen om te onthouden

| Begrip | Betekenis | Voorbeeld |
|--------|-----------|-----------|
| **Drempelwaarde** | Hoe streng het model kijkt | 0.3 = streng, 0.7 = soepel |
| **Recall** | Hoeveel fouten het model vindt | 85% = 85 van de 100 fouten gevonden |
| **Testset** | Een set foto's om het model te testen | 100 foto's: 50 goed, 50 fout |

---

## Wanneer kies je welke instelling?

| Situatie | Kies | Waarom |
|----------|------|--------|
| Veiligheid is belangrijk (bijv. medisch) | Streng (0.3) | Je wilt geen enkel defect missen |
| Kosten zijn belangrijk | Soepel (0.7) | Je wilt niet te veel weggooien |
| Balans tussen kwaliteit en kosten | Gemiddeld (0.5) | Goede balans |

---
*Bron: Vision-model configuratie — AI & Data Literacy | AIMM Module 2: Train | v1.0*
