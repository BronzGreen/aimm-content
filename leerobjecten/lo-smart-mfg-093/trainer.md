---
id: lo-smart-mfg-093-trainer
knowledge_object_id: ko-smart-mfg-093
version: trainer
title: 'Autoencoder: AI leert wat normaal is — trainer-pakket'
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 30
status: validated
updated_at: '2026-05-20'
correlation_id: ronde12-lo-smart-mfg-093
---

# Autoencoder: AI leert wat normaal is — voor de trainer

**Leerobject:** lo-smart-mfg-093
**Kennisobject:** ko-smart-mfg-093
**Doelgroep:** MBO-3 operator, B1 taalniveau
**Duur:** 30 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Storingsquiz met sensorgrafieken, duo-reflectie, korte uitleg met SVG-diagram, individueel actieplan |
| Kolb-startfase | Ervaren (zelf normaal/afwijkend beoordelen op grafieken) |
| Begeleidingsstijl | Trainen — drie stappen invoer-samenvatting-herstel als kapstok |
| Materialen | Vier werkbladen, 6 sensorgrafieken (4 normaal, 2 afwijkend), SVG-diagram |

## Wat de deelnemer leert

De deelnemer kan in eigen woorden uitleggen hoe een autoencoder afwijkingen in productiedata herkent. Aan de hand van een voorbeeld uit de eigen productielijn benoemt hij minimaal drie van de stappen invoer, samenvatting, herstel en reconstructiefout — en koppelt het terug aan zijn eigen patroonherkenning bij de quiz.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:08 | Storingsquiz: 6 sensorgrafieken normaal/afwijkend | Individuele quiz |
| Reflecteren | 0:08-0:15 | Hoe deed je dat? — duo-gesprek + plenair | Duo's en plenair |
| Theoretiseren | 0:15-0:23 | Drie stappen autoencoder + mens-AI-parallel | Trainer + diagram |
| Experimenteren | 0:23-0:30 | Actieplan: welke sensor op jouw machine? | Individueel + delen |

## Tips voor de trainer

- **Vermijd het woord "autoencoder" in de eerste 8 minuten.** Begin met "het systeem leert wat normaal is". Pas in fase 3 het woord invoeren, en altijd direct vertalen: "auto = vanzelf, encoder = samenvatter".
- **Houd reconstructiefout uit de wiskunde.** Twee grafieken naast elkaar, en de afwijking ertussen — niet MSE of Euclidische afstand. De vraag is altijd: is het herstel goed gelukt of niet?
- **Gebruik de mens-AI-parallel actief.** "Jij herkent ook wat raar is, zonder dat je een formule kent. Autoencoder doet hetzelfde — kent het normaal, signaleert afwijking, weet niet altijd waarom."
- **Onderscheid van LO-006 expliciet maken.** Visuele inspectie kent voorbeelden van defect én goed; autoencoder kent alleen normaal en signaleert alles wat afwijkt. Dit onderscheid is belangrijk voor LO-108 (SHAP).
- **Concreet maken in fase 4.** "Mijn spuitgietmachine" is geen actieplan. Doorvragen: welke sensor — temperatuur, druk, trillingen — en welk verdacht-moment?

## Valkuilen

- **Trainer geeft te snel het antwoord op de quiz.** "Foto 3 is afwijkend" sluit het zelf-zoeken af. Het mens-AI-scharnier werkt alleen als deelnemers eerst zelf hebben geworsteld.
- **Reconstructiefout wordt te wiskundig.** Bij MSE of Euclidische afstand denkt operator dat hij wiskunde moet snappen en haakt af. Houd het visueel: invoer naast herstel, verschil zien.
- **Verwarring met visuele inspectie (LO-006).** "Is dit hetzelfde als die foto's?" — bevestig de overeenkomst (AI vergelijkt met wat het kent), benoem het verschil scherp.

## Voorbereiding (30 min vooraf)

- [ ] Vier werkbladen printen, n + 2 reserve
- [ ] Zes sensorgrafieken voorbereiden (4 normaal, 2 afwijkend) — geprint of op beamer
- [ ] SVG-diagram autoencoder-architectuur klaar
- [ ] Flap-over met drie-stappen-kapstok (invoer → samenvatting → herstel)
- [ ] U-opstelling, beamer + HDMI testen

## Transferopdracht

Geef de deelnemer mee om deze week één machine en één sensor te kiezen waar hij een verdacht-moment vermoedt, en op te schrijven welk patroon hij dan ziet. Bij de volgende sessie wordt dit voorbeeld kort gedeeld als opstap naar LO-108 (SHAP).

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** `../../trainee/lo-smart-mfg-093/lo-smart-mfg-093.yaml` (en wb-01 t/m wb-04)
