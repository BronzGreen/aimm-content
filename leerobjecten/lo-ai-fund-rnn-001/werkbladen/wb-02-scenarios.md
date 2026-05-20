# Drie scenario-kaarten — welke variant past?
*Kolb fase 2 — Ervaren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Over dit werkblad**
> Je krijgt drie scenario-kaarten. Per kaart kies je de variant die het beste past: RNN, LSTM of BiLSTM. Twee criteria zijn doorslaggevend. Het eerste is **sequentielengte** (hoe lang is je context-venster?). Het tweede is **online of offline** (heb je de toekomst beschikbaar?). Geen "weet niet", kies een richting en leg het uit.
>
> **Tijd:** 12 minuten.
>
> **Waarom dit werkblad?**
> De drie varianten zien er op papier op elkaar. In de praktijk verschillen ze sterk. Wie kan zeggen waarom een trillings-voorspeller wel met BiLSTM werkt en een dashboard-meldingen-systeem niet, kan beter meedenken bij de leverancier. Dit werkblad oefent precies die afweging.

---

## Scenario A — Dashboard-meldingen op een actieve machine

> Een productiemachine in een continu draaiende lijn heeft een trillingssensor. Het systeem moet **realtime** alarmeren als er een afwijking is. Het context-venster is de afgelopen 50 samples (ongeveer 50 milliseconden bij een meetsnelheid van 1 kHz). Een alarm moet binnen seconden ontstaan. Wachten tot er meer data beschikbaar is, kan niet.

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

## Scenario B — Offline voorspeller op een aandrijfas

> Een fabriek heeft 24 uur aan **opgenomen** trillings-data van een aandrijfas. De analyse loopt in batches van 200 tot 500 samples per venster. Doel: zo nauwkeurig mogelijk de RUL (Remaining Useful Life, oftewel de resterende levensduur) voorspellen. Het loopt achteraf, er is geen tijdsdruk. Accuracy is alles.

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

## Scenario C — Korte storingsclassificatie op geluid

> Een sorteersysteem op een productie-cel ondersteunt zich met een akoestische sensor. Per onderdeel meet het systeem een 20-sample geluidsvenster. Doel: klassen of het deel correct gegrepen is (klik versus geen klik). Geen lange historie, geen toekomst nodig. Gewoon: past dit korte signaal in klasse A of B?

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

## Wat doen we hierna?

In fase 3 (Reflecteren) vergelijk je je antwoorden eerst met je buurman. Daarna stemt de groep plenair per scenario. De trainer bespreekt vooral scenario B als kerncase voor de meerwaarde van bidirectional reading. Houd je antwoorden bij de hand. We pakken straks de werkblad-pagina van fase 3 erbij.

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
