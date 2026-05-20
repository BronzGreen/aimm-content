# Handout: Drempelwaarden instellen in 4 stappen
*Drempelwaarden instellen — Predictive Maintenance Module 2*

**Naam:** ____________________  **Datum:** __________

---

> **Kernidee:** Een drempelwaarde is de grens waarbij het systeem waarschuwt. Je bepaalt die grens niet op gevoel, maar met data. In 4 stappen stel je betrouwbare drempelwaarden in.

---

## De 4 stappen

| Stap | Wat doe je? | Resultaat |
|:----:|-------------|-----------|
| **1** | **Normaalwaarden meten** — Meet de sensor bij minimaal 100 cycli. De machine draait normaal. | Je hebt 100 meetwaarden. |
| **2** | **Bandbreedte berekenen** — Bereken het gemiddelde en de spreiding. | Je weet wat "normaal" is. |
| **3** | **Drempel instellen** — Stel twee niveaus in: waarschuwing en alarm. | Het systeem weet wanneer het moet waarschuwen. |
| **4** | **Evalueren en bijstellen** — Na 2 weken: tel de alarmen. Stel bij. | De drempel klopt met de praktijk. |

---

## De vuistregel

*Onthoud deze formule. Die gebruik je bij stap 2.*

**Drempel = gemiddelde + 2 x spreiding**

| Begrip | Wat is het? | Voorbeeld |
|--------|-------------|-----------|
| **Gemiddelde** | Alle waarden bij elkaar, gedeeld door het aantal. | 100 metingen opgeteld / 100 = 0.28 mm/s |
| **Spreiding** | Hoe ver de waarden van het gemiddelde afwijken. | De meeste waarden zitten tussen 0.20 en 0.36 mm/s. Spreiding = 0.08 mm/s |
| **Drempel** | De grens. Waarden daarboven zijn afwijkend. | 0.28 + (2 x 0.08) = 0.44 mm/s |

---

## Twee niveaus

*Je stelt altijd twee grenzen in.*

| Niveau | Kleur | Wat betekent het? | Actie |
|--------|:-----:|-------------------|-------|
| **Waarschuwing** | Geel | De waarde is hoger dan normaal. | Extra letten. Check de machine. |
| **Alarm** | Rood | De waarde is veel te hoog. | Direct ingrijpen. Machine stilzetten. |

**Vuistregel voor de twee niveaus:**
- Waarschuwing = gemiddelde + 2x spreiding
- Alarm = gemiddelde + 3x spreiding

---

## Voorbeeld: operator Ahmed

*Lees dit voorbeeld. Je doet straks hetzelfde.*

Ahmed werkt aan de draaibank. Hij stelt drempelwaarden in voor de trillingssensor.

| Stap | Wat doet Ahmed? | Resultaat |
|:----:|-----------------|-----------|
| 1 | Hij meet 100 cycli onder normale omstandigheden. | 100 meetwaarden verzameld. |
| 2 | Hij berekent: gemiddelde = 0.28 mm/s, spreiding = 0.08 mm/s. | Normaal = 0.28 mm/s |
| 3 | Waarschuwing = 0.28 + (2 x 0.08) = **0.44 mm/s**. Alarm = 0.28 + (3 x 0.08) = **0.52 mm/s**. | Twee drempels ingesteld. |
| 4 | Na 2 weken: 3 alarmen, waarvan 2 vals. Hij verhoogt de waarschuwing naar 0.50 mm/s. | Nu 1 alarm per week. Altijd een echt probleem. |

---

## Belangrijk om te weten

- **Te lage drempel** = te veel valse alarmen. Je gaat de meldingen negeren.
- **Te hoge drempel** = je mist echte problemen. De machine valt uit.
- **Bijstellen is normaal.** De eerste drempel is een startpunt. Na 2 weken stel je bij.

---
*Bron: Drempelwaarden instellen — AIMM Predictive Maintenance Module 2 | v1.0*
