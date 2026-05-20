# Handout: Bagging versus Boosting
*Kolb fase 3: theoretiseren — twee families ensembles met PdM-voorbeelden*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Ensemble Learning**

---

## Over dit werkblad

Dit is je naslagwerk. De trainer loopt het met je door. Jij markeert wat voor jou nieuw is. Aan het einde heb je een mentaal model: **wat is het verschil tussen bagging en boosting, en wanneer past welke familie bij een PdM-probleem?** Dat model gebruik je in de laatste fase om je eigen toepassing te beoordelen.

**Kernidee:** Een ensemble combineert meerdere modellen tot één voorspeller. Er zijn twee hoofdfamilies: **bagging** (parallel) en **boosting** (sequentieel). Wat jullie net deden — drie experts laten stemmen — was een vorm van bagging.

**Tijd:** 14 minuten.

---

## De twee families op één rij

| | **Bagging** | **Boosting** |
|---|------------|---------------|
| **Hoe werkt het?** | Train modellen onafhankelijk op verschillende data-subsets, daarna middelen of stemmen | Train modellen sequentieel — elk model corrigeert de fouten van zijn voorganger |
| **Volgorde** | Parallel — de modellen weten niets van elkaar | Sequentieel — elk model bouwt voort op het vorige |
| **Wat verlaagt het?** | **Variance** (te wisselend antwoord op vergelijkbare data) | **Bias** (structurele afwijking, te eenvoudige modellen) |
| **Bekendste voorbeeld** | Random Forest | Gradient Boosting / AdaBoost |
| **Sterke kant** | Robuust, weinig overfitting, goed bij ruis | Hoge accuracy, kan complexe patronen leren |
| **Risico** | Minder grote sprong in accuracy dan boosting | Overfitting bij te veel iteraties |

---

## Bagging — de drie experts stemmen

> Bij bagging train je elk model op een **bootstrap sample**. Dat is een willekeurige greep uit de data, met teruglegging. Daardoor zien de modellen verschillende data en geven ze verschillende fouten. Bij elkaar opgeteld middelen die fouten elkaar uit.

**Random Forest** = bagging van decision trees:

- Elke boom wordt op een andere bootstrap-sample getraind
- Bij elke split wordt ook nog een willekeurige selectie van features gekozen
- Voorspelling = meerderheidsstem (classificatie) of gemiddelde (regressie)

**Werkvloer-vertaling:** denk aan een **camera-systeem** dat productiebeelden classificeert. Een random forest laat tientallen "stem-bomen" oordelen over één beeld. Elke boom heeft een net andere set trainingsbeelden gezien. Bij twijfel wint de meerderheid. Bij eenduidigheid winnen ze allemaal hetzelfde. Ruis op één boom heeft weinig invloed op het geheel.

> **Aha-moment:** _______________________________________________

---

## Boosting — elke expert leert van de vorige

> Bij boosting train je modellen **één voor één**. Elk nieuw model krijgt een hogere "weging" voor de cases die de voorgangers fout hadden. Daardoor wordt het ensemble steeds beter op de moeilijke gevallen.

**Gradient Boosting / AdaBoost** = sequentieel kleine modellen toevoegen:

- Begin met een eenvoudig model (zwakke leerder)
- Identificeer waar het fout zit
- Train een volgend model dat juist die fouten oppakt
- Combineer alle modellen met gewogen stem

**Werkvloer-vertaling:** denk aan een **storingsclassificatie-systeem** dat in 95% van de gevallen al goed werkt, maar de zeldzame "exotische" storingen mist. Bij boosting wordt elk volgend model getraind met extra aandacht voor precies die gemiste cases. Het ensemble groeit dus richting de moeilijke uithoeken in plaats van het al gemakkelijke midden.

> **Aha-moment:** _______________________________________________

---

## Waarom helpt dit bij PdM?

*PdM-data heeft twee uitdagingen: weinig failure-cases (data-onevenwicht) en heterogene sensors (verschillende soorten signaal). Ensembles vangen dat goed op.*

| PdM-uitdaging | Hoe ensembles helpen |
|---------------|---------------------|
| **Data-onevenwicht** (weinig failures) | Diversiteit van modellen voorkomt dat alleen de meerderheidsklasse geleerd wordt |
| **Sensor-heterogeniteit** (vibratie, temperatuur, druk samen) | Verschillende modellen kunnen verschillende sensor-combinaties belangrijk vinden |
| **Ruis op sensoren** | Bagging middelt de ruis weg |
| **Complexe non-lineaire patronen** | Boosting leert ze stap voor stap aan |

---

## Drie PdM-onderzoekstoepassingen

*Markeer in welke familie elk voorbeeld past.*

