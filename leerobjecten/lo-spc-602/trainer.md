---
id: lo-spc-602-trainer
knowledge_object_id: ko-spc-602
version: trainer
title: AI als aanvulling op SPC — wanneer klassieke regels tekortschieten — trainer-pakket
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
correlation_id: ronde27-lo-spc-602
---

# AI als aanvulling op SPC — wanneer klassieke regels tekortschieten — voor de trainer

**Leerobject:** lo-spc-602
**Kennisobject:** ko-spc-602
**Doelgroep:** Teamleider HBO (primair), teamleider MBO-4 (secundair); B2
**Duur:** 25 min (eerste helft van workshop-blok 'AI + alarmrationalisatie ontwerpen' van 50 min — direct gevolgd door lo-spc-603)
**Bloom:** evalueren

## In één oogopslag

| | |
|---|---|
| Werkvormen | Klassiek-vs-AI tabel met drie typische lijn-vragen + 2 eigen vragen, eigen lijn-screen op vijf criteria, plenaire peer-vergelijking met conclusie-uitwisseling |
| Kolb-startfase | Theoretiseren — kort kader (vergelijkingstabel), dán toepassen, dán peer-reflectie |
| Begeleidingsstijl | Coachen — bewust bekwaam, denker-HBO, géén instructie maar sparring + scherpe vragen |
| Materialen | wb-01 t/m wb-03, optioneel SHAP-screenshot uit publieke literatuur, flip-over met 'klassieke vraag vs AI-vraag'-tweedeling, parkeerflip voor SHAP/LIME-detail |

## Wat de deelnemer leert

De deelnemer kan beoordelen voor welke specifieke vraag op de eigen lijn een AI-uitbreiding op klassieke SPC zinvol is, kan benoemen waarom Nelson-rules dáárvoor tekortschieten, en kan inschatten welke randvoorwaarden (data, multivariate verbanden, explainable AI) nodig zijn. Aan het einde levert hij/zij een onderbouwde keuze tussen klassieke SPC of AI-uitbreiding voor minimaal één concrete vraag, plus minimaal twee randvoorwaarden waaraan de eigen organisatie wel of niet voldoet.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Theoretiseren | 0:00-0:08 | Klassiek vs AI — drie typische vragen + 2 eigen vragen | Individueel wb-01, geen uitleg vooraf |
| Experimenteren | 0:08-0:17 | Eigen lijn-screen op 5 criteria | Individueel wb-02, trainer rondloopt |
| Reflecteren | 0:17-0:25 | Plenaire peer-vergelijking, AI-keuze toetsen | Tweetallen 3 min + plenair 30 sec/persoon |

## Tips voor de trainer

- **Centrale onderscheid expliciet houden.** Klassieke SPC vraagt "is het proces NU anders dan normaal?", AI vraagt "welk patroon leidt naar verstoring?", XAI vraagt "welke signalen dragen het meest bij?". Beide vragen blijven relevant.
- **Bij "AI is magisch": vraag naar data.** "Hoeveel maanden labelled historie? Sensor-drift-cyclus?" Geen data = geen AI. Minimaal 6-12 maanden representatieve historie inclusief storingen. Verwijs naar Module 1 voor data-foundation.
- **Bij "Nelson afschaffen": stop kort.** "Het KO is hierover ondubbelzinnig: Nelson is NIET verouderd. Andere vraag dan AI. AI vult aan multivariate samenhang — niet vervangen." Reactor-voorbeeld: 10 sensoren binnen ±3σ, collectief alarmpatroon.
- **Bij black-box-acceptatie: maak concreet.** "Stel je operator krijgt alarm zonder uitleg — negeert hij of stopt hij op vermoeden? XAI is voorwaarde voor operator-vertrouwen, geen luxe." Reactor-voorbeeld: SHAP geeft 'druk 45%, temperatuur 30%, debiet 25%'.
- **Bij multivariate AI zonder voldoende historie: coach.** "Welke historie nu beschikbaar? Hoeveel daarvan dekt storingscondities? Sensor-drift-cyclus?" Vuistregel: 6-12 maanden + storingen. Zonder storingen in historie = geen patroon te leren.
- **SHAP/LIME op concept-niveau.** Eén zin per term: "SHAP geeft per signaal een bijdrage-percentage. LIME geeft een lokaal vereenvoudigd model rond één voorspelling." Verder niets — verwijs naar Technometrics 2024 review of Lundberg & Lee (2017) voor verdieping.
- **Coach, doceer niet.** Vaste opening: "Welke vraag beantwoordt jouw huidige SPC nu wél? Welke kan het niet?" Tel innerlijk tot 7. HBO-doelgroep komt voor sparring, niet instructie.
- **Verwarring met lo-spc-603 (alarmrationalisatie): parkeer voor volgende blok.**

## Valkuilen

- **Teamleider ziet AI als magisch (data niet nodig).** Vraag terug naar historie + MSA. Anders mislukt AI-pilot, vertrouwen in AI én SPC keldert.
- **Teamleider wil Nelson afschaffen.** Stop kort, expliciet onderscheid + reactor-voorbeeld. Anders adviseert hij SPC af te bouwen — operators raken referentiekader kwijt.
- **XAI overgeslagen, akkoord met black box.** Maak concreet wat operator zonder uitleg doet. Anders ROI = nul.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer + 2 reserve)
- [ ] Optioneel: SHAP-screenshot uit publieke literatuur als hand-around
- [ ] Flip-over: 'klassieke vraag vs AI-vraag'-tweedeling
- [ ] Parkeerflip: SHAP/LIME-detail, dashboardleveranciers
- [ ] Beamer + HDMI testen, presenter-modus
- [ ] Pennen, markeerstiften, timer (8/9/8 min) klaarleggen

## Transferopdracht

Geef de deelnemer mee dat hij/zij vóór de volgende sessie één concrete vraag op de eigen lijn identificeert waar de huidige monitoring tekortschiet. In een halve A4: welke vraag, welke variabelen samenhangend, hoeveel historische data, wat zou AI hierover kunnen zeggen wat Nelson niet kan? Voorlopige conclusie + 2 argumenten. Plus: gesprek met interne data-analist of IT-collega: "Hebben wij data-historie en XAI-tooling om hier iets zinvols mee te doen?"

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
