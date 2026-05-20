---
id: lo-smart-mfg-513-trainer
knowledge_object_id: ko-smart-mfg-513
version: trainer
title: 'Resultaten interpreteren: confusion matrix voor operators'
target_audience: operator
content_level: MBO-3
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: experimenteren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-513
---

# Confusion matrix lezen + verbeteractie — voor de trainer

**Leerobject:** lo-smart-mfg-513
**Kennisobject:** ko-smart-mfg-513 (+ ko-smart-mfg-514)
**Doelgroep:** MBO-3 operator (Module 2), B1 taalniveau
**Duur:** 45 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Confusion matrix eigen model lezen, duo-vergelijking, korte handout precision/recall, verbeteractie + simulatie |
| Kolb-startfase | Experimenteren — bewust bekwame doener werkt direct met eigen resultaten |
| Begeleidingsstijl | Coachen — vragen stellen, geen antwoorden |
| Materialen | Confusion matrix per duo, vier werkbladen, handout precision/recall + verbetercyclus, simulatie-werkblad, rekenmachines, whiteboard |

## Wat de deelnemer leert

De deelnemer kan een confusion matrix van zijn eigen model lezen, precision en recall in eigen woorden uitleggen, en een verbeteractie formuleren op basis van de modelresultaten. Bij de confusion matrix van zijn vorige configuratie leest hij correct af, benoemt of precision of recall het probleem is, en formuleert minimaal één gerichte verbeteractie.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Experimenteren | 0:00-0:10 | Confusion matrix invullen + precision/recall berekenen | Individueel |
| Reflecteren | 0:10-0:20 | Duo: vergelijk matrices — wat is erger, vals alarm of gemist defect? | Duo + plenair |
| Theoretiseren | 0:20-0:30 | Precision/recall in operatortaal + verbetercyclus | Trainer + handout |
| Experimenteren | 0:30-0:45 | Verbeteractie + simulatie hertest + pitch | Duo + plenair |

## Tips voor de trainer

- **Gebruik resultaten van de groep als voorbeeld.** "Bij Karim is de recall hoog maar precision laag — wat zegt dat?" Maak het concreet met groepsdata, geen abstracte uitleg.
- **Trade-off bespreken in fase 2.** "Wat is erger op jullie lijn: vals alarm (handmatige check) of gemist defect (klacht/uitval)?" Het antwoord stuurt de keuze tussen drie verbeterstrategieën.
- **Drie verbeterstrategieën als kapstok.** (1) Drempel verschuiven — snel, maar trade-off blijft. (2) Meer trainingsdata van zwakke categorie — duurzaam. (3) Labels herzien — als inconsistent. Deze structureren fase 4.
- **Verwijs naar LO-512 voor drempelwaarde, LO-514 voor data verbeteren.** Vandaag is dit LO de tussen-stap: van resultaten naar gerichte actie.
- **Pitch in fase 4 op proces, niet op cijfers.** "Wat verbeterde? Wat blijft moeilijk?" Niet: "Welke recall is best?"

## Valkuilen

- **Precision en recall worden door elkaar gehaald.** Houd één regel: precision = van wat ik 'defect' noem, hoeveel ECHT defect; recall = van alle echte defecten, hoeveel vind ik.
- **Verbeteractie blijft "drempel verlagen".** Eis afweging tussen drie strategieën — niet één-trucks-pony.
- **Plenaire afsluiting overslaan.** De pitch is feedback-rijk; sla niet over wegens tijdsdruk.

## Voorbereiding (30 min vooraf)

- [ ] Confusion matrix per duo voorbereiden (uit LO-511 resultaten of voorbeeld-set)
- [ ] Vier werkbladen + handout printen
- [ ] Rekenmachines, whiteboard
- [ ] Simulatie-werkblad voor hertest klaar
- [ ] Tafels in duo-opstelling

## Transferopdracht

Geef de deelnemer mee om voor zijn eigen product te bepalen of precision of recall belangrijker is, en dat te bespreken met zijn leidinggevende. Hij vraagt de kwaliteitsafdeling naar de afkeur- en doorlaatcijfers van het afgelopen kwartaal — dat zijn de echte trade-off-getallen voor het bedrijf.

## Verdere details

- **Volledig draaiboek:** zit ingebed in `lo-smart-mfg-513-trainer.yaml` (kolb_design.phases)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
