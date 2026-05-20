# Overfitting — wanneer 99% een alarmbel is — Draaiboek
*AI Fundamentals Module 1 (Gebruik) | Workshop-blok 42 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer herkent overfitting aan het verschil tussen training-score en productie-score. Benoemt drie signalen en drie tegenmaatregelen. Formuleert een gefundeerde vraag aan een AI-leverancier over het scoreverschil. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Eerste kennismaking met AI/ML; weet dat een model uit trainingsdata leert (idealiter lo-132 voltooid) |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat AI uit data leert, mist begrip van generalisatie |
| **Begeleidingsstijl** | Instrueren — sturend op concept, ervaringsgericht startend |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | AI Fundamentals Module 1 (Gebruik) — na trainingsdata (lo-132) en classificatie (lo-133) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | Twee scorekaarten naast elkaar | ervaren | 10 min |
| 00:10 - 00:20 | Duo-bespreking + term overfitting | reflecteren | 10 min |
| 00:20 - 00:32 | Handout: 3 signalen + 3 tegenmaatregelen | theoretiseren | 12 min |
| 00:32 - 00:42 | Diagnose op 3 nieuwe scorekaarten | experimenteren | 10 min |

**Totaal:** 42 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (twijfel over Model A) of fase 3 (cross-validatie-uitleg).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve per stuk. **Of** kies digitaal voor wb-04: laad `model-overfitting-sliders.jsx` op een React-sandbox en test op één tablet.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer (HDMI + audio).
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `OverfittingVideo`, ~90s) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Plan inzet aan begin fase 1 (stop NA scene 2 om 'overfitting' bottom-up te bewaren).
- [ ] Bereid stemkaartjes voor: 2 kleuren (rood = Model A, blauw = Model B). Eén set per deelnemer.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst"**, rechts **"Overfitting"** met 6 lege rijen (drie signalen + drie tegenmaatregelen).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01, set stemkaartjes.
- [ ] Houd wb-02, wb-03 en wb-04 apart op de trainertafel — gefaseerd uitdelen.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Twee scorekaarten naast elkaar
**00:00 - 00:10** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer ondervindt dat een hoog piek-getal (99%) niet automatisch een beter model is. Kiest een model en formuleert één zin met de reden.

**Werkvorm:** Trainer toont Model A (IK DOE), daarna Model B. Deelnemers kiezen individueel.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 42 minuten kijken we naar het belangrijkste alarmbel-signaal in AI — overfitting. Tegen het eind ken je de drie signalen, drie tegenmaatregelen, en de vraag die je voortaan aan elke leverancier stelt."*

2. **Trigger — een leveranciersclaim** (1 min) — toon slide 2. Vertel: *"Een leverancier komt langs en zegt 'ons model is 99% nauwkeurig'. Klinkt geweldig. Maar wat zegt dat eigenlijk? Tegen het eind van deze sessie kun je daarop een betere vraag stellen."*

2b. **Optioneel — toon de video** (1 min 30) — als je in tempo zit en visueel-ingestelde deelnemers hebt, toon `video/composition.tsx` (export id `OverfittingVideo`, ~90s) op de beamer. Pauzeer of stop NA scene 2 (divergerende curves). Zeg: *"Twee curves. Een blijft stijgen, de ander zakt. Wat zien jullie hier gebeuren?"* GEEN antwoord geven en GEEN term 'overfitting' noemen — laat het beeld doorwerken. Direct door naar wb-01.

3. **Deel wb-01 uit + Model A tonen** (2 min) — wb-01 uit. Toon slide 3 — Model A:
    - Training-score: **99%**
    - Score op een nieuwe machine: **60%**

    Denk hardop (IK DOE): *"99% klinkt geweldig. Maar kijk hier — op een andere machine zakt het naar 60%. Wat zegt dat?"* Pauze. GEEN antwoord geven.

4. **Model B tonen** (1 min) — toon slide 4 — Model B:
    - Training-score: **88%**
    - Score op een nieuwe machine: **86%**

    Vraag: *"Welke vertrouw je? En waarom?"* Stilte 5-7 sec. Geen aanwijzing.

5. **Individueel kiezen + reden noteren** (4 min) — zet timer op 4 min. Loop rond. Stel verdiepende vragen — geen hint:
    - *"Wat valt je op?"*
    - *"Welk getal vertel je aan je teamleider?"*
    - *"Wat zou je willen weten voor je kiest?"*

