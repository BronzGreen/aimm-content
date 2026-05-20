---
id: lo-ai-fund-135-trainer
knowledge_object_id: ko-ai-fund-135
version: trainer
title: Overfitting — wanneer een AI-model te-goed-leert — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 42
status: validated
updated_at: '2026-05-20'
correlation_id: ronde13-lo-ai-fund-135
---

# Overfitting — wanneer 99% een alarmbel is — voor de trainer

**Leerobject:** lo-ai-fund-135
**Kennisobject:** ko-ai-fund-135
**Doelgroep:** MBO-4 operator/teamleider, B1-B2 taalniveau
**Duur:** 42 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Twee scorekaarten vergelijken, duo-bespreking + plenaire stemming, trainer-handout, individuele diagnose |
| Kolb-startfase | Ervaren (twee scorekaarten zelf beoordelen) |
| Begeleidingsstijl | Instrueren — sturend op concept, ervaringsgericht startend |
| Materialen | 4 werkbladen, stemkaartjes in 2 kleuren, flip-over voor 3 signalen + 3 tegenmaatregelen |

## Wat de deelnemer leert

De deelnemer herkent overfitting aan het verschil tussen training-score en productie-score op onbekende data — niet aan de hoogte van een enkele score. Benoemt drie signalen (scoreverschil, klein dataset met complex model, faalt op nieuwe machine of batch) en drie tegenmaatregelen (meer diverse voorbeelden, simpeler model, cross-validatie). Formuleert een gefundeerde vraag aan een AI-leverancier over het scoreverschil tussen training en test.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:10 | Twee scorekaarten naast elkaar (Model A/B) | Trainer IK DOE + individueel kiezen |
| Reflecteren | 0:10-0:20 | Duo + plenair: term overfitting | Duo + 2-kleur stemkaartjes |
| Theoretiseren | 0:20-0:32 | Handout: 3 signalen + 3 tegenmaatregelen | Trainer + handout |
| Experimenteren | 0:32-0:42 | Diagnose op 3 nieuwe scorekaarten | Individueel + plenair vergelijken |

## Tips voor de trainer

- **Doe Model A voor (IK DOE).** *"99% klinkt geweldig. Maar kijk hier — op een andere machine zakt het naar 60%. Wat zegt dat?"* Pauze. Geen antwoord geven. Zo wordt de spanning opgebouwd.
- **Houd de term overfitting weg uit fase 1.** Pas in fase 2 plenair introduceren — nadat de groep zelf onder woorden heeft gebracht dat het verschil scheef is. Bottom-up.
- **Gebruik de collega-vergelijking in fase 2.** *"Een nieuwe collega die tien producten op één machine heeft gezien — herkent die feilloos. Op een ander machinetype: stilte."* Voorbeelden onthouden, geen patroon door — dat is overfitting in MBO-4-taal.
- **Verbind elk signaal aan Model A/B in fase 3.** Niet abstract uitleggen — Model A is de geleefde ervaring. 39 punten verschil, 50 voorbeelden, één machine, faalt op nieuw. Allemaal in één model.
- **Twijfel in fase 4 is goed nieuws.** Wie bij een grensgeval (5-8 punten verschil) "twijfel" schrijft, hanteert precies de gewenste kritische houding. Bevestig dat — niet afkeuren als "te onzeker".

## Valkuilen

- **Hoogste getal wint — onbewuste reflex.** Bij scorekaarten kiest iemand Model A omdat "99% is het hoogste". Bevestig de intuïtie, maak dan expliciet: kijk niet naar de hoogte, kijk naar het VERSCHIL. 39 punten voor A, 2 voor B — dat is het signaal.
- **Overfitting wordt vertaald als "te complex model".** Niet alleen complexiteit veroorzaakt overfitting. Definitie is wat het model DOET — voorbeelden onthouden in plaats van patroon doorgronden. Een simpel model op een te-klein dataset overfit ook.
- **"Meer data lost overfitting altijd op."** Bijna — maar het moet DIVERSE data zijn. Meer foto's van dezelfde machine helpt niet. Verband leggen met lo-ai-fund-132 (diversiteit als trainingsdata-eigenschap).

## Voorbereiding (25 min vooraf)

- [ ] 4 werkbladen printen (wb-01 t/m wb-04), n + 2 reserve per stuk
- [ ] Stemkaartjes in 2 kleuren (rood = Model A, blauw = Model B), 1 set per deelnemer
- [ ] Beamer + Slidev, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flip-over voor parkeerlijst + 6 lege rijen (3 signalen + 3 tegenmaatregelen)
- [ ] Werkbladen wb-02 t/m wb-04 apart op trainertafel — gefaseerd uitdelen

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week één concreet AI-systeem in de fabriek opzoekt — inspectiecamera, trillings-monitor, kwaliteits-classificatie of voorspelmodel. Drie vragen aan de leverancier of IT: op welke data is het model getraind (hoeveel voorbeelden, van welke machine of lijn)? Op welke onbekende data is het getest, en wat was daar de score? Hoe groot is het verschil tussen training en test? Drie antwoorden meenemen naar de volgende sessie. Als bonus: vraag een collega-operator *"heb jij ooit gezien dat een meting of inspectie het op de ene machine wel deed en op een nieuwe niet?"* — het probleem is vaak herkenbaar, alleen had niemand er een naam voor.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
