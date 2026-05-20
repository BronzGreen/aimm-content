# Handout 3 — Twee drempels, drempel-tuning en drie principes
*Drempels instellen en alarm-rationalisatie — Kolb fase 3: Theoretiseren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | Leerobject lo-industry40-303**

---

> **Over deze handout**
> Dit is een referentievel. Geen invulopdracht — wel lezen en markeren wat je belangrijk vindt. In werkblad 4 ga je deze regels toepassen op een eigen werkvloer-case. Houd deze handout bij je. Tijd: 10 minuten meelezen terwijl de trainer uitlegt.

---

## Deel 1 — Twee soorten drempels

Een digital twin (digitale tweeling) geeft een melding zodra een meetwaarde een drempel passeert. Maar er zijn TWEE soorten drempels. Verwarring tussen die twee is de bron van veel onnodige alarmen.

| Soort drempel | Wat betekent het? | Voorbeeld | Gevolg |
|---------------|--------------------|-----------|--------|
| **Operator-grens** *(drempel voor handeling)* | De waarde waarbij jij iets MOET doen. Machine blijft draaien. | Temperatuur 65 °C — controleer koeling | Logboek, controle, geen stilstand |
| **Alarm-grens** *(drempel voor stilstand)* | De waarde waarbij iets doorbreekt. Machine stopt of bel een leidinggevende. | Temperatuur 80 °C — automatische stilstand | Productie stopt, onderhoud erbij |

**Hetzelfde sensorsignaal, twee verschillende drempels.** Bij de tien meldingen van werkblad 1: melding 2 (65 °C) was operator-grens. Melding 4 (80 °C) was alarm-grens. Wie anders koos: dat was geen fout. Het verschil leren zien is precies wat deze sessie doet.

---

## Deel 2 — Drempel-tuning: een trade-off

Welke waarde kies je voor operator-grens en alarm-grens? Daar zit altijd een trade-off tussen twee fouten.

**Te laag — vals alarm.** Drempel ligt onder normale werking. Constante meldingen. Operators raken afgestompt. Bij het echte signaal kijkt niemand meer.

**Te hoog — gemist signaal.** Drempel ligt boven probleem-gedrag. Issue's worden pas zichtbaar als ze al kostbaar zijn. Het voorspellend voordeel is weg.

```
Meetwaarde
     ^
     |        ─── alarm-grens (stilstand) ───        te hoog: gemist signaal
     |
     |   .  ..  .   normaal gedrag  ..   .
     |  .   .   .   .   .   .   .   .  .
     |        ─── operator-grens (handeling) ─       te laag: vals alarm
     |________________________________________> tijd
```

**Goede aanpak — in vier stappen:**

1. **Begin met historische data.** Wat is normaal bij DEZE machine over de afgelopen weken? Wat is afwijking?
2. **Zet de eerste drempel rond de bovengrens van normaal.** Net boven wat de meeste tijd voorkomt.
3. **Stel bij na 2 tot 4 weken.** Past de drempel of niet? Past het bij seizoen, leverancier, operator?
4. **Vraag operators om feedback.** Welke meldingen waren zinnig? Welke waren ruis? Die kennis MOET terug in het systeem.

---

## Deel 3 — Drie principes uit EEMUA 191

Bij veel sensoren ontstaan zonder plan honderden alarmen per dag. Operators raken overspoeld. De industrie-standaard EEMUA 191 — al jaren de canonieke bron voor alarm-design — geeft drie principes om dit te voorkomen. Samen heet het **alarm-rationalisatie** (rationalisatie = logisch maken van een alarm-stroom).

| Principe | Wat betekent het? | Voorbeeld van schending |
|----------|-------------------|-------------------------|
| **1. Max-rate** | Maximaal ongeveer 10 alarmen per uur per operator. Meer is overload. | 240 alarmen in 24 uur = 10 per uur — net aan de grens, met pieken erboven |
| **2. Relevantie** | Elk alarm relevant voor DEZE operator op DIT moment. | Onderhouds-alarm tijdens productie-shift — hoort bij onderhoud, niet bij operator |
| **3. Actiegerichtheid** | Elk alarm heeft een concrete actie. | "Temperatuur 75 °C" — geen actie genoemd. Beter: "Temperatuur 75 °C — controleer koelsysteem klep 3" |

**Een alarm zonder actie is een waarneming, geen alarm.**

---

## Deel 4 — De autoleverancier: 240 naar 24

Een autoleverancier heeft een spuitgietmachine met 8 sensoren. Eerste maand na installatie: 240 alarmen per dag. De operator merkt op dat 80 procent niet-actionabel is — temperatuur-piek bij opstart, lege materiaal-detectie tijdens shift-wissel. Niets om iets aan te doen, maar wel een melding.

Na alarm-rationalisatie volgens EEMUA:

| Wat ze deden | Welk principe hersteld? |
|--------------|-------------------------|
| Opstartmeldingen verwijderd uit de alarm-stroom (verwacht gedrag, geen actie nodig) | Principe 3 — actiegerichtheid |
| Materiaal-detectie verschoven naar shift-leiders (zij kunnen er iets mee, operator niet tijdens shift) | Principe 2 — relevantie |
| Temperatuur-overschrijdingen kregen specifieker actie-advies ("controleer koelsysteem klep 3") | Principe 3 — actiegerichtheid |

**Resultaat: 24 alarmen per dag, allemaal actiegericht.** Operator-tevredenheid steeg. Kritische alarmen werden gemiddeld 12 minuten sneller opgepakt — precies omdat de ruis weg was.

Geen wonder. Geen nieuwe sensoren. Gewoon rationalisatie van wat al binnenkwam.

---

## Deel 5 — Drempels leven met de productie mee

Drempels zijn niet vast. Goede teams houden bij welke alarmen vaak vals zijn. Ze bespreken het maandelijks. Drie momenten waarop je drempels altijd opnieuw bekijkt:

- **Seizoenswisseling** — bijvoorbeeld een hete zomer met een 5 °C warmere werkruimte
- **Nieuwe materiaalleverancier** — andere stroom-eigenschappen, andere normale waarden
- **Nieuwe operator** — andere ervaring, mogelijk andere instellingen nodig

Wie drempels nooit bijstelt, krijgt na een jaar dezelfde situatie terug — 240 meldingen waar er 24 zinnig zouden zijn.

---

## Deel 6 — Korte begrippenlijst

- **Drempel** — een waarde waarboven een sensor een melding geeft
- **Operator-grens** — drempel voor handeling, machine draait door
- **Alarm-grens** — drempel voor stilstand of escalatie
- **Drempel-tuning** — afstellen van een drempel op basis van data en ervaring
- **Alarm-rationalisatie** — logisch maken van een alarm-stroom volgens vaste principes
- **Alarm-vermoeidheid** — afstomping door overdaad aan meldingen
- **EEMUA 191** — industrie-standaard voor alarm-systemen
- **Operator-feedback-loop** — proces waarin operator-ervaring terugvloeit naar drempel-instellingen

---

> **Wat gebeurt er hierna?**
> Werkblad 4 is jouw eigen werkvloer. Je kiest één sensor of component van jouw lijn. Je past de twee drempels en de drie principes toe. Geen IT-kennis nodig — wel gezond verstand en jouw werkvloer-ervaring.

---
*Bron: EEMUA Publication 191 — Alarm Systems: A Guide to Design, Management and Procurement (industrie-standaard, niet 1-op-1 gereproduceerd); Bakopoulos et al. (2024) Digital-Twin-Enabled Framework, Ch. 7 | AIMM — Module 2 Train | v1.0*
