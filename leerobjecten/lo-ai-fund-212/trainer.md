---
id: lo-ai-fund-212-trainer
knowledge_object_id: ko-ai-fund-212
version: trainer
title: Hoe weet je of een AI-model écht goed werkt? — trainer-pakket (confusion matrix,
  precision en recall)
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: analyseren
knowledge_type: declaratief
competency_stage: bewust_bekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-ai-fund-212
---

# Confusion matrix, precision en recall — voor de trainer

**Leerobject:** lo-ai-fund-212
**Kennisobject:** ko-ai-fund-212
**Doelgroep:** MBO-4 operator (primair), teamleider MBO-4 (secundair), B1-B2 taalniveau
**Duur:** 45 min
**Bloom:** analyseren — **Kirkpatrick:** gedrag
**Stadium (Hersey & Blanchard):** bewust_bekwaam — **Begeleidingsstijl (manier van begeleiden):** instrueren

## In één oogopslag

| | |
|---|---|
| Werkvormen | Twee uitgewerkte 2x2 confusion matrices lezen (vleesverwerker), precision en recall narekenen, plenair gesprek twee scenario's (luxe-segment + voedselveiligheid), eigen werkvloer-AI doorlichten |
| Kolb-startfase (leerfase) | Ervaren — deelnemer leest matrices in werkvloer-taal vóór de formules komen |
| Scaffolding-drieluik | IK DOE (matrix A hardop, 3 min) → WIJ DOEN (samen narekenen + duo's, 10 min) → JIJ DOET (eigen werkvloer-AI, 10 min) |
| Materialen | 4 werkbladen, beamer + Slidev, flip-over, rekenmachine per deelnemer |

## Wat de deelnemer leert

De deelnemer kan na deze sessie een confusion matrix (verwarrings-matrix) lezen, precision (precisie) en recall (terugvinden) zelf berekenen, en onderbouwd kiezen welke van de twee maten voor zijn eigen werkvloer-AI prioriteit moet krijgen. Hij benoemt de vier kwadranten in werkvloer-taal — terecht positief, vals positief (gemist), vals negatief (vals-alarm), terecht negatief — en kan twee contrasterende scenario's (luxe-segment versus voedselveiligheid) analyseren op welke fout duurder is. **Bloom analyseren** + **Kirkpatrick gedrag** — één concrete vraag voor leverancier/IT/kwaliteit deze week is de toets van transfer. **Derde hands-on LO Module 2 (Train).**

## Sessie-opbouw

| Kolb-fase (leerfase) | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 00:00-00:12 | Twee confusion matrices lezen (strenge + soepele drempel) | Individueel (trainer doet matrix A hardop voor — IK DOE, 3 min) |
| Theoretiseren | 00:12-00:22 | Precision en recall — formules + narekenen matrix A en B | Plenair (WIJ DOEN matrix A) + duo's (matrix B) |
| Reflecteren | 00:22-00:35 | Welke fout duurder? — twee scenario's + eigen werkvloer-keuze | Plenair gesprek + individueel schrijven + plenaire ronde |
| Experimenteren | 00:35-00:45 | Eigen werkvloer-AI doorlichten + vraag voor deze week | Individueel + plenaire één-zin-ronde |

## Tips voor de trainer

- **Instrueren, niet improviseren.** De formules vereisen wiskundige helderheid. Schrijf precision en recall apart op het bord, niet onder elkaar in één blok. Reken matrix A samen vóór duo's matrix B alleen aanpakken. *"Check elkaars breuk — niet je intuïtie."*
- **Conventie expliciet maken.** In dit LO is *"positief = model zegt GOED, negatief = model zegt AFGEKEURD"*. Zonder die conventie raken alle kwadranten verward. Schrijf vier werkvloer-zinnen op het bord en wijs er terug bij elke formule-stap.
- **Geen formule in fase 1.** Strikt scheiden: fase 1 = tellen + werkvloer-taal, geen woord precision/recall. Slides 3-5 tonen alleen de matrices en kwadrant-vragen. Bij vroege vraag naar de berekening: *"Wat zou je willen weten — of het model gelijk heeft als het afkeurt, of of het alle afkeur vindt?"* Beide vragen worden straks formules.
- **Trade-off zichtbaar maken.** Schrijf na fase 2 vier getallen groot op het bord — precision A = 77%, recall A = 85%, precision B = 57%, recall B = 100%. Vraag *"wat valt je op?"* en wacht 7 seconden. De groep moet zelf zien: één stijgt, de andere zakt.
- **Bedrijfslogica-regel laten ontstaan, niet doceren.** In fase 3 niet zelf 'luxe = precision, voedsel = recall' opschrijven. Stel kostenvragen: *"wat kost een vals positief op een handgemaakt horloge? En een vals negatief?"* Pas als de groep de regel formuleert, schrijf je hem op het bord.

## Top-3 valkuilen

- **Deelnemers verwarren TP/FP/FN/TN-kwadranten.** Conventie *"positief = goed, negatief = afgekeurd"* steeds expliciet, en de academische termen altijd direct in werkvloer-taal vertalen op het bord. Bij vergissing corrigeer je met de werkvloer-vertaling — niet met de term.
- **Trainer geeft zelf het antwoord op de duurder-vraag.** Bij scenario's luxe-segment en voedselveiligheid de redenatie aan de groep laten. Kostenvragen stellen, 7 seconden stilte, één deelnemer rekent voor. De regel is dán van de groep.
- **Rekenfouten in fase 2 onopgemerkt laten.** Plenair narekenen op het bord. Schrijf 20/(20+15) groot. *"Wie heeft een ander getal?"* Bij verschil: stap voor stap terug naar teller en noemer.

## Voorbereiding (20 min vooraf)

- [ ] 4 werkbladen printen (wb-01 t/m wb-04), 1 per deelnemer + 2 reserve
- [ ] Beamer + Slidev-presentatie testen, HDMI klaar
- [ ] Pen per deelnemer + 5 reserve, 2 reserve-rekenmachines (telefoon is OK)
- [ ] Flip-over of bord — drie velden voorbereiden: links 2x2 matrix-veld (voor matrix A), midden veld voor twee formules naast elkaar (verschijnt in fase 2), rechts veld voor bedrijfslogica-regel (verschijnt in fase 3)
- [ ] Vier werkvloer-zinnen vooraf opschrijven (op apart bordvlak, eerst afgedekt): *"goed product, terecht doorgelaten / goed product, onterecht afgekeurd / afgekeurd product, onterecht doorgelaten / afgekeurd product, terecht afgekeurd"*
- [ ] Voor jezelf: reken matrix A en B een keer zelf uit met pen op papier. Dat is je IK DOE-zelfvertrouwen voor fase 1 en 2.

## Transferopdracht

De deelnemer doet deze week drie stappen op zijn eigen lijn. **Stap 1:** kies één concrete AI-toepassing op je lijn — inspectiecamera, sorteersysteem, afkeur-camera of visuele eindcontrole. Schrijf op wat een vals positief is en wat een vals negatief is in jouw situatie. **Stap 2:** stel één concrete vraag aan leverancier, IT of kwaliteit. Bijvoorbeeld *"wat is de recall van onze afkeur-camera op de zomerlijn?"* of *"hoe vaak wordt de precision opnieuw gemeten?"* **Stap 3:** noteer het getal dat terugkomt — datum laatste rapport, precision/recall in dat rapport, of de drempelinstelling die nu actief is. Neem alle drie de uitkomsten mee naar de volgende sessie. Bonus: praat deze week één keer met een collega over een afkeur-moment op de lijn — *"was dit een vals positief of een vals negatief?"* Vaak ontdek je dat collega's de twee fout-soorten anders waarderen.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev-presentatie:** `lo-ai-fund-212-presentatie.slidev.md`
- **Trainee-versie:** [`trainee.md`](./trainee.md)
- **Werkbladen:** `../../trainee/lo-ai-fund-212/werkbladen/`
