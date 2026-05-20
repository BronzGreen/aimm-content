# Reflectie: Welk criterium woog voor jou het zwaarst?
*RNN/LSTM/BiLSTM — Buurman-check en plenaire reflectie*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Over dit werkblad**
> Je hebt drie scenario's beoordeeld. Nu vergelijk je je antwoorden met je buurman en met de groep. Reflectie volgt het STARRT-model: Situatie, Taak, Actie, Resultaat, Reflectie, Transfer.
>
> **Tijd:** 10 minuten — eerst 5 minuten in tweetallen, daarna 5 minuten plenair.

---

## 🟣 1. Situatie — welk scenario was het lastigst?

*Welk scenario vond je het moeilijkst om te beoordelen?*

○ A — Online vibration-monitoring   ○ B — Offline batch-RUL   ○ C — Korte signaalclassificatie

*Wat maakte het lastig?*

_______________________________________________

_______________________________________________

---

## 🟣 2. Taak — wat probeerde je af te wegen?

*Welke criteria stonden tegenover elkaar in jouw beslissing?*

| Mijn afweging | Speelde dit mee? |
|---------------|:----------------:|
| Sequentielengte — was het venster lang genoeg om long-term dependency een probleem te maken? | ○ |
| Online versus offline — had ik toekomstdata beschikbaar of niet? | ○ |
| Accuracy versus snelheid — wat woog zwaarder? | ○ |
| Complexiteit — past LSTM/BiLSTM bij wat de organisatie kan onderhouden? | ○ |

---

## 🟣 3. Actie — welk woord woog door?

*Welk woord uit de uitleg gebruikte je het vaakst om je antwoord te onderbouwen?*

○ Long-term dependency
○ Forget/input/output gate
○ Cell-state
○ Bidirectional / toekomstcontext
○ Online / realtime

*Toelichting:*

_______________________________________________

_______________________________________________

---

## 🟣 4. Resultaat — wat zei je buurman?

*Vergelijk met je buurman. Bij welke scenario's was je antwoord hetzelfde, en bij welke verschilde het?*

**Zelfde antwoord op:** ○ A   ○ B   ○ C

**Verschil bij:** ○ A   ○ B   ○ C

*Wat hoorde je van je buurman dat je zelf niet had gezien?*

_______________________________________________

_______________________________________________

---

## 🟣 5. Reflectie — welke variant is voor jou nu het duidelijkst?

*Welke variant kun je na deze oefening het beste uitleggen aan een collega?*

○ Vanilla RNN   ○ LSTM   ○ BiLSTM

*Welke roept nog vragen op?*

○ Vanilla RNN   ○ LSTM   ○ BiLSTM

*Welke vraag wil je daar nog over stellen?*

_______________________________________________

_______________________________________________

---

## 🟢 6. Transfer — denk aan je eigen lijn

*Welke tijdreeks van je eigen werk lijkt het meest op een van de drie scenario's?*

○ Lijkt op A (online, korter venster) — past LSTM
○ Lijkt op B (offline, langer venster) — past BiLSTM
○ Lijkt op C (korte, simpele classificatie) — past RNN
○ Geen herkenning yet

*Naam van die meting:* _______________________________________________

*Toelichting:*

_______________________________________________

_______________________________________________

---

## 🟢 7. Tip voor het leveranciersgesprek

*Welke vraag wil je IT of de leverancier stellen over jullie tijdreeks-PdM-systeem?*

○ Hoe lang is het context-venster (aantal samples)?
○ Is het systeem online/realtime of analyseert het achteraf?
○ Welke modelfamilie wordt gebruikt — RNN, LSTM of BiLSTM?
○ Anders: _______________________________________________

> **Tip voor de plenaire bespreking:** scenario B is meestal waar BiLSTM zijn meerwaarde laat zien. Bij A is BiLSTM principieel onmogelijk (toekomst niet beschikbaar). Zien jullie hetzelfde patroon in jullie organisaties?

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
