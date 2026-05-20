# Autoencoder: AI leert wat normaal is — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 30 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden uitleggen hoe een autoencoder afwijkingen in productiedata herkent, door minimaal 3 stappen van het proces correct te benoemen (invoer, samenvatting, herstel, reconstructiefout). |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Geen. Cross-track video lo-smart-mfg-092 (3 min) als optionele voorbereiding. |
| **Stadium (H&B)** | Bewust onbekwaam — kent zijn machines, kent geen AI-werking |
| **Begeleidingsstijl** | Trainen — veel sturing, veel ondersteuning |
| **Ruimte** | U-opstelling of clusters, beamer, flap-over, sensorgrafieken klaar |
| **Plek in module** | Workshop-blok 1 — opstap voor LO-108 (SHAP) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Storingsquiz: 6 sensorgrafieken normaal of niet? | ervaren | 8 min |
| 00:08 - 00:15 | Duo + groep: hoe wist je het? | reflecteren | 7 min |
| 00:15 - 00:23 | Drie stappen + reconstructiefout | theoretiseren | 8 min |
| 00:23 - 00:30 | Actieplan eigen machine | experimenteren | 7 min |

**Totaal:** 30 minuten — geen pauze. **Buffer:** 30 sec per blok.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print de 6 sensorgrafieken (4 normaal, 2 met duidelijke afwijking) per duo, OF zet ze klaar op slide 2.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Kies een voorbeeldmachine die past bij de doelgroep (spuitgieten, CNC, verpakking).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over op met de drie stappen-kapstok: invoer → samenvatting → herstel.
- [ ] Open slide 1.
- [ ] Test timer.

---

## Blok-details

### Blok 1: Storingsquiz — sensorgrafieken normaal of niet?
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer beoordeelt 6 grafieken op buikgevoel — patroonherkenning zonder formules.

**Werkvorm:** Individuele quiz met werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 30 minuten kijken we naar een type AI dat leert wat normaal is. Het wordt vandaag concreet: jij gaat eerst doen wat de AI doet."*

2. **Werkblad uitdelen + opdracht** (1 min) — deel wb-01 uit. Toon slide 2 met de 6 grafieken. Zeg: *"6 sensorgrafieken — bijvoorbeeld trillingen van een machine. Per grafiek beslis: normaal of afwijkend? En schrijf op waaraan je het ziet. Geen goed of fout — je oordeel telt."*

3. **Individueel werken** (5 min) — zet timer op 5 min. Loop rond. Geen sturende vragen. Bij vastlopen: *"Vergelijk met de andere grafieken — welke ziet er anders uit dan de rest?"*

4. **Verzamelmoment** (1 min) — *"Pen neer. We gaan zo bespreken — niet nu al delen."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] 6 sensorgrafieken (geprint per duo of op slide 2)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voorzeggen. Het zelf-oordeel is hier de leerstof.
> - Bij snel klaar: vraag *"Welke grafiek vond je twijfelachtig? Schrijf op waarom."*
> - Het woord 'autoencoder' valt nog niet — bewaar voor fase 3.

> **Differentiatie:**
> - **MBO-3 basis:** als iemand niet weet waar te kijken: vraag *"Welke grafiek zou je als laatste kiezen voor 'normaal'?"*
> - **MBO-4 sneller:** vraag *"Welke 2 grafieken lijken het meest op elkaar? En welke wijken het meest af van die groep?"*

> **Valkuil — trainer geeft antwoord:**
> Niet doen. Het didactische scharnier in fase 3 ('jij deed wat de autoencoder doet') werkt alleen als ze zelf hebben geworsteld.

---

### Blok 2: Duo + groep — hoe wist je het?
**00:08 - 00:15** | 7 min | Kolb-fase: reflecteren

**Doel:** Deelnemer benoemt zelf de strategie van patroonherkenning — wat een autoencoder ook doet.

**Werkvorm:** Duo-gesprek + plenair, met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit.

