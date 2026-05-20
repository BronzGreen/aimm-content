---
id: lo-industry40-303-trainee
knowledge_object_id: ko-industry40-303
version: trainee
title: Drempels instellen en alarm-rationalisatie — operator-grens vs alarm-grens
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: analyseren
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde17-lo-industry40-303
---

# Drempels instellen en alarm-rationalisatie — wanneer is een melding nog een melding?

Stel je voor: jij doet de ochtenddienst op een spuitgietmachine. Vóór de koffie zijn er al 30 alarmen voorbijgekomen op het scherm. Aan het einde van de dag staan er 240. Eerlijk gezegd: je leest ze niet meer allemaal. Niemand op jullie lijn doet dat. En dat is precies het probleem. Een alarm dat niemand meer leest, is geen alarm meer. Het is ruis. Dit heet alarm-vermoeidheid (overdaad aan meldingen). En de oplossing zit niet in betere operators — die zit in betere drempels.

## Wat leer je?

Je kunt na deze sessie het verschil benoemen tussen een operator-grens (drempel voor handeling) en een alarm-grens (drempel voor stilstand). Je kunt op basis van historische data een eerste drempel voorstellen en onderbouwen. En je kunt een alarm-stroom analyseren met drie principes uit de industrie-standaard EEMUA 191: max-rate, relevantie en actiegerichtheid.

## Twee soorten drempels — niet hetzelfde

Een digital twin (digitale tweeling) geeft een melding zodra een meetwaarde een drempel passeert. Maar er zijn TWEE soorten drempels. Verwarrend voor wie het voor het eerst tegenkomt — en oorzaak van veel onnodige alarmen.

**Operator-grens (drempel voor handeling).** De waarde waarbij jij iets MOET doen. De machine blijft draaien. Bijvoorbeeld: temperatuur 65 graden — controleer de koeling. Geen stilstand. Geen telefoon naar onderhoud.

**Alarm-grens (drempel voor stilstand).** De waarde waarbij iets doorbreekt. De machine stopt automatisch. Of er gaat een telefoon naar de leidinggevende. Bijvoorbeeld: temperatuur 80 graden — automatische stilstand en onderhoud bellen.

Hetzelfde sensorsignaal, twee verschillende drempels. Daar zit het ontwerp.

## Drempel-tuning — een trade-off

Welke waarde kies je voor operator-grens en alarm-grens? Daar zit altijd een trade-off tussen twee fouten.

**Te laag — vals alarm.** Drempel ligt onder normale werking. Constante meldingen. Operators raken afgestompt. Bij het echte signaal kijkt niemand meer.

**Te hoog — gemist signaal.** Drempel ligt boven probleem-gedrag. Issue's worden pas zichtbaar als ze al kostbaar zijn. Het voorspellend voordeel is weg.

## Goede aanpak — vier stappen

Een drempel ontwerp je niet op gevoel. De volgorde:

1. **Begin met historische data.** Wat is normaal bij deze machine over de afgelopen weken? Wat is afwijking?
2. **Zet de eerste drempel rond de bovengrens van normaal.** Net boven wat de meeste tijd voorkomt.
3. **Stel bij na 2 tot 4 weken.** Past de drempel of niet?
4. **Vraag operators om feedback.** Welke meldingen waren zinnig? Welke waren ruis?

Drempels die nooit worden bijgesteld, raken verouderd. De productie verandert — de drempels niet. Dat is bij elke werkvloer waar drempels al jaren hetzelfde staan, het verborgen probleem.

## Alarm-rationalisatie — drie principes uit EEMUA 191

Bij veel sensoren ontstaan zonder plan honderden alarmen per dag. Operators raken overspoeld. De industrie-standaard EEMUA 191 — al jaren de canonieke bron voor alarm-design — geeft drie principes om dit te voorkomen. Samen heet het alarm-rationalisatie (rationalisatie = logisch maken van een alarm-stroom).

**Principe 1 — Max-rate.** Maximaal ongeveer 10 alarmen per uur per operator. Meer is overload. De operator kan niet meer kiezen wat belangrijk is.

