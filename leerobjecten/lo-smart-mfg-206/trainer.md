---
id: lo-smart-mfg-206-trainer
knowledge_object_id: ko-smart-mfg-206
version: trainer
title: Sensordata interpreteren met SHAP — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 25
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-smart-mfg-206
---

# Sensordata interpreteren met SHAP — voor de trainer

**Leerobject:** lo-smart-mfg-206
**Kennisobject:** ko-smart-mfg-206
**Doelgroep:** MBO-3 operator, B1 taalniveau
**Duur:** 25 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Storingsquiz 3 SHAP-grafieken, duo-reflectie, korte handout 5-stappenplan, individueel actieplan |
| Kolb-startfase | Ervaren — bewust bekwame doener leert door doen |
| Begeleidingsstijl | Trainen — 5 stappen + vuistregeltabel als kapstok |
| Materialen | Vier werkbladen, SVG-diagram, beamer, flap-over |

## Wat de deelnemer leert

De deelnemer kan een SHAP-grafiek lezen en de top-3 sensoren benoemen die bijdragen aan een anomaliemelding. Hij groepeert de sensoren per systeem (spil, koeling, voeding) en kiest de juiste eerste actie op basis van de vuistregeltabel.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:08 | Storingsquiz 3 SHAP-grafieken | Individuele quiz |
| Reflecteren | 0:08-0:15 | Duo: vergelijk je antwoorden | Duo |
| Theoretiseren | 0:15-0:20 | 5-stappenplan + vuistregeltabel | Trainer + handout |
| Experimenteren | 0:20-0:25 | Actieplan: bij eerstvolgende melding op jouw machine | Individueel |

## Tips voor de trainer

- **Groeperen per systeem is de kern van stap 2.** Bij "spiltemperatuur 55%" doorvragen: "Welke andere sensor zit in hetzelfde systeem?" Op flap-over twee kolommen: spilsysteem (temperatuur, trillingen) versus koelsysteem (koelmiddelniveau).
- **SHAP = vingerwijzing, niet conclusie.** Bij "als SHAP dit aangeeft, dan is het toch zo?": "SHAP geeft de getallen, jouw oordeel geeft de richting." In stap 5 staat expliciet: jouw machinekennis telt mee.
- **Houd het visueel — niet wiskundig.** "Het percentage zegt: hoeveel deze sensor bijdraagt aan de melding." Geen Shapley values of cooperative game theory.
- **Concreet maken in fase 4.** "Ik ga SHAP gebruiken" is geen actieplan. Doorvragen: welke sensor geeft bij jouw machine vaak problemen? Wat is je eerste actie als die in de top-3 staat?
- **SHAP-grafiek niet beschikbaar in eigen dashboard?** Geen probleem — laat de quiz toch doen als gedachte-oefening en zet op werkblad 4 als actie: "Vraag IT/teamleider of SHAP geactiveerd kan worden."

## Valkuilen

- **Deelnemer staart naar percentages zonder ze te groeperen.** Maak op flap-over twee kolommen per systeem.
- **AI-uitleg voelt als 'het systeem zegt het, dus klopt het'.** Maak het advies-karakter onmiskenbaar — operator-oordeel boven SHAP bij conflict.
- **Trainer duikt te snel in technische SHAP-theorie.** Geen Shapley values; houd het bij percentages en kleur.

## Voorbereiding (25 min vooraf)

- [ ] Vier werkbladen printen, n + 2 reserve
- [ ] SVG-diagram (5-stappenplan) op beamer
- [ ] Flap-over met sleutelwoorden + parkeerlijst
- [ ] U-opstelling of clusters van 4
- [ ] Beamer + HDMI getest

## Transferopdracht

Geef de deelnemer mee om bij de eerstvolgende anomaliemelding op de eigen machine de top-3 sensoren te benoemen, ze per systeem te groeperen en de eerste actie op te schrijven volgens het 5-stappenplan. Hij vergelijkt zijn keuze met wat hij hoort/voelt aan de machine voordat hij actie neemt.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** `../../trainee/lo-smart-mfg-206/lo-smart-mfg-206.yaml` (en wb-01 t/m wb-04)
