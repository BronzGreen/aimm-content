# Classificatie — etiket plus zekerheid — Draaiboek
*AI Fundamentals Module 1 (Gebruik) | Workshop-blok 40 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan uitleggen wat classificatie is, het onderscheid maken tussen binair en multi-class, het zekerheidspercentage correct interpreteren en bij een twijfelgeval (60/40) een gemotiveerde handelwijze beschrijven. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | ko-ai-fund-131 (supervised learning) doorlopen — weet dat AI van voorbeelden leert |
| **Stadium (H&B)** | Bewust onbekwaam — heeft AI-uitslagen gezien, mist taal voor klasse/zekerheid |
| **Begeleidingsstijl** | Instrueren — sturend met ruimte voor eigen oordeel bij twijfelgevallen |
| **Ruimte** | U-opstelling of clusters van 4, beamer met goede beeldkwaliteit, flip-over |
| **Plek in module** | AI Fundamentals Module 1 (Gebruik) — eerste hands-on confrontatie met AI-output op de werkvloer |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | IK DOE — Binair voorbeeld (CNC-onderdeel) | ervaren | 8 min |
| 00:08 - 00:18 | WIJ DOEN — Multi-class in duo's | ervaren | 10 min |
| 00:18 - 00:28 | Handout: binair vs multi-class + zekerheid | theoretiseren | 10 min |
| 00:28 - 00:40 | JIJ DOET — Twijfelgeval 60/40 | experimenteren | 12 min |

**Totaal:** 40 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 3 (percentage-misinterpretatie) of fase 4 (plenaire afsluiting).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve. Let op: wb-02 is per DUO.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Test de foto-kwaliteit op de beamer: het CNC-onderdeel + 4 multi-class voorbeelden moeten herkenbaar zijn vanaf de achterste rij.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst"**, rechts **"Classificatie"** met 4 lege rijen (classificatie / binair / multi-class / zekerheid).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02 (per duo), wb-03 en wb-04 (per deelnemer) apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: IK DOE — Binair voorbeeld
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer ziet hoe een classificatie-uitkomst eruitziet (klasse + zekerheidspercentage) en herkent dat de output een ETIKET is, geen getal.

**Werkvorm:** Trainer demonstreert hardop denken (IK DOE). Deelnemers kijken mee, noteren in één zin.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 40 minuten kijken we naar classificatie — wat het systeem op je scherm eigenlijk zegt als het 'goed' of 'afgekeurd' meldt. En vooral: wat je doet als het systeem twijfelt."*

2. **Trigger** (1 min) — toon slide 2. Vertel: *"Op steeds meer werkvloeren staat een camera of sensor. Goed of afgekeurd. Kras of barst. Het scherm geeft een uitslag — maar wat staat daar nou eigenlijk? Daar gaan we vandaag een mentaal model voor bouwen."*

3. **Deel wb-01 uit + toon foto** (1 min) — toon slide 3. Op het scherm: een CNC-gefreesd metalen plaatje met een lichte braam aan de rand. Daarnaast de modeluitvoer: *"Klasse: braam gedetecteerd — zekerheid 92%"*. *"Hier op het werkblad is ruimte voor één zin. Niets meer."*

4. **IK DOE — hardop denken** (4 min) — denk uit, langzaam:
    - *"Wat zie ik? Een metalen plaatje, lichte braam aan de rand. Herkenbaar werk."*
    - *"Wat geeft het model terug? Niet een getal — een ETIKET. Het zegt: dit is een braam. Een woord, een categorie."*
    - *"Wat betekent dat percentage erbij? Het model is voor 92% zeker dat dit een braam is. Hoge zekerheid."*
    - *"Wat zou ik als operator doen? Bij 92% kan ik de uitslag bijna altijd volgen. Bij lage zekerheid — bijvoorbeeld 60% — moet ik zelf kijken. Daar komen we straks bij."*
    - *"Twee opties hier — goed of braam. Twee klassen. Dat heet BINAIR. Schrijf dat op je werkblad."*

