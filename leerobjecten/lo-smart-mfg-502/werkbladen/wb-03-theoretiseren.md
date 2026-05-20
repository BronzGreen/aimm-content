# Handout: Vier Criteria voor Datakwaliteit
*Data-audit — Predictive Maintenance Module 3: Op Maat*

---

> **Kernboodschap:** Goede data is de basis voor een goed model. Slechte data levert slechte voorspellingen. Met deze vier criteria beoordeel je of jouw data goed genoeg is.

---

## De vier criteria

| Criterium | Wat betekent het? | Voorbeeld uit de fabriek | Waarom belangrijk? |
|-----------|------------------|------------------------|-------------------|
| **Volledigheid** | Geen grote gaten in de data | Je sensor meet elke 5 minuten. Maar in juli is er een week geen data. Dat is een gat. | Het model leert van patronen. Als er gaten zijn, mist het model informatie. |
| **Consistentie** | De sensor meet steeds op dezelfde manier | Je trillingssensor meet in mm/s. Maar na een update meet hij ineens in g. Dat is niet consistent. | Als de eenheid verandert, denkt het model dat de machine anders draait. |
| **Nauwkeurigheid** | Wat de sensor meet klopt met de werkelijkheid | Je temperatuursensor zegt 40 graden. Maar als je met een thermometer meet is het 55 graden. Dat klopt niet. | Een onnauwkeurige sensor geeft verkeerde signalen aan het model. |
| **Tijdstempel** | Bij elk meetpunt staat een datum en tijd | Je data heeft een tijdstempel per seconde. Zo weet je precies wanneer iets veranderde. | Zonder tijdstempel weet je niet wanneer een afwijking begon. |

---

## Hoeveel data heb je nodig?

| Hoeveelheid | Geschikt? | Toelichting |
|-------------|----------|-------------|
| Minder dan 1 maand | Nee | Te weinig om patronen te herkennen. |
| 1 tot 3 maanden | Misschien | Genoeg voor een eerste test. Niet voor een betrouwbaar model. |
| **3 maanden of meer** | **Ja** | Genoeg om seizoenspatronen en slijtage te zien. |
| 6 maanden of meer | Zeer goed | Hoe meer data, hoe beter het model leert. |

---

## Veelvoorkomende problemen

| Probleem | Wat je ziet | Wat je kunt doen |
|----------|-----------|-----------------|
| **Gaten in de data** | Dagen of weken zonder meetpunten | Check of de sensor aan stond. Vraag de technische dienst. |
| **Verkeerde eenheden** | Waarden die ineens heel anders zijn | Check of er een update of kalibratie is geweest. |
| **Geen tijdstempel** | Data zonder datum en tijd | Vraag of de PLC een klok heeft. Soms moet je die instellen. |
| **Data niet bewaard** | De PLC overschrijft oude data | Vraag of de data naar een server kan worden gestuurd. |

---

## Checklist: is mijn data goed genoeg?

- [ ] Ik heb minimaal 3 maanden data
- [ ] Er zitten geen grote gaten in de data
- [ ] De sensor meet steeds in dezelfde eenheid
- [ ] De meetwaarden kloppen met de werkelijkheid
- [ ] Bij elk meetpunt staat een datum en tijd
- [ ] De data bevat ook momenten met storingen

*Kun je alle vakjes aanvinken? Dan ben je klaar voor een pilot.*
*Kun je niet alles aanvinken? Gebruik het actieplan om de gaten te dichten.*

---
*Bron: Data-audit framework — AIMM Predictive Maintenance | Module 3: Op Maat | v1.0*
