# Handout: Vuistregels voor trainingsdata
*Eigen trainingsdata maken — AI Vision Op Maat*

**Naam:** ____________________  **Datum:** __________

---

> **Kernidee:** Een AI-model leert van foto's. Hoe beter de foto's, hoe beter het model. Met deze 5 vuistregels maak je foto's waar een AI-model goed van kan leren.

---

## De 5 vuistregels

| # | Vuistregel | Waarom? | Voorbeeld |
|---|-----------|---------|-----------|
| 1 | **Vast standpunt** | De camera staat steeds op dezelfde plek. Dan ziet het model steeds hetzelfde beeld. | Markeer de plek met tape. |
| 2 | **Gelijke belichting** | Schaduwen en lichtflitsen maken het model in de war. | Gebruik een lamp. Geen direct zonlicht. |
| 3 | **Schone achtergrond** | Rommel op de achtergrond leidt het model af. | Wit vel papier of grijs doek. |
| 4 | **Genoeg foto's** | Een model heeft veel voorbeelden nodig. Minimaal 50 per categorie. | 3 operators, 3 dagen, 300 foto's. |
| 5 | **Labelcriteria afspreken** | Als iedereen andere regels gebruikt, raakt het model in de war. | Spreek af: wanneer is een kras een defect? |

---

## Voorbeeld uit de praktijk

> Bij een ander bedrijf maakten 3 operators samen een opstelling.
> Ze gebruikten een telefoon, een bureaulamp en een wit vel papier.
> In 3 dagen maakten ze 300 foto's. Eerst spraken ze af:
> - Een kras langer dan 2 mm is een defect.
> - Een vlekje kleiner dan 1 mm is geen defect.
> - Een deuk is altijd een defect.
> Door deze afspraken labelden ze 95% van de foto's hetzelfde.

---

## Hoeveel foto's heb je nodig?

| Situatie | Minimum per categorie | Totaal |
|----------|:---------------------:|:------:|
| Eerste test | 50 goed + 50 defect | 100 |
| Goed model | 150 goed + 150 defect | 300 |
| Meerdere defecten | 100 per type defect | 300+ |

---

## Vergelijk met jullie eigen ervaring

*Welke vuistregel hadden jullie al toegepast?*

- [ ] Vast standpunt
- [ ] Gelijke belichting
- [ ] Schone achtergrond
- [ ] Genoeg foto's
- [ ] Labelcriteria afgesproken

*Welke vuistregel misten jullie?*

_______________________________________________

_______________________________________________

*Wat ga je aanpassen in jullie opstelling?*

_______________________________________________

_______________________________________________

---
*Bron: ko-smart-mfg-522 — Eigen trainingsdata maken | AIMM AI Vision Op Maat | v1.0*
