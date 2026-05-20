---
id: lo-ai-fund-133-trainer
knowledge_object_id: ko-ai-fund-133
version: trainer
title: Classificatie — AI die producten of signalen in categorieën indeelt — trainer-pakket
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
correlation_id: ronde12-lo-ai-fund-133
---

# Classificatie — etiket plus zekerheid — voor de trainer

**Leerobject:** lo-ai-fund-133
**Kennisobject:** ko-ai-fund-133
**Doelgroep:** MBO-4 operator, B1-B2 taalniveau
**Duur:** 40 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | IK DOE binair voorbeeld, duo's multi-class, plenaire handout, individueel twijfelgeval |
| Kolb-startfase | Ervaren (gefreesd onderdeel + uitslag bekijken) |
| Begeleidingsstijl | Instrueren — sturend, met ruimte voor eigen oordeel bij twijfelgevallen |
| Materialen | 4 werkbladen, foto's (CNC-onderdeel + 4 multi-class), flip-over voor 4 begrippen |

## Wat de deelnemer leert

De deelnemer kan uitleggen dat classificatie een KLASSE (etiket) als output geeft — geen getal — en het onderscheid maken tussen binair (twee opties) en multi-class (meer dan twee). Het zekerheidspercentage interpreteert hij correct als "hoe zeker is het model" en niet als "hoeveel procent van het product is X". Bij een twijfelgeval (60/40) beschrijft hij een redelijke handelwijze (doorlaten, handmatig nakijken of drempel-aanpassen) gemotiveerd vanuit de context van de eigen lijn.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren (IK DOE) | 0:00-0:08 | Binair voorbeeld — CNC-onderdeel | Trainer demonstreert hardop denken |
| Ervaren (WIJ DOEN) | 0:08-0:18 | Multi-class — vier foto's | Duo's bespreken |
| Theoretiseren | 0:18-0:28 | Handout: binair/multi-class + zekerheid | Trainer + handout |
| Experimenteren (JIJ DOET) | 0:28-0:40 | Twijfelgeval 60/40 | Individueel werkblad |

## Tips voor de trainer

- **Doe het binaire voorbeeld langzaam voor (IK DOE).** Spreek hardop uit: klasse + zekerheid. *"Het model geeft een ETIKET terug, geen getal. Dat percentage is HOE ZEKER het model is."* Tempo bepaalt of de groep mee kan.
- **Laat de term "multi-class" bottom-up komen.** In fase 2: deelnemers tellen zelf de klassen (vier). Pas dan benoem je dat dit "multi-class" heet. Niet andersom.
- **De percentage-misinterpretatie is HET kernpunt.** Veel operators denken dat "78% kras" iets zegt over het product. Het zegt iets over het MODEL. Gebruik de collega-vergelijking: "Een collega die kijkt en zegt — ik denk een kras, maar twijfel een beetje. Die twijfel is wat het percentage uitdrukt."
- **Bij het twijfelgeval (60/40) geen één juist antwoord geven.** Drie handelwijzen zijn alle drie legitiem afhankelijk van context. Het inzicht is dat de operator zelf afweegt — kennis van de lijn weegt mee. Dat is haar professionaliteit.
- **Vermijd technisch jargon.** Geen softmax, geen logits, geen Q-learning. "Klasse" en "zekerheid" zijn genoeg. Algoritmes komen elders.

## Valkuilen

- **Percentage als product-eigenschap.** Iemand zegt: "78% kras betekent dat 78% van het oppervlak een kras heeft." Stop direct. Maak expliciet dat het de zekerheid van het MODEL is, niet een meting van het product.
- **Classificatie en regressie verward.** Iemand noemt "23 cycli tot uitval" als classificatie-voorbeeld. Maak het onderscheid hardop: classificatie = WOORD, regressie = GETAL. Vuistregel meegeven.
- **"Boven 90% is altijd te vertrouwen."** Niet als regel stellen. Er is GEEN vast getal — fout-kosten bepalen drempels. Sierdeel anders dan veiligheidscomponent. Operator-oordeel weegt mee.

## Voorbereiding (25 min vooraf)

- [ ] 4 werkbladen printen (wb-01 t/m wb-04), n + 2 reserve. Let op: wb-02 is per duo
- [ ] Foto's testen op beamer — beeldkwaliteit cruciaal voor foto-interpretatie
- [ ] Beamer + Slidev, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flip-over voor parkeerlijst + 4 begrippen-overzicht (classificatie / binair / multi-class / zekerheid)
- [ ] Werkbladen wb-02 (per duo), wb-03 en wb-04 (per deelnemer) gefaseerd uitdelen

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week eenmaal langs een kwaliteits- of inspectiesysteem op de eigen lijn loopt — een camera, een dashboard met goed/afgekeurd-meldingen, of een storingsclassificatie. Drie dingen noteren: welk type classificatie (binair of multi-class), welke klassen het systeem kent, en de laagste zekerheid die in die week voorkomt. Daarnaast: vraag aan een collega *"Wat doe jij als het systeem twijfelt?"* — vaak hanteert iedereen een eigen huisregel, en dat is een mooi gesprek voor het hele team.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
