# Visuele inspectie met deep learning — Draaiboek
*AI-Kwaliteitscontrole Module 1 (Gebruik) | Workshop-blok 40 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden uitleggen hoe AI-kwaliteitscontrole werkt door de drie stappen (camera, AI-analyse, beslissing) correct te benoemen en een voorbeeld te geven. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Geen — opstap-LO van de vision-pipeline. Eventueel cross-track video lo-smart-mfg-095 vooraf. |
| **Stadium (H&B)** | Bewust onbekwaam — kent kwaliteitscontrole, kent geen AI-werking |
| **Begeleidingsstijl** | Trainen — veel sturing, veel ondersteuning |
| **Ruimte** | U-opstelling of clusters van 4, beamer, flap-over, productfoto's geprint of digitaal |
| **Plek in module** | Workshop-blok 2 — opstap voor LO-010 (productietijd-besparing) en LO-101 (spuitgieten) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | Storingsquiz: goed of afgekeurd? | ervaren | 10 min |
| 00:10 - 00:20 | Duo-gesprek: waar was je het oneens? | reflecteren | 10 min |
| 00:20 - 00:30 | Drie stappen + classificatie vs segmentatie | theoretiseren | 10 min |
| 00:30 - 00:40 | Actieplan: AI op jouw werkplek | experimenteren | 10 min |

**Totaal:** 40 minuten — geen aparte pauze (workshop-blok binnen module 1).
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print 6 productfoto's (3 goed, 3 afgekeurd) per duo, OF zet ze klaar op slide 2.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bedenk één voorbeeldproduct uit jouw branche (isolatiepaneel, spuitgietproduct, gefreesd onderdeel).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over zichtbaar op met de drie stappen-kapstok (camera → AI → beslissing).
- [ ] Schrijf op een tweede flap-over alvast: links **"Vragen voor later"**, rechts **"AI = extra paar ogen"**.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Storingsquiz — goed of afgekeurd?
**00:00 - 00:10** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer geeft een eigen kwaliteitsoordeel op 6 productfoto's. Dit wordt het ankerpunt voor de AI-uitleg in fase 3.

**Werkvorm:** Individuele quiz met werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 40 minuten kijken we hoe een camera met AI defecten herkent op de productielijn. Tegen het eind weet je hoe het werkt en waar het op jouw werkplek zou kunnen helpen."*

2. **Trigger** (1 min) — vraag: *"Wie controleert nu zelf producten op kwaliteit? Waar let je dan op?"* Vang 2-3 reacties. Reageer alleen met *"herkenbaar"* — geen oordeel.

3. **Werkblad uitdelen + introduceren** (1 min) — deel wb-01 uit. Toon slide 2 met de 6 foto's. Zeg: *"Bekijk de foto's. Schrijf per foto op: goedgekeurd of afgekeurd, en wat je ziet. Er is geen goed of fout — het gaat om jouw beoordeling."*

4. **Individueel werken** (6 min) — zet timer op 6 min. Loop rustig rond. Stel geen sturende vragen. Als iemand vastloopt: *"Wat zou je doen als je dit op je lijn zag?"*

5. **Verzamelmoment** (1 min) — *"Pen neer. We gaan zo bespreken — niet nu al delen."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] 6 productfoto's (geprint per duo of op slide 2)
- [ ] Pen per deelnemer
- [ ] Slide 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voorzeggen. De waarde van de quiz is dat duo's verschillend oordelen.
> - Als iemand alle 6 binnen 2 minuten klaar heeft: vraag *"Schrijf bij elke foto ook één twijfel op."*
> - Houd de drie stappen-kapstok in je achterhoofd, gebruik hem nog niet.

> **Differentiatie:**
> - **MBO-3 basis:** als iemand een foto leeg laat: vraag *"Wat zie je überhaupt op deze foto? Beschrijf in één woord."*
> - **MBO-4 sneller:** vraag *"Welke foto vond je het lastigst? Waarom?"* — input voor fase 2.

> **Valkuil — deelnemer voelt zich getoetst:**
> Bevestig direct: *"Er is geen goed of fout — jouw beoordeling telt."* Niet uitleggen wat het juiste antwoord is.

---

