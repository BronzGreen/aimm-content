# Draaiboek: Trainingsdata labelen en een model configureren

**Leerobject:** lo-smart-mfg-511
**Kennisobjecten:** ko-smart-mfg-511, ko-smart-mfg-512
**Doelgroep:** MBO-3 operators (Module 1 afgerond)
**Totale duur:** 50 minuten
**Groepsgrootte:** 6-12 deelnemers
**Format:** Interactieve workshop (Kolb-cyclus, 4 fasen, coachend)

---

## Voorbereiding (30 min voor aanvang)

### Materialen klaarzetten

| Materiaal | Aantal | Locatie |
|---|---|---|
| 20 productfoto's (A4, kleur) of op scherm | 1 set + beamer | Scherm of tafel |
| Werkblad labelen | 1 per deelnemer | Op de stoelen |
| Werkblad reflectie-labelen | 1 per deelnemer | Op de stoelen |
| Handout best practices trainingsdata | 1 per deelnemer | Apart stapeltje (pas uitdelen bij fase 3) |
| Werkblad model-configuratie | 1 per duo | Apart stapeltje (pas uitdelen bij fase 4) |
| Whiteboard + stiften | 1 | Vooraan |
| Pennen | 1 per deelnemer | Op de stoelen |

### Foto's voorbereiden

**BELANGRIJK:** Module 2 is anders dan Module 1. Daar ging het om beoordelen (goed/defect). Hier gaat het om **labelen** — classificeren met het doel een model te trainen. De foto's moeten daarom meer ambigu zijn dan in Module 1.

**Samenstelling 20 foto's:**
- 8 duidelijk goede producten (waarvan 2 met onschuldige variatie die tot discussie leidt)
- 8 duidelijk defecte producten (mix van krassen, deuken, kleurafwijkingen)
- 4 grensgevallen (is die kleine kras een defect of normale slijtage? Is die kleurvariatie een probleem?)

De grensgevallen zijn cruciaal: ze zorgen voor meningsverschillen in de reflectiefase. Dat is precies de leervaring.

### Verschil met Module 1

| Module 1 (Gebruik) | Module 2 (Train) |
|---|---|
| Trainer doet voor (worked examples) | Operator doet zelf (geen voorbeelden) |
| Begeleidingsstijl: trainen | Begeleidingsstijl: coachen |
| Competentiestadium: bewust onbekwaam | Competentiestadium: bewust bekwaam |
| 10 foto's, driedelige scaffolding | 20 foto's, direct zelfstandig |
| Focus: herkennen | Focus: labelen voor AI-training |

---

## Sessie-opbouw

### Fase 1: EXPERIMENTEREN — Foto's labelen (15 min)

**0:00-0:02 | Korte instructie (2 min)**

Zeg iets als:

> "In Module 1 hebben jullie foto's beoordeeld en vergeleken met een AI. Vandaag draaien we het om: jullie gaan het AI-model trainen. Stap 1: foto's labelen. Dit is precies wat er in de fabriek ook gebeurt als een bedrijf AI-inspectie wil gaan gebruiken."

Deel de werkbladen labelen uit. Geef de instructie:

> "20 foto's. Per foto: goed of defect? Als defect: welk type? En hoe zeker ben je? Werk zelfstandig."

**0:02-0:15 | Zelfstandig labelen (13 min)**

Toon de foto's op het scherm (30-40 seconden per foto). De deelnemers vullen hun werkblad in.

**COACHEND, NIET INSTRUEREND:** Loop rond. Kijk mee. Stel vragen als iemand vastloopt:
- "Wat zie je op deze foto?"
- "Hoe zeker ben je?"
- "Zou je collega hetzelfde zeggen?"

Geef GEEN antwoorden. Geef GEEN hints. Het verschil met Module 1 is cruciaal: daar deed je voor, hier laat je los.

**Noteer** wie inconsistent labelt (bijv. dezelfde kras de ene keer wel, de andere keer niet als defect). Je gebruikt deze observatie in fase 2.

**VALKUIL:** De verleiding is groot om te helpen. De grensgevallen zijn bewust ambigu. De meningsverschillen zijn de leervaring.

---

### Fase 2: REFLECTEREN — Labels vergelijken (10 min)

**0:15-0:20 | Duo-vergelijking (5 min)**

Zeg:

> "Vergelijk nu je labels met je buurman. Bij welke foto's waren jullie het oneens?"

Laat duo's 5 minuten vergelijken. Loop langs. Luister.

**0:20-0:25 | Plenaire terugkoppeling (5 min)**

Vraag 2-3 duo's om hun meest interessante meningsverschil te delen. Schrijf op het whiteboard:

> **"Dezelfde foto. Twee verschillende labels. Wat betekent dat voor een AI-model?"**

Leid het gesprek naar de kern. Stel de vraag:

> "Als jullie het niet eens zijn over wat een defect is — hoe kan een AI het dan goed doen?"

**BELANGRIJK:** Maak het niet competitief. Er is geen goed of fout. Het gaat om bewustwording dat consistente labels essentieel zijn.

---

### Fase 3: THEORETISEREN — Best practices (10 min)

**0:25-0:30 | Presentatie (5 min)**

Verwijs terug naar het whiteboard:

> "Jullie ontdekten net het grootste probleem bij AI-training: inconsistente labels."

Loop de drie stappen door:
1. Consistente foto's (licht, achtergrond, hoek)
2. Correcte en consistente labels (criteria afspreken)
3. Verdeling trainingsset (80%) en testset (20%)

Gebruik de analogie:

