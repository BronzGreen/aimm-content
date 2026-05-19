# Handout: Visuele inspectie met AI
*Deep Learning voor kwaliteitscontrole*

**Naam:** ____________________  **Datum:** __________

---

> **Over deze handout**
> Dit is een samenvatting van hoe AI-kwaliteitscontrole werkt. Volg de uitleg van de trainer. Vul de ontbrekende woorden in.

---

## Hoe werkt het? Drie stappen

| Stap | Wat gebeurt er? | Wie doet het? |
|------|----------------|---------------|
| **Stap 1: Camera-opname** | Een camera maakt een foto van het product | De camera (automatisch) |
| **Stap 2: AI-analyse** | Een AI-model bekijkt de foto | De computer |
| **Stap 3: Beslissing** | Het product is goed, moet terug, of gaat eruit | De computer + operator |

---

## Twee manieren van beoordelen

*Vul het verschil in tussen classificatie en segmentatie:*

| | Classificatie | Segmentatie |
|---|--------------|-------------|
| **Wat doet het?** | Zegt alleen "goed" of "afgekeurd" | Markeert precies _________ het defect zit |
| **Legt het uit waarom?** | _________ | Ja |
| **Wat heeft de voorkeur?** | | _________ |

---

## Data augmentatie

*Soms heb je weinig foto's van defecte producten. Data augmentatie lost dit op.*

**Wat is data augmentatie?**

Je maakt meer trainingsbeelden door ze te veranderen:

- [ ] Spiegelen (links-rechts omdraaien)
- [ ] Stukken weglaten
- [ ] Helderheid aanpassen
- [ ] Draaien

*Hierdoor leert het AI-model beter.*

---

## Voorbeeld uit de praktijk

*(Bron: Cruz et al. 2024, Artificial Intelligence in Manufacturing, pp. 129-131 — U-net segmentatie voor isolatiepanelen.)*

> **Fabrikant van isolatiepanelen**
> Een camera maakt van elk paneel een foto na het frezen. Het AI-model markeert krassen, scheuren en onregelmatigheden. De nauwkeurigheid is 99,5%. Panelen met kleine defecten gaan terug. Beschadigde panelen gaan direct eruit.

*Hoeveel procent haalt het AI-model?* ___________

*Wat doet het systeem bij een klein defect?* ___________________________________

*Wat doet het systeem bij een groot defect?* ___________________________________

---

## Kernbegrippen

| Begrip | Betekenis |
|--------|-----------|
| **Deep learning** | Een soort AI die leert van veel voorbeelden |
| **Classificatie** | Het AI-model zegt alleen goed of fout |
| **Segmentatie** | Het AI-model laat zien waar het defect zit |
| **Data augmentatie** | Meer trainingsbeelden maken door ze te veranderen |
| **Visuele inspectie** | Kwaliteitscontrole met een camera |

---
*Bron: AI Kwaliteitscontrole — Deep Learning | AIMM Module 1: Gebruik | v1.0*
