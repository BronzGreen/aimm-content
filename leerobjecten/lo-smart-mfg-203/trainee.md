---
id: lo-smart-mfg-203-trainee
knowledge_object_id: ko-smart-mfg-203
version: trainee
title: 'Modelresultaten interpreteren: wat betekent een anomaliescore?'
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
correlation_id: ronde16-lo-smart-mfg-203
---

# Anomaliescores interpreteren

> **Leervraag:** Hoe bepaal je bij een anomaliescore of je moet negeren, monitoren of ingrijpen?

---

## Waarom is dit belangrijk?

In Module 1 heb je gezien wat predictive maintenance kan. Maar een dashboard met anomaliescores is alleen nuttig als jij weet wat je ermee moet doen. Een score van 65 — is dat erg? Moet je stoppen? Of mag je doordraaien? Jij bent degene die dat beslist. Met het juiste stappenplan maak je betere beslissingen en voorkom je onnodige stilstand of gemiste waarschuwingen.

---

## Deel 1: Scores beoordelen — ronde 1 (12 min)

Je krijgt zes anomaliescores van machines (0-100). Bij elke score staat welke sensoren actief zijn en wat er recent is gebeurd.

Jij beslist per score:
- **Negeren** — niets aan de hand
- **Monitoren** — extra in de gaten houden
- **Ingrijpen** — actie ondernemen

Schrijf bij elke keuze op **waarom** je dat kiest. Welke sensor gaf de doorslag? Wat zegt de context?

> **Tip:** Er is geen goed of fout in deze ronde. Het gaat om jouw inschatting op basis van je ervaring.

---

## Deel 2: Groepsbespreking (10 min)

Bespreek met de groep:
- Bij welke scores was het makkelijk?
- Bij welke scores twijfelde je?
- Hoe bepaalde je de grens tussen monitoren en ingrijpen?
- Keek je naar het getal, naar de sensoren, of naar allebei?

Luister naar hoe anderen het aanpakten. Was dat anders dan jij?

---

## Deel 3: Het verkeerslichtmodel (8 min)

Nu krijg je het model dat in de praktijk wordt gebruikt:

| Zone | Score | Wat doe je? |
|------|-------|-------------|
| **Groen** | 0-30 | Normaal — geen actie nodig |
| **Oranje** | 30-70 | Let op — uitzoeken en monitoren |
| **Rood** | 70-100 | Ingrijpen — inspectie of onderhoud plannen |

### Het 5-staps actieplan bij een hoge score

Als je een oranje of rode score ziet, doorloop je deze vijf stappen:

1. **Kijk welke sensor** de hoogste bijdrage levert
2. **Check of er een logische verklaring is** (productwissel, onderhoud, seizoen)
3. **Vergelijk met eerdere situaties** — is dit normaal voor deze machine?
4. **Beslis:** monitoren of ingrijpen
5. **Documenteer** je beslissing en het resultaat

> **Let op:** Soms is een score misleidend. Na onderhoud kan de score tijdelijk hoger zijn. Bij een productwissel veranderen de sensorwaarden. Het 5-staps plan helpt je om niet overhaast te reageren.

---

## Deel 4: Scores beoordelen — ronde 2 (15 min)

Beoordeel dezelfde zes anomaliescores opnieuw. Gebruik nu het verkeerslichtmodel en het 5-staps actieplan.

Vergelijk ronde 1 met ronde 2:
- Bij welke score veranderde je beslissing?
- Waarom?
- Werd je beoordeling beter of juist niet?

Bespreek met je buurman welke scores je anders beoordeelt en waarom.

---

## Samenvatting

| Wat je geleerd hebt | Hoe je het toepast |
|--------------------|--------------------|
| Verkeerslichtmodel (groen/oranje/rood) | Bij elke anomaliescore de zone bepalen |
| 5-staps actieplan | Bij oranje en rode scores systematisch doorlopen |
| Context meewegen | Productwissel, onderhoud en seizoen herkennen als verklaring |

---

## Transferopdracht

Doe dit deze week op je eigen werkvloer:

1. Kijk minimaal **drie keer** naar het anomalie-dashboard
2. Pas het verkeerslichtmodel toe: is de score groen, oranje of rood?
3. Volg bij oranje of rood het 5-staps actieplan
4. Schrijf op wat je zag, wat je deed, en wat het resultaat was
5. Neem dit mee naar de volgende bijeenkomst

> **Doe ook:** Vraag een collega om dezelfde score te beoordelen en vergelijk jullie aanpak.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-anomaliescores-ronde1.md`](./werkbladen/wb-anomaliescores-ronde1.md) — Ronde1
2. [`wb-anomaliescores-ronde2.md`](./werkbladen/wb-anomaliescores-ronde2.md) — Ronde2
3. [`wb-handout-verkeerslichtmodel.md`](./werkbladen/wb-handout-verkeerslichtmodel.md) — Verkeerslichtmodel
4. [`wb-reflectie-groepsdiscussie.md`](./werkbladen/wb-reflectie-groepsdiscussie.md) — Groepsdiscussie

## Verder

- Onderliggend kennisobject: [`ko-smart-mfg-203`](../../kennisbank/smart_manufacturing/predictive_maintenance/ko-smart-mfg-203.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
- Interactief: [`interactive/model.html`](./interactive/model.html)
