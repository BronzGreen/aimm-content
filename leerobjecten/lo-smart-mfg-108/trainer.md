---
id: lo-smart-mfg-108-trainer
knowledge_object_id: ko-smart-mfg-108
version: trainer
title: 'SHAP: welke sensor draagt bij aan de anomalie? — trainer-pakket'
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
correlation_id: ronde20-lo-smart-mfg-108
---

# SHAP: welke sensor draagt bij aan de anomalie? — voor de trainer

**Leerobject:** lo-smart-mfg-108
**Kennisobject:** ko-smart-mfg-108
**Doelgroep:** MBO-3 operator, B1 taalniveau
**Duur:** 30 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Storingsquiz 5 anomaliemeldingen, duo-reflectie, korte uitleg SHAP-grafiek, individuele oefening met 3 grafieken |
| Kolb-startfase | Ervaren — bewust frustrerende quiz: zonder SHAP raadt niemand het goed |
| Begeleidingsstijl | Trainen — drie leesregels (groot/rood/blauw) als kapstok |
| Materialen | Vier werkbladen, SVG-balkdiagram, flap-over leesregels, beamer verplicht |

## Wat de deelnemer leert

De deelnemer kan in een SHAP-grafiek de drie sensoren aanwijzen die het meest bijdragen aan een anomalie en per sensor in eigen woorden uitleggen waarom die afwijkt. Bij een SHAP-visualisatie op een dashboard na een anomaliemelding leest hij groot/rood/blauw correct af.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:08 | Storingsquiz 5 meldingen — welke sensor? | Individuele quiz |
| Reflecteren | 0:08-0:15 | Hoe doe je dit nu zonder SHAP? | Duo + plenair |
| Theoretiseren | 0:15-0:23 | Drie leesregels SHAP — groot, rood, blauw | Trainer + diagram |
| Experimenteren | 0:23-0:30 | Drie nieuwe SHAP-grafieken zelf lezen | Individueel + duo |

## Tips voor de trainer

- **Vermijd de afkorting SHAP tot fase 3.** Begin met "het systeem laat zien WAAR het probleem zit". Pas wanneer de grafiek begrepen is, kort de naam: "SHAP — een grafiekje dat AI-uitleg geeft".
- **De frustratie in fase 1 is leerkracht.** "Zonder SHAP raadt niemand het goed — dat is precies de pijn die SHAP oplost." Maak van de fout-ervaring de springplank.
- **Drie leesregels vasthouden.** Groot = belangrijk; rood = hoger dan normaal; blauw = lager dan normaal. Niets meer. Geen 'features' of 'feature importance'.
- **SHAP is advies, geen bevel.** Maak expliciet: "Klopt dat met wat je hoort/voelt aan de machine?" Bij conflict wint het oordeel van de operator. Schrijf op flap-over: SHAP wijst aan, jij beslist.
- **Geef ruimte in fase 4.** "Doe minimaal 1 grafiek goed. Twee is mooi. Drie is bonus." Kwaliteit boven snelheid.

## Valkuilen

- **Trainer schiet door naar 'feature importance' / 'machine learning interpretability'.** MBO-3 raakt het spoor kwijt. Drie woorden volstaan: sensor, bijdrage, kleur.
- **Quiz-frustratie wordt niet genormaliseerd.** Sfeer-dip die niet hersteld wordt. Expliciet zeggen: "iedereen raadt fout — daar leren we van".
- **Operator vertrouwt SHAP blindelings.** "SHAP zegt sensor X, dus ik vervang die." Maak het advies-karakter onmiskenbaar.

## Voorbereiding (35 min vooraf)

- [ ] Vier werkbladen printen, n + 2 reserve
- [ ] SHAP-balkdiagram met legenda klaar op slides
- [ ] 5 anomaliemeldingen + 3 oefen-SHAP-grafieken op slides
- [ ] Flap-over met drie leesregels (groot=belangrijk / rood=afwijkend hoog / blauw=afwijkend laag)
- [ ] Beamer + HDMI getest — dit LO is niet zonder beamer te geven
- [ ] U-opstelling, timer met geluid

## Transferopdracht

Geef de deelnemer mee om bij de eerstvolgende anomaliemelding op zijn werkvloer de SHAP-grafiek te lezen volgens de drie regels en de actie te onderbouwen. Hij vergelijkt zijn oordeel met wat hij hoort/voelt aan de machine en noteert het voor het team. Verwijs vooruit naar LO-205 (werkorder) en LO-094 (terecht/vals alarm).

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** `../../trainee/lo-smart-mfg-108/lo-smart-mfg-108.yaml` (en wb-01 t/m wb-04)
