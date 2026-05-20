# Actieplan: Zou een ensemble onze PdM verbeteren?
*Kolb fase 4: experimenteren — eigen organisatie-scan en familie-keuze*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Ensemble Learning**

---

## Over dit werkblad

Je hebt nu het concept ensemble (in fase 1), de reflectie (fase 2) en de bagging/boosting-handout (fase 3) doorlopen. Tijd om het op je eigen lijn te leggen. Zoek één PdM-toepassing die je kent — RUL voorspellen, classificeren van uitvalmodes, anomaliedetectie. Beschrijf de data-uitdaging en kies welke ensemble-familie zou passen.

"Onbekend" is een geldige uitkomst. Vaak betekent het: dit is precies de vraag die je deze week aan IT moet stellen.

**Tijd:** 12 minuten.

---

## 1. Mijn PdM-toepassing

**Welke machine of systeem?**

_______________________________________________

**Wat wordt voorspeld?**

○ RUL (resterende levensduur)
○ Classificatie van uitvalmode (welke fout)
○ Anomalie (afwijkend gedrag)
○ Anders: _______________________________________________

> **Geen eigen PdM op de lijn?** Pak dan een herkenbare toepassing: een sorteersysteem met camera, een storingsclassificatie via het ERP, een dashboard dat anomalieën meldt, of een voorraad-voorspeller voor reserve-onderdelen. Allemaal toepassingen waar de ensemble-vraag direct speelt.

---

## 2. Data-uitdaging

*Vul de data-realiteit van jouw machine in.*

| Vraag | Mijn antwoord |
|-------|---------------|
| Hoeveel failure-cases per jaar (ongeveer)? | ○ 0-5  ○ 5-20  ○ 20-100  ○ > 100  ○ Onbekend |
| Aantal sensors / data-kolommen | ○ 1-3  ○ 4-10  ○ > 10  ○ Onbekend |
| Heterogeniteit (verschillende soorten signaal: vibration + temperatuur + druk)? | ○ Ja  ○ Nee  ○ Onbekend |
| Hebben we nu al een AI-systeem actief? | ○ Ja  ○ Nee  ○ Onbekend |

**Mijn data-situatie samengevat:**

○ **Onevenwichtig** (weinig failures, veel oké) — ensembles voegen veel toe
○ **Evenwichtig** (genoeg failures) — ensembles voegen minder toe
○ **Onbekend** — eerst inventariseren

---

## 3. Welke familie zou passen?

*Op basis van de handout uit fase 3.*

| Mijn situatie | Welke familie ligt voor de hand? |
|---------------|----------------------------------|
| Onevenwichtige, ruisachtige data | **Bagging** (Random Forest) |
| Hoge accuracy nodig, structurele fouten in eenvoudige modellen | **Boosting** (Gradient Boosting) |
| Heterogene sensors, weinig failure-cases | **Bagging** of **Stacking** |
| Sequentiële uitvalpatronen | **Boosting** |

**Mijn keuze:** ○ Bagging   ○ Boosting   ○ Twijfel — beide kandidaat

*Onderbouw kort:*

_______________________________________________

_______________________________________________

---

## 4. Past een ensemble — eerlijk gekeken?

| Vraag | Mijn antwoord |
|-------|---------------|
| Hebben we genoeg gelabelde data voor enige ML? | ○ Ja  ○ Nee  ○ Onbekend |
| Is een enkel model nu al voldoende? | ○ Ja  ○ Nee  ○ Onbekend |
| Is de extra complexiteit van een ensemble haalbaar (rekenkracht, onderhoud)? | ○ Ja  ○ Nee  ○ Onbekend |
| Lossen ensembles ons grootste data-probleem op (onevenwicht, ruis)? | ○ Ja  ○ Nee  ○ Onbekend |

*Mijn oordeel:*  ○ Een ensemble is hier passend   ○ Twijfel — onderzoek nodig   ○ Een enkel model volstaat

---

## 5. Concrete acties — deze week

| # | Actie | Wanneer | Met wie | ✓ |
|---|-------|---------|---------|---|
| 1 | Mijn PdM-toepassing in 5 zinnen op papier zetten | | | ☐ |
| 2 | Vraag aan IT/leverancier: gebruikt het systeem een ensemble of enkel model? | | | ☐ |
| 3 | Vraag aan IT/leverancier: bagging-style of boosting-style? | | | ☐ |
| 4 | Vraag aan IT/leverancier: hoeveel failure-cases hebben we voor training? | | | ☐ |

---

## 6. Mogelijke obstakels

*Wat zou dit gesprek kunnen tegenhouden?*

_______________________________________________

_______________________________________________

---

## 7. Een korte video als geheugensteun

> **Bekijk deze week één keer:** zoek op YouTube naar "random forest explained simple". Je ziet dan letterlijk hoe meerdere decision trees samen stemmen. Dat maakt het concept ensemble nóg tastbaarder.

- [ ] Video bekeken — datum: __________

---

## 8. Een werkvloer-spiegel — voorraad-voorspeller

> **Praat één keer deze week** met iemand van inkoop of magazijn. Vraag hoe de **voorraad** aan reserve-onderdelen geschat wordt. Vaak draait er onder de motorkap al een vorm van model — soms zelfs een ensemble. De vraag "ben jij tevreden over die schatting, en wat zou er beter kunnen?" leidt vaak tot herkenbare data-problemen die exact lijken op die in PdM: weinig failure-cases, heterogene factoren, ruis op signaal.

**Met wie ga je praten?** _______________________________________________

**Wat denkt hij/zij?**

_______________________________________________

_______________________________________________

---

## Mijn PdM-toepassing — vijf zinnen om mee te nemen

1. **Welke toepassing:** _______________________________________________

2. **Data-uitdaging (onevenwicht, heterogeen, etc.):** _______________________________________________

3. **Familie die past (bagging/boosting):** _______________________________________________

4. **Onderbouwing:** _______________________________________________

5. **Eerste vraag aan leverancier of IT:** _______________________________________________

---

## Wat doen we hierna?

> **Volgende sessie:** Neem dit mee. We bespreken kort per deelnemer: wat zegt de leverancier of IT? Past de gekozen aanpak bij de data-uitdaging die je beschreef? De trainer helpt je beoordelen of een ensemble hier echt waarde toevoegt — of dat een eenvoudiger model met betere data minstens zo goed werkt. Beide zijn waardevolle uitkomsten.

**Review-datum:** __________  **Buddy/coach:** __________

---
*Bron: Ensemble Learning — AIMM Curriculum | Module 2: Train | v1.1*