6. **Tussenstand** (1 min) — vraag: *"Wie heeft gekozen? Wie twijfelt nog?"* Bevestig dat schuren mag. *"Twijfel is precies wat we in fase 2 plenair uitwerken."*

**Materiaal:**
- [ ] Slides 1-4
- [ ] wb-01-scorekaarten (1 per deelnemer)
- [ ] Timer
- [ ] Pen
- [ ] Stemkaartjes klaar voor fase 2
- [ ] Optioneel: `video/composition.tsx` (Remotion `OverfittingVideo`, ~90s) — pre-rendered MP4 of live preview

> **Tips voor de trainer:**
> - Tempo bij IK DOE — langzaam, getallen apart benoemen.
> - Bij vastloper: open vraag, geen hint.
> - Geef GEEN oordeel — een keuze voor Model A is een legitieme leerstof.

> **Valkuil — term overfitting in fase 1:**
> Verleidelijk om in fase 1 al te zeggen 'Model A toont overfitting'. Niet doen. Bewaar tot fase 2 plenair — eerst moet de groep zelf onder woorden brengen wat er scheef zit.

> **Valkuil — hint geven:**
> 'Kijk eens naar het verschil' is al een hint. Beter: 'wat valt je op?'. Laat de groep zelf wringen met de getallen.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de getallen-paren ook op flip-over, niet alleen op slide. Visueel anker.
> - **Teamleider sneller:** Vraag bij snel klaar: 'wat zou je aan de leverancier vragen voor je kiest?' Voorbereiding op transferopdracht.

**Transitie naar volgende blok:** *"Nu met je buurman — wat verraadt het verschil?"*

---

### Blok 2: Duo-bespreking + introductie term overfitting
**00:10 - 00:20** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander en herkent dat het scoreverschil het signaal is. De term overfitting wordt geïntroduceerd.

**Werkvorm:** 5 minuten in tweetallen — daarna plenaire stemming + benoemen + term introduceren.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Zeg: *"Tweetal met je buurman. Vergelijk je keuze en je reden. Welk getal of welk verschil verraadt voor jullie wat hier scheef zit?"*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Verzamel 2-3 sterke redenen voor plenair. Tel innerlijk tot 7 voor je iemand bijstuurt.

3. **Plenaire stemming** (1 min) — toon slide 5. *"Steek de kleur omhoog van het model dat jij zou vertrouwen: rood = Model A, blauw = Model B."* Tel hardop, schrijf uitslag op flip-over.

4. **Plenair benoemen** (3 min) — toon slide 6. Vraag eerst een duo dat voor A koos: *"Wat overtuigde jullie?"* Wacht 5-7 sec. Daarna een duo dat voor B koos.

   *"Wat verraadt het verschil tussen 99% en 60%? Het MODEL heeft de trainingsdata uit het hoofd geleerd in plaats van het patroon. Op nieuwe data valt het stil. Dat heet OVERFITTING — te-goed-leren."*

   Schrijf op flip-over: *"Overfitting = voorbeelden onthouden, niet patroon zien"*.

   Vergelijking: *"Stel een nieuwe collega heeft tien producten op één machine gezien. Herkent die feilloos. Zet hem op een ander machinetype — hij staat stil. Voorbeelden onthouden, geen patroon door. Dat is precies wat overfitting is."*

5. **Brug naar fase 3** (30 sec) — *"Drie signalen om dit te herkennen, drie dingen die je eraan kunt doen."*

**Materiaal:**
- [ ] Slides 5-6
- [ ] wb-02-reflectie
- [ ] Stemkaartjes (2 kleuren per deelnemer)
- [ ] Flip-over voor stemmingsuitslag
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag.
> - Bij stilte tijdens stemming: noem zelf 'wie heeft Model A?' om ijs te breken.
> - Bevestig keuze voor A zonder oordeel — leerstof, geen falen.

> **Valkuil — term overfitting te vroeg:**
> Wacht tot na de plenaire stemming. Eerst de groep zelf laten benoemen wat scheef is — dan landt de term als BENOEMING van wat ze al voelden.

> **Valkuil — direct het antwoord geven:**
> 'B is duidelijk de winnaar' werkt niet — de groep moet eerst zelf wringen. Pas na 2-3 duo-antwoorden samenvattend.

