# Drie scenario-kaarten — welke variant past?
*RNN/LSTM/BiLSTM — Variant-keuze per situatie*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Wat ga je doen?**
> Je krijgt drie scenario-kaarten. Per kaart kies je de variant die het beste past — RNN, LSTM of BiLSTM. Twee criteria zijn doorslaggevend: **sequentielengte** (hoe lang is je context-venster?) en **online/offline** (heb je de toekomst beschikbaar?). Geen "weet niet" — kies een richting en leg het uit.
>
> **Tijd:** 12 minuten.

---

## Scenario A — Online vibration-monitoring

> Een productiemachine in een continu draaiende lijn heeft een trillingssensor. Het systeem moet **realtime** alarmeren als er een afwijking is. Het context-venster is de afgelopen 50 samples (ongeveer 50 ms bij 1 kHz). Een alarm moet binnen seconden ontstaan — wachten tot er meer data beschikbaar is, kan niet.

**Welke variant past?**   ○ RNN   ○ LSTM   ○ BiLSTM

*Welk criterium woog het zwaarst?*

○ Sequentielengte (50 samples is kort — RNN zou kunnen)
○ Online beslissing (toekomst niet beschikbaar — BiLSTM kan niet)
○ Long-term dependency (LSTM handelt dat beter)

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

_______________________________________________

---

## Scenario B — Offline batch-RUL-analyse

> Een fabriek heeft 24 uur aan **opgenomen** vibration-data van een aandrijfas, in batches van 200-500 samples per analyse-venster. Doel: zo nauwkeurig mogelijk de RUL (Remaining Useful Life) voorspellen. Het loopt achteraf, geen tijdsdruk — accuracy is alles.

**Welke variant past?**   ○ RNN   ○ LSTM   ○ BiLSTM

*Welk criterium woog het zwaarst?*

○ Sequentielengte (lange context — RNN te zwak, LSTM nodig)
○ Offline beschikbaar (toekomst óók beschikbaar — BiLSTM toegevoegde waarde)
○ Accuracy belangrijker dan snelheid

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

_______________________________________________

---

## Scenario C — Korte signaalclassificatie

> Een vision-AI op een productie-cel ondersteunt zich met een akoestische sensor. Per onderdeel meet het systeem een 20-sample geluidsvenster. Doel: classificeren of het deel correct gegrepen is (klik versus geen klik). Geen lange historie, geen toekomst nodig — gewoon: past dit korte signaal in klasse A of B?

**Welke variant past?**   ○ RNN   ○ LSTM   ○ BiLSTM

*Welk criterium woog het zwaarst?*

○ Sequentielengte (zeer kort — basis-RNN kan al voldoen)
○ Geen long-term dependency-probleem
○ Online beslissing — geen toekomst beschikbaar

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

_______________________________________________

---

## Mijn samenvatting

| # | Mijn keuze | Doorslaggevend criterium |
|---|------------|--------------------------|
| A | ○ RNN  ○ LSTM  ○ BiLSTM | |
| B | ○ RNN  ○ LSTM  ○ BiLSTM | |
| C | ○ RNN  ○ LSTM  ○ BiLSTM | |

---

## Welk scenario was het lastigst?

**Lastigste scenario:** ○ A   ○ B   ○ C

*Wat maakte het lastig?*

_______________________________________________

_______________________________________________

> **Tip:** A is duidelijk LSTM (online, geen toekomst, voldoende lang voor long-term dependency). B is de kerncase voor BiLSTM (offline + lange sequentie, accuracy belangrijk). C kan met basis-RNN (kort, simpel). Klopt jouw redenering daarmee?

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