2. **Duo-gesprek** (3 min) — toon slide 3. Zeg: *"Bespreek met je buurman: hoe koos je? Waar lette je op?"* Zet timer op 3 min. Loop rond. Luister naar:
    - patronen ('vorm van de curve', 'de pieken', 'het ritme')
    - vergelijkingsstrategieen ('deze week ik door dat de andere er anders uitzagen')

3. **Plenaire bespreking** (3 min) — toon slide 4. Drie open vragen:
    - *"Hoe deed je dat? Waar lette je op?"*
    - *"Wat was makkelijk? Wat was lastig?"*
    - *"Heb je een normaal beeld in je hoofd zonder dat iemand je dat heeft uitgelegd?"*
    - Schrijf 3-4 sleutelwoorden op flap-over (vorm, ritme, vergelijken, raar voelt, anders dan de rest).

4. **Verbinden** (30 sec) — *"Wat jullie net deden — leren wat normaal is door veel voorbeelden te zien — dat is precies wat AI doet bij anomaliedetectie. Daar hebben we een naam voor: autoencoder."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Slides 3-4
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf op flap-over alleen wat de groep zegt.
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden.
> - Bij sceptische opmerking: parkeer voor fase 3.

> **Valkuil — verwarring met visuele inspectie:**
> Als iemand zegt 'is dit hetzelfde als die foto's van LO-006?': bevestig overeenkomst, benoem verschil: 'visuele inspectie kent goed EN fout. Autoencoder kent alleen NORMAAL.'

> **Differentiatie:**
> - **Gemengde groep:** duo's MBO-3 + MBO-4 — bewaak dat MBO-4 sparringpartner is, geen voorzegger.

---

### Blok 3: Drie stappen + reconstructiefout
**00:15 - 00:23** | 8 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer kan de drie stappen invoer → samenvatting → herstel benoemen en de reconstructiefout uitleggen.

**Werkvorm:** Trainer-geleide handout-bespreking met SVG-diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **Het woord uitleggen** (1 min) — toon slide 5. *"Autoencoder. Auto = vanzelf. Encoder = samenvatter. Een vanzelf-samenvatter. Klinkt ingewikkeld — is het niet."*

3. **Drie stappen** (3 min 30) — toon slide 6 met diagram. Loop ze één voor één langs:
    - *"Stap 1: invoer. Sensordata van bijvoorbeeld een productiecyclus. Een trillingscurve, een drukpatroon."*
    - *"Stap 2: samenvatting. Het model maakt er een korte beschrijving van. Alsof je in 5 woorden zegt wat de machine doet."*
    - *"Stap 3: herstel. Vanuit die samenvatting probeert het model de oorspronkelijke data weer terug te bouwen."*
    - Wijs op de flap-over de drie stappen aan.

4. **Reconstructiefout** (2 min) — toon slide 7:
    - *"Het verschil tussen wat erin ging (stap 1) en wat eruit komt (stap 3) heet de reconstructiefout."*
    - *"Klein verschil = het model kent het patroon — normaal."*
    - *"Groot verschil = het model kan het niet goed terugbouwen — afwijking — alarm."*
    - Concreet voorbeeld: *"Spuitgietmachine. Cyclus 1 t/m 100 normaal, het model leert. Cyclus 101: matrijs raakt los, trillingen anders dan normaal — het model kan het niet goed terugbouwen — alarm."*

5. **Mens-AI-parallel** (1 min) — toon slide 8: *"Wat jullie deden in de quiz: jullie wisten wat normaal eruitziet, en bij grafieken die afweken voelde dat raar. Dat is wat de autoencoder doet — alleen sneller en zonder vermoeidheid."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-8
- [ ] diagram-lo-smart-mfg-093.svg (op slide 6)
- [ ] Flap-over (drie stappen-kapstok)

> **Tips voor de trainer:**
> - Vermijd wiskunde (MSE, Euclidische afstand). Reconstructiefout = verschil tussen plaatje voor en plaatje na.
> - Houd hetzelfde voorbeeld vast: spuitgietmachine met trillingen.
> - Bij vraag over latente ruimte: parkeer voor MBO-4-doorvraag, niet plenair behandelen.

