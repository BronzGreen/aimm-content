# Actieplan: Welke leerklasse past bij ons?
*Vier ML-leerklassen — Eigen organisatie-scan*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Vier ML-leerklassen voor PdM**

---

> **Wat ga je doen?**
> Je hebt nu het framework: vier leerklassen × drie PdM-probleemtypen. Tijd om het op je eigen organisatie te leggen. Zoek één PdM- of monitoring-toepassing waar je AI zou willen inzetten. Beschrijf de data-realiteit eerlijk: hoeveel labels hebben jullie écht? Wat wil je voorspellen? En welke leerklasse past dan?
>
> **Tijd:** 12 minuten.

---

## 🔵 1. Mijn toepassing

**Welke machine of systeem?**

_______________________________________________

**Wat zou je met AI willen doen?**

_______________________________________________

_______________________________________________

---

## 🔵 2. Datasituatie — eerlijk gekeken

*Schat in voor jouw organisatie. "Onbekend" is een waardevolle eerste uitkomst — dat betekent: vraag het na.*

| Vraag | Mijn antwoord |
|-------|---------------|
| Houden we systematisch failure-events bij (datum + machine + oorzaak)? | ○ Ja  ○ Soms  ○ Nee  ○ Onbekend |
| Aantal gelabelde uitvalcases over de afgelopen 1-3 jaar? | ○ 0-10  ○ 10-50  ○ 50-200  ○ > 200  ○ Onbekend |
| Is de oorzaak gecategoriseerd (uitvalmode-codes)? | ○ Ja  ○ Soms  ○ Nee  ○ Onbekend |
| Aantal sensor-meetpunten dat continu draait? | ○ 1-3  ○ 4-10  ○ > 10  ○ Onbekend |

**Mijn data-conclusie:**

○ Veel gelabelde data → supervised mogelijk
○ Weinig gelabeld + veel ongelabeld → semi-supervised
○ Geen labels, alleen sensorstroom → unsupervised
○ Online beslissingen, met feedback → reinforcement
○ Onbekend — eerst inventariseren

---

## 🔵 3. Wat wil je voorspellen?

*Markeer wat het meest van toepassing is.*

| Doel | Probleemtype | Past bij leerklasse |
|------|--------------|---------------------|
| ☐ Een **getal** — RUL, dagen tot volgende uitval, levensduur-percentage | Regression | Supervised |
| ☐ Een **klasse** — welke uitvalmode? gaat hij stuk binnen 100 cycli ja/nee? | Classification | Supervised of semi-supervised |
| ☐ Een **patroon** — welke productiecycli zijn afwijkend? welke machines gedragen zich vergelijkbaar? | Clustering / anomaliedetectie | Unsupervised |
| ☐ Een **beslissing** — uitstellen / doen / vervangen, dynamisch geoptimaliseerd | Beleidsleren | Reinforcement |

---

## 🟠 4. Welke leerklasse past — gegeven jullie data?

*Op basis van het beslisschema uit fase 3.*

**Mijn keuze:** ○ Supervised   ○ Unsupervised   ○ Semi-supervised   ○ Reinforcement

*Onderbouwing in eigen woorden — combineer datasituatie + probleemtype:*

_______________________________________________

_______________________________________________

_______________________________________________

---

## 🟠 5. Past dit — eerlijk gekeken?

| Vraag | Mijn antwoord |
|-------|---------------|
| Is mijn gekozen leerklasse uitvoerbaar gegeven onze data? | ○ Ja  ○ Twijfel  ○ Nee |
| Mist er nog data die we eerst zouden moeten verzamelen? | ○ Ja  ○ Nee  ○ Onbekend |
| Hebben we IT-capaciteit om deze leerklasse te ondersteunen? | ○ Ja  ○ Twijfel  ○ Nee |
| Past dit bij wat de organisatie strategisch belangrijk vindt? | ○ Ja  ○ Twijfel  ○ Nee |

*Mijn oordeel:*

○ We kunnen nu starten   ○ Eerst data verzamelen   ○ Eerst leerklasse-keuze valideren met IT   ○ Idee parkeren

---

## 🟢 6. Concrete acties — deze week

| # | Actie | Wanneer | Met wie | ✓ |
|---|-------|---------|---------|---|
| 1 | Mijn toepassing in 5 zinnen op papier zetten | | | ☐ |
| 2 | Vraag aan onderhoud/IT: registreren we systematisch failures? | | | ☐ |
| 3 | Vraag aan ERP-beheerder: zit er failure-categorisering in onze data? | | | ☐ |
| 4 | Vraag aan leverancier: welke leerklasse vereist jullie aanpak? | | | ☐ |

---

## 🔴 7. Mogelijke obstakels

*Wat zou dit project kunnen tegenhouden?*

_______________________________________________

_______________________________________________

---

## 🟣 8. Een gesprek met onderhoudscollega

> **Praat één keer deze week:** "Houden wij eigenlijk systematisch bij waarom een machine stuk gaat?" Je ontdekt vaak dat de informatie er wel is (logboeken, ERP-vrije tekstvelden) maar niet bruikbaar gestructureerd. Dat is een waardevolle ontdekking voor elk AI-project.

**Met wie ga je praten?** _______________________________________________

**Wat denkt hij/zij?**

_______________________________________________

_______________________________________________

---

## Mijn toepassing — vijf zinnen om mee te nemen

1. **Welke toepassing:** _______________________________________________

2. **Datasituatie eerlijk:** _______________________________________________

3. **Wat ik wil voorspellen (probleemtype):** _______________________________________________

4. **Leerklasse die past:** _______________________________________________

5. **Eerste vraag aan IT, onderhoud of leverancier:** _______________________________________________

---

> 📅 **Volgende sessie:** Neem dit mee. We bespreken kort per deelnemer: wat heb je gevonden? De trainer helpt je een gefundeerde leerklasse-keuze te maken — of te concluderen dat data-verzameling de eerste stap moet zijn.

**Review-datum:** __________  **Buddy/coach:** __________

---
*Bron: Vier ML-leerklassen — AIMM Curriculum | Module 2: Train | v1.0*