**Principe 2 — Relevantie.** Elk alarm moet relevant zijn voor DEZE operator op DIT moment. Een onderhouds-alarm tijdens de productie-shift? Dat hoort naar onderhoud, niet naar de operator.

**Principe 3 — Actiegerichtheid.** Elk alarm moet een concrete actie hebben. Niet "temperatuur 75 graden". Wel "temperatuur 75 graden — controleer koelsysteem klep 3". Een alarm zonder actie is een waarneming, geen alarm.

## Operator-feedback-loop — drempels leven

Drempels zijn niet vast. Goede teams houden bij welke alarmen vaak vals zijn. Ze bespreken het maandelijks. Ze passen aan op basis van werkvloer-ervaring. Wie de alarmen niet bijhoudt, krijgt na een jaar dezelfde situatie terug — 240 meldingen waar er 24 zinnig zouden zijn.

Dit is het human-in-the-loop principe uit een vorige sessie, toegepast op alarmen. AI of een digital twin kan een alarm-stroom voorstellen. Maar de operator op de werkvloer weet welke meldingen er echt toe doen. Die kennis MOET terug in het systeem.

## Een dag uit een autoleverancier — van 240 naar 24

Een autoleverancier heeft een spuitgietmachine met 8 sensoren. Eerste maand na installatie: 240 alarmen per dag. De operator merkt op dat 80 procent niet-actionabel is — temperatuur-piek bij opstart, lege materiaal-detectie tijdens shift-wissel. Niets om iets aan te doen, maar wel een melding.

Na alarm-rationalisatie volgens EEMUA:

- Opstartmeldingen verwijderd uit de alarm-stroom — verwacht gedrag, geen actie nodig (principe 3 hersteld).
- Materiaal-detectie verschoven naar shift-leiders — die kunnen er wel iets mee (principe 2 hersteld).
- Echte temperatuur-overschrijdingen kregen specifieker actie-advies — concrete handeling toegevoegd (principe 3 versterkt).

Resultaat: 24 alarmen per dag, allemaal actiegericht. Operator-tevredenheid steeg. En kritische alarmen werden gemiddeld 12 minuten sneller opgepakt — precies omdat de ruis weg was.

Geen wonder. Geen nieuwe sensoren. Gewoon rationalisatie van wat al binnenkwam.

## Na deze sessie

Doe deze week drie kleine stappen op je eigen lijn. Geen IT-kennis nodig.

1. **Tel de alarmen.** Hoeveel alarmen geeft jouw machine in een typische dienst? Schrijf het aantal op. Markeer hoeveel daarvan jij echt hebt opgevolgd en hoeveel je hebt genegeerd.
2. **Kies één alarm dat jij vaak negeert.** Vraag jezelf: schendt dit melding principe 1 (te veel), principe 2 (verkeerde ontvanger) of principe 3 (geen actie verbonden)? Schrijf het principe op.
3. **Stel één concrete vraag.** Aan je teamleider of IT. Bijvoorbeeld: "Waarom staat de temperatuur-drempel op 65 graden — is dat ooit aangepast aan deze lijn?" of "Wie beheert de alarm-instellingen op deze machine?"

Neem alle drie uitkomsten mee naar de volgende sessie.

Praat deze week ook één keer met een ervaren collega over alarmen die jullie als team negeren. Vraag: "Welk alarm is volgens jou compleet zinloos en waarom?" Vaak komen daar drie of vier meldingen uit die niemand mist. Dat is een nuttige inventaris voor een eerste rationalisatie-ronde.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-alarm-stroom.md`](./werkbladen/wb-01-alarm-stroom.md) — Alarm stroom
2. [`wb-02-reflecteren-duo.md`](./werkbladen/wb-02-reflecteren-duo.md) — Reflecteren duo
3. [`wb-03-theorie-handout.md`](./werkbladen/wb-03-theorie-handout.md) — Theorie handout
4. [`wb-04-experimenteren-eigen-lijn.md`](./werkbladen/wb-04-experimenteren-eigen-lijn.md) — Experimenteren eigen lijn

## Verder

- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