> **Valkuil — collega-vergelijking overslaan:**
> Die maakt overfitting tastbaar voor MBO-4. Niet weglaten — de abstracte term landt anders niet.

> **Differentiatie:**
> - **Gemengde groep:** Bij duo's: combineer operator (kent eigen data) met teamleider (kent leverancier-claims). Verschillende invalshoeken op hetzelfde verschil.

**Transitie naar volgende blok:** *"Drie signalen + drie tegenmaatregelen — daar gaan we het nu rechte over hebben."*

---

### Blok 3: Handout — drie signalen en drie tegenmaatregelen
**00:20 - 00:32** | 12 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer plaatst de scorekaart-ervaring in een gestructureerd framework: drie signalen voor herkenning + drie tegenmaatregelen.

**Werkvorm:** Trainer-geleide handout-bespreking (WIJ DOEN) met directe verbinding naar Model A/B.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **Drie signalen introduceren** (1 min) — toon slide 7. *"Drie dingen waaraan je overfitting herkent. Niet één — alle drie samen bouwen het verhaal."*

3. **Loop de drie signalen af** (5 min) — toon slide 8:

    - **Signaal 1: Groot scoreverschil** (2 min). *"Training 99% → nieuwe machine 60%. Verschil 39 punten. Bij Model B: 88% → 86%. Verschil 2 punten. Het VERSCHIL is het signaal — niet de hoogte. Een leverancier die alleen één getal noemt, is verdacht."* Schrijf op flip-over.

    - **Signaal 2: Klein dataset met complex model** (1 min 30). *"50 trillings-voorbeelden van één machine, getraind met een ingewikkeld neuraal netwerk. Het model heeft te veel ruimte om voorbeelden te onthouden in plaats van het patroon te leren."* Schrijf op flip-over.

    - **Signaal 3: Faalt op nieuwe machine of batch** (1 min 30). *"Wat in het lab werkte, werkt niet op de werkvloer. Wat bij de leverancier werkt, faalt bij jullie. Het showroom-effect."* Schrijf op flip-over.

4. **Drie tegenmaatregelen introduceren** (1 min) — toon slide 9. *"Drie dingen die helpen."*

5. **Loop de drie tegenmaatregelen af** (4 min) — toon slide 10:

    - **Tegenmaatregel 1: Meer voorbeelden** (1 min 30). *"Niet alleen meer foto's — meer DIVERSE voorbeelden. Variatie zoals we in trainingsdata-LO zagen: meer ploegen, machines, situaties. In het voorbeeld uit Russell & Norvig 2021: 50 voorbeelden van één machine → toegevoegd 5 machines → score op nieuwe machines steeg naar 90%."* Schrijf op flip-over.

    - **Tegenmaatregel 2: Simpeler model** (1 min). *"Minder complexiteit kan minder ruis vasthouden. Soms is een eenvoudiger algoritme robuuster. Niet altijd de mooiste oplossing — wel vaak de meest werkbare."* Schrijf op flip-over.

    - **Tegenmaatregel 3: Cross-validatie** (1 min 30). *"Test het model herhaald op data die het NIET tijdens training zag. Verdeel je dataset in stukken, train op een deel, test op een ander deel. Standaard onderdeel van professioneel AI-werk — vraag de leverancier hoe zij dit doen."* Schrijf op flip-over.

6. **Praktische realiteit** (1 min) — toon slide 11. *"Leveranciers tonen vaak één hoog getal. Jouw rol als operator: vraag door naar het verschil. Showroom-modellen op één machine zijn vaak overfitted. Het herkennen van dit patroon is een vaardigheid die jaren ervaring bespaart."*

7. **Brug naar fase 4** (30 sec) — *"Nu drie nieuwe scenario's. Jij beoordeelt."*

**Materiaal:**
- [ ] Slides 7-11
- [ ] wb-03-handout-overfitting
- [ ] Markeerstift per deelnemer
- [ ] Flip-over

> **Tips voor de trainer:**
> - Verbind elk signaal expliciet aan Model A/B — die zijn de geleefde ervaring.
> - Bij tegenmaatregel 1: leg het verband met lo-132 (diversiteit) — meer ploegen, meer machines.
> - Geef ruimte voor vragen — vooral cross-validatie kan vragen oproepen.

> **Valkuil — doorrazen door de drie signalen:**
> Laat elke signaal landen voor de volgende. Met name signaal 2 (klein dataset + complex model) is vaak nieuw — niet als bijzin behandelen.