5. **Notitievraag** (1 min) — *"Schrijf in één zin op wat dit model teruggeeft. Een getal of een etiket?"* Wacht 1 minuut. Geen plenair antwoord vragen — dat komt in fase 3.

**Materiaal:**
- [ ] Slides 1-3
- [ ] wb-01-binair-voorbeeld (1 per deelnemer)
- [ ] Foto CNC-onderdeel + modeluitvoer op scherm
- [ ] Pen

> **Tips voor de trainer:**
> - Tempo bij hardop denken — langzaam, ruimte voor mee-denken.
> - Maak het verschil tussen 'klasse' en 'percentage' expliciet — twee componenten.
> - Vermijd jargon (logit, softmax) — alleen 'klasse + zekerheid'.

> **Valkuil — '92% van het product is braam':**
> Iemand interpreteert het percentage als product-eigenschap. Niet hier al adresseren — bewaar het voor fase 3 (handout-uitleg). Hier alleen: 'het is hoe zeker het model is van zijn antwoord'.

> **Valkuil — 'binair' overslaan:**
> Verleidelijk om de term niet uit te spreken. Doe het wel — dat is het contrast met 'multi-class' in fase 2.

> **Differentiatie:**
> - **MBO-4 basis:** Gebruik concreet voorbeeld dat aansluit (CNC-frees met braam is universeel herkenbaar). Indien beschikbaar: foto van de eigen werkvloer.
> - **Teamleider sneller:** Vraag bij notitie: 'wat zou jij doen als de zekerheid 50% was?' Bewaring voor fase 4.

**Transitie naar volgende blok:** *"Nu zelf — vier foto's met meerdere klassen. In duo's."*

---

### Blok 2: WIJ DOEN — Multi-class herkenning in tweetallen
**00:08 - 00:18** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer herkent dat een classificatiemodel ook MEER dan twee klassen kan hebben (multi-class), en identificeert het onderdeel met de laagste zekerheid.

**Werkvorm:** Tweetallen — WIJ DOEN. Bespreken vier foto's met modeluitvoer.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Eén per duo. Toon slide 4. *"In duo's. Vier foto's van afgekeurde onderdelen. Bij elke foto staat een modeluitvoer: klasse + zekerheid."*

2. **Toon modeluitvoer** (30 sec) — *"Foto 1 — kras, zekerheid 78%. Foto 2 — barst, zekerheid 85%. Foto 3 — kleurfout, zekerheid 91%. Foto 4 — vormafwijking, zekerheid 66%."*

   *"Bespreek met je buurman: wat is de output bij elke foto — een klasse of een getal? Welke heeft de laagste zekerheid? Wat zou je daarmee doen?"*

3. **Tweetallen werken** (6 min) — zet timer op 6 min. Loop rond. Stel vragen — geen antwoord:
    - *"Hoeveel verschillende klassen ziet dit model?"*
    - *"Hoe heet dat — meer dan twee?"*
    - *"Welke heeft de laagste zekerheid? Wat zou jij daarmee doen?"*

4. **Plenair benoemen** (3 min) — toon slide 5. Vraag: *"Hoeveel klassen ziet dit model?"* Wacht 5-7 sec. Als iemand 'vier' zegt: *"Klopt — vier klassen. Meer dan twee. Dat heet MULTI-CLASS. Schrijf op het werkblad."* Schrijf op flip-over: 'multi-class = MEER DAN TWEE'.

   *"Welke foto heeft de laagste zekerheid? Foto 4, vormafwijking, 66%. Wat zou jij daarmee doen?"* Vang 2 antwoorden — niet bespreken, brug naar fase 3.

**Materiaal:**
- [ ] Slides 4-5
- [ ] wb-02-multi-class (1 per duo)
- [ ] Foto's 4 multi-class voorbeelden op scherm
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag.
> - Laat de term 'multi-class' bottom-up komen — eerst tellen, dan benoemen.
> - Bij rond-lopen: noteer welke duo's automatisch over 'zekerheid' beginnen — gebruik dat in plenair.