> **Valkuil — autoencoder klinkt te abstract:**
> Vertaal altijd direct: 'auto = vanzelf, encoder = samenvatter — een vanzelf-samenvatter'. Gebruik mens-AI-parallel.

> **Differentiatie:**
> - **MBO-3 basis:** schrijf 'invoer → samenvatting → herstel' op flap-over. Niet meer.
> - **MBO-4 sneller:** noem latente ruimte en de vergelijking met datacompressie. Bron Goodfellow et al. (2016).

---

### Blok 4: Actieplan eigen machine
**00:23 - 00:30** | 7 min | Kolb-fase: experimenteren

**Doel:** Deelnemer benoemt waar in de eigen werksituatie een autoencoder kan helpen.

**Werkvorm:** Individueel werkblad + duo + plenair kort delen.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-04 uit. Toon slide 9. Drie vragen: *"Welke machine? Welke sensor? Welk verdacht-moment ken je?"*

2. **Individueel werken** (3 min) — zet timer op 3 min. Loop rond. Help concretiseren:
    - *"Welke machine merk je vaak iets raars aan?"*
    - *"Welke sensor zou jou kunnen waarschuwen — temperatuur, druk, trillingen, geluid?"*
    - *"Wat is voor jou een verdacht-moment dat je nu al voelt zonder dat een sensor het meet?"*

3. **Duo-uitwisseling** (1 min 30) — *"Deel je antwoord met je buurman. 45 sec elk."*

4. **Plenaire deel-ronde** (1 min 30) — vraag 2-3 deelnemers om kort te delen (max 30 sec per persoon).

5. **Afsluiting + transferopdracht** (30 sec) — toon slide 10. *"Deze week: let op patronen in je productiedata. Noteer een moment waar je zelf denkt: dit is niet normaal. Vraag je teamleider of er al sensordata wordt verzameld. Volgende sessie: hoe weet je WELKE sensor het probleem veroorzaakt — dat heet SHAP, LO-108."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 9-11
- [ ] Timer

> **Tips voor de trainer:**
> - Concreet maken is hier de competentie. Vage actieplannen ('mijn machine') terugsturen met *"welke sensor specifiek?"*
> - Bij twijfel: *"Welk geluid hoor je dat collega's niet horen?"* Open de deur naar zintuiglijke ervaring.
> - Bewaar 30 sec voor de transferopdracht.

> **Differentiatie:**
> - **MBO-3 basis:** één machine + één sensor is genoeg.
> - **MBO-4 sneller:** vraag *"Welke twee sensoren zou je aan elkaar moeten koppelen om patroon te zien?"*

> **Valkuil — actieplan blijft te vaag:**
> Concreet doorvragen. Verbinden met sensor-track LO-201 als die ook gevolgd wordt.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 enkelzijdig |
| ☐ | 6 sensorgrafieken | per duo OF beamer | 4 normaal, 2 afwijkend |
| ☐ | Pennen | n + 5 | |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (drie stappen-kapstok) | 1 vel | Vooraf voorbereid |
| ☐ | Timer | 1 | Met geluid |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 6 sensorgrafieken normaal/afwijkend | Eigen patroonherkenning als startpunt |
| 2 reflecteren | Duo + groep: hoe deed je dat? | Strategie expliciet — 'wat normaal is' |
| 3 theoretiseren | Drie stappen + reconstructiefout | Autoencoder begrepen op kapstok-niveau |
| 4 experimenteren | Eigen machine + sensor + verdacht-moment | Concrete transfer naar de werkvloer |

**Slagingscriterium:** Drie stappen kunnen benoemen + één eigen toepassing met machine en sensor.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd
- [ ] Genoteerd: welke sensoren werden genoemd? (input voor LO-108 en LO-201)
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `completed` (drie stappen), `attempted` (actieplan)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | LO-093*
*Bron: Goodfellow et al. (2016). Deep Learning, hfdst 14. | Sakurada & Yairi (2014). Anomaly Detection Using Autoencoders.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