> **Valkuil — 'meer data lost alles op':**
> Preciseer: meer DIVERSE data. Meer foto's van dezelfde lijn helpt niet. Verband leggen met lo-132.

> **Valkuil — cross-validatie als 'technisch detail' wegwuiven:**
> Het is precies de vraag die de operator aan de leverancier kan stellen — 'hoe heeft u cross-validatie gedaan?'. Concrete handelingsperspectief.

> **Differentiatie:**
> - **MBO-4 basis:** 3 signalen + 3 tegenmaatregelen letterlijk overschrijven op flip-over voor visueel anker.
> - **Teamleider sneller:** Vraag: 'welke tegenmaatregel is bij jullie het makkelijkst toepasbaar?' Voorbereiding op fase 4.

**Transitie naar volgende blok:** *"Nu drie scenario's op het werkblad. Je krijgt 6 minuten."*

---

### Blok 4: Diagnose op drie scorekaarten + transferopdracht
**00:32 - 00:42** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer past het framework toe op drie nieuwe mini-scorekaarten: is dit overfitting (ja/nee/twijfel) en welke tegenmaatregel. Sluit af met transferopdracht aan leverancier.

**Werkvorm:** Individueel werkblad (JIJ DOET) — kort plenair vergelijken.

**Instructie:**

1. **Deel wb-04 uit** (30 sec) — **OF** deel tablets uit met `model-overfitting-sliders.jsx` geopend. Toon slide 12. Zeg bij papier: *"Laatste 10 minuten. Drie nieuwe scorekaarten. Per scenario: is dit overfitting? Welke tegenmaatregel zou jij voorstellen? Twijfel mag — vraagteken is een geldig antwoord."* Zeg bij digitaal: *"Twee sliders — complexiteit en data-omvang. Probeer minimaal drie verschillende combinaties uit. Per combinatie zie je live de curves voor trainings-fout en productie-fout, en de diagnose: onder-fit, goed-getraind, of over-fit. Onderzoek: wat verschuift het sweet-spot — meer data of minder complexiteit?"*

2. **Drie scenario's toelichten** (1 min) — toon slide 13:
    - **Scenario A:** Training 95% / test 92% — 200 voorbeelden van 4 machines. Verschil 3 punten.
    - **Scenario B:** Training 97% / test 65% — 30 voorbeelden van 1 machine. Verschil 32 punten.
    - **Scenario C:** Training 80% / test 78% — 500 voorbeelden van 2 machines. Verschil 2 punten.

3. **Individueel werken** (6 min) — zet timer op 6 min. Loop rond. Help bij twijfel met ÉÉN vraag: *"hoe groot is het verschil tussen leren en onbekende data?"* Bevestig dat twijfel een goed antwoord is.

4. **Kort plenair vergelijken** (2 min) — toon slide 14. Vraag per scenario: *"Wie zegt overfitting? Wie zegt nee? Wie twijfelt?"* Tel handen, geen lange bespreking. Maak per scenario kort de diagnose:
    - *"Scenario A — gezond. Verschil 3 punten, 200 voorbeelden over 4 machines. Generaliseert."*
    - *"Scenario B — overfitting. Verschil 32 punten, klein dataset, één machine. Tegenmaatregel: meer diverse voorbeelden."*
    - *"Scenario C — gezond ondanks lage score. Het model is gewoon niet zo goed, MAAR het scoreverschil is klein. Geen overfitting — wel het overwegen van een ander model."*

5. **Transferopdracht** (30 sec) — toon slide 15. *"Deze week: zoek één AI-systeem in jouw fabriek. Inspectiecamera, trillings-monitor, kwaliteitsclassificatie, voorspelmodel. Vraag aan de leverancier of IT drie dingen: op welke data is het model getraind — hoeveel voorbeelden, van welke machine? Op welke onbekende data is het getest? Wat is het verschil tussen die scores? Drie antwoorden meenemen naar de volgende sessie. Bonus: vraag een collega 'heb jij ooit gezien dat iets op één machine wel deed en op een nieuwe niet?' — vaak herkenbaar, alleen geen naam voor."*

**Materiaal:**
- [ ] Slides 12-15
- [ ] wb-04-diagnose (1 per deelnemer) **OF** tablets/laptops met `model-overfitting-sliders.jsx` geopend
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij twijfel: bevestig — dat is precies de gewenste kritische houding.
> - Bij 'we hebben geen AI op de lijn': hypothetisch ('stel...') mag.
> - Eindig op tijd — transferopdracht mag NIET wegvallen.

