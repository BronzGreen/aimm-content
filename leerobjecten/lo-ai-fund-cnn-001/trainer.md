---
id: lo-ai-fund-cnn-001-trainer
knowledge_object_id: ko-ai-fundamentals-cnn-001
version: trainer
title: CNN-architectuur — hoe een neuraal netwerk patronen leert herkennen — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 50
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-ai-fund-cnn-001
---

# CNN-architectuur — voor de trainer

**Leerobject:** lo-ai-fund-cnn-001
**Kennisobject:** ko-ai-fundamentals-cnn-001
**Doelgroep:** MBO-4 operator/teamleider, B2 taalniveau
**Duur:** 50 min
**Bloom:** begrijpen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Mini-college met meeschrijven, vier data-cases, plenaire bespreking, individueel actieplan |
| Kolb-startfase (de fase in de leercyclus waarmee de sessie begint) | Theoretiseren (mentaal model neerzetten, dan toepassen) |
| Begeleidingsstijl (instrueren / trainen / coachen / mentoren) | Trainen — gestructureerd voordoen + IK DOE / WIJ DOEN / JIJ DOET |
| Materialen | 4 werkbladen, SVG-diagram (CNN-architectuur), beamer, vergrootglas als rekwisiet |

## Wat de deelnemer leert

De deelnemer kan de standaardarchitectuur van een CNN benoemen — input, convolutielaag, pooling, fully connected, output — en uitleggen wat elke laag doet. Aan de hand van vier werkvloer-data-voorbeelden beoordeelt hij of een CNN passend is, op basis van lokale connectiviteit en ruimtelijke/volgordelijke structuur. Vereist data-lit-101 afgerond.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Theoretiseren | 0:00-0:17 | Mini-college: vier lagen van een CNN met diagram | Trainer + werkblad |
| Ervaren | 0:17-0:29 | Vier data-voorbeelden — past CNN hier? | Individueel + IK DOE worked example |
| Reflecteren | 0:29-0:39 | Plenaire bespreking + buurman-check | Duo + plenair |
| Experimenteren | 0:39-0:50 | Eigen lijn-scan: waar zou CNN passen? | Individueel actieplan |

## Tips voor de trainer

- **Gebruik het vergrootglas fysiek.** De speurder-analogie wordt tastbaar als je het voorwerp oppakt en over een denkbeeldige foto schuift. *"Krasje hier — krasje daar — randje — randje."*
- **Vermijd de wiskunde.** Operators haken af bij matrices. Bevestig: *"Je hoeft de wiskunde niet te kunnen — wel het idee. De rest laten we aan de leverancier."*
- **Convolutie versus pooling op flipover scherp tegenover elkaar.** Convolutie = patronen ZOEKEN. Pooling = comprimeren / robuust maken. Eén zoekt, één vat samen.
- **Voorbeeld A doe je voor (IK DOE), B-D doen ze zelf.** Worked example werkt — niet meer dan één case voor.
- **Verwijs voor ERP-tabel (case D) naar lo-ai-fund-ensemble-001.** Random forest of gradient boosting past bij tabular data zonder ruimtelijke structuur.

## Valkuilen

- **Deelnemer haakt af op "het is wiskunde".** Pak het vergrootglas, schuif fysiek. Het idee landt via beelden, niet via formules.
- **Convolutielaag en pooling-laag worden door elkaar gehaald.** Maak op flipover de twee functies tegenover elkaar. Geen ruimte voor verwarring.
- **Scenario D (ERP-tabel) wordt onterecht als CNN-case beoordeeld.** Stel de tegenvraag: *"Heeft de volgorde van kolommen betekenis?"* Antwoord: nee. Geen ruimtelijke structuur, geen CNN.

## Voorbereiding (15 min vooraf)

- [ ] 4 werkbladen printen (architectuur-invullen, data-voorbeelden, reflectie, actieplan), 1 per deelnemer + 2 reserve
- [ ] SVG-diagram (CNN-architectuur) op A3 zichtbaar in de zaal
- [ ] Beamer + Slidev-presentatie testen, HDMI-kabel klaar
- [ ] Vergrootglas (rekwisiet) klaarleggen
- [ ] Optioneel: korte feature-map-video (60-90 sec) klaarzetten voor fase 4
- [ ] Pen + markeerstift per deelnemer
- [ ] Flipover + dikke stiften voor parkeerlijst en lagen-flowschema

## Transferopdracht

Sluit af met: deelnemers kijken deze week op de eigen lijn — of bij een klant — naar een vision-AI of trillingsanalyse-systeem. Vraag de leverancier of IT-collega: gebruikt het systeem een CNN? Wat is de input — beeld of tijdreeks? Welk type defect herkent het, en welk juist niet? Schrijf de antwoorden op en koppel ze aan de architectuur-uitleg.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
