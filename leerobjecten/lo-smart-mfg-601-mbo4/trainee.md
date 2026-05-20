---
id: lo-smart-mfg-601-mbo4-trainee
knowledge_object_id: ko-smart-mfg-601
version: trainee
title: Gelabelde data is de echte bottleneck bij computer vision
target_audience: operator
content_level: MBO-4
language_level: B2
bloom_level: toepassen
knowledge_type: conditioneel
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 40
status: validated
updated_at: '2026-05-20'
correlation_id: ronde28-lo-smart-mfg-601-mbo4
---

# Hoeveel labelwerk kost een AI-camerasysteem eenmalig, en hoeveel inspectietijd bespaart het per jaar?

Als MBO-4 operator of aanstaande teamleider praat je steeds vaker mee over beslissingen rond kwaliteitscontrole. *"Kunnen we niet een AI-systeem kopen?"* — die vraag krijg jij van je productie-manager. Deze sessie geeft je de getallen om die vraag serieus te benaderen.


## Wat leer je?

Je kunt de kosten-baten-afweging van handmatig labelen uitleggen aan een teamleider, met schatting van labeltijd en daarmee te winnen inspectietijd.

## Waarom de data het werk is, niet het model

Een AI-camerasysteem leert herkennen wat goed is en wat afkeur. Maar het leert dat niet uit zichzelf. Iemand moet het systeem **labelen**: deze foto is goed, deze foto is een kras, deze foto is een deuk. Pas met genoeg gelabelde foto's kan het model patronen leren.

Voor een werkbaar systeem heb je per defect-categorie ongeveer **150 foto's** nodig. Voor drie categorieën dus 450. Bij **1 tot 3 minuten labeltijd per foto** kost dat **5 tot 20 uur** eenmalig werk, afhankelijk van strengheid en consistentie.

Dat klinkt veel. Maar reken het eens af tegen de jaarlijkse handmatige inspectie.

## De ROI-vergelijking

Stel: jouw productielijn maakt **400 producten per dienst**, **5 diensten per week**, **48 weken per jaar**. Per product is **30 seconden** handmatige inspectie nodig.

Jaarlijkse inspectietijd:

> 400 × 5 × 48 × 30 sec = **80 uur per jaar**

Eenmalig labelwerk voor een AI-systeem:

> 450 foto's × 2 min = **15 uur eenmalig**

Ratio: **15 uur eenmalig vs 80 uur per jaar**. Het labelwerk verdient zich na **iets meer dan 2 maanden** terug.

## Het schema voor jouw lijn

| Vraag | Hoe je het schat |
|---|---|
| Hoeveel labeluren eenmalig? | aantal categorieën × 150 foto's × 2 min |
| Hoeveel inspectie-uren per jaar? | producten/dienst × diensten/week × weken/jaar × tijd/inspectie |
| Wat is de ratio? | labeluren ÷ inspectie-uren-per-jaar |
| Wanneer terugverdient? | ratio × 12 maanden |

Drie getallen, één rekensom. Geen complete businesscase — wél een gesprek-startend cijfer.

## De variatie-factor

Niet elke productlijn is gelijk. Hoe meer **variatie** in je product, hoe meer foto's nodig.

| Type product | Foto's per categorie |
|---|---|
| Strakke, uniforme producten (bijv. metalen connectoren) | 150 (basis-vuistregel) |
| Productlijn met variatie (verschillende series, posities, belichting) | 300-500 |
| Sterk wisselende producten of nieuwe defecten regelmatig | 500+ |

Stel ook de vraag: **wie labelt?** Twee labelaars leveren niet automatisch dubbele data. Als ze inconsistent labelen (de een noemt het kras, de ander groef), wordt de dataset zwakker, niet sterker. Eén goed afgestemde labelaar beats twee ongecoördineerde.

## Wat de getallen niet vertellen

Een ratio van 2 maanden klinkt aantrekkelijk. Maar het besluit hangt niet alleen van de ratio af:

- **Hardware-kosten** — camera, computers, kabels, schermen kosten tienduizenden euro's
- **Software-licenties** — vaak jaarlijkse fee
- **Onderhoud** — het systeem moet onderhouden worden, herijkt
- **Cultuur** — de afdeling moet vertrouwen krijgen in het systeem
- **Continuïteit** — wat als de leverancier failliet gaat?

De getallen openen het gesprek. Ze beëindigen het niet.

## Het gesprek met je teamleider

Als je deze drie cijfers hebt — labeluren, inspectie-uren-per-jaar, ratio — kun je naar je teamleider met:

> *"Voor onze lijn schat ik [X] uur labelwerk eenmalig versus [Y] uur jaarlijkse inspectie. Ratio is [Z] maanden terugverdientijd op het labelwerk. Klopt deze afweging volgens jou? Wat zou je aanpassen?"*

Concrete getallen in plaats van abstracte argumenten. Dat is het verschil tussen een operator die meedenkt en een operator die wacht op richtingen.

## Na deze sessie

Stel binnen één week de getallen uit deze sessie voor aan je teamleider of productie-manager. Vraag: *"Is deze afweging realistisch voor onze lijn?"* Noteer het antwoord. Let vooral op welke cijfers zij aanvullen of bijstellen — dat is de praktijkcorrectie op jouw schatting. Lees daarnaast één artikel over ROI van AI-kwaliteitscontrole (zoekterm: *"ROI AI quality inspection"*). Een Engelstalige bron is prima — op MBO-4-niveau kom je die bronnen gewoon tegen.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-storingsquiz.md`](./werkbladen/wb-01-storingsquiz.md) — Storingsquiz
2. [`wb-02-reflectie.md`](./werkbladen/wb-02-reflectie.md) — Reflectie
3. [`wb-03-theorie-handout.md`](./werkbladen/wb-03-theorie-handout.md) — Theorie handout
4. [`wb-04-roi-afweging.md`](./werkbladen/wb-04-roi-afweging.md) — Roi afweging

## Verder

- Onderliggend kennisobject: [`ko-smart-mfg-601`](../../kennisbank/smart_manufacturing/computer_vision_kwaliteit/ko-smart-mfg-601.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
