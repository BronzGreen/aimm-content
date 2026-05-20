# Van anomaliescore naar onderhoud: het verkeerslichtmodel — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 30 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan anomaliescores vertalen naar de juiste onderhoudsactie met het verkeerslichtmodel — kiest bij minimaal 3 van 4 scenario's de juiste kleurzone en bijbehorende actie + maakt complete werkorder. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 afgerond. LO-201 en LO-202 ideaal. LO-108 (SHAP) is een plus. |
| **Stadium (H&B)** | Bewust bekwaam — wil zelf beslissingen nemen, zoekt bevestiging |
| **Begeleidingsstijl** | Coachen — observeren, doorvragen, niet voorzeggen |
| **Ruimte** | U-opstelling of clusters van 4. Beamer + scherm. Dashboard-printscreens of simulator. Flap-over. |
| **Plek in module** | Workshop-blok 3 — afsluitend LO van PdM-pipeline (201 → 202 → 205) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Storingsquiz: 4 dashboardscenario's beoordelen | ervaren | 8 min |
| 00:08 - 00:15 | Duo-reflectie: vergelijk je keuzes | reflecteren | 7 min |
| 00:15 - 00:20 | Theorie: verkeerslichtmodel + werkorder-stappen | theoretiseren | 5 min |
| 00:20 - 00:30 | Eigen werkorder maken | experimenteren | 10 min |

**Totaal:** 30 minuten — strak. **Buffer:** 30 sec per blok.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print dashboard-printscreens 4 scenario's — per duo OF zet ze klaar op slide 2-5.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bereid je voor op de combinatieregels (één hoog vs meerdere matig vs hoog+laag).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over op met verkeerslichtmodel-kapstok: vier kleurblokken (groen 0-30, geel 30-50, oranje 50-70, rood 70+) met bijbehorende acties.
- [ ] Schrijf op tweede flap-over: **SCORE = ADVIES, GEEN BEVEL**.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Storingsquiz — 4 dashboardscenario's
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer beoordeelt 4 dashboardscenario's en kiest per scenario een kleur + actie. Ankerpunt voor de theorie in fase 3.

**Werkvorm:** Individuele oefening met scoringsformulier wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (45 sec) — toon slide 1. Zeg: *"Vorige sessies hebben jullie sensordata leren lezen (LO-201) en drempelwaarden ingesteld (LO-202). Vandaag de laatste stap: wat doe je met die scores? Wanneer grijp je in?"*

2. **Trigger** (45 sec) — vraag: *"Wie heeft op zijn werkvloer wel eens een hoge score gezien op het dashboard?"* Vang 1-2 reacties. Geen oordeel.

3. **Werkblad uitdelen + opdracht** (1 min) — deel wb-01 uit. Toon slide 2. Zeg:
    - *"Vier dashboardscenario's. Per scenario: kies de kleur — groen, geel, oranje of rood. Schrijf op welke actie en binnen welke termijn. Schrijf ook waarom."*
    - *"Geen kapstok nu. Gebruik je gevoel en je ervaring uit LO-201/202."*

4. **Werken** (5 min 30) — zet timer op 5 min 30. Loop rustig rond. Stel geen sturende vragen. Bij vastlopen: *"Wat zou je doen als dit JOUW machine was?"*