> **Valkuil — term multi-class te snel introduceren:**
> Niet zelf zeggen 'dit is multi-class' bij het uitdelen. Laat de groep zelf het aantal klassen tellen — dan landt de term.

> **Valkuil — alleen op hoge zekerheid focussen:**
> Foto 3 (91%) is makkelijk. Foto 4 (66%) is de leerstof. Daar gaat het straks om bij het twijfelgeval.

> **Differentiatie:**
> - **MBO-4 basis:** Bij duo's: zet operator + operator als groep — gemakkelijker zelfde taal.
> - **Gemengde groep:** Operator + teamleider — operator brengt kijken, teamleider de afweging.

**Transitie naar volgende blok:** *"Nu de theorie op een rij — binair, multi-class, en wat dat percentage eigenlijk betekent."*

---

### Blok 3: Plenair — binair vs multi-class + zekerheid
**00:18 - 00:28** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer plaatst het verschil binair/multi-class in een framework en begrijpt de juiste interpretatie van het zekerheidspercentage.

**Werkvorm:** Trainer-geleide handout (WIJ DOEN).

**Instructie:**

1. **Deel wb-03 uit** (30 sec). *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **Classificatie samenvatten** (2 min) — toon slide 6. *"Classificatie is een AI-taak waarbij het model een ETIKET plakt op iets. Een woord, een categorie. Geen getal."* Schrijf op flip-over: 'classificatie = ETIKET'. *"Twee smaken: binair (twee opties) en multi-class (meer dan twee)."*

3. **Binair vs multi-class** (2 min) — toon slide 7. *"Binair: goed/afgekeurd, OK/NOK, aan/uit. Twee klassen. Multi-class: kras/barst/kleurfout/vormafwijking. Drie of meer klassen. Allebei werken hetzelfde — het model krijgt iets, geeft een etiket terug."*

4. **Zekerheid — de valkuil** (4 min) — toon slide 8. *"Bij elk etiket hoort een zekerheid."* Schrijf op het bord of flip-over: *"Klasse: braam — zekerheid 92%."* Vraag: *"Wat betekent dat percentage?"* Wacht 5-7 sec.

   Vang antwoorden. Maak dan expliciet: *"Hier zit een valkuil. Die 92% zegt NIET dat 92% van het product een braam is. Het zegt: het model is voor 92% zeker dat dit een braam is. Het gaat over het vertrouwen van het model in zijn eigen antwoord — niet over de eigenschap van het product."*

   *"Vergelijk: stel je hebt een collega die langs de band loopt en bij een onderdeel zegt 'ik denk dat het een kras is, maar ik twijfel een beetje'. Die twijfel — dat is wat het percentage uitdrukt. Hoge zekerheid = weinig twijfel. Lage zekerheid = veel twijfel."*

   *"Bij hoge zekerheid (boven 90%) kun je de uitslag bijna altijd volgen. Bij lage zekerheid wordt het interessant — daar komt de operator in beeld."*

5. **Onderscheid met regressie** (1 min) — toon slide 9. *"Belangrijk: classificatie geeft een KLASSE — een woord. Er bestaat ook AI die een GETAL voorspelt — bijvoorbeeld 'deze machine gaat over 23 dagen stuk'. Dat heet regressie. Vuistregel: woord = classificatie, getal = regressie. Regressie komt in een volgend leerobject."*

6. **Brug naar fase 4** (30 sec) — *"Nu een twijfelgeval. Wat doe jij als het model zelf twijfelt?"*

**Materiaal:**
- [ ] Slides 6-9
- [ ] wb-03-handout-classificatie
- [ ] Markeerstift per deelnemer
- [ ] Flip-over

> **Tips voor de trainer:**
> - De percentage-misinterpretatie is HET kernpunt — neem er tijd voor.
> - Gebruik de collega-vergelijking — die maakt het tastbaar.
> - Vermijd technisch jargon (softmax, logits) — 'zekerheid van het model' is genoeg.

