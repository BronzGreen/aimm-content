# Vergelijkingstabel: van RNN naar LSTM naar BiLSTM
*Kolb fase 1 — Theoretiseren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: RNN/LSTM/BiLSTM**

---

> **Over dit werkblad**
> Je luistert naar het mini-college. De trainer bouwt het verhaal op in drie stappen. Eerst basis-RNN (Recurrent Neural Network, oftewel een terug-koppelend netwerk). Daarna LSTM (Long Short-Term Memory, een netwerk met drie gates). Als laatste BiLSTM (een LSTM die de tijdreeks van twee kanten leest). Per variant noteer je: welk probleem lost het op, wat is de typische use-case, en is het geschikt voor online of offline gebruik?
>
> **Tijd:** 18 minuten.
>
> **Waarom dit werkblad?**
> Veel PdM-systemen (Predictive Maintenance, oftewel voorspellend onderhoud) kijken niet naar één meetwaarde. Ze kijken naar een venster van tientallen tot honderden samples. Welke variant erachter zit, bepaalt of het systeem snel kan alarmeren of juist precies achteraf kan analyseren. Dit werkblad maakt dat verschil zichtbaar.

---

## 1. De analogie van het schrift

> **RNN** = je schrijft alleen op wat er net gebeurde. Bij een lang verhaal vergeet je het begin.
> **LSTM** = je gebruikt drie soorten markeringen: **doorstrepen** (wat vergeten), **bijschrijven** (wat onthouden), **voorlezen** (wat doorgeven).
> **BiLSTM** = twee mensen lezen het schrift. Eén leest van voor naar achter, en de tweede van achter naar voor. Samen vatten ze het beter samen.

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
| **Beperking** | long-term dependency (verleden vervaagt) | geen toekomst beschikbaar | alleen offline mogelijk |

---

## 3. De drie gates van een LSTM-cel

*Schrijf in eigen woorden op wat elke gate doet.*

| Gate | Wat doet hij? |
|------|---------------|
| **Forget gate** (vergeet-gate) | |
| **Input gate** (input-gate) | |
| **Output gate** (output-gate) | |

*En wat is de cell-state (de geheugen-lijn die meeloopt)?*

_______________________________________________

_______________________________________________

---

## 4. Het long-term dependency-probleem

> Een basis-RNN onthoudt de vorige timestep, en die de timestep daarvoor. Maar hoe verder terug, hoe vager. Bij een trillings-venster van 200 samples is het signaal van sample 5 bijna kwijt op sample 195. LSTM lost dit op met de drie gates. Die kiezen wat door de tijd reist.

*Vink aan wat je hierin herkent.*

- [ ] Ik snap waarom een basis-RNN op lange sequenties tekortschiet
- [ ] Ik snap dat de drie gates "selectief geheugen" geven
- [ ] Ik snap dat de cell-state als een lopende schrijflijn werkt
- [ ] Ik kan het in eigen woorden navertellen

---

## 5. BiLSTM — de bidirectional voorsprong

> Bij **online** detectie (een dashboard-melding die in seconden moet komen) heb je geen toekomstdata. Je kent alleen het verleden tot nu. Bij **offline** analyse (achteraf op historische data) heb je beide kanten beschikbaar. BiLSTM gebruikt dat: één LSTM leest van begin naar einde, een tweede van einde naar begin. Samen kennen ze de volledige context rond elk meetpunt.

*Wanneer is BiLSTM duidelijk béter dan een gewone LSTM?*

○ Online vibration-alarm in een actieve machine
○ Offline RUL-analyse op 24 uur opgenomen data
○ Korte signaalclassificatie zonder lange context

---

## 6. Werkvloer-voorbeelden om bij te denken

*Welke meting op de werkvloer past bij welke variant? Maak een eerste schets.*

| Werkvloer-toepassing | Eerste gok |
|-----------------------|------------|
| **Voorspeller** op een aandrijfas, achteraf op 24 uur data | ○ RNN  ○ LSTM  ○ BiLSTM |
| **Dashboard-meldingen** met realtime trillings-alarm | ○ RNN  ○ LSTM  ○ BiLSTM |
| **Storingsclassificatie** op een kort geluidsfragment | ○ RNN  ○ LSTM  ○ BiLSTM |

---

## 7. Eerste check: snap ik het?

*Vink aan wat je nu kunt.*

- [ ] Ik kan uitleggen waarom een RNN-familie nodig is voor tijdreeksen
- [ ] Ik kan de drie gates van LSTM benoemen
- [ ] Ik snap het verschil tussen unidirectional LSTM en BiLSTM
- [ ] Ik kan beoordelen wanneer BiLSTM niet kan (online + tijdsdruk)

> **Tip:** Lukt een vraag nog niet? Markeer hem. In fase 2 ga je drie scenario's beoordelen. Daar valt het verschil tussen de varianten vaak op zijn plek.

---

## Wat doen we hierna?

In fase 2 (Ervaren) krijg je drie scenario-kaarten. Per kaart kies je de variant die het beste past. De tabel die je hier invult, neem je daar als hulpmiddel mee. Houd je antwoorden bij de hand. We pakken straks de werkblad-pagina van fase 2 erbij.

---
*Bron: RNN/LSTM/BiLSTM — AIMM Curriculum | Module 2: Train | v1.0*