5. **Verzamelmoment** (30 sec) — *"Pen neer. Tel je keuzes. We bespreken in duo's."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2 (4 scenario's op slide 2 of slides 2-5)
- [ ] Dashboard-printscreens (per duo) als geen beamer
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voorzeggen. De waarde is dat duo's verschillende kleuren kiezen — daar ligt fase 2.
> - Houd verkeerslichtmodel-kapstok bedekt (papier eroverheen). Onthul pas in fase 3.
> - Bij MBO-4 die snel klaar is: vraag *"Wat zou je willen weten dat NIET in dit dashboard staat?"*

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt op scenario 3-4: *"Doe scenario 1 + 2 grondig. Beter twee goed dan vier half."*
> - **MBO-4 sneller:** vraag *"Hoe zeker ben je per scenario? Op een schaal van 1-10?"*

> **Valkuil — operator volgt blind de score:**
> Bij iemand die zegt 'score 45 dus geen actie': maak nu al een aantekening. Adresseer dit in fase 3 expliciet — *"Je kent je machine."*

---

### Blok 2: Duo-reflectie — vergelijk je keuzes
**00:08 - 00:15** | 7 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt — door vergelijking — dat keuzes uiteenlopen en dat een gedeeld kader nodig is.

**Werkvorm:** Duo-reflectie met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen + duo's vormen** (30 sec) — deel wb-02 uit. *"Zoek een buurman."* Toon slide 3.

2. **Duo-gesprek** (4 min) — zet timer op 4 min. Drie vragen op het werkblad:
    - *"Bij welk scenario verschilden jullie het meest? Welke kleur koos jij, welke je buurman?"*
    - *"Wanneer vertrouw je de score? Wanneer vertrouw je je eigen gevoel?"*
    - *"Bij welk scenario twijfelde je het meest? Waarom?"*
    Loop rond. Verzamel 2-3 sterke voorbeelden voor plenaire ronde.

3. **Plenaire deel-ronde** (2 min 30) — toon slide 4. Vraag:
    - *"Bij welk scenario verschilden jullie het meest?"* Vang 2 antwoorden.
    - *"Wanneer vertrouw je de score, wanneer je gevoel?"* Vang 1-2 antwoorden.
    - *"Wat zou helpen om met meer zekerheid te kiezen?"* Mik op antwoord: een kapstok / kader.
    Schrijf op flap-over: 2-3 sleutelwoorden. Onthul de verkeerslichtmodel-flap-over: *"Die kapstok krijgen we nu."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over (verkeerslichtmodel) — onthullen aan eind blok 2
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden los.
> - De zin *"Wanneer vertrouw je de score, wanneer je gevoel?"* is de hoeksteen. Bewaar ruimte voor het antwoord.
> - Bij scepsis ('we mogen toch niet zelf beslissen?'): erken, parkeer voor fase 3 (score = advies).

> **Differentiatie:**
> - **Gemengde groep:** in plenaire bespreking eerst MBO-3, dan MBO-4.

> **Valkuil — duo wordt afrekening:**
> Als duo's beginnen te ruzieën over wie 'gelijk had': zeg *"Niet wie gelijk had. WAAR jullie verschilden. Daar zit de leerwinst."*

---

### Blok 3: Theorie — verkeerslichtmodel + werkorder
**00:15 - 00:20** | 5 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert het verkeerslichtmodel en het 5-stappen-werkorder kennen — als kapstok voor wat hij in fase 1 al deed.

**Werkvorm:** Trainer-geleide korte handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (15 sec) — deel wb-03 uit. *"Pak je markeerstift."*

2. **Verkeerslichtmodel** (2 min) — toon slide 5 (diagram). Loop de vier kleuren langs:
    - *"Groen, score 0-30: geen actie nodig."*
    - *"Geel, 30-50: verhoogde monitoring, dagelijks checken."*
    - *"Oranje, 50-70: plan onderhoud binnen 2 weken."*
    - *"Rood, 70+: plan inspectie binnen 48 uur."*
    Wijs naar de flap-over. *"Dit is wat jullie in fase 1 al gevoelsmatig deden — nu met getallen."*

3. **Combinatieregels** (1 min) — toon slide 6. *"Drie vuistregels:"*
    - *"Eén sensor hoog = lokaal probleem of sensorstoring. Check die ene component."*
    - *"Meerdere sensoren matig verhoogd = systeembreed. Check koeling, smering, voeding."*
    - *"Hoog en laag tegelijk = combinatie. Temperatuur hoog + koelmiddeldruk laag = koelprobleem."*

4. **Werkorder 5 stappen** (1 min 30) — toon slide 7. Loop ze langs:
    - *"1: welke machine. 2: welke sensoren — wat wees SHAP aan? 3: urgentie — welke kleur. 4: voorgestelde actie — inspectie, onderhoud, vervanging. 5: deadline — uit het verkeerslichtmodel."*
    - Voorbeeld Marjan kort: *"Machine 2, hydraulisch systeem, oranje, inspectie, binnen 2 weken. SHAP-grafiek als bijlage."*

5. **Kernprincipe** (15 sec) — wijs naar tweede flap-over. *"SCORE = ADVIES, GEEN BEVEL. Als score zegt 45 maar jij hoort iets raars: plan toch een inspectie. AI ondersteunt jouw vakkennis, vervangt het niet."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-7
- [ ] diagram-lo-smart-mfg-205.svg (op slide 5)
- [ ] Flap-over (verkeerslichtmodel) + flap-over (score = advies)

> **Tips voor de trainer:**
> - 5 minuten — strak. Geen seconde meer.
> - Verwijs naar fase 1: *"Score 45 — wat koos je? Geel? Klopt met de kapstok."*
> - Bij vraag over grenzen-precisie (49 vs 51): *"Richtgrenzen, geen wetten. Trend telt mee."*

> **Differentiatie:**
> - **MBO-3 basis:** alleen vier kleuren + 5-stappen-werkorder. Niet uitweiden.
> - **MBO-4 sneller:** noem dat de grenzen aanpasbaar zijn voor kritische processen (25 voor groen, 60 voor rood).

> **Valkuil — te veel uitweiden naar SHAP:**
> SHAP is LO-108. Hier alleen verwijzen: 'wat wees SHAP aan = stap 2 in werkorder.' Niet uitleggen.

---

### Blok 4: Eigen werkorder maken
**00:20 - 00:30** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer kiest een eigen machine, bedenkt een scenario en schrijft een complete werkorder volgens het 5-stappenplan.

**Werkvorm:** Individueel actieplan met coaching — werkblad wb-04-experimenteren.

**Instructie:**

1. **Werkblad uitdelen + opdracht** (45 sec) — deel wb-04 uit. Toon slide 8. Zeg:
    - *"Kies één machine waar je vaak op werkt. Bedenk een scenario: welke sensoren wijken af? Welke kleur? Schrijf een complete werkorder met de 5 stappen."*
    - *"Ankerpunt: de technicus die jouw werkorder leest weet niet wat jij weet. Schrijf alsof hij niets weet."*

2. **Werken** (6 min) — zet timer op 6 min. Loop rond. Coach-modus:
    - *"Welke machine? Wees specifiek."*
    - *"Welke sensoren? Hoe weet je dat?"*
    - *"Welke kleurzone? Klopt met je drempelwaarden uit LO-202?"*
    - *"Wat is de actie? En de deadline?"*
    Niet voorzeggen. Bij gat in werkorder: *"Wat ontbreekt nog?"*

3. **Plenaire deel-ronde** (2 min) — toon slide 9. Vraag 2 deelnemers:
    - *"Lees je werkorder voor."* Bevestig de 5 stappen + check kleurzone klopt.
    - Bij ontbrekende info: *"Wat zou je nog toevoegen voor de technicus?"*

4. **Transferopdracht** (1 min 15) — toon slide 10. Zeg:
    - *"Morgen: check het dashboard van jouw machine. Bepaal de kleurzone. Beslis of actie nodig is."*
    - *"Deze week: oefen 1 week lang elke ochtend — dashboard checken, kleur bepalen, actie noteren. Bespreek met je teamleider in het werkoverleg."*
    - *"Over 1 week: deel in groepsapp je drie meest opvallende observaties."*
    - *"En: vraag aan iemand in je team om je werkorder van vandaag te lezen. Klopt het? Snap hij het?"*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen + markeerstift per deelnemer
- [ ] Slides 8-10
- [ ] Timer

> **Tips voor de trainer:**
> - Bewaar 1 minuut voor transferopdracht. Niet overslaan.
> - Bij snel klaar: *"Hoe zou je de SHAP-grafiek (LO-108) bij je werkorder voegen?"*
> - Houd het concreet. Vage werkorders ('kijken') terugsturen met *"Wat moet de technicus DOEN?"*

> **Differentiatie:**
> - **MBO-3 basis:** laat duo's de werkorder samen schrijven, individueel afronden.
> - **MBO-4 sneller:** vraag *"Hoe zou je verschillende sensoren tegen elkaar afwegen? En hoe zou je dat onderbouwen voor je teamleider?"*

> **Valkuil — werkorder te beknopt:**
> Houd de 5 stappen vast. Bij 'kijken': *"Wat KIJKEN — visueel? Met een tool? Welke zone?"*

> **Valkuil — geen toegang tot dashboard:**
> Bied alternatief: dagelijks de drie kritische sensoren uit LO-201/202 checken. Verkeerslichtmodel werkt OOK op drempel-overschrijdingen.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig (4 scenario's) |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig (model + werkorder) |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 dubbelzijdig (eigen werkorder-template) |
| ☐ | Dashboard-printscreens | per duo OF op beamer | 4 scenario's |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (verkeerslichtmodel) | 1 vel | Vooraf voorbereid, bedekt in fase 1-2 |
| ☐ | Flap-over (score = advies) | 1 vel | Onthuld in fase 3 |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 4 dashboardscenario's beoordelen | Kleur + actie + termijn op gevoel |
| 2 reflecteren | Duo: wanneer vertrouw je score, wanneer gevoel? | Behoefte aan kapstok |
| 3 theoretiseren | Verkeerslichtmodel + werkorder 5 stappen | Score = advies, geen bevel |
| 4 experimenteren | Eigen werkorder schrijven | Concrete werkorder met 5 stappen |

**Slagingscriterium:** Minimaal 3 van 4 scenario's correct + werkorder met 5 stappen ingevuld.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: welke werkorders werden gemaakt? (input voor module 3 — eigen business case)
- [ ] Sceptici genoteerd voor 1-op-1 in volgende sessie
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `attempted` (werkorder), `completed` (werkorder ingevuld)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | Van anomaliescore naar onderhoud*
*Bron: Sesana et al. (2024). Artificial Intelligence in Manufacturing, pp. 474-475 + operationele best practices.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
