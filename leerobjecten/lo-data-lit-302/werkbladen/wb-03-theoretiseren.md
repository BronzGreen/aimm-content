# Datakwaliteit: Drie Criteria
*Datakwaliteit-audit — Theorie-handout*

**Naam:** ____________________  **Datum:** __________

---

> **Kernidee:** Goede data is data die je kunt vertrouwen. Je checkt data op drie punten: is het er allemaal? Klopt het met andere bronnen? Is het up-to-date?

---

## Het audit-framework

| Criterium | Betekenis | Voorbeeld goed | Voorbeeld slecht |
|-----------|-----------|---------------|-----------------|
| **Volledigheid** | Alle data is er. Geen lege velden, geen missende records. | Elke machine heeft een logboek-regel per dienst. | De nachtdienst vult het logboek niet in. |
| **Consistentie** | De data klopt met andere bronnen. Geen tegenspraak. | MES en logboek tonen dezelfde stoptijden. | MES zegt 2 uur stilstand, logboek zegt 30 minuten. |
| **Actualiteit** | De data is recent genoeg voor beslissingen. | Kwaliteitsdata van vandaag. | Excel-bestand van vorige maand. |

---

## Het scoringsschema

*Gebruik deze scores in je audit. Kies per databron en per criterium de juiste score.*

| Score | Betekenis | Wanneer geef je dit? |
|-------|-----------|---------------------|
| **++** | Uitstekend | Data is altijd compleet, klopt altijd, is altijd actueel. |
| **+** | Voldoende | Data is meestal goed. Soms een klein probleem. |
| **-** | Onvoldoende | Data mist vaak, klopt niet altijd, of is regelmatig oud. |
| **--** | Kritiek | Data is structureel onbetrouwbaar. Beslissingen op basis van deze data zijn risicovol. |

---

## Voorbeeld: Audit van een logboek

| Criterium | Score | Waarom? |
|-----------|:-----:|---------|
| Volledigheid | + | Dagdienst vult altijd in. Nachtdienst soms niet. |
| Consistentie | - | Iedereen schrijft storingen anders op. Geen vaste termen. |
| Actualiteit | ++ | Wordt elke dienst ingevuld. |

---

## Veelgemaakte fouten

- **Alles op "++" zetten** -- Wees eerlijk. Iedereen heeft zwakke databronnen.
- **Geen voorbeelden geven** -- Een score zonder reden is niet bruikbaar.
- **Alleen digitale bronnen checken** -- Vergeet het whiteboard en het papieren logboek niet.

---

## Wat onthoud je?

*Schrijf de drie criteria in je eigen woorden op.*

1. Volledigheid = _______________________________________________

2. Consistentie = _______________________________________________

3. Actualiteit = _______________________________________________

---
*Bron: Datakwaliteit-audit framework | AIMM Data Literacy Module 3 | v1.0*