> **Valkuil — 'twijfel' afkeuren:**
> Als iemand bij een grensgeval (verschil 5-8 punten) 'twijfel' schrijft, is dat het juiste antwoord. Het signaal dat de operator zelf nadenkt in plaats van een regel toe te passen.

> **Valkuil — plenair vergelijken te lang:**
> 2 min is genoeg. Per scenario alleen tellen + kort diagnose. Geen lange bespreking, anders eet je de transferopdracht op.

> **Valkuil — scenario C overslaan:**
> Dat is precies het contra-intuïtieve geval: lage score maar geen overfitting. Operators leren hier dat overfitting niet hetzelfde is als 'slecht model'.

> **Differentiatie:**
> - **MBO-4 basis:** Eén scenario goed beoordeeld is genoeg, mits de overweging klopt. Niet alle drie hoeven beslist.
> - **Teamleider sneller:** Vraag bij snel klaar: 'welke leverancier zou jouw vraag deze week het minst leuk vinden?'

**Transitie naar afsluiting:** Niet van toepassing — einde sessie.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-scorekaarten | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-overfitting | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-diagnose | n + 2 | A4 dubbelzijdig (3 scorekaarten) — **OF** vervang door tablets met `model-overfitting-sliders.jsx` |
| ☐ | Optioneel: `video/composition.tsx` (Remotion `OverfittingVideo`) | 1 | ~90s, fase 1 |
| ☐ | Optioneel: tablets met `model-overfitting-sliders.jsx` | n | Vervangt wb-04 in fase 4 |
| ☐ | Stemkaartjes 2 kleuren (A/B) | n sets | Rood / blauw |
| ☐ | Markeerstiften (fluo) | n | Voor wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 1 | Parkeerlijst + 3 signalen + 3 tegenmaatregelen |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 4/5/6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Flexibiliteit — als het anders loopt

- **Als blok 1 uitloopt:** kort de tussenstand in (30 sec naar 15 sec). Het langzaam tonen van Model A en B is essentieel — daar niet op besparen.
- **Als blok 2 uitloopt:** kort het plenair benoemen in tot 2 min. De term overfitting moet plenair uitgesproken worden — vergelijking met collega ook.
- **Als blok 3 uitloopt:** kort cross-validatie-uitleg in tot 1 min. De drie signalen zijn cruciaal — niet daarop besparen.
- **Als blok 4 uitloopt:** individueel werken naar 4 min, plenair naar 1 min, transferopdracht in 30 sec. Nooit overslaan.
- **Als de groep te klein is (< 6):** sla de stemming over, ga direct naar bespreking. Iedereen krijgt het woord.
- **Als de groep te groot is (> 12):** verdeel in twee subgroepen tijdens fase 2 (5 min buurman + 5 min subgroep) en kort plenair in tot 2 min.

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Twee scorekaarten kiezen | Eerste keuze + reden (twijfel mag) |
| 2 reflecteren | Duo + term overfitting | Inzicht: verschil is signaal, niet hoogte |
| 3 theoretiseren | Handout 3 signalen + 3 tegenmaatregelen | Werkbaar framework + cross-validatie als operator-vraag |
| 4 experimenteren | Diagnose op 3 scenario's | Toepassing + transferopdracht aan leverancier |

**Slagingscriterium:** scoreverschil als signaal herkennen + minimaal 2 van 3 scenario's correct diagnosticeren + concrete leveranciersvraag geformuleerd.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met stemming-uitslag + signalen/tegenmaatregelen gefotografeerd
- [ ] Genoteerd: hoeveel deelnemers kozen Model A vóór de bespreking? (hardnekkigheid 'hoogste wint')
- [ ] Notitie voor volgende sessie: welke leveranciers worden bevraagd? Welke systemen onderzocht?
- [ ] xAPI-statements verstuurd: `experienced` (scorekaarten), `completed` (handout + diagnose), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 1 (Gebruik) | Overfitting — wanneer 99% een alarmbel is*
*Bronnen: Russell & Norvig (2021) AI: A Modern Approach. | Goodfellow et al. (2016) Deep Learning. | Hastie et al. (2009) Elements of Statistical Learning.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
