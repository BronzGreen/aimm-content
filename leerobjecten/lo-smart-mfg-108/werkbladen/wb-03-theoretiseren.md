# Handout: SHAP-grafiek lezen
*SHAP-visualisatie — Lundberg & Lee, 2017*

**Naam:** ____________________  **Datum:** __________
**Module 1 — AI gebruiken op de werkvloer**

---

> **Wat is SHAP?**
> SHAP staat voor SHapley Additive exPlanations. Het is een techniek die uitlegt waarom een AI-systeem een melding geeft. SHAP toont per sensor hoe groot de bijdrage is aan het probleem. Grote balk = grote bijdrage.

---

## Zo lees je een SHAP-grafiek

*De SHAP-grafiek is een balkdiagram. Elke balk is een sensor. Hoe langer de balk, hoe meer die sensor bijdraagt aan de anomalie.*

| Stap | Wat doe je? | Voorbeeld |
|------|------------|-----------|
| 1 | Kijk naar de bovenste balk | Die sensor draagt het meest bij |
| 2 | Lees de naam van de sensor | Bijv. "Koelmiddeltemperatuur" |
| 3 | Kijk naar de kleur | Rood = afwijking omhoog. Blauw = afwijking omlaag |
| 4 | Bekijk de top 3 | Die drie sensoren verklaren meestal het probleem |
| 5 | Bepaal je actie | Controleer het systeem van de bovenste sensor |

---

## Drie niveaus van uitleg

*SHAP werkt op drie niveaus. Voor jou als operator is niveau 1 het belangrijkst.*

| Niveau | Vraag | Voor wie? |
|--------|-------|-----------|
| **1. Individueel** | Waarom geeft de machine nu een melding? | Operator |
| **2. Groep** | Welke sensoren werken samen bij dit probleem? | Operator / Teamleider |
| **3. Globaal** | Welke sensoren zijn altijd het belangrijkst? | Teamleider |

---

## Voorbeeld: de Heller 400 CNC-machine

*Dit is een echt voorbeeld. Lees het en beantwoord de vragen.*

De AI geeft een anomaliemelding. De operator opent de SHAP-grafiek. De grafiek toont 76 sensoren. De top 3 zijn:

| Positie | Sensor | Bijdrage |
|---------|--------|----------|
| 1 | Hydraulische druk | Zeer hoog |
| 2 | Hydraulische temperatuur | Hoog |
| 3 | Hydraulische pomp debiet | Gemiddeld |

**Wat is het patroon?**

Alle drie sensoren gaan over het hydraulische systeem.

**Wat doet de operator?**

Hij controleert het hydraulische systeem.

**Hoeveel tijd bespaart dit?**

Zonder SHAP: 45 minuten zoeken. Met SHAP: 12 minuten.

---

## Belangrijke woorden

| Woord | Betekenis |
|-------|-----------|
| **Anomalie** | Iets dat niet normaal is. Een afwijking. |
| **Sensor** | Een meetapparaat op de machine. Meet druk, temperatuur, trillingen of andere dingen. |
| **Bijdrage** | Hoeveel een sensor meehielp aan het signaal. |
| **SHAP-grafiek** | Een balkdiagram dat per sensor de bijdrage toont. |
| **Dashboard** | Het scherm waarop je de gegevens ziet. |

---

## Onthoud dit

- Kijk altijd eerst naar de langste balk.
- De top 3 sensoren vertellen het verhaal.
- Alle sensoren uit hetzelfde systeem? Dan is dat systeem het probleem.
- Je hoeft niet te snappen hoe SHAP rekent. Je hoeft alleen de grafiek te lezen.

---
*Bron: SHAP (SHapley Additive exPlanations) — Lundberg & Lee, 2017 | AIMM Predictive Maintenance | v1.0*
