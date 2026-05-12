# Handout: Vier ML-leerklassen voor PdM
*Vier ML-leerklassen — Het complete framework*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Vier ML-leerklassen voor PdM**

---

> **Kernidee:** ML-gebaseerde PdM kent vier leerklassen die elk passen bij een andere data-situatie. De juiste keuze maken is geen technische detail — het bepaalt of je AI-project überhaupt kan starten met de data die je hebt.

---

## De vier leerklassen op één rij

| | **Supervised** | **Unsupervised** | **Semi-supervised** | **Reinforcement** |
|---|---------------|-----------------|---------------------|-------------------|
| **Data nodig** | Gelabelde failure-data | Alleen ongelabelde sensor-data | Weinig gelabeld + veel ongelabeld | Geen vooraf, leert door interactie |
| **Wat leert het?** | Voorspellingen op basis van bekende voorbeelden | Patronen, clusters, afwijkingen | Combinatie — gebruikt het beetje labels en ongelabelde data | Welke beslissing levert op de lange termijn rendement op |
| **Online of offline?** | Beide | Vaak offline | Beide | Vooral online |
| **Sterk bij** | Voldoende failure-historie + duidelijk doel | Veel data, geen labels | Realistische PdM (weinig labels in praktijk) | Continu adaptieve beslissingen |
| **Risico** | Werkt alleen bij goede labels | Patroon vinden ≠ uitleggen wat het betekent | Complexe pipeline | Veel feedback / lange leertijd |

---

## Drie PdM-probleemtypen — welke leerklasse past?

*De meeste PdM-projecten zijn één van deze drie typen. Markeer welke leerklasse erbij past.*

| Probleemtype | Voorbeeld | Past bij leerklasse |
|--------------|-----------|---------------------|
| **Classification** — categorie voorspellen | Kans op uitval binnen 100 cycli (ja/nee) | ○ Supervised  ○ Semi-supervised |
| **Regression** — getal voorspellen | RUL — hoeveel cycli nog over? | ○ Supervised |
| **Clustering** — groeperen op gelijkenis | Welke machines lijken op elkaar in gedrag? | ○ Unsupervised |
| **Online beslissen** — beleid optimaliseren | Per dag: uitstellen / doen / vervangen | ○ Reinforcement |

---

## Per leerklasse — uitgewerkt

### 🔵 1. Supervised Learning

> Je hebt **gelabelde data**: voor veel cases weet je achteraf wat goed of fout was. Het model leert het patroon en kan op nieuwe cases voorspellen.

**Bij PdM:** RUL-voorspelling, classificatie van uitvalmodes.
**Voorbeeld:** Aircraft engine RUL met 5 jaar uitvalhistorie.
**Aha-moment:** _______________________________________________

### 🟣 2. Unsupervised Learning

> Je hebt **geen labels** — alleen sensordata. Het model zoekt zelf patronen, clusters, of afwijkingen.

**Bij PdM:** Anomaliedetectie, clustering van machinegedrag.
**Voorbeeld:** Nieuwe lijn zonder failure-registratie — vinden welke productiecycli "ongebruikelijk" zijn.
**Aha-moment:** _______________________________________________

### 🟢 3. Semi-supervised Learning

> Je hebt **een paar gelabelde** voorbeelden en **veel ongelabelde**. Het model gebruikt beide: het label-stuk om te leren wat goed/fout is, en het ongelabeld-stuk om de structuur in de data beter te begrijpen.

**Bij PdM:** Dit is wat veel fabrieken werkelijk hebben — weinig systematisch gelabelde uitval, veel productiedata.
**Voorbeeld:** 50 gelabelde uitvalcases + 5000 ongelabelde cycli → classifier voor failure-risico.
**Aha-moment:** _______________________________________________

### 🟠 4. Reinforcement Learning

> Het model leert door **te beslissen, gevolg te ervaren, en zich aan te passen**. Geen vaste labels — een beloningssignaal achteraf.

**Bij PdM:** Adaptieve onderhoudsbeslissingen — uitstellen of nu doen?
**Voorbeeld:** Onderhoudsbeleid dat over tijd leert wat het meeste rendement geeft.
**Aha-moment:** _______________________________________________

---

## Het beslisschema in vier stappen

| Vraag | Antwoord → leerklasse |
|-------|----------------------|
| 1. Heb je systematische uitvalhistorie met labels? | Ja, veel → **Supervised** |
| | Een beetje (zeg 20-100 cases) → **Semi-supervised** |
| | Bijna niks → ga door |
| 2. Wat moet er voorspeld worden? | Een getal (RUL) → **Supervised regression** |
| | Een klasse (welke fout) → **Supervised classification** |
| | Een patroon zonder vooraf labels → **Unsupervised clustering** |
| 3. Beslis je continu en wil je beleid leren? | Ja → **Reinforcement** |

---

## Kernbegrippen om te onthouden

| Begrip | Betekenis |
|--------|-----------|
| **Label** | Achteraf-categorie of -getal dat zegt: dit was goed/fout, dit was de uitval |
| **Feature** | Een meetwaarde die als input dient (vibration-piek, temperatuur, druk) |
| **Trainingsdata** | De data die het model gebruikt om te leren |
| **Validatiedata** | Aparte set om te testen of het model echt generaliseert |
| **Anomalie** | Afwijkend patroon — niet noodzakelijk een gelabelde fout |
| **Beleid (policy)** | Bij reinforcement: de strategie die zegt "in deze situatie kies ik dit" |

---

## Controleer jezelf

*Vink aan wat je nu kunt.*

- [ ] Ik kan de vier leerklassen benoemen
- [ ] Ik weet bij elke leerklasse welke datasituatie nodig is
- [ ] Ik kan de drie PdM-probleemtypen koppelen aan leerklassen
- [ ] Ik kan een PdM-scenario bekijken en daaruit afleiden welke leerklasse passend is

> **Onthoud:** De juiste leerklasse-keuze is geen technische bijzaak. Bij PdM bepaalt de **datasituatie** vaak welke aanpak überhaupt mogelijk is. Een leverancier die "supervised RUL" aanbiedt zonder uitvalhistorie te eisen, weet niet wat hij doet — of jij hebt hem niet de goede vraag gesteld.

---
*Bron: Vier ML-leerklassen — AIMM Curriculum | Module 2: Train | v1.0*
