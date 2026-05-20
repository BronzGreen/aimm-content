# Het model verbeteren — meer data, betere labels — Draaiboek
*AI-Vision Module 2 (Train) | Workshop-blok 60 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan de fouten van een vision-model analyseren, gericht trainingsdata + labels toevoegen, en de prestatieverbetering kwantificeren in recall/precision per categorie. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 + LO-511 (data labelen), LO-512 (drempelwaarde), LO-513 (confusion matrix). Heeft een vision-model in productie of pilot. |
| **Stadium (H&B)** | Bewust bekwaam — wil zelf het model verbeteren |
| **Begeleidingsstijl** | Coachen — open vragen, faciliteer eigen ontdekking |
| **Ruimte** | Clusters van 4 met laptops (toegang tot vision-dashboard); foto-opstelling indien beschikbaar; whiteboard, beamer |
| **Plek in module** | Tweede helft Module 2 — bouwt op LO-513, leidt naar LO-094 (human-in-the-loop) en Module 3 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Foutenanalyse confusion matrix | ervaren | 12 min |
| 00:12 - 00:20 | Duo-reflectie: foutenpatroon | reflecteren | 8 min |
| 00:20 - 00:30 | Iteratie-cyclus + lakdefect-casus | theoretiseren | 10 min |
| 00:30 - 01:00 | Eigen iteratie uitvoeren | experimenteren | 30 min |

**Totaal:** 60 minuten — geen aparte pauze, korte stretch tussen fase 3 en 4.
**Buffer:** 1-2 min flexibel binnen de fasen.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Test `model-lo-smart-mfg-514.html` op een laptop — werkt de interactieve foutenanalyse?
- [ ] Open `diagram-lo-smart-mfg-514.svg` in een tweede tab — voor fase 3.
- [ ] Bedenk welke deelnemers wel/geen toegang hebben tot een eigen model. Plan duo's bij gemengde toegang.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over op met de iteratie-kapstok: **analyse → data → labels → hertest**.
- [ ] Schrijf op een tweede flap-over: **"Wat is bij jullie de zwakste categorie?"** — voor de plenaire deel-ronde.
- [ ] Camera/smartphone klaar per deelnemer (of gedeeld).
- [ ] Open slide 1 + dashboard van eigen vision-model (waar mogelijk) of demo-model in `model-lo-smart-mfg-514.html`.

---

## Blok-details

### Blok 1: Foutenanalyse confusion matrix
**00:00 - 00:12** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer identificeert in zijn eigen (of demo-) model minimaal 2 categorieën met recall onder 80% en bepaalt welke categorie de hefboom is.

**Werkvorm:** Individuele analyse met werkblad wb-01-ervaren + interactief model + (waar beschikbaar) eigen vision-dashboard.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"Het model dat je hebt draaien is niet 'klaar'. Het is een eerste versie. De komende 60 minuten leer je hoe je het zelf beter maakt — zonder leverancier."*

2. **Trigger** (1 min) — vraag: *"Wie van jullie heeft het idee: 'ons model werkt wel, maar mist soms iets'? Wat mist het meestal?"* Vang 2-3 reacties. Reageer: *"Dat 'iets' is wat we vandaag aanpakken. Niet algemeen — heel specifiek per categorie."*

3. **Werkblad uitdelen + opdracht** (1 min) — deel wb-01 uit. Toon slide 2. Zeg: *"Open je vision-dashboard, kijk naar de confusion matrix. Of gebruik de foutenanalyse op je laptop. Vraag: welke 2 categorieën hebben recall onder 80%? Schrijf op het werkblad welke fouten het model wel pakte en welke het miste."*

4. **Individueel werken** (8 min) — zet timer op 8 min. Loop rond. Bij vragen: *"Wat zegt de confusion matrix over deze categorie? Hoeveel kreeg het model goed van de echte defecten? En hoeveel ging er door?"* Geen voorzeggers — laat ze de matrix zelf lezen.

5. **Kort verzamelmoment** (1 min) — *"Pen neer. Welk getal heb je voor je zwakste categorie? Eén woord op de flap-over."* Schrijf 4-5 categorieën op met hun recall-percentage.

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] model-lo-smart-mfg-514.html (op laptop per duo OF beamer)
- [ ] Toegang tot eigen vision-dashboard (waar mogelijk)
- [ ] Pen per deelnemer
- [ ] Slides 1-3
- [ ] Timer
- [ ] Flap-over (zwakste categorieën)

> **Tips voor de trainer:**
> - Niet zelf de confusion matrix uitleggen — dat is LO-513. Verwijs terug bij vragen.
> - Bij 'hoeveel categorieën moet ik?' — twee is genoeg, drie is bonus.

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt op de matrix-getallen, sturen: *"Welke rij heeft het laagste percentage rechts onder? Begin daar."*
> - **MBO-4 sneller:** vraag *"Wat zou je doen als alle categorieën boven 90% zaten? Welke is dan de hefboom?"*

