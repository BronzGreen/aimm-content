# Vier scenario-kaarten: welke ML-leerklasse past?
*Vier ML-leerklassen — Datasituatie versus leervorm*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Vier ML-leerklassen voor PdM**

---

> **Wat ga je doen?**
> Je krijgt vier scenario-kaarten uit verschillende fabrieken. Per scenario kies je welke ML-leerklasse past: **supervised**, **unsupervised**, **semi-supervised** of **reinforcement learning**. Twee dingen tellen: heeft de fabriek **gelabelde uitvalhistorie**, en wat moet er **voorspeld** worden? Bij twijfel mag je een vraagteken zetten — die nemen we straks samen door.
>
> **Tijd:** 14 minuten.

---

## De vier leerklassen — kort

| Leerklasse | Datasituatie | Wat doet het? |
|------------|--------------|---------------|
| **Supervised** | Gelabelde data (we weten wat goed/fout was) | Voorspellen op basis van bekende voorbeelden |
| **Unsupervised** | Geen labels | Patronen vinden zonder vooraf te weten wat hoort bij wat |
| **Semi-supervised** | Weinig gelabeld + veel ongelabeld | Combineren — leren van het beetje dat we hebben |
| **Reinforcement** | Online beslissingen, beloning achteraf | Leren door te proberen en feedback krijgen |

---

## Scenario A — Fabriek met 5 jaar uitvalhistorie

> Een verpakkingsfabriek registreert al 5 jaar systematisch elke storing: datum, machine, oorzaakcode (lager / motor / sensor / anders), reparatietijd. Daarnaast loopt continu vibration- en temperatuurmeting. Doel: **RUL voorspellen** — hoeveel cycli heeft deze machine nog vóór de volgende uitval?

**Welke leerklasse past?**

○ Supervised   ○ Unsupervised   ○ Semi-supervised   ○ Reinforcement   ○ ?

*Welk woord uit het scenario woog het zwaarst?*

_______________________________________________

*Onderbouwing:*

_______________________________________________

_______________________________________________

---

## Scenario B — Fabriek zonder uitvalhistorie

> Een nieuwe productielocatie heeft uitgebreide sensor-meetdata (vibratie, temperatuur, druk, stroom) maar **geen systematische storings-historie** — uitval wordt mondeling besproken in de ploegoverdracht, niet vastgelegd. Doel: **afwijkende patronen vinden** in de sensorstroom — anomalieën die wijzen op iets ongebruikelijks.

**Welke leerklasse past?**

○ Supervised   ○ Unsupervised   ○ Semi-supervised   ○ Reinforcement   ○ ?

*Welk woord uit het scenario woog het zwaarst?*

_______________________________________________

*Onderbouwing:*

_______________________________________________

_______________________________________________

---

## Scenario C — Fabriek met paar gelabelde cases

> Een fabriek heeft over de afgelopen 3 jaar **50 gelabelde uitvalcases** (klein aantal — in de praktijk gaat het zelden stuk) en daarnaast **5000 ongelabelde productiecycli**. Doel: **classificeren** of een lopende cyclus tot uitval gaat leiden binnen 100 cycli.

**Welke leerklasse past?**

○ Supervised   ○ Unsupervised   ○ Semi-supervised   ○ Reinforcement   ○ ?

*Welk woord uit het scenario woog het zwaarst?*

_______________________________________________

*Onderbouwing:*

_______________________________________________

_______________________________________________

---

## Scenario D — Continu beslissen over onderhoud

> Een dure productiemachine kost veel als hij ongepland stilstaat, maar onderhoud kost ook geld en planningstijd. Per dag wordt een beslissing genomen: **uitstellen, doen, of vervangen**. Het systeem moet leren wat de beste beslissing is over tijd, op basis van **uitkomst-feedback**: leverde dit onderhoud rendement op of niet?

**Welke leerklasse past?**

○ Supervised   ○ Unsupervised   ○ Semi-supervised   ○ Reinforcement   ○ ?

*Welk woord uit het scenario woog het zwaarst?*

_______________________________________________

*Onderbouwing:*

_______________________________________________

_______________________________________________

---

## Mijn samenvatting

| Scenario | Mijn keuze | Doorslaggevend woord |
|----------|------------|----------------------|
| A — 5 jaar uitvalhistorie | | |
| B — Geen uitvalhistorie | | |
| C — 50 gelabeld + 5000 ongelabeld | | |
| D — Online onderhoudsbeslissingen | | |

---

## Welk scenario was het lastigst?

**Lastigste scenario:** ○ A   ○ B   ○ C   ○ D

*Wat maakte het lastig?*

_______________________________________________

_______________________________________________

> **Tip:** Niet zeker? Vraagteken zetten is prima. Scenario C (semi-supervised) en D (reinforcement) worden vaak gemist — daar gaan we straks samen op door.

---
*Bron: Vier ML-leerklassen — AIMM Curriculum | Module 2: Train | v1.0*