| Voorbeeld | Familie |
|-----------|---------|
| **RUL-prognose voor aircraft engines** (Li 2026) — meerdere regressors trainen, voorspellingen middelen, fout daalt door variance-reductie | ○ Bagging  ○ Boosting |
| **Tool wear in dry milling** (Wu et al.) — random forest op vibration-features, robuust bij weinig failure-cases | ○ Bagging  ○ Boosting |
| **Pipe failure prediction** — boosted decision tree, leert sequentieel waar de zeldzame failures zaten | ○ Bagging  ○ Boosting |

---

## Een extra werkvloer-case ter inkleuring

> Een **dashboard** op de werkvloer toont per uur de uitvalkans van vijf kritische machines. Onder de motorkap draaien drie modellen. Eén kijkt naar trillingen, één naar temperatuur, één naar vermogensverloop. Hun voorspellingen worden samengevoegd tot één rangschikking. De planner ziet alleen die rangschikking — niet de drie aparte modellen.

*Welke familie ligt voor de hand bij dit dashboard — en waarom?*

_______________________________________________

_______________________________________________

> **Hint:** drie modellen die onafhankelijk werken en daarna worden samengevoegd, is het patroon van bagging. Boosting zou betekenen: het tweede model probeert specifiek de fouten van het eerste te verbeteren — een ander mechanisme.

---

## En de **voorraad** dan?

> Sommige bedrijven gebruiken een ensemble om dagelijks de **voorraad** aan reserve-onderdelen te schatten. Te veel = duur. Te weinig = stilstand. Een boosted model leert sequentieel waar het voorspeld heeft mis-zat: bestelde te veel motoren in januari, te weinig lagers in mei. Elke ronde bouwt op de fouten van de vorige.

*Welke familie is dit — bagging of boosting? En waarom past dat?*

_______________________________________________

_______________________________________________

---

## Belangrijk om te onthouden

| Begrip | Betekenis |
|--------|-----------|
| **Ensemble** | Meerdere modellen samen één voorspelling laten geven |
| **Zwakke leerder** | Eén losstaand, eenvoudig model — alleen niet sterk |
| **Bagging** | Parallel + middelen → verlaagt variance (Random Forest) |
| **Boosting** | Sequentieel + corrigeren → verlaagt bias (Gradient Boosting) |
| **Bootstrap sample** | Willekeurige greep uit de data, met teruglegging |
| **Variance** | Te wisselend antwoord — model is te gevoelig voor de specifieke trainingsdata |
| **Bias** | Structurele afwijking — model is te eenvoudig om het patroon te vatten |
| **Diversiteit** | De voorwaarde voor ensemble-winst — als alle modellen hetzelfde fout doen, voegt samenvoegen niets toe |

---

## Wat zegt dit over een leverancier-aanbieding?

| Wat de leverancier zegt | Wat dat betekent |
|------------------------|------------------|
| "Wij gebruiken random forest" | Bagging-stijl — robuust, weinig overfitting, makkelijker uit te leggen |
| "Wij gebruiken XGBoost of LightGBM" | Boosting-stijl — vaak hoogste accuracy, gevoeliger voor afstemming |
| "Wij combineren meerdere modellen" | Vraag door: bagging, boosting, of stacking (een derde, complexer mechanisme)? |
| "Wij gebruiken één model" | Geen ensemble — vraag waarom, vooral bij weinig failure-cases |

---

## Controleer jezelf

*Vink aan wat je nu kunt.*

- [ ] Ik kan in eigen woorden uitleggen wat een ensemble is
- [ ] Ik ken het verschil tussen bagging en boosting
- [ ] Ik weet bij welk PdM-probleem ensembles vooral helpen (onevenwicht, heterogene data)
- [ ] Ik kan minstens één voorbeeld per familie noemen (random forest = bagging; gradient boosting = boosting)
- [ ] Ik kan een leverancier-claim toetsen aan een familie

> **Onthoud:** Wat jullie net deden in het diagnose-spel — drie experts laten stemmen — was bagging in het klein. Dat is precies waarom ensembles in PdM-onderzoek consequent betere resultaten leveren dan losse modellen. Maar diversiteit is de voorwaarde: als alle modellen dezelfde fout maken, helpt samenvoegen niets.

---

## Wat doen we hierna?

In de laatste fase pas je dit framework toe op je eigen organisatie. Welke PdM-toepassing heeft jouw lijn? Hoeveel failure-cases zijn er? En welke familie zou passen — bagging of boosting? Houd deze handout dichtbij. De tabellen en het beslisschema gebruik je direct op je actieplan.

---
*Bron: Ensemble Learning — AIMM Curriculum | Module 2: Train | v1.1*
