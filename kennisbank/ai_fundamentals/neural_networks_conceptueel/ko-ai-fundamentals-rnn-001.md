---
id: ko-ai-fundamentals-rnn-001
title: 'RNN, LSTM en BiLSTM: tijdreeks-modellen met geheugen'
type: concept_uitleg
domain: ai_fundamentals
subdomain: neural_networks_conceptueel
summary: RNN's verwerken tijdreeks-data maar lijden aan het long-term dependency-probleem;
  LSTM lost dit op met forget/input/output-gates en cell-state geheugen; BiLSTM combineert
  een voorwaartse en achterwaartse LSTM voor optimale context.
source_centrality: 0.85
source_ref: Li (2026). Hybrid Data-Model AI for Structural Monitoring, §2.1.2 (p.
  20-21)
status: validated
updated_at: '2026-05-20'
correlation_id: ronde22-lo-ai-fund-rnn-001
---

# RNN, LSTM en BiLSTM: tijdreeks-modellen met geheugen

## Recurrent Neural Network (RNN)

Een RNN is een neural network speciaal geschikt voor **tijdreeks-data**:
elke timestep gebruikt zowel de huidige input als de hidden state
van de vorige timestep. Daardoor kan het netwerk volgordeafhankelijke
patronen leren.

**Beperking:** het long-term dependency-probleem — naarmate de
sequentie langer wordt, kan het netwerk informatie van eerdere
timesteps niet meer effectief gebruiken (vanishing gradients).

## Long Short-Term Memory (LSTM)

Hochreiter et al. introduceerden LSTM in 1997 om de long-term
dependency op te lossen. Een LSTM-cel heeft een **expliciete
cell-state C_t** plus drie gates die elk bepalen wat er met die
state gebeurt:

### Forget gate (f_t)
Bepaalt welke informatie uit de vorige cell-state wordt **verwijderd**.
- σ-activatie levert waarden tussen 0 (vergeet) en 1 (behoud).
- f_t = σ(W_f · [h_{t-1}, I_t] + b_f)

### Input gate (i_t)
Bepaalt welke nieuwe informatie wordt **toegevoegd**.
- Eén deel selecteert wat te updaten (σ-activatie)
- Eén deel genereert een kandidaat-vector (tanh-activatie)
- Cell-update: C_t = f_t · C_{t-1} + i_t · C̃_t

### Output gate (O_t)
Selecteert welke informatie uit de huidige cell-state naar de
hidden state h_t gaat.
- h_t = O_t · tanh(C_t)

## Bidirectional LSTM (BiLSTM)

Een BiLSTM stapelt twee LSTM-netwerken:
- **Forward LSTM** — verwerkt de sequentie van begin naar eind.
- **Backward LSTM** — verwerkt dezelfde sequentie van eind naar
  begin.

Het eindresultaat is de **concatenatie** van beide hidden states.
Daardoor heeft de BiLSTM op elk tijdstap zowel verleden- als
toekomstcontext binnen het venster — beter voor offline taken zoals
batch-anomaliedetectie of RUL-voorspelling op opgeslagen data.

## Wanneer welk model?

| Scenario | Beste keuze |
|---|---|
| Korte sequentie, simpel signaal | Vanilla RNN |
| Lange sequentie, online inference | LSTM |
| Lange sequentie, offline batch + accuracy belangrijk | BiLSTM |


## Praktijkvoorbeeld

Voor PdM op vibration-data van een lager: een 200-sample window
bevat zowel "voor"- als "na"-patronen rond een mogelijke afwijking.
BiLSTM gebruikt beide richtingen om te beoordelen of het meetpunt
echt afwijkend is — superieur aan een unidirectional LSTM die
alleen voorgeschiedenis kent.
