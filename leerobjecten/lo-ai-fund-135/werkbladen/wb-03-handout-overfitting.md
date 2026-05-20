# Werkblad 3 — Drie signalen en drie tegenmaatregelen
*Overfitting (te-goed-leren) — Theorie-handout*

**Tijdsindicatie:** 12 minuten

---

## Wat is overfitting (te-goed-leren)?

Een model heeft de trainingsdata uit het hoofd geleerd. Het ziet het patroon niet. Op nieuwe data zakt de score.

---

### Drie signalen

#### Signaal 1 — Groot verschil tussen training en test

Trainings-score is hoog. Test-score is veel lager. Het verschil is het signaal. Niet de hoogte.

#### Signaal 2 — Klein dataset met complex model

Weinig voorbeelden. Veel rekenkracht. Het model gaat details onthouden. Geen algemeen patroon leren.

#### Signaal 3 — Model faalt op nieuwe machine of nieuwe batch

Op machine A doet het model het goed. Op machine B niet. Of op een nieuwe batch zakt de score.

---

### Drie tegenmaatregelen

#### Maatregel 1 — Meer voorbeelden

Voorbeeld uit de praktijk. Een model trainde op 50 trillings-voorbeelden van één machine. Het scoorde laag op nieuwe machines. Daarna kwam data van 5 machines erbij. De score op nieuwe machines steeg naar 90%.

#### Maatregel 2 — Simpeler model

Een eenvoudig model heeft minder ruimte om details te onthouden. Het leert het algemene patroon.

#### Maatregel 3 — Cross-validatie (testen op data die het model nog niet zag)

Houd een deel van de data apart. Test het model op die onbekende data. Zo zie je de echte score.

---

### Terug naar de scorekaarten van fase 1

| Model | Trainings-score | Productie-score | Diagnose |
|---|---|---|---|
| A | 99% | 60% | Overfitting — het verschil is groot |
| B | 88% | 86% | Geen overfitting — verschil is klein |

Bron: Russell & Norvig (2021).

---

### Mijn aha-moment

Wat was voor mij nieuw? Markeer dit in de tekst hierboven.

In één zin:

________________________________________________________________

---

### Vakwoorden in dit leerobject

- **Overfitting (te-goed-leren)** — het model heeft de trainingsdata uit het hoofd geleerd.
- **Trainings-score** — score op de data waarop het model leerde.
- **Test-score / productie-score** — score op data die het model niet eerder zag.
- **Cross-validatie** — testen op apart gehouden data.
- **Dataset** — verzameling voorbeelden waaruit het model leert.

---

*AIMM × BronzGreen — AI Fundamentals · Module 1 · Overfitting*
