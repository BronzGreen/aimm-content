# Actieplan: Welke variant past bij mijn tijdreeks?
*RNN/LSTM/BiLSTM — Eigen tijdreeks-scan*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Wat ga je doen?**
> Je hebt nu drie varianten en drie scenario's doorlopen. Tijd om het op je eigen lijn te leggen. Zoek één tijdreeks-meting die je kent — vibration van een lager, temperatuur van een oven, druk van hydrauliek, stroomverbruik van een motor. Beschrijf hem en kies welke variant zou passen.
>
> **Tijd:** 10 minuten.

---

## 🔵 1. Mijn tijdreeks

**Wat wordt er gemeten?**

○ Vibration / trilling
○ Temperatuur
○ Druk
○ Stroomverbruik / vermogen
○ Akoestiek / geluid
○ Anders: _______________________________________________

**Op welke machine of systeem?**

_______________________________________________

**Sample-rate (hoe vaak per seconde wordt er gemeten)?**

_______________________________________________

---

## 🔵 2. Online of offline?

*Wat doet het systeem eigenlijk met deze tijdreeks?*

| Vraag | Mijn antwoord |
|-------|---------------|
| Wordt er **realtime** gemonitord (alarm binnen seconden)? | ○ Ja  ○ Nee  ○ Onbekend |
| Wordt er **achteraf** geanalyseerd (batch, RUL, rapport)? | ○ Ja  ○ Nee  ○ Onbekend |
| Beide? | ○ Ja |

**Mijn keuze:** ○ Online (realtime)   ○ Offline (batch)   ○ Beide

---

## 🔵 3. Hoe lang is het context-venster?

*Hoeveel samples kijkt het systeem terug per beslissing?*

○ Kort (< 50 samples)
○ Middel (50 - 200 samples)
○ Lang (> 200 samples)
○ Onbekend

---

## 🟠 4. Welke variant zou passen?

*Op basis van de keuze-tabel uit fase 1.*

| Mijn situatie | Variant die past |
|---------------|------------------|
| Online + korte sequentie | RNN of LSTM |
| Online + middel/lange sequentie | LSTM |
| Offline + middel/lange sequentie | **BiLSTM** (meerwaarde van toekomstcontext) |
| Korte simpele classificatie | RNN volstaat |

**Mijn keuze:** ○ RNN   ○ LSTM   ○ BiLSTM

*Welk criterium was doorslaggevend?*

○ Sequentielengte
○ Online versus offline
○ Accuracy belangrijker dan snelheid
○ Iets anders: _______________________________________________

*Onderbouw kort:*

_______________________________________________

_______________________________________________

---

## 🟠 5. Past mijn keuze — eerlijk gekeken?

| Vraag | Mijn antwoord |
|-------|---------------|
| Is mijn beoogde variant uitvoerbaar gegeven onze IT-capaciteit? | ○ Ja  ○ Nee  ○ Onbekend |
| Hebben we genoeg gelabelde data om de variant te trainen? | ○ Ja  ○ Nee  ○ Onbekend |
| Wordt het accuracy-voordeel van BiLSTM (indien gekozen) groot genoeg gewaardeerd? | ○ Ja  ○ Nee  ○ N.v.t. |

---

## 🟢 6. Concrete acties — deze week

| # | Actie | Wanneer | Met wie | ✓ |
|---|-------|---------|---------|---|
| 1 | Mijn tijdreeks-toepassing in 5 zinnen op papier zetten | | | ☐ |
| 2 | Vraag aan IT/leverancier: hoe lang is het context-venster? | | | ☐ |
| 3 | Vraag aan IT/leverancier: online of offline? | | | ☐ |
| 4 | Vraag aan IT/leverancier: welke modelfamilie wordt gebruikt? | | | ☐ |

---

## 🔴 7. Mogelijke obstakels

*Wat zou dit gesprek kunnen tegenhouden?*

_______________________________________________

_______________________________________________

---

## 🟣 8. Een gesprek met een collega

> **Praat één keer deze week:** "Vinden wij dat ons monitoring-systeem snel genoeg alarmeert, of liever preciezer en achteraf?" Dat gesprek toont hoe de keuze tussen LSTM en BiLSTM ook een organisatie-keuze is — niet alleen technisch.

**Met wie ga je praten?** _______________________________________________

**Wat denkt hij/zij?**

_______________________________________________

_______________________________________________

---

## Mijn tijdreeks — vijf zinnen om mee te nemen

1. **Wat wordt gemeten:** _______________________________________________

2. **Online of offline:** _______________________________________________

3. **Lengte van het context-venster:** _______________________________________________

4. **Variant die past (RNN/LSTM/BiLSTM):** _______________________________________________

5. **Eerste vraag aan IT of leverancier:** _______________________________________________

---

> 📅 **Volgende sessie:** Neem dit mee. We bespreken kort per deelnemer of de variant inderdaad past bij je situatie.

**Review-datum:** __________  **Buddy/coach:** __________

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