> "Stel je voor dat je een toets maakt en je hebt de antwoorden al gezien. Dat is geen eerlijke test. Zo werkt het ook met een AI-model en de testset."

**0:30-0:35 | Handout (5 min)**

Deel de handout uit. Laat deelnemers 2 minuten lezen. Stel:

> "Welke best practice had je geholpen bij het labelen van de 20 foto's?"

Laat 2-3 deelnemers reageren.

**VALKUIL:** Maak de theorie niet te lang. Maximaal 10 minuten. De operators hebben de kernboodschap al ervaren in fase 1-2.

---

### Fase 4: EXPERIMENTEREN — Model configureren (15 min)

**0:35-0:40 | Instructie + werkblad (5 min)**

Deel het configuratie-werkblad uit. Leg uit:

> "Nu gaan jullie een model configureren. Jullie krijgen de resultaten van een model bij drie drempelwaarden: streng (0.3), gebalanceerd (0.5), en soepel (0.7). Per drempel zie je hoeveel defecten het model vindt en hoeveel valse alarmen. Jullie kiezen de beste drempel."

Leg kort uit wat de drempelwaarde doet:

> "De drempel bepaalt hoe streng het model is. Laag = streng, alles is verdacht. Hoog = soepel, alleen duidelijke defecten."

**0:40-0:47 | Duo-opdracht (7 min)**

Duo's werken samen aan het werkblad. Loop langs. Stel coachende vragen:
- "Waarom kozen jullie deze drempel?"
- "Wat gebeurt er als jullie strenger worden?"
- "Wat als jullie product een veiligheidsonderdeel is?"

**0:47-0:50 | Presentatie (3 min)**

Laat 2 duo's hun keuze presenteren (1 min per duo). Bespreek het verschil:

> "Duo A koos 0.3 — streng. Duo B koos 0.5 — gebalanceerd. Allebei goed! Het hangt af van je product en je risico."

**Transferopdracht:**

> "Label de 10 foto's die je in Module 1 hebt gemaakt. Maak 10 extra foto's. Let op consistent licht. Neem je gelabelde set mee naar de volgende bijeenkomst."

---

## Differentiatie

### Snelle deelnemers

- Laat ze bij fase 1 al na 12 foto's de rest overslaan en beginnen met het vergelijken
- Geef een bonusopdracht: "Bedenk labelcriteria voor 3 defecttypes op je eigen werkvloer"
- Zet ze als sparringpartner bij een duo dat moeite heeft in fase 4

### Deelnemers die moeite hebben

- Geef bij fase 1 de tip: "Begin met de makkelijke foto's en doe de lastige aan het einde"
- Koppel ze bij de reflectie aan een sterkere deelnemer
- Bij fase 4: help ze de tabellen te lezen ("hier staat hoeveel defecten het model vond")
- Bied aan het werkblad na de sessie samen door te nemen

### Deelnemers die al ervaring hebben met data/labelen

- Vraag ze hun ervaring te delen in de reflectiefase
- Geef ze de rol van kwaliteitscontroleur: "Controleer steekproefsgewijs de labels van 3 andere deelnemers"
- Laat ze nadenken over edge cases: "Welk type defect zou het moeilijkst zijn om te labelen?"

---

## Veelgemaakte fouten

| Fout | Gevolg | Oplossing |
|---|---|---|
| Toch voorbeelden geven (Module 1-reflex) | Operator leert niet zelfstandig labelen | Bewust coachen: vragen stellen, niet voordoen |
| Foto's te makkelijk (geen grensgevallen) | Geen meningsverschillen in reflectie | Minimaal 4 ambigue foto's opnemen |
| Foto's te moeilijk (alleen grensgevallen) | Frustratie, geen succeservaring | Mix: 16 duidelijk + 4 ambigu |
| Drempelwaarde-concept te technisch uitleggen | Afhakers | Gebruik termen als "streng" en "soepel", niet "threshold" |
| Theorie te uitgebreid | Geen tijd voor configuratie-opdracht | Max 10 min theorie, verwijs naar handout |
| Antwoorden geven bij labelen | Geen eigen leervaring | Alleen coachende vragen stellen |

---

## Didactische verantwoording

| Principe | Hoe toegepast |
|---|---|
| **Coachend** (Hersey & Blanchard) | Bewust bekwaam = weinig sturing, veel ondersteuning. Vragen stellen i.p.v. voordoen. |
| **Productieve fout** (Kapur) | De grensgevallen zijn bewust ambigu. De meningsverschillen bij labelen zijn de leervaring. |
| **Kolb — experimenteren eerst** | Operator doet direct zelf, reflecteert op meningsverschillen, krijgt dan theorie. |
| **CAR-model** (Deci & Ryan) | Competentie: bouwt op Module 1. Autonomie: eigen keuzes. Relatie: duo-vergelijking. |
| **Transfer** | De gelabelde foto's van de eigen werkvloer zijn de brug naar Module 3. |
| **Scaffolding afgebouwd** | Module 1: Ik doe/Wij doen/Jij doet. Module 2: Jij doet/Wij bespreken. |

---

## Na de sessie

- [ ] Werkbladen labelen innemen (voor learning analytics)
- [ ] Noteer observaties: wie labelde inconsistent? Wie was verrast door de meningsverschillen?
- [ ] Check: heeft iedereen de transferopdracht begrepen (20 gelabelde foto's meenemen)?
- [ ] Bereid de confusion matrix voor de tweede activiteit voor (LO-513)

---

*AIMM Pipeline | lo-smart-mfg-511 | Draaiboek trainer-versie*
*Didactische bronnen: Kapur (2016), Hersey & Blanchard (1977), Kolb (1984), Deci & Ryan (2000)*