> **Valkuil — geen toegang tot eigen model (vk-05):**
> Bevestig: *"Geen probleem."* Werk met het demo-model. Vraag wel: *"Welke categorie is bij jullie waarschijnlijk de zwakste? Schrijf dat als hypothese — we testen dat deze week."*

> **Valkuil — 'meer data is altijd beter' (vk-01):**
> Bevestig de gedachte. Scherp aan: *"Goede gedachte — gerichte data is nóg beter. 30 foto's van de zwakste categorie zijn waardevoller dan 200 willekeurige."*

---

### Blok 2: Duo-reflectie — foutenpatroon
**00:12 - 00:20** | 8 min | Kolb-fase: reflecteren

**Doel:** Deelnemer verbindt het foutenpatroon aan een hypothese over de oorspronkelijke trainingsdata: data-tekort, label-fouten, of nieuw type defect?

**Werkvorm:** Duo-reflectie met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 4.

2. **Duo's vormen** (30 sec) — *"Zoek iemand met (waar mogelijk) een andere zwakke categorie. Bespreek: waarom faalt het model juist daar?"*

3. **Duo-gesprek** (5 min) — zet timer op 5 min. Loop rond. Stel verdiepende vragen:
    - *"Hoeveel foto's zaten er van die categorie in de oorspronkelijke set? Was dat genoeg?"*
    - *"Zie je dit type defect tegenwoordig vaker dan toen je trainde?"*
    - *"Zijn de labels van die categorie door één persoon gemaakt of door meerdere?"*

4. **Plenaire deel-ronde** (2 min) — toon slide 5. Vraag 2 duo's: *"Wat is jullie hypothese: data-tekort, label-fouten, of nieuw defect?"* Schrijf op flap-over de drie oorzaken met turflijst.

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 4-5
- [ ] Flap-over (drie oorzaken)
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf alleen wat de groep zegt — niet voorzeggen welke oorzaak het is.
> - Tel innerlijk tot 7 na de hoofdvraag.

> **Valkuil — bang om model te verergeren (vk-02):**
> Erken: *"Begrijpelijke zorg — daarom is peer-check er. Komt zo terug in fase 4."*

> **Differentiatie:**
> - **Gemengde groep:** vorm duo's MBO-3 + MBO-4. MBO-4 stelt vragen, voorziet niet.

---

### Blok 3: Iteratie-cyclus + lakdefect-casus
**00:20 - 00:30** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer begrijpt de iteratie-cyclus (analyse → data → labels → hertest) en ziet een concreet voorbeeld waar het werkt: kleurafwijkingen 60% → 85% recall na 80 extra foto's.

**Werkvorm:** Trainer-geleide bespreking met diagram + handout.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift."*

2. **Iteratie-cyclus** (3 min) — toon slide 6 (diagram-lo-smart-mfg-514.svg). Loop de vier stappen langs:
    - *"Analyse: confusion matrix lezen — welke categorie zit onder 80%?"*
    - *"Data: 30+ gerichte foto's van die categorie maken op je eigen lijn."*
    - *"Labels: consistent labelen + peer-check — minder dan 1 op 10 inconsistent."*
    - *"Hertest: model opnieuw trainen, recall/precision per categorie vergelijken."*

3. **Lakdefect-casus** (5 min) — toon slide 7. Loop het voorbeeld stap voor stap door:
    - *"Vóór iteratie: krassen 95% recall, kleurafwijkingen 60% recall."*
    - *"Actie: 80 extra foto's met kleurafwijkingen toegevoegd, peer-gecheckt."*
    - *"Na iteratie: krassen 95% recall, kleurafwijkingen 85% recall."*
    - *"Inzicht: gerichte data van zwakste categorie heft prestatie omhoog zonder andere categorieën te verslechteren."*

4. **Koppeling aan eigen casus** (1 min 30) — *"Pak je werkblad. Bij welke stap zit jij nu? Welke categorie ga je aanpakken?"* Twee deelnemers laten reageren.

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 6-7
- [ ] diagram-lo-smart-mfg-514.svg (op slide 6)
- [ ] Flap-over (iteratie-kapstok)

> **Tips voor de trainer:**
> - Houd het tempo strak — 10 min is voldoende, niet meer.
> - Vier stappen + één casus = klaar. Niet de hele theorie.

> **Valkuil — trainer duikt te diep (vk-04):**
> Geen 'transfer learning', geen 'data augmentation', geen hyperparameters. Twee acties: (1) gerichte data, (2) consistente labels. Klaar.

> **Differentiatie:**
> - **MBO-3 basis:** gebruik altijd de lakdefect-casus, niet de eigen.
> - **MBO-4 sneller:** noem kort 'data-centric AI' als achtergrond, parkeer voor LO-094.

---

### Blok 4: Eigen iteratie uitvoeren
**00:30 - 01:00** | 30 min | Kolb-fase: experimenteren

