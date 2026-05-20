# SHAP: welke sensor draagt bij aan de anomalie? — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 30 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in een SHAP-grafiek de drie sensoren aanwijzen die het meest bijdragen aan een anomalie en kan per sensor in eigen woorden uitleggen waarom die afwijkt. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | LO-093 (autoencoder) — kent het concept anomaliedetectie |
| **Stadium (H&B)** | Bewust onbekwaam — krijgt anomaliemeldingen, weet niet hoe ze te lezen |
| **Begeleidingsstijl** | Trainen — veel sturing, veel ondersteuning |
| **Ruimte** | U-opstelling, beamer + scherm verplicht, flap-over met drie leesregels |
| **Plek in module** | Workshop-blok 2 — opvolger van LO-093, opstap voor LO-205 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Storingsquiz: 5 anomaliemeldingen — raden | ervaren | 8 min |
| 00:08 - 00:15 | Hoe doe je het nu zonder uitleg-AI? | reflecteren | 7 min |
| 00:15 - 00:23 | SHAP-grafiek leren lezen | theoretiseren | 8 min |
| 00:23 - 00:30 | Drie nieuwe SHAP-grafieken — actie | experimenteren | 7 min |

**Totaal:** 30 minuten — geen pauze. **Buffer:** 30 sec per blok.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Controleer dat slides 2-6 (5 anomaliemeldingen) en slide 11 (3 oefen-grafieken) goed zichtbaar zijn op groot scherm.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bedenk welke spuitgiet/CNC-context past bij de groep (zie ankerinformatie).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over op met de drie leesregels: 'Groot = belangrijk', 'Rood = hoger dan normaal', 'Blauw = lager dan normaal'.
- [ ] Open slide 1.
- [ ] Test timer.

---

## Blok-details

### Blok 1: Storingsquiz — 5 anomaliemeldingen, raden
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer ervaart hoe moeilijk het is om zonder SHAP-uitleg de juiste sensor te vinden.

**Werkvorm:** Quiz met directe feedback — werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"Je krijgt een melding van een AI-systeem: 'er is iets mis op machine 4'. Maar WAT precies? Vandaag gaan we kijken hoe het systeem dat zelf vertelt — met een grafiek die SHAP heet."*

2. **Werkblad uitdelen + opzet** (1 min) — deel wb-01 uit. *"Vijf meldingen, vijf machines. Bij elke melding noem ik de symptomen. Jij gokt welke sensor het probleem veroorzaakt. Daarna zie je het juiste antwoord."*

3. **Quiz draaien** (5 min 30) — toon slides 2-6. Eén voor één:
    - Melding 1 (slide 2): *"Spuitgietmachine 4. Cyclus 1247. Iets klopt niet. Welke sensor?"* — geef 30 sec — onthul antwoord — kort feedback (positief bij goed, *"Begrijpelijk dat je dat dacht — kijk waarom het anders is"* bij fout).
    - Herhaal voor melding 2-5.

4. **Verzamelmoment** (30 sec) — *"Hoeveel had je goed? Schrijf op je werkblad."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-6 (cover + 5 anomaliemeldingen)
- [ ] Beamer, groot scherm
- [ ] Timer

> **Tips voor de trainer:**
> - Doel is NIET dat ze goed gokken. Doel is dat ze de pijn voelen — daarom werkt fase 3.
> - Bij elke goeie gok: bevestig kort, niet uitvergroten ('je had geluk' is OK).
> - Bij elke fout: *"Niemand kan dit zonder uitleg — dat is normaal."*

> **Differentiatie:**
> - **MBO-3 basis:** als iemand niets durft te raden: vraag *"Welke sensor zou je het eerst checken op je eigen machine?"*
> - **MBO-4 sneller:** vraag *"Wat zou je willen weten om beter te kunnen raden?"* (= introductie van SHAP-behoefte).

> **Valkuil — sfeer wordt mat door veel fouten:**
> Genormaliseer: 'Zonder SHAP raadt niemand het goed.' Maak van de fout-ervaring de springplank voor fase 3.

---

### Blok 2: Hoe doe je het nu zonder uitleg-AI?
**00:08 - 00:15** | 7 min | Kolb-fase: reflecteren