> **Valkuil — percentage-uitleg doorrazen:**
> Verleidelijk om snel door te gaan. Niet doen — juist hier struikelen deelnemers op de werkvloer.

> **Valkuil — '90% is altijd te vertrouwen' als regel:**
> Niet als regel stellen. Wel: 'bij hoge zekerheid kun je BIJNA altijd volgen — maar context bepaalt'. Drempels staan ter discussie in fase 4.

> **Differentiatie:**
> - **MBO-4 basis:** Eén steekzin per begrip op flip-over.
> - **Teamleider sneller:** Vraag: 'kan een model ook drie klassen tegelijk geven, met percentages die samen 100% zijn?' Antwoord: ja — bij multi-class met softmax. Bij 60/40-twijfel zie je het model verdeeld tussen twee opties.

**Transitie naar volgende blok:** *"Nu jouw werkblad — een twijfelgeval. Twaalf minuten."*

---

### Blok 4: JIJ DOET — Twijfelgeval 60/40
**00:28 - 00:40** | 12 min | Kolb-fase: experimenteren

**Doel:** Deelnemer past het mentale model toe op een 60/40-twijfelgeval, beantwoordt drie vragen, formuleert in eigen woorden wat een operator doet bij lage zekerheid.

**Werkvorm:** Individueel werkblad (JIJ DOET) — plenaire afsluiting.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Toon slide 10. *"Laatste 12 minuten. Een metalen frame. Het model zegt: klasse goed — zekerheid 60%. Klasse vormafwijking — zekerheid 40%. Drie vragen op het werkblad."*

2. **Drie vragen toelichten** (1 min) — toon slide 11. *"(1) Wat zegt dit model eigenlijk? (2) Wat zou jij doen — doorlaten, handmatig nakijken, of de instelling van het systeem aanpassen? (3) Wanneer is een zekerheid 'hoog genoeg' voor jouw lijn?"*

3. **Individueel werken** (7 min) — zet timer op 7 min. Loop rond. Stel vragen — geen antwoord:
    - *"Hoe zeker moet een model zijn voor jij het vertrouwt?"*
    - *"Is dit een veiligheidscomponent of iets minder kritisch?"*
    - *"Wat kost een doorgelaten fout in jullie productie?"*
    Bij vastloper: stel ÉÉN hulpvraag, niet drie tegelijk.

4. **Plenaire afsluiting** (3 min) — toon slide 12. Vraag 2-3 deelnemers: *"Wat zou jij doen?"* Verzamel verschillende antwoorden. Maak dan expliciet:
    - *"Doorlaten kan — als de fout-kosten laag zijn. Sierdeel met een mogelijke vormafwijking — soms doorlaatbaar."*
    - *"Handmatig nakijken is bijna altijd de veilige keuze. Vooral bij veiligheid of dure onderdelen. Bij twijfel: kijken."*
    - *"Instelling aanpassen is een gesprek met de teamleider — past de drempel voor 'afgekeurd' bij deze lijn? Vooral als veel grensgevallen op dezelfde drempel zitten."*

5. **Belangrijke conclusie** (30 sec) — *"Er bestaat GEEN vast getal voor 'hoog genoeg'. Het hangt af van wat een fout kost. Een doorgelaten kras op een sierdeel is iets anders dan op een remblok. Jouw kennis van de lijn maakt hier het verschil. Dat is precies waarom operators in beeld blijven."*

6. **Transferopdracht** (30 sec) — toon slide 13. *"Deze week: kijk eenmaal langs het kwaliteits- of inspectiesysteem op je lijn. Drie dingen noteren: welk type classificatie (binair of multi-class), welke klassen het systeem kent, en de laagste zekerheid die je tegenkomt. Vraag ook aan een collega 'wat doe jij als het systeem twijfelt?' — vaak hanteert iedereen een eigen huisregel."*

**Materiaal:**
- [ ] Slides 10-13
- [ ] wb-04-twijfelgeval
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij vastloper: stel de hulpvragen één voor één, niet allemaal tegelijk.
> - Plenaire ronde mag verschillende antwoorden tonen — dat is het inzicht.
> - De afsluiting moet expliciet zeggen: GEEN vast getal — context bepaalt.

