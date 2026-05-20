---
id: lo-smart-mfg-204-trainee
knowledge_object_id: ko-smart-mfg-204
version: trainee
title: 'Je eerste predictief model configureren: een stapsgewijze handleiding'
target_audience: operator
content_level: MBO-3
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: experimenteren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde17-lo-smart-mfg-204
---

# Je eerste model configureren in 5 stappen

> **Leervraag:** Hoe configureer je zelf een eenvoudig predictief model met de 5-stappen handleiding?

---

## Waarom is dit belangrijk?

In Module 1 heb je gezien wat predictive maintenance kan. Nu ga je het zelf doen. Dit is de stap van "snappen" naar "kunnen". Als je een model kunt configureren met voorbeelddata, kun je het straks ook met je eigen machine. En dan voorkom je stilstand in plaats van dat je erop reageert.

---

## Deel 1: Zelf configureren (15 min)

Je krijgt een dataset van een verpakkingsmachine: 100 cycli sensordata met drie sensoren (temperatuur sealbalken, trillingen aandrijfmotor, druk pneumatiek).

Gebruik de 5-stappen handleiding als naslagkaart en doorloop alle stappen:

### De 5 stappen

1. **Kies de machine** — In dit geval de verpakkingsmachine. Kijk naar de storingshistorie.
2. **Selecteer sensoren** — Kies minimaal 2 van de 3 sensoren. Welke sensoren vertellen het meest over de gezondheid van de machine?
3. **Bekijk de normaaldata** — Wat is normaal voor deze machine? Wat is het gemiddelde? Wat is de spreiding?
4. **Stel drempelwaarden in** — Wanneer moet het systeem waarschuwen? Wanneer alarm slaan?
5. **Draai een eerste test** — Test je instellingen met de testdata. Hoeveel valse alarmen krijg je? Mis je iets?

Vul alles in op het configuratie-werkblad.

> **Tip:** Er is geen perfect antwoord. Het gaat erom dat je het proces doorloopt en begrijpt wat elke stap doet.

---

## Deel 2: Vergelijk met je buurman (10 min)

Leg je configuratie-werkblad naast dat van je buurman. Bespreek:

- Welke sensoren kozen jullie? Dezelfde of andere?
- Welke drempels stelden jullie in? Waarom die waarden?
- Hoeveel valse alarmen kreeg je bij de test?
- Wat zou je anders doen als je opnieuw begon?

Vul het reflectie-werkblad samen in.

---

## Deel 3: Drie vuistregels (5 min)

Na de vergelijking krijg je drie vuistregels voor het instellen van drempels:

| Vuistregel | Wat het betekent |
|-----------|-----------------|
| **Te strak = te veel valse alarmen** | Als je drempels te scherp staan, slaat het systeem steeds alarm terwijl er niets aan de hand is. Mensen gaan de alarmen negeren. |
| **Te los = je mist echte problemen** | Als je drempels te ruim staan, merk je een storing pas als het te laat is. |
| **Bijstellen is normaal** | Twee tot drie rondes bijstellen is standaard. Geen enkel model is de eerste keer perfect. |

> **Vraag jezelf af:** Welke vuistregel is het meest relevant voor jouw configuratie?

---

## Deel 4: Bijstellen en opnieuw testen (15 min)

Pas je drempelwaarden aan op basis van:
- De feedback van je buurman
- De drie vuistregels
- Je eigen testresultaten uit ronde 1

Draai een tweede test. Vergelijk:
- Hoeveel valse alarmen nu? Minder dan ronde 1?
- Mis je nog steeds een echte afwijking?

Vul het bijstel-werkblad in met je oude en nieuwe waarden.

---

## Samenvatting

| Ronde 1 | Ronde 2 |
|---------|---------|
| Eerste poging, eigen inschatting | Bijgesteld op basis van ervaring en vuistregels |
| Meer valse alarmen (vaak) | Minder valse alarmen |
| Leren door te doen | Leren door bij te stellen |

**De les:** bijstellen is het proces, niet het falen. Elk model wordt beter door te testen en aan te passen.

---

## Transferopdracht

Doe dit deze week:

1. Kies een machine op je eigen werkvloer waarvoor je een predictief model zou willen opzetten
2. Schrijf de eerste twee stappen uit: welke machine en waarom? Welke sensoren zou je gebruiken?
3. Neem dit mee naar Module 3

> **Doe ook:** Vraag de technische dienst om de storingshistorie van jouw gekozen machine op te vragen. Die heb je nodig in Module 3.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-bijstellen-ronde2.md`](./werkbladen/wb-bijstellen-ronde2.md) — Ronde2
2. [`wb-configuratie-model.md`](./werkbladen/wb-configuratie-model.md) — Model
3. [`wb-handout-vuistregels.md`](./werkbladen/wb-handout-vuistregels.md) — Vuistregels
4. [`wb-reflectie-duo.md`](./werkbladen/wb-reflectie-duo.md) — Duo

## Verder

- Onderliggend kennisobject: [`ko-smart-mfg-204`](../../kennisbank/smart_manufacturing/predictive_maintenance/ko-smart-mfg-204.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
- Interactief: [`interactive/model.html`](./interactive/model.html)