**Doel:** Deelnemer voert (of plant gedetailleerd) een echte iteratie: 30+ extra foto's verzamelen, consistent labelen, peer-check uitvoeren, hertraining plannen.

**Werkvorm:** Individueel + duo-peer-check + plenaire afronding.

**Instructie:**

1. **Werkblad uitdelen + briefing** (2 min) — deel wb-04 uit. Toon slide 8. Zeg: *"Vier delen: (1) zwakste categorie kiezen, (2) 30 foto's verzamelen — nu of plan, (3) labels maken + peer-check, (4) hertraining-moment plannen."*

2. **Stap 1 — categorie + plan** (5 min) — zet timer op 5 min. Loop rond. Help concretiseren: *"Welke shift? Welke camera? Welke 5 labels laat je peer-checken?"*

3. **Stap 2 — foto's verzamelen** (10 min) — als de foto-opstelling beschikbaar is: deelnemers gaan in duo's foto's maken. Eén fotografeert, één labelt direct. Wissel halverwege. Anders: deelnemer schrijft een gedetailleerd verzamelplan met datum, shift, camera, hoeveelheid.

4. **Stap 3 — labels + peer-check** (8 min) — duo's wisselen 5 willekeurige labels. Vraag: *"Hoeveel inconsistent? Onder 1 op 10 — kan erin. Boven 1 op 10 — eerst labelcriteria herzien."*

5. **Stap 4 — hertrainings-plan** (3 min) — zet timer op 3 min. Op werkblad: wanneer hertrainen, wie heeft toegang tot het script, hoe meet je de verbetering (recall/precision voor en na).

6. **Afsluiting + transferopdracht** (2 min) — toon slide 9. *"Deze week: tweede iteratie plannen. Volgende kwaliteitsoverleg: resultaten bespreken. Vraag een collega van een naburige lijn hetzelfde te doen."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Camera/smartphone per deelnemer
- [ ] Foto-opstelling indien beschikbaar
- [ ] Pen + markeerstift per deelnemer
- [ ] Slides 8-9
- [ ] Timer
- [ ] Toegang tot trainingsset/dashboard waar mogelijk

> **Tips voor de trainer:**
> - Concreet maken is de competentie. Vage plannen ('ik ga foto's maken') terugsturen met *"welke dag, welke shift, hoeveel?"*
> - Bewaar 2 min voor de transferopdracht — niet overslaan.

> **Differentiatie:**
> - **MBO-3 basis:** één categorie, 30 foto's, één peer-check. Genoeg.
> - **MBO-4 sneller:** vraag *"Welke tweede categorie zou je daarna aanpakken? Welke ROI verwacht je?"* Of laat een hertrainings-script bekijken.
> - **Gemengde groep:** vorm duo's gemengd. MBO-4 helpt met dashboard-navigatie. MBO-3 brengt productkennis voor labels.

> **Valkuil — iteratie blijft theorie (vk-03):**
> Druk door tot er een datum, shift, hoeveelheid en peer-naam staan. Liever 3 haalbare stappen dan één vage.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort fase 4 in tot 27 min door stap 2 op 7 min te zetten. Sla transferopdracht nooit over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (iteratie-kapstok) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over (oorzaken + hypothesen) | 1 vel | |
| ☐ | Camera/smartphone | n | Eigen toestel of geleend |
| ☐ | Foto-opstelling (verlichting + achtergrond) | 1 set | Optioneel — krachtig waar beschikbaar |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptops voor dashboard | n/2 | Toegang tot eigen vision-systeem |
| ☐ | model-lo-smart-mfg-514.html | 1 | Test vooraf |
| ☐ | diagram-lo-smart-mfg-514.svg | 1 | Op slide 6 |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Confusion matrix lezen, 2 zwakke categorieën vinden | Recall <80% per categorie identificeerbaar |
| 2 reflecteren | Hypothese: data-tekort, labels of nieuw defect | Oorzaak per categorie helder |
| 3 theoretiseren | Iteratie-cyclus + lakdefect-casus | 4 stappen begrepen, casus als blueprint |
| 4 experimenteren | 30+ foto's, peer-check, hertrainings-plan | Iteratie uitgevoerd of concreet gepland |

**Slagingscriterium:** ≥2 zwakke categorieën geïdentificeerd, 30+ gerichte foto's gepland of verzameld, peer-check uitgevoerd of gepland (<1 op 10 inconsistent), en hertrainings-plan met datum + eigenaar.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: welke categorieën zijn breed zwak in de groep (input voor LO-094)
- [ ] Deelnemers zonder toegang tot eigen model voor 1-op-1 markeren
- [ ] xAPI-statements verstuurd: `analyzed` (foutenanalyse), `improved` (iteratie), `completed` (hertrainings-plan)

---

*AIMM Curriculum | AI-Vision Module 2 (Train) | Het model verbeteren — meer data, betere labels*
*Bron: Cruz et al. (2024). AI in Manufacturing; Ng (2021). Data-centric AI.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
