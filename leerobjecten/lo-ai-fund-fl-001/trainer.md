---
id: lo-ai-fund-fl-001-trainer
knowledge_object_id: ko-ai-fundamentals-fl-001
version: trainer
title: Federated Learning — samen leren zonder data te delen — trainer-pakket
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
correlation_id: ronde21-lo-ai-fund-fl-001
---

# Federated Learning — voor de trainer

**Leerobject:** lo-ai-fund-fl-001
**Kennisobject:** ko-ai-fundamentals-fl-001
**Doelgroep:** MBO-4 operator/teamleider, B2 taalniveau
**Duur:** 50 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Mini-college vergelijkingsschema, drie scenario-kaarten, plenaire stemming, individueel actieplan |
| Kolb-startfase (de fase in de leercyclus waarmee de sessie begint) | Theoretiseren (paradigma eerst neerzetten, dan toepassen) |
| Begeleidingsstijl (instrueren / trainen / coachen / mentoren) | Instrueren — vooral conceptuele uitleg + scenario-toets |
| Materialen | 4 werkbladen, SVG-diagram (centraal vs federated), beamer, flipover |

## Wat de deelnemer leert

De deelnemer kan in eigen woorden uitleggen wat federated learning is, hoe het verschilt van klassieke centrale ML-training, en in welke situatie het op de eigen werkvloer voordeel oplevert — privacy, bandbreedte of IP-bescherming. Aan de hand van drie scenario's beoordeelt hij of FL een geschikte aanpak is, op basis van de drie kenmerken (data lokaal, alleen parameters delen, centrale aggregatie). Vereist data-lit-101 afgerond.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Theoretiseren | 0:00-0:15 | Drie kenmerken van FL — vergelijkingsschema | Trainer + werkblad |
| Ervaren | 0:15-0:27 | Drie scenario-kaarten — past FL hier? | Individueel + IK DOE worked example |
| Reflecteren | 0:27-0:37 | Buurman-check + plenaire stemming | Duo + plenair |
| Experimenteren | 0:37-0:50 | Eigen organisatie-scan | Individueel actieplan |

## Tips voor de trainer

- **Begin met het ziekenhuis-voorbeeld.** Ziekenhuizen die samen een diagnose-model trainen zonder patiëntdata uit te wisselen — herkenbaar, niet-bedreigend. Daarna brug naar maakindustrie.
- **Schrijf de drie woorden naast elkaar op flipover.** Edge-AI / cloud-AI / federated learning. Pas dan vallen de definities op hun plek — anders blijft het wazig.
- **Single point of failure expliciet benoemen.** Stel de vraag terug: *"Wat gebeurt er met onze training als de centrale server platgaat?"* Beperking eerlijk noemen — anders ontstaat een te rooskleurig beeld.
- **Scenario A is bewust grijs.** Zusterfabrieken — past FL? Soms. *"Stel jullie hebben binnen het concern al één gedeelde database — heb je FL dan nog nodig?"*
- **Houd 't conceptueel.** Geen gradient averaging, FedAvg of differential privacy. Parkeer technische vragen op flipover voor self-study.

## Valkuilen

- **FL wordt verward met cloud-AI of edge-AI.** Schrijf de drie naast elkaar op flipover. Zonder dat onderscheid blijft FL een buzzword.
- **Single point of failure wordt niet doorgrond.** Stel de tegenvraag — laat ze even denken voordat je het uitlegt.
- **Trainer duikt in technische details.** Bij IT-affiniteit-vragen: parkeer op flipover, vandaag conceptueel. Anders raakt MBO-4 zonder IT-achtergrond het spoor kwijt.

## Voorbereiding (15 min vooraf)

- [ ] 4 werkbladen printen (vergelijkingsschema, scenario's, reflectie, actieplan), 1 per deelnemer + 2 reserve
- [ ] SVG-diagram (centraal vs federated) op A3 zichtbaar
- [ ] Beamer + Slidev klaar, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flipover voor parkeerlijst en sleutelwoorden (edge / cloud / federated)
- [ ] Timer of mobiel met geluid

## Transferopdracht

Sluit af met: deelnemers zoeken deze week één concrete situatie in hun organisatie of bij een klant waar productiedata om privacy- of IP-redenen niet centraal verzameld kan worden. In vijf zinnen: welke data, met wie samenwerken, welk modeldoel, FL passend?, en wie binnen de organisatie hierover gaat. Praat één keer informeel met een IT- of data-collega: *"Kennen jullie federated learning?"*

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