> **Valkuil — zelf een 'juist antwoord' geven:**
> Er is geen één juist antwoord op de 60/40-casus. Drie opties zijn alle drie legitiem. Het inzicht is de afweging — niet één regel.

> **Valkuil — afsluiting opslokken:**
> Als blok 3 is uitgelopen: kort het individueel werken in tot 5 min, plenair tot 2 min. Sla de transferopdracht nooit over.

> **Differentiatie:**
> - **MBO-4 basis:** Eén handelwijze + gemotiveerd is genoeg. Niet alle drie hoeven afgewogen.
> - **Teamleider sneller:** Vraag ook: 'wat zou JIJ met je team afspreken over twijfelgevallen?' Stimulus voor teamafspraak.

**Transitie naar afsluiting:** Niet van toepassing — einde sessie.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-binair-voorbeeld | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-multi-class | n/2 + 2 | A4 dubbelzijdig, per duo |
| ☐ | wb-03-handout-classificatie | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-twijfelgeval | n + 2 | A4 enkelzijdig |
| ☐ | Foto's op beamer | 1 set | CNC-onderdeel + 4 multi-class — vooraf testen |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 1 | Parkeerlijst + 4 begrippen-overzicht |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 6/7-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen, beeldkwaliteit cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Flexibiliteit — als het anders loopt

- **Als blok 1 uitloopt:** kort de notitievraag in tot 30 sec, ga direct door. De IK DOE-demonstratie zelf is essentieel.
- **Als blok 2 uitloopt:** kort plenair benoemen in tot 2 min — focus alleen op 'hoeveel klassen' en 'welke heeft laagste zekerheid'.
- **Als blok 3 uitloopt:** sla het onderscheid met regressie over (terugkomende in een volgend LO) en koppel direct naar fase 4. De percentage-uitleg is het hart.
- **Als blok 4 uitloopt:** individueel werken tot 5 min, plenair tot 2 min, transferopdracht in 30 sec. Nooit afsluiting overslaan.
- **Als de groep te klein is (< 6):** geen duo's in fase 2, ga direct plenair na 5 min individueel.
- **Als de groep te groot is (> 12):** verdeel in twee subgroepen tijdens fase 2 en kort plenair in tot 2 min.
- **Als de beamer-beeldkwaliteit slecht is:** print de 4 multi-class foto's vooraf op A4 en geef per duo een set. Onmisbaar — foto's moeten herkenbaar zijn.

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren (IK DOE) | Binair voorbeeld voordoen | Begrip: classificatie = klasse + zekerheid |
| 2 ervaren (WIJ DOEN) | Multi-class in duo's | Term 'multi-class' bottom-up verworven |
| 3 theoretiseren | Handout + percentage-uitleg | Inzicht: zekerheid = vertrouwen MODEL, niet product |
| 4 experimenteren (JIJ DOET) | Twijfelgeval 60/40 + plenaire afsluiting | Handelwijze gemotiveerd vanuit context |

**Slagingscriterium:** classificatie als 'klasse + zekerheid' kunnen uitleggen + onderscheid binair/multi-class + redelijke handelwijze bij twijfelgeval gemotiveerd.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met 4 begrippen-overzicht gefotografeerd
- [ ] Genoteerd: hoeveel deelnemers interpreteerden het percentage eerst als product-eigenschap?
- [ ] Notitie voor volgende sessie: welke twijfelgevallen zijn aangekondigd? Welke huisregels in de groep?
- [ ] xAPI-statements verstuurd: `experienced` (binair + multi-class), `completed` (handout), `attempted` (twijfelgeval + transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 1 (Gebruik) | Classificatie — etiket plus zekerheid*
*Bronnen: Russell & Norvig (2021) AI: A Modern Approach. | Goodfellow et al. (2016) Deep Learning. | Manufacturing-ML uitlegmateriaal 2024-2025.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
