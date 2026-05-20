# Werkblad: Actieplan modelverbetering

**Leerobject:** Resultaten interpreteren en het model verbeteren
**Kolb-fase:** Experimenteren (2e ronde)
**Type:** Actieplan-werkblad
**Tijd:** 15 minuten

---

## Stap 1: Analyseer de fouten van je model

Kijk terug naar je confusion matrix.

| Vraag | Jouw antwoord |
|---|---|
| Hoeveel **valse alarmen** had je model? | _____ |
| Hoeveel **gemiste defecten** had je model? | _____ |
| Welk type defect miste het model het vaakst? | _________________________ |
| Wat is het grootste probleem? | [ ] Valse alarmen / [ ] Gemiste defecten |

---

## Stap 2: Kies een verbeterstrategie

| Strategie | Wanneer? | Kies je deze? |
|---|---|---|
| **Meer data toevoegen** | Het model mist een specifiek type defect | [ ] Ja |
| **Labels verbeteren** | De labels waren inconsistent (meningsverschillen bij duo-vergelijking) | [ ] Ja |
| **Drempelwaarde bijstellen** | De balans precision/recall klopt niet | [ ] Ja |

**Welke strategie kies je?** _________________________________

**Waarom?** _________________________________________________

---

## Stap 3: Formuleer je verbeteractie

### Als je kiest voor "meer data":

| Vraag | Jouw antwoord |
|---|---|
| Welk type defect voeg je toe? | _________________________ |
| Hoeveel extra foto's maak je? | _____ foto's |
| Wat verandert er in de trainingsset? | _________________________ |

### Als je kiest voor "labels verbeteren":

| Vraag | Jouw antwoord |
|---|---|
| Welke criteria spreken jullie af? | _________________________ |
| Hoeveel labels controleer je opnieuw? | _____ labels |
| Wie controleert mee? | _________________________ |

### Als je kiest voor "drempel bijstellen":

| Vraag | Jouw antwoord |
|---|---|
| Huidige drempelwaarde | _____ |
| Nieuwe drempelwaarde | _____ |
| Verwacht effect op recall | Van _____% naar ~_____% |
| Verwacht effect op precision | Van _____% naar ~_____% |

---

## Stap 4: Test het resultaat

Pas je verbeteractie toe (gebruik het simulatie-werkblad) en bekijk de nieuwe confusion matrix.

### Nieuwe confusion matrix (na verbetering)

|  | Model: GOED | Model: DEFECT | Totaal |
|---|---|---|---|
| **Werkelijk GOED** | _____ | _____ | _____ |
| **Werkelijk DEFECT** | _____ | _____ | _____ |

**Nieuwe precision:** _____% (was: _____%)

**Nieuwe recall:** _____% (was: _____%)

**Is het model verbeterd?** Ja / Nee

**Wat zou de volgende verbeterstap zijn?**

_____________________________________________________________

---

## Pitch voorbereiding (1 minuut)

1. "Het grootste probleem van ons model was: _______________________"
2. "Wij kozen als verbeterstrategie: ______________________________"
3. "Het resultaat: precision ging van _____% naar _____%, recall van _____% naar _____%"
4. "De volgende stap zou zijn: ____________________________________"

---

*AIMM Pipeline | ko-smart-mfg-514 | Werkblad actieplan verbetering*
