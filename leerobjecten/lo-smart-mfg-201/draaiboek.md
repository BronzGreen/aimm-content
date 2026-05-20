# Sensordata lezen: temperatuur, druk en trillingen — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 40 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan sensordata lezen, een basislijn bepalen, trends herkennen en pieken van ruis onderscheiden — bij minimaal 3 van 4 scenario's correct het type afwijking benoemen en de juiste actie kiezen. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 (Gebruik) afgerond — kent de begrippen sensor, basislijn, trend, piek |
| **Stadium (H&B)** | Bewust bekwaam — heeft basiservaring, wil het nu zelf kunnen |
| **Begeleidingsstijl** | Coachen — observeren, vragen stellen, niet voorzeggen |
| **Ruimte** | U-opstelling of clusters van 4. Echte machine OF simulator op laptops. Beamer + scherm. Flap-over. |
| **Plek in module** | Workshop-blok 1 — opstap voor LO-202 (drempelwaarden) en LO-205 (onderhoudsbeslissingen) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Sensordata oefenen — basislijn bepalen | experimenteren | 15 min |
| 00:15 - 00:25 | Storingsquiz: 4 scenario's — type afwijking | ervaren | 10 min |
| 00:25 - 00:35 | Duo-reflectie: wat ging goed, wat lastig? | reflecteren | 10 min |
| 00:35 - 00:40 | Theorie: 3 stappen + transferopdracht | theoretiseren | 5 min |

**Totaal:** 40 minuten — geen aparte pauze (workshop-blok binnen module 2).
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Test of de echte machine beschikbaar is met aflezing van temperatuur/druk/trillingen. Zo niet: open `model-lo-smart-mfg-201.html` op de laptops.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bedenk welk machinetype de groep het meest gebruikt (CNC-frees, spuitgiet, draaibank) — kies dat als hoofdvoorbeeld.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over zichtbaar op met de tekst: **"Wat is normaal voor JOUW machine?"**
- [ ] Schrijf op een tweede flap-over alvast de drie stappen-kapstok: **basislijn → trend → piek vs ruis**.
- [ ] Test de simulator (of zet de echte machine in basisstand).
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Sensordata oefenen — basislijn bepalen
**00:00 - 00:15** | 15 min | Kolb-fase: experimenteren

**Doel:** Deelnemer meet zelf sensorwaarden, berekent een basislijn, beoordeelt 6 waarden als normaal, trend of piek.

**Werkvorm:** Duo-oefening aan de machine OF met de simulator op laptops — werkblad wb-01-experimenteren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 40 minuten leer je sensordata lezen op JOUW machine. Niet op een gemiddelde fabriek-machine. Op de jouwe."*

2. **Trigger** (1 min) — vraag: *"Wie heeft wel eens een storing gehad die niemand zag aankomen?"* Vang 1-2 reacties. Reageer met *"herkenbaar"*. Geen oordeel.

3. **Werkblad uitdelen + opdracht** (1 min) — deel wb-01 uit. Toon slide 2. Zeg: *"In duo's. Een meet, de ander schrijft. Halverwege wisselen. Doe 6 metingen. Bereken jullie basislijn. En beoordeel daarna 6 voorbeeldwaarden: normaal, trend, of piek?"*

4. **Duo's vormen + start** (30 sec) — *"Zoek een buurman. Pak een machine of laptop met simulator. Begin met meting 1."*

5. **Werken** (10 min) — zet timer op 10 min. Loop rond. Coach-modus: niet voorzeggen. Stel verdiepende vragen:
    - *"Wat zou je verwachten als basislijn?"*
    - *"Hoe weet je of een afwijking groot of klein is?"*
    - *"Hoe lang zou je moeten meten om zeker te weten dat dit normaal is?"*

6. **Verzamelmoment** (1 min 30) — toon slide 3. Vraag plenair: *"Wat was jullie basislijn? Iemand een verrassing tegengekomen?"* Vang 2-3 reacties. Schrijf 2-3 getallen op de flap-over. Zeg: *"Zelfde machinetype, andere getallen. Dat IS het inzicht: jouw machine heeft eigen normaalwaarden."*

**Materiaal:**
- [ ] wb-01-experimenteren.md (per deelnemer)
- [ ] Pen + markeerstift per deelnemer
- [ ] Slides 1-3
- [ ] Echte machine OF model-lo-smart-mfg-201.html (per duo)
- [ ] Flap-over voor basislijn-getallen
- [ ] Timer

> **Tips voor de trainer:**
> - Coach. Niet voorzeggen. De waarde van fase 1 is dat operators ZELF ontdekken dat hun basislijn afwijkt.
> - Bij snelle duo's: vraag *"Welke variabele zou jij OOK willen meten die niet in de sensoren zit?"* (geluid, geur, gevoel).
> - Bij vastlopen: *"Wat zou je doen als je dit getal op je werk zag?"*

