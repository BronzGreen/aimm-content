---
werkblad: wb-01
titel: "Drempel-simulatie — drie rondes, drie drempels, drie gevolgen"
behorend_bij: lo-smart-mfg-701-trainee
kolb_fase: ervaren + experimenteren
duur: 25 minuten (verdeeld over blokken 1, 2 en 4)
werkvorm: individueel + duo + individueel
---

# Werkblad 1 — Drempel-simulatie

## Waarom doen we dit?

Op papier is een drempel-keuze makkelijk. In de praktijk voel je pas wat het doet. Dit werkblad geeft je **drie rondes** om het te voelen — eerst intuïtief, dan bewust, dan in context.

---

## De dataset

Hieronder 50 fictieve inspectie-resultaten. Per regel:

- **ID**: foto-nummer
- **Model zegt**: *goed* of *afkeur*
- **Confidence**: hoe zeker het model is (0-100%)
- **Werkelijkheid**: wat het product echt is (goed of defect)

| ID | Model zegt | Conf. | Werkelijkheid |
|----|-----------|-------|---------------|
| 1  | afkeur | 98% | defect |
| 2  | goed   | 95% | goed |
| 3  | afkeur | 87% | defect |
| 4  | goed   | 91% | goed |
| 5  | afkeur | 74% | defect |
| 6  | goed   | 68% | goed |
| 7  | afkeur | 82% | **goed** |
| 8  | goed   | 92% | goed |
| 9  | afkeur | 76% | defect |
| 10 | goed   | 55% | **defect** |
| 11 | afkeur | 94% | defect |
| 12 | goed   | 88% | goed |
| 13 | afkeur | 65% | **goed** |
| 14 | goed   | 72% | goed |
| 15 | afkeur | 89% | defect |
| 16 | goed   | 60% | **defect** |
| 17 | afkeur | 79% | defect |
| 18 | goed   | 97% | goed |
| 19 | afkeur | 71% | defect |
| 20 | goed   | 63% | goed |
| 21 | afkeur | 95% | defect |
| 22 | goed   | 85% | goed |
| 23 | afkeur | 58% | **goed** |
| 24 | goed   | 78% | goed |
| 25 | afkeur | 81% | defect |
| 26 | goed   | 49% | **defect** |
| 27 | afkeur | 93% | defect |
| 28 | goed   | 84% | goed |
| 29 | afkeur | 69% | defect |
| 30 | goed   | 77% | goed |
| 31 | afkeur | 54% | **goed** |
| 32 | goed   | 90% | goed |
| 33 | afkeur | 86% | defect |
| 34 | goed   | 57% | **defect** |
| 35 | afkeur | 80% | defect |
| 36 | goed   | 96% | goed |
| 37 | afkeur | 67% | defect |
| 38 | goed   | 73% | goed |
| 39 | afkeur | 62% | **goed** |
| 40 | goed   | 64% | goed |
| 41 | afkeur | 88% | defect |
| 42 | goed   | 70% | goed |
| 43 | afkeur | 75% | defect |
| 44 | goed   | 83% | goed |
| 45 | afkeur | 51% | **goed** |
| 46 | goed   | 46% | **defect** |
| 47 | afkeur | 97% | defect |
| 48 | goed   | 79% | goed |
| 49 | afkeur | 73% | defect |
| 50 | goed   | 89% | goed |

*De vetgedrukte rijen zijn fouten — waar model en werkelijkheid niet overeenkomen.*

**Context van ronde 1:** je weet niets over het product. Kies intuïtief.

---

## Ronde 1 — Intuïtieve drempel

**Mijn drempel:** ______%

**Regel:** als confidence onder mijn drempel ligt, stuur het systeem de foto door naar mij.

**Tellen — doorloop de dataset:**

| Hoeveel... | Aantal |
|------------|--------|
| ... worden naar mij doorgestuurd (onder drempel)? | _____ |
| ... worden automatisch afgekeurd (boven drempel, model zegt afkeur)? | _____ |
| ... worden automatisch goedgekeurd (boven drempel, model zegt goed)? | _____ |

**Nu de fouten:**

| Hoeveel... | Aantal |
|------------|--------|
| **Vals alarm** automatisch (model zegt afkeur, werkelijkheid goed, boven drempel)? | _____ |
| **Gemist defect** automatisch (model zegt goed, werkelijkheid defect, boven drempel)? | _____ |

**Waarom koos ik deze drempel?**

____________________________________________________

---

## Tussen-reflectie — duo-gesprek (10 min)

Bespreek met je buurman:

- Wat was jouw drempel?
- Hoeveel vals alarm, hoeveel gemist defect?
- Welke keuze zou je in ronde 2 anders maken, nu je dit weet?

**Eén inzicht dat ik uit het gesprek haal:**

____________________________________________________

____________________________________________________

---

## Ronde 2 — Medicatie-inspectie

**Context:** je werkt bij een fabrikant van medicijnen. Het systeem inspecteert pil-blisters op ontbrekende tabletten. Elk gemist defect kan een patiënt treffen — juridisch en ethisch catastrofaal. Vals alarm kost €2 materiaal + 1 minuut controle.

**Nieuwe drempel voor deze context:** ______%

**Tellen (zelfde dataset):**

| | Aantal |
|---|---|
| Vals alarm automatisch | _____ |
| Gemist defect automatisch | _____ |
| Doorgestuurd naar operator | _____ |

**Mijn keuze-motivatie:**

____________________________________________________

____________________________________________________

---

## Ronde 3 — Verpakkingspapier

**Context:** je werkt bij een fabrikant van cadeaupapier. Het systeem inspecteert rollen op kleurafwijkingen. Een gemist defect = de klant krijgt een iets afwijkende kleur (klachten zeldzaam). Vals alarm = een rol van €25 weg.

**Nieuwe drempel voor deze context:** ______%

**Tellen (zelfde dataset):**

| | Aantal |
|---|---|
| Vals alarm automatisch | _____ |
| Gemist defect automatisch | _____ |
| Doorgestuurd naar operator | _____ |

**Mijn keuze-motivatie:**

____________________________________________________

____________________________________________________

---

## Overzicht — alle drie rondes

| | Ronde 1 (intuïtie) | Ronde 2 (medicatie) | Ronde 3 (verpakkingspapier) |
|---|---|---|---|
| Drempel | _____% | _____% | _____% |
| Vals alarm | _____ | _____ | _____ |
| Gemist defect | _____ | _____ | _____ |
| Doorgestuurd | _____ | _____ | _____ |

**Kloppen ronde 2 en 3 bij wat je zou verwachten?**

____________________________________________________

____________________________________________________

**Welke ronde voelde het makkelijkst, welke het moeilijkst? Waarom?**

____________________________________________________

____________________________________________________

---

*Naam: ______________________  |  Datum: ______________________*

*lo-smart-mfg-701-trainee | werkblad 1*
