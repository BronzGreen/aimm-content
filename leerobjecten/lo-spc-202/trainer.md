---
id: lo-spc-202-trainer
knowledge_object_id: ko-spc-202
version: trainer
title: Gevoeligheid versus vals alarm — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 40
status: validated
updated_at: '2026-05-20'
correlation_id: ronde15-lo-spc-202
---

# Gevoeligheid versus vals alarm — voor de trainer

**Leerobject:** lo-spc-202
**Kennisobject:** ko-spc-202
**Doelgroep:** MBO-3 operator (primair), MBO-4 (secundair); B1-B2
**Duur:** 40 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Alarm-rekenoefening (96 metingen/dag, drie regelsets, individueel), STARRT-reflectie + buurman-check, handout met ARL-tabel + gefaseerde aanpak |
| Kolb-startfase | Ervaren — eerst rekenen op realistische cijfers, dán theoretische kader |
| Begeleidingsstijl | Trainen — bewust onbekwaam, IK DOE 371/96 ≈ 3,9 |
| Materialen | wb-01 t/m wb-03, A3-print diagram-lo-spc-202.svg, rekenmachines/telefoons, flip-over met drie koppen Kaal / WECO / Nelson |

## Wat de deelnemer leert

De deelnemer kan uitleggen waarom méér signaalregels niet automatisch beter is door het onderscheid signaal/vals alarm te benoemen, en kan op basis van de ARL-getallen (371 voor kale Shewhart; 91,75 voor +WECO — Champ & Woodall 1987) voorspellen hoeveel vals alarm een regelset oplevert. Aan het einde berekent hij/zij in minimaal 2 van de 3 regelsets correct het aantal valse alarmen per dag bij 96 metingen, en benoemt waarom alarm-fatigue een echt productierisico is.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:15 | Alarm-rekenoefening: 3 regelsets op 96 metingen/dag | IK DOE 371/96, JIJ DOET WECO + Nelson |
| Reflecteren | 0:15-0:27 | STARRT — eigen ervaring met vals alarm | Individueel + tweetallen + plenair (1-2 vrijwillig) |
| Theoretiseren | 0:27-0:40 | Handout: 3 regelsets + ARL + gefaseerde aanpak | Trainer-geleide doorloop, A3, markeren |

## Tips voor de trainer

- **Demonstreer eerst één rekensom plenair.** "96 punten/dag, ARL 371. Dan is 371/96 ≈ 3,9 — eens per ~4 dagen vals alarm. Prima te doen." Pas dán deelnemers zelf laten rekenen voor WECO en Nelson.
- **Houd Nelson op één zin.** "8 regels, strenger dan WECO, meer vals alarm. De regels zelf komen in latere sessies." Niet meer. Anders verdrinkt de centrale boodschap (gevoeligheid vs vals alarm).
- **Bij rekensom-blokkade: ondersteun, niet beschamen.** "De rekensom is delen — je rekenmachine doet het. Wat ik wil weten is wat je voelt bij de uitkomst. 96/91,75 ≈ 1 vals alarm per dag. Wat vind je daarvan?"
- **Erken twijfel over 91,75.** "Dat is theoretisch, bij een exact WECO-geconfigureerd stabiel proces. Bedoeling: orde van grootte — veel meer dan kale Shewhart, veel minder dan Nelson. Jouw lijn heeft een eigen plek; dat ga je deze week opzoeken." Verbind aan transferopdracht.
- **Bij defensief "ik negeer alarmen nooit": niet in discussie.** "Je bent blijkbaar goed afgestemd — schrijf op: welke regelset staat aan, en hoe heb je dat geleerd?" Verplaats van verdedigen naar reflectie.
- **Bewaak reflectie-modus in tweetallen.** Bij discussie: "We zijn in reflectie-modus, niet bespreking-modus. Elkaar horen is het doel — niet gelijk krijgen. Nog 1 minuut."

## Valkuilen

- **Alle 8 Nelson-regels willen leren.** "Een deel staat in de handout. Vandaag gaat het niet om regels kennen — om de afweging begrijpen." Verwijs naar module 3. Anders verdrinkt de centrale boodschap.
- **Twijfel aan het getal 91,75.** Niet ontkennen, contextualiseren als orde van grootte en de variatie verbinden aan de transferopdracht. Anders verliest de theoretische onderbouwing gezag.
- **CUSUM/EWMA-vraag.** Park: "Andere kaarttypes met een ander gevoeligheidsprofiel — eventueel module 3. Vandaag Shewhart, want 90% van de lijnen gebruikt dat." Schrijf op parkeerflip.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer + 2 reserve)
- [ ] diagram-lo-spc-202.svg op A3 printen, achter in zaal hangen
- [ ] Flip-over: drie koppen Kaal / WECO / Nelson
- [ ] Beamer + HDMI testen, slide 8 met SVG (gefaseerde aanpak + bronslide optioneel)
- [ ] 4-5 reserve rekenmachines (deelnemers gebruiken eigen telefoon)
- [ ] Pennen, markeerstiften, timer klaarleggen

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week op de eigen lijn navraagt welke signaalregels actief zijn (alleen ±3σ / +WECO / +Nelson), via teamleider, dashboard of engineering. Notitie in werkschrift: welke regels, hoe vaak alarm per dag, klopt dat met wat je nu weet over ARL? Plus één gesprek met de teamleider: "Waarom staat op onze lijn deze regelset en niet een andere?" Vaak een bewuste keuze — of niemand weet het meer (ook informatie).

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
