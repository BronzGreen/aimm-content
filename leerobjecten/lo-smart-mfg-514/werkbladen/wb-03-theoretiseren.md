# Handout: Het model verbeteren in 4 stappen
*Iteratief modelverbeteren -- Computer Vision kwaliteitscontrole*

**Naam:** ____________________  **Datum:** __________
**Module 2 -- Train | Leerobject: Het model verbeteren**

---

> **Kernidee:** Een AI-model is nooit af. Je verbetert het stap voor stap. Je zoekt fouten, voegt data toe, verbetert labels en test opnieuw. Dit heet *iteratief verbeteren*.

---

## De verbetercyclus

| Stap | Wat doe je? | Voorbeeld |
|------|------------|-----------|
| **1. Fouten analyseren** | Bekijk waar het model faalt. Welk fouttype gaat slecht? | Recall krassen 95%, kleurafwijkingen 60% |
| **2. Data toevoegen** | Maak extra foto's van het zwakke fouttype. | 80 extra foto's van kleurafwijkingen |
| **3. Labels verbeteren** | Controleer of de labels kloppen. Corrigeer fouten. | "Goed" was eigenlijk "lichte kras" |
| **4. Hertrainen en testen** | Train het model opnieuw. Test met nieuwe foto's. | Recall kleurafwijkingen stijgt naar 85% |

---

## Belangrijke begrippen

| Begrip | Wat betekent het? |
|--------|------------------|
| **Recall** | Hoeveel fouten vindt het model? (van alle echte fouten) |
| **Precision** | Hoeveel van de gevonden fouten zijn echt? (geen vals alarm) |
| **Iteratief** | Stap voor stap herhalen tot het goed genoeg is |
| **Label** | De naam die je aan een foto geeft: "goed", "kras", "kleurafwijking" |
| **Hertrainen** | Het model opnieuw laten leren met nieuwe of betere data |

---

## Wanneer is het model goed genoeg?

> Een model hoeft niet perfect te zijn. Het moet goed genoeg zijn voor jouw productielijn. Bespreek met je team: welke score is acceptabel?

| Situatie | Minimale recall |
|----------|----------------|
| Veiligheidsproducten | 99% of hoger |
| Cosmetische fouten | 85-95% |
| Interne kwaliteitscheck | 80-90% |

---

## De gouden regel

> Beter data geeft een beter model. Meer data is niet altijd beter. **Gerichte** data wel.

*Voorbeeld:*
- Het model mist kleurafwijkingen.
- Je maakt 80 foto's van kleurafwijkingen.
- Je controleert alle labels.
- Je traint opnieuw.
- De recall stijgt van 60% naar 85%.

---

## Samenvatting

- [ ] Ik begrijp wat recall en precision betekenen
- [ ] Ik snap de vier stappen van de verbetercyclus
- [ ] Ik weet dat een model nooit "af" is
- [ ] Ik begrijp dat gerichte data beter werkt dan meer data

---
*Bron: Iteratief modelverbeteren -- AI Vision kwaliteitscontrole | AIMM Module 2: Train | v1.0*
