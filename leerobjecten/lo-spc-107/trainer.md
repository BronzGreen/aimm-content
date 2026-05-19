---
id: lo-spc-107-trainer
knowledge_object_id: ko-spc-107
version: trainer
title: Control limits versus specificatiegrenzen — trainer-pakket
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
updated_at: '2026-05-19'
correlation_id: ronde8-lo-spc-107
---

# Control limits versus specificatiegrenzen — voor de trainer

**Leerobject:** lo-spc-107
**Kennisobject:** ko-spc-107
**Doelgroep:** MBO-3 operator (primair), MBO-4 (secundair); B1
**Duur:** 40 min
**Bloom:** begrijpen tot analyseren

## In één oogopslag

| | |
|---|---|
| Werkvormen | Spot-the-fout (3 voorbeeldkaarten, individueel), STARRT-reflectie, plenaire bespreking, handout met vergelijkingstabel + 3σ-formule + NIST-waarschuwing |
| Kolb-startfase | Ervaren — eerst zelf de foute kaart aanwijzen, dán de theorie |
| Begeleidingsstijl | Trainen — bewust onbekwaam, scherpe scaffolding rond UCL/LCL versus specs |
| Materialen | wb-01 t/m wb-03, A3-print diagram-lo-spc-107.svg (afgedekt tot blok 3), flip-over met PROCES/PRODUCT-kolommen + kernzin "Binnen specs ≠ onder controle" |

## Wat de deelnemer leert

De deelnemer kan in eigen woorden uitleggen wat het verschil is tussen control limits (UCL/LCL — proces-grenzen, uit data berekend op 3σ) en specificatiegrenzen (USL/LSL — product-grenzen, van de klant/ontwerp). Aan het einde van de sessie wijst hij/zij op een voorbeeld-regelkaart aan welke kaart fout is opgezet (control limits gelijk aan specs) en onderbouwt dat met de NIST-waarschuwing: signaalverlies. Voorwaarde voor lo-spc-108 (Cp/Cpk) en lo-spc-203 (out-of-control respons).

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:15 | Spot-the-fout: 3 voorbeeldkaarten — welke is fout? | IK DOE kaart 1 hardop, JIJ DOET 2 + 3 individueel |
| Reflecteren | 0:15-0:27 | STARRT — hoe zit het op jullie eigen kaarten? | Individueel + tweetallen + plenair |
| Theoretiseren | 0:27-0:40 | Handout: vergelijkingstabel + 3σ + NIST-waarschuwing | Trainer-geleide doorloop, A3 onthullen, markeren |

## Tips voor de trainer

- **Doe kaart 1 hardop voor (IK DOE).** "UCL en LCL liggen op 99 en 101 — precies de specs. Dat voelt logisch. Maar let op wat hier mis aan is..." Pas dan deelnemers zelf laten oordelen over kaart 2 + 3.
- **Park de "wel handig"-reactie kort.** Bij "dan weet je toch gewoon wanneer een stuk afgekeurd wordt": "Klopt voor de afkeur-vraag — maar de regelkaart is niet voor de afkeur-vraag. Noteer je gedachte; in blok 3 zie je waarom." Anders landt de NIST-waarschuwing niet.
- **Reageer ontspannen op "ik weet het niet".** "Je had het niet hoeven weten — niemand heeft het je verteld. Wat je nu wel weet is dat je de vraag kunt stellen." Schrijf op flip: "niet-weten is hier de startpositie, geen eindpunt." Beschermt CAR-relatie.
- **Geen statistiek-overload bij de 3σ-formule.** "σ is een maat voor hoeveel je metingen normaal heen en weer springen. Excel rekent het uit — je hoeft het zelf nooit te doen. Maar je moet wél weten wat UCL en LCL zíjn."
- **Bij "welke moet ik dan gebruiken?"** Wijs naar PROCES/PRODUCT-flipover: "Allebei, voor verschillende vragen. UCL/LCL voor: ingrijpen ja/nee. Specs voor: stuk naar de klant ja/nee. Nooit één lijn voor beide vragen."

## Valkuilen

- **Deelnemer vindt kaart B "wel handig" (specs als control limits).** Niet meteen corrigeren — parkeren tot blok 3, daar terugkoppelen: "Een trend van 99,8 naar 100,1 geeft hier geen signaal — terwijl het proces wel verschuift." Zonder interventie verlaat de deelnemer de sessie met "specs als UCL/LCL werkt prima".
- **Schaamte bij "ik weet het niet".** Ontspannen, normaliserend reageren — anders dichtklappen, passieve invul-modus, en het verhaal "deze workshop was niet voor mensen als ik" naar collega's.
- **Statistiek-overload bij 3σ-uitleg.** Frons + pen neer = teken om niet door te schieten. Houd het op "klein = dichtbij, groot = ver uit elkaar". Verwijs naar ISO 7870-2 voor wie meer wil. Anders mist deelnemer de scenariomatrix in blok 3.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer + 2 reserve)
- [ ] diagram-lo-spc-107.svg op A3 printen, afgedekt achter in zaal tot blok 3
- [ ] Flip-over: twee vellen — PROCES/PRODUCT-kolommen + kernzin "Binnen specs ≠ onder controle"
- [ ] Beamer + HDMI testen, presenter-modus, slides 4 en 8 met SVG-diagram klaar
- [ ] Pennen, markeerstiften, timer klaarleggen
- [ ] Voorbereiding zelf: kaart 1 hardop oefenen ("UCL = gemiddelde + 3σ" twee keer herhalen)

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week naar één regelkaart op de eigen lijn loopt, de waarden van UCL/LCL noteert, en aan teamleider of SPC-coördinator vraagt: "Komen deze grenzen uit de klantspecs of uit procesmetingen (3σ)?" Antwoord noteren. Tweede observatie: hangen er kaarten met specs EN control limits (twee aparte lijnen — goede praktijk) of één regel die beide rollen vervult (signaal)?

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