### Blok 2: Duo-gesprek — waar was je het oneens?
**00:10 - 00:20** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt dat menselijke beoordeling subjectief is — en dat dat de stap naar AI-inspectie logisch maakt.

**Werkvorm:** Duo-gesprek met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 3.

2. **Duo's vormen** (30 sec) — *"Zoek iemand met wie je nog niet gesproken hebt. Vergelijk je antwoorden van de quiz."*

3. **Duo-gesprek** (6 min) — zet timer op 6 min. Loop rond. Luister naar wat er besproken wordt. Verzamel 2-3 sterke voorbeelden. Stel verdiepende vragen:
    - *"Bij welke foto verschilden jullie het meest?"*
    - *"Wat maakte de beslissing lastig?"*
    - *"Wat zou helpen om sneller en zekerder te beslissen?"*

4. **Plenaire deel-ronde** (3 min) — toon slide 4. Vraag:
    - *"Bij welke foto verschilden jullie het meest?"* Vang 2 antwoorden.
    - *"Wat maakt deze beoordeling lastig?"* Vang 2-3 antwoorden (vermoeidheid, twijfel, onduidelijke randen, persoonlijke maatstaf).
    - Schrijf 3-4 sleutelwoorden op flap-over. Zeg dan: *"Dit zijn precies de plekken waar AI kan helpen — of moeite kan hebben."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf op de flap-over alleen wat de groep zegt — niet jouw lijstje.
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden los.
> - Bij sceptische opmerking ('AI maakt ons overbodig'): erken eerst, parkeer voor fase 3.

> **Valkuil — AI als banenkiller-frame:**
> Bevestig: *"Goeie vraag — daar komen we zo op."* Schrijf op flap-over: AI = extra paar ogen. Werk uit in fase 3.

> **Differentiatie:**
> - **Gemengde groep:** vorm duo's MBO-3 + MBO-4. Bewaak: MBO-4 luistert eerst, deelt daarna.

---

### Blok 3: Drie stappen + classificatie vs segmentatie
**00:20 - 00:30** | 10 min | Kolb-fase: theoretiseren

**Doel:** De ervaring uit fase 1 wordt gekoppeld aan de drie stappen van AI-inspectie en aan het verschil tussen classificatie en segmentatie.

**Werkvorm:** Trainer-geleide handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **Drie stappen** (3 min) — toon slide 5. Loop ze één voor één langs:
    - *"Stap 1: camera-opname. Een gewone industriele camera maakt foto's of video van elk product."*
    - *"Stap 2: AI-analyse. Het AI-model bekijkt het beeld en herkent defecten."*
    - *"Stap 3: beslissing. Goed = door. Te repareren = terug. Beschadigd = uit de lijn."*
    - Wijs naar de flap-over-kapstok.

3. **Classificatie vs segmentatie** (4 min) — toon slide 6. Maak het visueel:
    - *"Classificatie: het AI-model zegt 'goed' of 'afgekeurd'. Maar het laat niet zien WAAR het defect zit."*
    - *"Segmentatie: het model kleurt de pixels aan waar iets fout is. Je kunt het ZIEN."*
    - Vraag: *"Welke van de twee zou jij willen op je lijn?"* (bijna altijd: segmentatie)
    - Bevestig: *"Precies — segmentatie is in de industrie de voorkeur, omdat je het kunt controleren."*

4. **Voorbeeld + data augmentatie** (2 min 30) — toon slide 7. Vertel:
    - *"Voorbeeld: een productielijn voor isolatiepanelen. Een camera fotografeert elk paneel na frezen. Het AI-model markeert de zijkanten. Twee rechthoeken = OK. Eén rechthoek = freesfout."*
    - *"En één trucje: data augmentatie. Je hebt vaak weinig defecte voorbeelden — gelukkig. Met data augmentatie variëer je bestaande beelden (spiegelen, helderheid). Daarmee leert het model uit minder data."*
    - *"In de praktijk: van 89% naar 99,5% nauwkeurig."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-7
- [ ] diagram-lo-smart-mfg-006.svg (op slide 5)
- [ ] Flap-over (drie stappen-kapstok)