> **Differentiatie:**
> - **MBO-3 basis:** geef 1 sensortype tegelijk (eerst temperatuur, daarna druk, daarna trilling). Niet alles tegelijk.
> - **MBO-4 sneller:** vraag *"Hoe zou je de spreiding berekenen, niet alleen het gemiddelde?"* = bruggetje naar LO-202.

> **Valkuil — leverancier-syndroom ('die getallen staan toch al ingesteld?'):**
> Erken eerst. Dan: *"Klopt, fabriek heeft een standaard. Maar jouw machine, jouw productie, jouw omgeving wijken af. Vandaag meten we de echte."*

> **Valkuil — sensordata als absolute waarheid:**
> Bij 'sensor zegt 73 graden': *"En wat zegt je oor? Je hand boven de behuizing? Sensor + zintuig samen geeft het volledige beeld."*

---

### Blok 2: Storingsquiz — 4 scenario's
**00:15 - 00:25** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer past kennis uit fase 1 toe op 4 realistische scenario's en kiest per scenario het juiste type afwijking en de bijbehorende actie.

**Werkvorm:** Individuele quiz — werkblad wb-02-ervaren.

**Instructie:**

1. **Werkblad uitdelen + introduceren** (1 min) — deel wb-02 uit. Toon slide 4. Zeg: *"Vier scenario's met sensordata. Per scenario: wat zie je — basislijn, trend, piek of ruis? En wat doe je?"*

2. **Werken** (7 min) — zet timer op 7 min. Loop rond. Geef GEEN antwoorden. Stel vragen:
    - *"Waar kijk je naar — gemiddelde of de laatste meting?"*
    - *"Hoe lang zie je dit al?"*
    - *"Drie keer of vaker = signaal — geldt dat hier?"*

3. **Verzamelmoment** (1 min 30) — *"Pen neer. Tel je correcte antwoorden. Schrijf op werkblad: aantal goed."* Niet plenair bespreken — dat doen we in fase 3.

4. **Anker** (30 sec) — toon slide 5. Zeg: *"Iedereen heeft fouten gemaakt. Dat is goed. Daar leren we van in de duo-bespreking."*

**Materiaal:**
- [ ] wb-02-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 4-5
- [ ] Timer

> **Tips voor de trainer:**
> - Niet plenair de antwoorden geven na de quiz. Dat verpest de duo-leerwinst in fase 3.
> - Bij faalangst: *"Niemand heeft 4 op 4 — dit is oefenen, niet toetsen."*
> - Loop rustig. Stilte is je vriend.

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt op scenario 3-4: *"Doe scenario 1 + 2 grondig. Beter twee goed dan vier half."*
> - **MBO-4 sneller:** vraag *"Wat zou je willen meten dat NIET in dit scenario staat?"* — opent autonomie.

> **Valkuil — quiz als toets:**
> Als iemand vraagt *"telt dit?"*: *"Nee. Dit telt voor jezelf. Het echte werk gebeurt in de duo-bespreking."*

---

### Blok 3: Duo-reflectie
**00:25 - 00:35** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt — door vergelijking met de oefenpartner — wat hij goed deed en waar zijn redenering hapert.

**Werkvorm:** Duo-gesprek met werkblad wb-03-reflecteren.

**Instructie:**

1. **Werkblad uitdelen + duo's vormen** (1 min) — deel wb-03 uit. *"Zelfde duo als in fase 1. Vergelijk je quiz-antwoorden."* Toon slide 6.

2. **Duo-gesprek** (6 min) — zet timer op 6 min. Loop rond. Luister naar:
    - Welk scenario verschilden ze het meest?
    - Welke redenering werd herkend?
    - Welke vraag bleef hangen?
    Verzamel 2-3 sterke voorbeelden voor de plenaire ronde.

3. **Plenaire deel-ronde** (3 min) — toon slide 7. Vraag drie vragen:
    - *"Bij welk scenario verschilden jullie het meest? Wat maakte het lastig?"* Vang 2 antwoorden.
    - *"Hoe bepaalde je het verschil tussen trend en piek?"* Vang 2 antwoorden.
    - *"Wie heeft op zijn eigen machine ooit een trend gezien die hij nu anders zou interpreteren?"* Vang 1-2 verhalen.
    Schrijf op flap-over: 3 sleutelwoorden uit hun antwoorden.

**Materiaal:**
- [ ] wb-03-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 6-7
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden los.
> - Bij scepsis ('we kunnen dit nooit zelf bijhouden'): erken, parkeer voor transferopdracht.
> - Schrijf op de flap-over alleen wat de groep zegt. Geen eigen lijstje.

> **Differentiatie:**
> - **Gemengde groep:** in plenaire bespreking eerst MBO-3, dan MBO-4. Bewaak: MBO-4 = aanvullen, niet overnemen.

