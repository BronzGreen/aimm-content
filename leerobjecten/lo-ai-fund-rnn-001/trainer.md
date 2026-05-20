---
id: lo-ai-fund-rnn-001-trainer
knowledge_object_id: ko-ai-fundamentals-rnn-001
version: trainer
title: RNN, LSTM en BiLSTM — neurale netwerken met geheugen voor tijdreeksen — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 50
status: validated
updated_at: '2026-05-20'
correlation_id: ronde22-lo-ai-fund-rnn-001
---

# RNN, LSTM en BiLSTM — voor de trainer

**Leerobject:** lo-ai-fund-rnn-001
**Kennisobject:** ko-ai-fundamentals-rnn-001
**Doelgroep:** MBO-4 operator/teamleider, B2 taalniveau
**Duur:** 50 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Mini-college met schrift-analogie, drie scenario-kaarten, plenaire stemming, individueel actieplan |
| Kolb-startfase (de fase in de leercyclus waarmee de sessie begint) | Theoretiseren (mentaal model + analogie eerst, dan toepassen) |
| Begeleidingsstijl (instrueren / trainen / coachen / mentoren) | Instrueren — gestructureerde uitleg met fysieke rekwisieten |
| Materialen | 4 werkbladen, SVG-diagram (LSTM-cel met 3 gates), schrift + 3-kleur post-its |

## Wat de deelnemer leert

De deelnemer kan uitleggen waarom een RNN-familie nodig is voor tijdreeks-data (geheugen over timesteps), het verschil benoemen tussen vanilla RNN, LSTM en BiLSTM, en beoordelen welke variant past bij een gegeven scenario op basis van sequentielengte en online/offline-criterium. Vereist data-lit-101 + tijdreeks-begrip; bij voorkeur ook lo-ai-fund-cnn-001 doorlopen.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Theoretiseren | 0:00-0:18 | Mini-college: van RNN naar LSTM naar BiLSTM | Trainer + vergelijkingstabel |
| Ervaren | 0:18-0:30 | Drie scenario-kaarten — welke variant past? | Individueel + IK DOE worked example |
| Reflecteren | 0:30-0:40 | Buurman-check + plenaire stemming | Duo + plenair |
| Experimenteren | 0:40-0:50 | Eigen tijdreeks-scan | Individueel actieplan |

## Tips voor de trainer

- **Bouw het verhaal in drie stappen op.** RNN → LSTM → BiLSTM, met telkens één sleutelvraag: *wat lost dit op?* Volgorde is essentieel, anders stapelen de begrippen.
- **Gebruik schrift en drie post-its fysiek.** Schrift = tijdreeks. Forget gate = doorstrepen (rood post-it). Input gate = bijschrijven (groen). Output gate = voorlezen (geel). Tastbaar, niet abstract.
- **Geen formules.** Vermijd matrixrekening, sigmoid-functies, tanh. De drie gates zijn een mentaal model, geen wiskunde.
- **Doe scenario A voor (worked example).** *"Online, korte geschiedenis, geen toekomst beschikbaar → LSTM."* Daarna B en C zelf.
- **Twee criteria voor de keuze:** online of offline? Hoe ver staan gerelateerde gebeurtenissen uit elkaar in de reeks? Schrijf die twee assen op flipover.

## Valkuilen

- **Long-term dependency wordt gezien als "lange tijdreeks".** Maak scherp: het gaat om hoe ver UITEEN gerelateerde gebeurtenissen zitten — niet de lengte zelf. Trillingspiek nu door wrijving 100 samples geleden.
- **BiLSTM wordt gekozen voor online scenario's.** Stel de vraag: *"Heb je voor deze case de toekomst beschikbaar?"* Online = nee. BiLSTM heeft toekomst nodig om van achter naar voor te lezen.
- **Drie gates worden door elkaar gehaald.** Pak het schrift en de post-its fysiek. Drie gates, drie acties — koppeling helpt.

## Voorbereiding (15 min vooraf)

- [ ] 4 werkbladen printen (vergelijkingstabel, scenario's, reflectie, actieplan), 1 per deelnemer + 2 reserve
- [ ] SVG-diagram (LSTM-cel met 3 gates) op A3 zichtbaar
- [ ] Schrift / blocnote als rekwisiet (1)
- [ ] Drie post-it-kleuren (rood/groen/geel) — 1 setje voor demonstratie
- [ ] Beamer + Slidev klaar, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flipover voor parkeerlijst + drie varianten

## Transferopdracht

Sluit af met: deelnemers kijken deze week of er op de eigen lijn — of bij een klant — een PdM-systeem actief is dat tijdreeks-data analyseert. Vraag IT of leverancier: hoe lang is het context-venster (samples)? Realtime of offline batch? Welke modelfamilie (RNN / LSTM / BiLSTM)? Antwoorden koppelen aan de keuzetabel.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
