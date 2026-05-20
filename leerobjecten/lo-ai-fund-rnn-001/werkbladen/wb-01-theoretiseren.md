# Vergelijkingstabel: van RNN naar LSTM naar BiLSTM
*RNN/LSTM/BiLSTM — Drie varianten met geheugen*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Wat ga je doen?**
> Je luistert naar het mini-college. De trainer bouwt het verhaal op in drie stappen: (1) basis RNN, (2) LSTM met drie gates, (3) BiLSTM met twee leesrichtingen. Per variant noteer je: welk probleem lost het op, wat is de typische use-case, en is het geschikt voor online of offline gebruik?
>
> **Tijd:** 18 minuten.

---

## 1. De analogie van het schrift

> **RNN** = je schrijft alleen op wat er net gebeurde — bij een lang verhaal vergeet je het begin.
> **LSTM** = je gebruikt drie soorten markeringen: **doorstrepen** (wat vergeten), **bijschrijven** (wat onthouden), **voorlezen** (wat doorgeven).
> **BiLSTM** = twee mensen lezen het schrift, één van **voor naar achter** en één van **achter naar voor** — samen vatten ze het beter samen.

*Welke analogie helpt jou het meest?*

○ Het schrift   ○ Drie soorten markeringen   ○ Twee lezers   ○ Anders: ____________

---

## 2. Vul de vergelijkingstabel in

*Tijdens de uitleg vul je deze tabel in. Korte zinnen. Bij twijfel mag je een vraagteken zetten.*

| | **RNN** (basis) | **LSTM** | **BiLSTM** |
|---|----------------|----------|------------|
| **Welk probleem lost het op?** | | | |
| **Welke timesteps gebruikt het?** | alleen verleden | alleen verleden | verleden + toekomst |
| **Geheugenmechanisme** | korte loop | drie gates + cell-state | twee LSTM's gecombineerd |
| **Typische use-case** | | | |
| **Online of offline?** | | | |
| **Beperking** | long-term dependency | (geen toekomst beschikbaar) | (alleen offline) |

---

## 3. De drie gates van een LSTM-cel

*Schrijf in eigen woorden op wat elke gate doet.*

| Gate | Wat doet hij? |
|------|---------------|
| **Forget gate** (vergeet-gate) | |
| **Input gate** (input-gate) | |
| **Output gate** (output-gate) | |

*En wat is de cell-state?*

_______________________________________________

_______________________________________________

---

## 4. Het long-term dependency-probleem

> Een gewoon RNN onthoudt de vorige timestep, en die de timestep daarvoor — maar hoe verder terug, hoe vager. Bij een vibration-venster van 200 samples is het signaal van sample 5 bijna kwijt op sample 195. LSTM lost dit op met de drie gates die kiezen wat door de tijd reist.

*Vink aan wat je hierin herkent.*

- [ ] Ik snap waarom een gewoon RNN op lange sequenties tekortschiet
- [ ] Ik snap dat de drie gates "selectief geheugen" geven
- [ ] Ik snap dat de cell-state als een lopende schrijflijn werkt
- [ ] Ik kan het in eigen woorden navertellen

---

## 5. BiLSTM — de bidirectional voorsprong

> Bij **online** detectie (realtime alarmeren) heb je geen toekomstdata — je kent alleen het verleden tot nu. Bij **offline** analyse (achteraf op historische data) heb je beide kanten beschikbaar. BiLSTM gebruikt dat: één LSTM leest van begin naar einde, een tweede van einde naar begin. Samen kennen ze de volledige context rond elk meetpunt.

*Wanneer is BiLSTM duidelijk béter dan een gewone LSTM?*

○ Online vibration-alarm in een actieve machine
○ Offline RUL-analyse op 24 uur opgenomen data
○ Korte signaalclassificatie zonder lange context

---

## 6. Eerste check: snap ik het?

*Vink aan wat je nu kunt.*

- [ ] Ik kan uitleggen waarom RNN-familie nodig is voor tijdreeksen
- [ ] Ik kan de drie gates van LSTM benoemen
- [ ] Ik snap het verschil tussen unidirectional LSTM en BiLSTM
- [ ] Ik kan beoordelen wanneer BiLSTM niet kan (online + tijdsdruk)

> **Tip:** Lukt een vraag nog niet? Markeer hem. In fase 2 ga je drie scenario's beoordelen — daar valt het verschil tussen de varianten vaak op zijn plek.

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
