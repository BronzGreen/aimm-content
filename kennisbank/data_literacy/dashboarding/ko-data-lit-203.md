---
id: ko-data-lit-203
title: 'Je eigen dashboard configureren: KPI''s kiezen en instellen'
type: framework
domain: data_literacy
subdomain: dashboarding
summary: 'Een dashboard configureren begint met de vraag: wat wil ik weten? Kies de
  KPI''s die passen bij jouw doel, stel drempelwaarden in, en bepaal hoe vaak je kijkt.'
source_centrality: 0.7
source_ref: AIMM Competentieframework Data Literacy, competentie dashboarding.train
status: validated
updated_at: '2026-05-19'
correlation_id: ronde10-lo-data-lit-203
---

# Je eigen dashboard configureren: KPI's kiezen en instellen

Een dashboard configureren begint met de vraag: wat wil ik weten? Kies de KPI's die passen bij jouw doel, stel drempelwaarden in, en bepaal hoe vaak je kijkt.

In Module 1 heb je geleerd een dashboard te LEZEN. Nu leer je een dashboard te CONFIGUREREN: welke KPI's kies je, en wanneer is een waarde goed of slecht?

### Stap 1: Wat wil je weten?

Voordat je een dashboard instelt, stel je jezelf een vraag:
- **Wil je weten of de productie op schema ligt?** --> Productieaantal, OEE
- **Wil je weten of de kwaliteit goed is?** --> Afkeurpercentage, foutcodes
- **Wil je weten of de machine goed draait?** --> Stilstandtijd, temperatuur
- **Wil je weten of je team op tijd levert?** --> Doorlooptijd, leverbetrouwbaarheid

Kies maximaal 4-6 KPI's. Meer is verwarrend.

### Stap 2: KPI's selecteren

Een goede KPI voldoet aan drie voorwaarden:
1. **Meetbaar** -- je kunt er een getal aan hangen
2. **Beinvloedbaar** -- je kunt er iets aan veranderen
3. **Relevant** -- het zegt iets over jouw doel

Voorbeeld:
- Luchtvochtigheid buiten: meetbaar, maar NIET beinvloedbaar. Geen goede KPI.
- Aantal ongeplande stops: meetbaar, beinvloedbaar, relevant. Goede KPI.

### Stap 3: Drempelwaarden instellen

Bij elke KPI hoort een drempel: wanneer is het goed, wanneer niet?

| KPI | Groen (goed) | Oranje (let op) | Rood (actie nodig) |
|-----|-------------|----------------|-------------------|
| OEE | > 85% | 70-85% | < 70% |
| Stilstand | < 30 min | 30-60 min | > 60 min |
| Afkeur | < 1,5% | 1,5-2,5% | > 2,5% |
| Doorlooptijd | < 3 uur | 3-4 uur | > 4 uur |

Drempelwaarden zijn niet universeel. Ze hangen af van jouw productieproces, jullie doelstellingen, en wat realistisch is.

### Stap 4: Hoe vaak kijk je?

- **Realtime** -- voor kritieke processen (temperatuur, druk)
- **Per dienst** -- voor productie-KPI's (OEE, aantallen)
- **Per dag** -- voor kwaliteits-KPI's (afkeurpercentage)
- **Per week** -- voor trends (doorlooptijd, leverbetrouwbaarheid)

### De valkuil: te veel KPI's

Als alles belangrijk is, is niets belangrijk. Een goed dashboard past op een scherm. Als je moet scrollen, heb je te veel KPI's.


## Praktijkvoorbeeld

Een operator op een spuitgietlijn wil weten of zijn machine goed draait. Hij kiest drie KPI's:
1. **Cyclustijd** -- doel: 45 seconden. Groen: 42-48 sec. Rood: > 52 sec.
2. **Afkeurpercentage** -- doel: < 1%. Groen: < 1%. Oranje: 1-2%. Rood: > 2%.
3. **Materiaaltemperatuur** -- doel: 210 graden. Groen: 205-215. Rood: < 200 of > 220.

Hij checkt de cyclustijd per shot (realtime), het afkeurpercentage per dienst, en de temperatuur continu. Drie KPI's, drie drempels, drie ritmes. Overzichtelijk.