**Doel:** Deelnemer benoemt zijn huidige strategie van storingsdiagnose — en zijn behoefte aan ondersteuning.

**Werkvorm:** Duo + plenair, met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 7.

2. **Duo-gesprek** (3 min) — drie open vragen:
    - *"Hoe doe je het nu op je werkvloer als een machine raar doet?"*
    - *"Waar kijk/luister/voel je naar?"*
    - *"Wat zou je willen weten dat je nu niet ziet?"*
    Loop rond. Luister naar concrete strategieen.

3. **Plenaire bespreking** (3 min) — toon slide 8. Verzamel:
    - Wat doe je nu? (kijken, ruiken, voelen, dashboard checken, collega vragen)
    - Wat is lastig? (veel sensoren tegelijk, niet weten welke eerste, tijdsdruk)
    Schrijf 4-5 sleutelwoorden op flap-over.

4. **Verbinden** (30 sec) — *"Wat jullie missen — een soort schatkaart die zegt 'kijk daar eerst' — dat is wat SHAP doet."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Slides 7-8
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag.
> - Ankerwoord: 'schatkaart'. Werkt beter dan 'visualisatie' of 'analyse'.
> - Bij sceptische opmerking ('het systeem moet maar gewoon werken'): erken, parkeer.

> **Differentiatie:**
> - **Gemengde groep:** duo's MBO-3 + MBO-4 — MBO-4 herkent dashboard-strategie, MBO-3 herkent zintuigen-strategie.

---

### Blok 3: SHAP-grafiek leren lezen
**00:15 - 00:23** | 8 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert de drie leesregels van een SHAP-grafiek toepassen op een voorbeeld.

**Werkvorm:** Trainer-geleide handout-bespreking met SVG-diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift."*

2. **Eerste blik op SHAP-grafiek** (1 min 30) — toon slide 9 (voorbeeldgrafiek). *"Dit is een SHAP-grafiek. Per sensor één balk. Drie dingen om naar te kijken — meer niet."*

3. **Drie leesregels** (3 min) — toon slide 10 één regel per keer:
    - *"Regel 1: groot = belangrijk. Hoe groter de balk, hoe meer die sensor bijdraagt aan de melding."*
    - *"Regel 2: rood = hoger dan normaal. Sensor meet meer dan het AI verwachtte."*
    - *"Regel 3: blauw = lager dan normaal. Sensor meet minder dan het AI verwachtte."*
    - Wijs naar de flap-over-kapstok.

4. **Voorbeeld-grafiek hardop lezen** (2 min 30) — terug naar slide 9. *"Trillingssensor — grote rode balk: hoofdverdachte, sterk verhoogd. Temperatuursensor — middel rode balk: tweede verdachte, ook verhoogd. Druksensor — kleine groene/normale balk: niet verdacht."*
    - *"Conclusie: eerst trillingsmotor controleren, daarna temperatuur."*
    - Vraag: *"Welke sensor zou jij als eerst checken op deze melding?"* Vang 1-2 antwoorden.

5. **SHAP = advies, geen bevel** (30 sec) — *"SHAP zegt waar de meest verdachte sensor zit. Maar JIJ kijkt nog steeds zelf. Klopt het met wat je hoort/voelt? Bij conflict — jouw oordeel telt. Schrijf op voor het team."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 9-10
- [ ] diagram-lo-smart-mfg-108.svg (op slide 9)
- [ ] Flap-over (drie leesregels)

> **Tips voor de trainer:**
> - Houd het strict bij groot/rood/blauw. Geen 'feature importance', geen 'SHAP values'.
> - Lees de voorbeeldgrafiek hardop voor — dat is het demonstratiemodel voor fase 4.
> - Bij vraag 'wat staat SHAP voor?': 'Komt uit een formule, hoef je niet te onthouden. SHAP = grafiekje dat AI-uitleg geeft.'

> **Valkuil — SHAP klinkt te wiskundig:**
> Vermijd afkorting. Bij vraag: 'het is een grafiekje, naam komt uit formule, hoef je niet te onthouden.'

