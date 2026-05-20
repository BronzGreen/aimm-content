---
id: lo-ai-fund-ensemble-001-trainer
knowledge_object_id: ko-ai-fundamentals-ensemble-001
version: trainer
title: Ensemble learning — meerdere modellen die samen sterker zijn — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 48
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-ai-fund-ensemble-001
---

# Ensemble learning — voor de trainer

**Leerobject:** lo-ai-fund-ensemble-001
**Kennisobject:** ko-ai-fundamentals-ensemble-001
**Doelgroep:** MBO-4 operator/teamleider, B2 taalniveau
**Duur:** 48 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Diagnose-spel met mystery cases, duo-vergelijking, trainer-handout, individueel actieplan |
| Kolb-startfase (de fase in de leercyclus waarmee de sessie begint) | Ervaren (5 cases met 3 modellen — zelf voelen wat een ensemble doet) |
| Begeleidingsstijl (instrueren / trainen / coachen / mentoren) | Trainen — IK DOE / WIJ DOEN / JIJ DOET drieluik |
| Materialen | 4 werkbladen, diagram bagging vs boosting, geen technische apparatuur extra |

## Wat de deelnemer leert

De deelnemer kan uitleggen wat een ensemble is (meerdere modellen die samen één voorspelling vormen), het verschil benoemen tussen bagging (parallel, variance) en boosting (sequentieel, bias), en herkennen wanneer een ensemble passend is voor een PdM-probleem — bij onevenwichtige data en heterogene sensors. Vereist data-lit-101 afgerond, bij voorkeur ook lo-ai-fund-ml-001.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:13 | Diagnose-spel: één expert vs. drie experts | Individueel met 5 mystery cases |
| Reflecteren | 0:13-0:22 | Buurman-check + plenair tellen "wins" | Duo + plenair |
| Theoretiseren | 0:22-0:36 | Bagging vs boosting + drie PdM-voorbeelden | Trainer + handout |
| Experimenteren | 0:36-0:48 | Eigen PdM-toepassing — past ensemble? | Individueel actieplan |

## Tips voor de trainer

- **Doe case 1 voor (IK DOE) — worked example.** Toon hoe expert A één diagnose geeft, B en C een andere — meerderheid wint. Dan loslaten op cases 2-5.
- **Tel plenair op het bord hoe vaak het ensemble won.** Maakt het concept tastbaar — *"in 4 van 5 cases gaf het ensemble een ander, beter antwoord."*
- **Bij blok 2 strak doorvragen.** *"Wanneer voegde de meerderheid niets toe?"* — dat opent het diversiteit-thema voor blok 3.
- **Verbind diagnose-spel direct met bagging.** *"Wat jullie net deden — drie meningen middelen — was een vorm van bagging."* Zonder die brug blijft de theorie abstract.
- **Concrete PdM-cases benoemen in blok 3.** Tool wear (random forest), pipe failure (boosted trees), aircraft RUL (bagging-style). Niet abstract praten — namen noemen.

## Valkuilen

- **Diagnose-spel wordt te snel als "meerderheid wint altijd" afgedaan.** Stel: *"Stel alle drie experts maken dezelfde fout — wint de meerderheid dan ook?"* Diversiteit is voorwaarde — drie identieke modellen = geen ensemble.
- **Bagging en boosting worden door elkaar gehaald.** Op flipover scherp tegenover elkaar: parallel/sequentieel én variance/bias. Twee axes.
- **Ensembles worden als universele oplossing gezien.** Bevestig de neiging, maar: ensembles zijn duurder en moeilijker te interpreteren. Bij ruim genoeg data + één goed afgestemd model presteren ze soms maar marginaal beter.

## Voorbereiding (15 min vooraf)

- [ ] 4 werkbladen printen (diagnose-spel, reflectie, handout bagging-boosting, actieplan), 1 per deelnemer + 2 reserve
- [ ] SVG-diagram (bagging vs boosting) op A3 zichtbaar
- [ ] Beamer + Slidev klaar, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flipover voor "wins-tracker" (hoe vaak ensemble vs losse modellen)
- [ ] Timer of mobiel met geluid

## Transferopdracht

Sluit af met: deelnemers kijken deze week of er op de eigen lijn een PdM-systeem actief is dat uitval voorspelt. Vraag IT of leverancier: gebruikt het systeem een ensemble of een enkel model? Bagging-style (random forest) of boosting-style (gradient boosting)? Hoeveel failure-cases zijn beschikbaar voor training? Antwoorden meenemen naar de volgende sessie.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