> **Valkuil — reflectie wordt afrekening:**
> Als duo's beginnen te vergelijken wie meer goed had: zeg *"Niet wie meer goed had — WAAR jullie verschilden. Daar zit de leerwinst."*

---

### Blok 4: Theorie — 3 stappen + transferopdracht
**00:35 - 00:40** | 5 min | Kolb-fase: theoretiseren

**Doel:** Theorie bevestigt en kapselt in wat operators in fase 1-3 zelf hebben ontdekt. Operator vertaalt naar één concrete actie deze week.

**Werkvorm:** Trainer-geleide korte handout-bespreking + transferopdracht.

**Instructie:**

1. **Werkblad uitdelen** (15 sec) — deel wb-04 uit. *"Pak je markeerstift."*

2. **3 stappen samenvatten** (2 min) — toon slide 8 (diagram). Loop ze één voor één langs:
    - *"Stap 1: basislijn — meet 5 dagen, elke 30 min, jouw normaalwaarde."*
    - *"Stap 2: trend — vergelijk deze week met vorige week. Stijgt het?"*
    - *"Stap 3: piek vs ruis — drie keer of vaker = signaal. Eén losse piek die verdwijnt = ruis."*
    Wijs naar de flap-over-kapstok. *"Dit is wat jullie net zelf hebben gedaan."*

3. **Transferopdracht** (2 min) — toon slide 9. Zeg:
    - *"Deze week: kies één machine. Doe 5 metingen verspreid over 3 werkdagen, op vaste tijden. Bereken het gemiddelde van temperatuur, druk en trillingen. Stuur die drie getallen in de groepsapp binnen 3 dagen."*
    - *"Dat zijn jouw eerste eigen basislijn-getallen, uniek voor jouw machine."*
    - *"En: let ook op niet-numerieke signalen. Geluid, geur, vibratie die je voelt. Vraag de onderhoudstechnicus welke sensorwaarden hij belangrijk vindt bij JOUW machine. Volgende sessie vergelijken we — en bouwen we daarop voort: drempelwaarden in LO-202."*

4. **Afsluiting** (45 sec) — *"Schrijf op het werkblad: welke machine, welke 5 meetmomenten. Dat is je commitment."* Loop rond, check dat het ingevuld is.

**Materiaal:**
- [ ] wb-04-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 8-10
- [ ] diagram-lo-smart-mfg-201.svg (op slide 8)
- [ ] Flap-over (3 stappen-kapstok)
- [ ] Timer

> **Tips voor de trainer:**
> - 5 minuten — geen seconde meer. Theorie bevestigt, vervangt niet.
> - Lees de handout SAMEN, niet voor.
> - De transferopdracht is het belangrijkste van fase 4 — niet overslaan.

> **Differentiatie:**
> - **MBO-3 basis:** één machine, één sensor (niet alle drie). Eenvoudiger commitment = meer kans op uitvoering.
> - **MBO-4 sneller:** geef bron mee (AIMM Competentieframework v0.1) en vooruitwijzing naar drempelwaarden in LO-202.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort de 3-stappen-samenvatting in tot 1 min (alleen flap-over wijzen). Sla transferopdracht NOOIT over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-experimenteren.md | n + 2 | A4 dubbelzijdig (basislijn-meetblad) |
| ☐ | wb-02-ervaren.md | n + 2 | A4 enkelzijdig (4 scenario's) |
| ☐ | wb-03-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-04-theoretiseren.md | n + 2 | A4 dubbelzijdig (handout + transferopdracht) |
| ☐ | Echte machine OF simulator op laptops | 1 per duo | model-lo-smart-mfg-201.html |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (basislijn-getallen) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over (3 stappen-kapstok) | 1 vel | Vooraf voorbereid |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 experimenteren | Basislijn meten op machine of simulator | Eigenaarschap: jouw machine, jouw normaalwaarden |
| 2 ervaren | 4 scenario's beoordelen | Trend, piek, ruis kunnen onderscheiden |
| 3 reflecteren | Duo-gesprek over keuzes | Inzicht waar redenering hapert |
| 4 theoretiseren | 3 stappen + transferopdracht | 3 basislijn-getallen in groepsapp binnen 3 dagen |

**Slagingscriterium:** Minimaal 3 van 4 scenario's correct + transferopdracht concreet ingevuld.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: wie heeft welke basislijn-getallen toegezegd? (volgmoment LO-202)
- [ ] Sceptici genoteerd voor 1-op-1 in volgende sessie
- [ ] xAPI-statements verstuurd: `attempted` (oefening), `completed` (quiz), `passed` (quiz score >= 0.75)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | Sensordata lezen*
*Bron: AIMM Competentieframework v0.1 (PM-02). Sesana et al. (2024). Artificial Intelligence in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