> **Valkuil — operator vertrouwt SHAP blind:**
> Maak expliciet: SHAP = advies. Jij vergelijkt met machine. Bij conflict: jij wint.

> **Differentiatie:**
> - **MBO-3 basis:** drie leesregels op flap-over zichtbaar tijdens hele rest van sessie.
> - **MBO-4 sneller:** noem feature importance kort. Bron Lundberg & Lee (2017).

---

### Blok 4: Drie nieuwe SHAP-grafieken — actie
**00:23 - 00:30** | 7 min | Kolb-fase: experimenteren

**Doel:** Deelnemer past de drie leesregels zelfstandig toe op nieuwe grafieken en formuleert een actie.

**Werkvorm:** Individuele oefening + duo-bespreking, werkblad wb-04-experimenteren.

**Instructie:**

1. **Werkblad uitdelen + introductie** (30 sec) — deel wb-04 uit. Toon slide 11 (drie SHAP-grafieken). Zeg: *"Drie nieuwe grafieken. Per grafiek: welke sensor controleer je als eerste, en waarom? Doe minimaal 1, twee is mooi, drie is bonus."*

2. **Individueel werken** (4 min) — zet timer op 4 min. Loop rond. Help met de drie leesregels:
    - *"Welke balk is het grootst?"*
    - *"Welke kleur — rood of blauw?"*
    - *"Wat betekent dat? Te hoog of te laag?"*
    Geef directe feedback bij vragen.

3. **Duo-bespreking** (1 min 30) — *"Bespreek met je buurman één grafiek waarover je twijfelde. Waar koos je voor en waarom?"*

4. **Plenaire afsluiting** (1 min) — vraag 1-2 deelnemers om hun keuze toe te lichten op één grafiek. Bevestig met de drie leesregels.

5. **Transferopdracht** (30 sec) — toon slide 12. *"Deze week: vraag bij een storingsmelding aan je leidinggevende of er een SHAP-grafiek beschikbaar is. Bekijk hem samen. Maak een foto, noteer welke sensor bovenaan stond. Volgende sessie: van anomaliescore naar werkorder — LO-205."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 11-13
- [ ] Timer

> **Tips voor de trainer:**
> - Kwaliteit boven snelheid. Eén grafiek goed gelezen is meer waard dan drie haastig.
> - Bij twijfel-grafiek: laat duo's eerst bespreken voor je plenair antwoordt.
> - Bewaar 30 sec voor de transferopdracht.

> **Differentiatie:**
> - **MBO-3 basis:** 1-2 grafieken is genoeg.
> - **MBO-4 sneller:** vraag *"Wat als twee sensoren een dubbele oorzaak hebben? Welke check je eerst?"*

> **Valkuil — drie grafieken is te veel:**
> Geef expliciet ruimte: minimaal 1. Stuur op kwaliteit.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 dubbelzijdig (drie grafieken) |
| ☐ | Pennen | n + 5 | |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (drie leesregels) | 1 vel | Vooraf voorbereid |
| ☐ | Beamer + GROOT scherm | 1 set | Verplicht — grafieken moeten leesbaar zijn |
| ☐ | Timer | 1 | Met geluid |
| ☐ | presentatie.slidev.md geopend | 1 | |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 5 anomaliemeldingen — raden | Pijn van 'zonder uitleg-AI raad ik fout' |
| 2 reflecteren | Hoe doe je het nu? | Eigen strategie zichtbaar + behoefte aan ondersteuning |
| 3 theoretiseren | Drie leesregels SHAP | Grafiek lezen op kapstok-niveau |
| 4 experimenteren | 3 nieuwe grafieken — actie | Zelfstandig SHAP-gebruik |

**Slagingscriterium:** Drie leesregels kunnen toepassen op één SHAP-grafiek + actie noemen.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd
- [ ] Quiz-scores genoteerd (gemiddelde — voor / na — leerwinst)
- [ ] Wie raadde 4-5 goed? (kandidaat voor module 3)
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `completed` (drie leesregels), `attempted` (oefening)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | LO-108 SHAP*
*Bron: Lundberg & Lee (2017). A Unified Approach to Interpreting Model Predictions. | Molnar (2022). Interpretable Machine Learning.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
