# Handout: Bagging versus Boosting
*Ensemble Learning — Twee families, twee strategieën*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Ensemble Learning**

---

> **Kernidee:** Een ensemble combineert meerdere modellen tot één voorspeller. Er zijn twee hoofdfamilies: **bagging** (parallel) en **boosting** (sequentieel). Wat jullie net deden — drie experts laten stemmen — was een vorm van bagging.

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

> Bij bagging train je elk model op een **bootstrap sample** — een willekeurige greep uit de data, met teruglegging. Daardoor zien de modellen verschillende data en geven ze verschillende fouten. Bij elkaar opgeteld middelen die fouten elkaar uit.

**Random Forest** = bagging van decision trees:
- Elke boom wordt op een andere bootstrap-sample getraind
- Bij elke split wordt ook nog een willekeurige selectie van features gekozen
- Voorspelling = meerderheidsstem (classificatie) of gemiddelde (regressie)

> **Aha-moment:** _______________________________________________

---

## Boosting — elke expert leert van de vorige

> Bij boosting train je modellen **één voor één**. Elk nieuw model krijgt een hogere "weging" voor de cases die de voorgangers fout hadden. Daardoor wordt het ensemble steeds beter op de moeilijke gevallen.

**Gradient Boosting / AdaBoost** = sequentieel kleine modellen toevoegen:
- Begin met een eenvoudig model (zwakke leerder)
- Identificeer waar het fout zit
- Train een volgend model dat juist die fouten oppakt
- Combineer alle modellen met gewogen stem

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

---

## Controleer jezelf

*Vink aan wat je nu kunt.*

- [ ] Ik kan in eigen woorden uitleggen wat een ensemble is
- [ ] Ik ken het verschil tussen bagging en boosting
- [ ] Ik weet bij welk PdM-probleem ensembles vooral helpen (onevenwicht, heterogene data)
- [ ] Ik kan minstens één voorbeeld per familie noemen (random forest = bagging; gradient boosting = boosting)

> **Onthoud:** Wat jullie net deden in het diagnose-spel — drie experts laten stemmen — was bagging in het klein. Dat is precies waarom ensembles in PdM-onderzoek consequent betere resultaten leveren dan losse modellen.

---
*Bron: Ensemble Learning — AIMM Curriculum | Module 2: Train | v1.0*