> **Tips voor de trainer:**
> - Houd het tempo rustig — drie stappen + één onderscheid + één trucje is genoeg voor 10 min.
> - Bij vraag over U-net of F1-score: parkeer (vragen-voor-later). MBO-4-er onthoudt het, MBO-3 negeert het.
> - Na 99,5%-nauwkeurigheid: stilte van 3 sec, daarna *"En toch heb jij straks nog steeds werk — daar gaat fase 4 over."*

> **Valkuil — te technisch (U-net, F1):**
> Houd de drie stappen als kapstok. Termen alleen op verzoek MBO-4. Voor MBO-3: 'het AI-model is heel goed getraind, met data augmentatie als trucje.'

> **Differentiatie:**
> - **MBO-3 basis:** gebruik altijd hetzelfde voorbeeld (isolatiepaneel of jouw branche). Niet wisselen.
> - **MBO-4 sneller:** noem U-net en data augmentatie, geef bron Cruz et al. (2024) mee voor de geinteresseerden.

---

### Blok 4: Actieplan — AI op jouw werkplek
**00:30 - 00:40** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer vertaalt AI-kwaliteitscontrole naar één concrete toepassing op de eigen lijn.

**Werkvorm:** Individueel actieplan + groepsbespreking.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-04 uit. Toon slide 8. Zeg: *"Drie vragen: welk product? Welk specifiek defect? Wat zou de beslissing van de AI zijn — goed, terug, of weg?"*

2. **Individueel werken** (5 min) — zet timer op 5 min. Loop rond. Help concretiseren:
    - *"Welk product loopt op jouw lijn? Een specifiek voorbeeld."*
    - *"Welk defect zoek je nu met je ogen? Krassen, maatfout, kleur, vorm?"*
    - *"Waar zou de camera moeten staan? Voor of na de bewerking?"*

3. **Plenaire deel-ronde** (3 min 30) — vraag 3-4 deelnemers om hun toepassing kort te delen (max 30 sec per persoon). Vat samen op flap-over: product, defect, plek camera.

4. **Afsluiting + transferopdracht** (1 min) — toon slide 9. *"Deze week: kijk bewust naar één kwaliteitscontrole op je werk. Welke defecten zoek je? Hoe lang duurt het? Zou een camera dit ook kunnen zien? Vraag je teamleider of er al plannen zijn voor AI-inspectie. Volgende sessie: hoeveel productietijd dat scheelt — LO-010."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 8-10
- [ ] Timer

> **Tips voor de trainer:**
> - Concreet maken is de competentie. Vage actieplannen ('AI op alles') terugsturen met *"welk product specifiek?"*
> - Bij twijfel: *"Wat is de meest tijdrovende controle die je nu doet?"* Vaak is dát de eerste AI-toepassing.
> - Bewaar 30 sec voor de transferopdracht — niet overslaan.

> **Differentiatie:**
> - **MBO-3 basis:** één toepassing is genoeg. Niet vragen om data-aspecten of cameramodel.
> - **MBO-4 sneller:** vraag *"Welke data zou je moeten verzamelen om dit model te trainen?"* — dat opent de deur naar LO-101 / module 2.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort fase 4 in tot 8 min door werktijd op 4 min te zetten. Sla transferopdracht nooit over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 enkelzijdig |
| ☐ | 6 productfoto's | per duo OF beamer | 3 goed, 3 afgekeurd |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (drie stappen-kapstok) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over reserve | 1 vel | Voor parkeerlijst |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 6 productfoto's beoordelen op werkblad | Eigen kwaliteitsoordeel als startpunt |
| 2 reflecteren | Duo: waar was je het oneens? | Inzicht: menselijke beoordeling is subjectief |
| 3 theoretiseren | Drie stappen + classificatie vs segmentatie | AI-werking begrepen op kapstok-niveau |
| 4 experimenteren | Eigen werkplek toepassing | Concrete transfer naar de lijn |

**Slagingscriterium:** Drie stappen kunnen benoemen + één eigen toepassing met product + defect.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: welke toepassingen werden genoemd? (input voor LO-010 en LO-101)
- [ ] Sceptici genoteerd voor 1-op-1 in volgende sessie
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `completed` (drie stappen), `attempted` (actieplan)

---

*AIMM Curriculum | AI-Kwaliteitscontrole Module 1 (Gebruik) | Visuele inspectie met deep learning*
*Bron: Cruz et al. (2024). Artificial Intelligence in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
