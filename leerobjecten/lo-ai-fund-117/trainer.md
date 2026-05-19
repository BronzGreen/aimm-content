---
id: lo-ai-fund-117-trainer
knowledge_object_id: ko-ai-fund-117
version: trainer
title: Drie vormen van machine learning — welke past bij welke maakindustrie-data?
  — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 42
status: validated
updated_at: '2026-05-19'
correlation_id: ronde9-lo-ai-fund-117
---

# Drie vormen van machine learning — voor de trainer

**Leerobject:** lo-ai-fund-117
**Kennisobject:** ko-ai-fund-117
**Doelgroep:** MBO-4 operator/teamleider, B1-B2 taalniveau
**Duur:** 42 min
**Bloom:** begrijpen
**Casus:** Sanne op Lijn B bij Van Daalen Plastics — Joyce (kwaliteit, InspectAI) en Karim (onderhoud, CycleAdvise)

## In één oogopslag

| | |
|---|---|
| Werkvormen | Vier scenariokaarten (contrastpaar 1A↔1B + twee externe cases), buurman-check, handout, individueel verkenningsblad, één-zin-rondje |
| Kolb-startfase | Ervaren (Sanne kijkt mee bij Joyce en Karim — twee Lijn-B-systemen + twee externe cases) |
| Begeleidingsstijl | Trainen — IK DOE op 1A, daarna contrast 1A↔1B, daarna 2 en 3 zelfstandig |
| Materialen | 4 werkbladen, beamer + Slidev, flipover voor signaalwoorden |

## Wat de deelnemer leert

De deelnemer kan de drie basisvormen herkennen: supervised (gelabelde voorbeelden), unsupervised (patronen zonder labels), reinforcement (leren door proberen met beloning). Belangrijk inzicht uit dit LO: **leerprincipe is niet hetzelfde als data-vorm**. Sanne ziet op Lijn B dat InspectAI (4.000 gelabelde foto's, Joyce) en CycleAdvise (4.000 gelabelde tabel-rijen, Karim) beide supervised zijn — totaal andere data, zelfde principe. Twee externe cases (lasrobot, verpakkingsrobot) maken het palet compleet. Voor de eigen lijn formuleert hij welke vorm past, of de data meer op foto's of een tabel lijkt, en welke vraag aan IT, kwaliteit of onderhoud te stellen. **Module 1B in de Sanne-casus** — na Module 1A (kennismaking met beide AI-systemen). Verwijst vooruit naar Module 1D (drempelkeuzes), 1C (kritisch denken bij bias) en lo-ai-fund-ml-001 (vier ML-leerklassen voor PdM).

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:12 | Vier scenariokaarten — IK DOE op 1A, daarna contrast 1B en zelf 2-3 | Individueel + IK DOE + contrast |
| Reflecteren | 0:12-0:22 | Buurman-check, contrast 1A↔1B expliciet, plenaire stemming | Duo + plenair |
| Theoretiseren | 0:22-0:32 | Handout drie vormen + drie-stappen-vraag | Trainer + handout |
| Experimenteren | 0:32-0:42 | Eigen lijn-verkenning + één-zin-rondje | Individueel + plenair-rondje |

## Tips voor de trainer

- **Doe case 1A hardop voor — kort.** Een minuut is genoeg. Spreek over Joyce die heeft gelabeld. Daarna leid je in 30 sec het contrast naar 1B: 'Op dezelfde lijn werkt nog een AI — Karim heeft een tabel gelabeld. Wat denk je: zelfde vorm of een andere?' Pas dan 1B zelf laten doen.
- **Maak het contrast 1A↔1B heilig.** Het kerninzicht van dit LO is: leerprincipe ≠ data-vorm. Twee Lijn-B-systemen tonen dat. Werkblad 1 heeft een expliciete vergelijktabel.
- **Per case één SIGNAALWOORD benoemen.** 1A: 'Joyce heeft gelabeld'. 1B: 'Karim heeft gelabeld'. 2: 'geen administratie'. 3: 'score per poging'.
- **Reinforcement bewust kort houden.** In de maakindustrie kom je vooral supervised en unsupervised tegen.
- **Cognitive load bewaken.** Twee AI-systemen tegelijk is intensief. Houd de uitleg per systeem kort — focus blijft op het contrast, niet op InspectAI of CycleAdvise zelf (die komen elders uitgebreider aan bod).
- **Maak de drie-stappen-vraag (slide 11) heilig.** Heeft iemand goed/fout aangegeven? → supervised. Feedback per poging? → reinforcement. Patronen vinden? → unsupervised.
- **Parkeer semi-supervised expliciet.** Komt iemand er mee: bevestig, parkeer naar lo-ai-fund-ml-001.

## Valkuilen

- **Deelnemers verwarren leerprincipe met data-vorm.** Iemand denkt: 'foto's = supervised, tabel = iets anders'. Bevestig: data-vorm zegt niks over de vorm. Wat telt is of er bij elk voorbeeld een antwoord staat. 1A en 1B zijn beide supervised — dat is precies waarom we ze naast elkaar laten zien.
- **Supervised wordt gezien als de "echte AI", anderen als minderwaardig.** Bevestig dat supervised veel gebruikt is — maar alleen als labels er zijn. Veel data heeft GEEN labels — dan is unsupervised mogelijk.
- **Cognitive overload door twee Lijn-B-systemen.** Risico bestaat. Beperk uitleg per systeem tot wie labelt (Joyce/Karim) en wat de data is (foto's/tabel). Geen technische diepte over InspectAI of CycleAdvise hier — dat komt in 1D en 1C.
- **Reinforcement uitgebreid behandelen.** Komt in de praktijk weinig voor bij operators. Houd 2 min.
- **Algoritmen uitleggen (k-means, deep learning, Q-learning).** Parkeer op flipover.

## Voorbereiding (25 min vooraf)

- [ ] 4 werkbladen printen (wb-01 t/m wb-04), 1 per deelnemer + 2 reserve
- [ ] Slidev-presentatie testen, HDMI klaar
- [ ] Flipover voorbereiden met 'Parkeerlijst' links en kolommen voor de vier cases rechts
- [ ] Optioneel: screenshot van een (fictieve) CycleAdvise-trainingstabel om plenair te tonen — versterkt 1B-herkenning
- [ ] Pen + markeerstift per deelnemer
- [ ] Timer of mobiel met geluid voor 5/6-min metingen

## Transferopdracht

Geef de deelnemer mee dat hij deze week één plek kiest op Lijn B of op zijn eigen lijn waar AI-ondersteuning nuttig zou zijn — inspectiestation, spuitgietmachine, sensor in het magazijn. Drie dingen noteren: (1) welke data verzamelen we daar nu al — foto's, tabel, iets anders? (2) heeft iemand goed of fout aangegeven in die data? (3) welke vorm past — supervised, unsupervised of reinforcement? Plus: lijkt het meer op InspectAI (foto's) of CycleAdvise (tabel)? Bonus: praat met een collega van kwaliteit of onderhoud over of er ergens wordt vastgelegd wanneer iets misgaat. Notities komen mee naar de volgende sessie.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
- **Vervolg-LO (verdieping):** `../trainer/lo-ai-fund-ml-001/`
- **Casus-bron:** `docs/casus-ai-fundamentals.md` (v2)
