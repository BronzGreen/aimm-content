# Federated Learning — samen leren zonder data te delen — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 50 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden uitleggen wat federated learning is, hoe het verschilt van klassieke centrale ML-training, en in welke situatie het op de eigen werkvloer voordeel oplevert (privacy, bandbreedte, IP-bescherming). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | data-lit-101 doorlopen; globaal beeld van een ML-model (input → model → voorspelling) |
| **Stadium (H&B)** | Bewust bekwaam — kent klassieke ML, mist mentaal model van gedistribueerd leren |
| **Begeleidingsstijl** | Instrueren — sterk sturend op concept, ruimte voor eigen scenario-keuzes |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen AI Fundamentals Module 2 (Train) — paradigma-LO naast CNN, RNN, Ensemble en ML-leerklassen |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Mini-college: drie kenmerken van FL | theoretiseren | 15 min |
| 00:15 - 00:27 | Drie scenario-kaarten — past FL hier? | ervaren | 12 min |
| 00:27 - 00:37 | Buurman-check + plenaire bespreking | reflecteren | 10 min |
| 00:37 - 00:50 | Eigen organisatie-scan: actieplan | experimenteren | 13 min |

**Totaal:** 50 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (concept-vragen) of fase 3 (uitwisseling).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve per stuk.
- [ ] Print `diagram-lo-ai-fund-fl-001.svg` op A3 (centraal vs. federated). Hang in de zaal of leg op trainertafel.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `FederatedLearningVideo`, ~91s) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Inzet als visuele opening van fase 1, naast of in plaats van het diagram-doorlopen.
- [ ] Bereid op een flip-over alvast voor: links **"Parkeerlijst — verdieping voor later"**, rechts **"Drie kenmerken FL"** met ruimte voor (1) (2) (3).
- [ ] Bedenk één eigen anekdote voor de medische opening — bijv. ziekenhuissamenwerking of Google Keyboard. Schrijf de kernzin op.

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel — uitdelen pas op het moment.
- [ ] Schrijf op de tweede flip-over: links 'Centraal' / rechts 'Federated' — als hulp bij fase 1.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Mini-college — drie kenmerken van federated learning
**00:00 - 00:15** | 15 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer ontwikkelt een mentaal model van FL aan de hand van drie operationele kenmerken: (1) data blijft lokaal, (2) alleen modelparameters reizen, (3) centrale server aggregeert. Deelnemer vult tijdens de uitleg een vergelijkingsschema in (centraal vs. federated).

**Werkvorm:** Trainer-geleid mini-college met diagram. Deelnemers vullen tijdens de uitleg actief het werkblad in.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 50 minuten kijken we naar een ML-paradigma dat je naam gaat zien als jullie organisatie nadenkt over data-samenwerking: federated learning. Tegen het eind kun je in eigen woorden uitleggen wat het is, en kun je drie scenario's beoordelen op of het past."*

2. **Trigger — medische opening** (2 min) — toon slide 2. Vertel: *"Stel je voor: vijf ziekenhuizen willen samen een AI-model trainen om vroeg-stadium tumoren te herkennen op MRI-beelden. Iedereen wil meedoen. Maar geen ziekenhuis mag patiëntbeelden uit het pand laten gaan — privacywet. Hoe doen ze het dan?"* Pauze 5 seconden. Vraag: *"Iemand een idee?"* Vang 1-2 reacties. Reageer met *"Dat is precies de denkrichting: niet de data delen, maar iets anders."*

3. **Toon het diagram — centraal vs. federated** (3 min) — toon slide 3. Wijs op het A3 en op het scherm.
    - Wijs links: *"Klassieke ML — alle data gaat naar één centrale plek, daar wordt het model getraind."*
    - Wijs rechts: *"Federated — model gaat naar de data toe. Lokaal trainen op de eigen data. Daarna gaan alleen de modelparameters — gewichten — naar een centrale server. Die middelt ze tot één globaal model en stuurt het terug. Volgende ronde."*

4. **Deel wb-01 uit** (30 sec). Zeg: *"Tijdens de drie kenmerken die ik nu uitleg vul je dit schema in. Per kenmerk: wat gebeurt er bij klassieke ML, wat gebeurt er bij FL? Markeer het verschil dat jou het meest verrast."*

5. **Drie kenmerken — één voor één** (7 min) — toon slides 4-6:
    - **Kenmerk 1 — data blijft lokaal** (2 min). Slide 4. Zeg: *"Eerste kenmerk: ruwe data verlaat de fabriek of edge-device niet. Geen sensorlogs, geen camerabeelden, geen ERP-rijen die over een leiding worden gestuurd. Wat lokaal is, blijft lokaal."* Wacht 5 sec. *"Welke implicatie heeft dat voor privacy?"* Vang 1 antwoord — bevestig: GDPR-compliance, IP-bescherming, klantvertrouwen.
    - **Kenmerk 2 — alleen modelparameters reizen** (2 min). Slide 5. Zeg: *"Tweede kenmerk: wat WEL over het netwerk gaat zijn de geleerde gewichten — de parameters van het neurale netwerk. Dat is heel andere data dan ruwe sensorlogs. Veel kleiner, en je kunt er geen patiëntfoto of productformule uit reconstrueren — al zijn er geavanceerde aanvallen, daarover later meer."* Maak op flip-over: 'modelparameters << ruwe data'.
    - **Kenmerk 3 — centrale server aggregeert** (3 min). Slide 6. Zeg: *"Derde kenmerk: er is een centrale aggregator. Die verzamelt de parameters van alle nodes, middelt ze, en stuurt het verbeterde globale model terug voor de volgende trainingsronde. Dit heet FedAvg in de literatuur."* Pauze 3 sec. *"Wie ziet hier al een beperking?"* Wacht. Het antwoord is: single point of failure. Bevestig: *"Klopt — als de aggregator plat ligt, ligt de hele trainingsronde stil. Vanilla FL is niet decentraal — er bestaan decentrale varianten, maar die laten we vandaag links liggen."*

6. **Maak de stap naar maakindustrie** (1 min 30) — toon slide 7. *"Eerste FL-toepassing was Google Keyboard — woordvoorspelling op je telefoon, model leert van wat jij typt zonder dat Google jouw teksten ziet. Tweede grote golf: medisch — ziekenhuissamenwerkingen voor diagnose-modellen. Nu: maakindustrie — multi-fabriek PdM, OEM-leverancier-ketens, sectorgenoten met dezelfde machinetypes."*

**Materiaal:**
- [ ] Slides 1-7
- [ ] wb-01-vergelijkingsschema (1 per deelnemer + markeerstift)
- [ ] A3-diagram zichtbaar
- [ ] Flip-over met drie kenmerken klaar

> **Tips voor de trainer:**
> - Tempo is belangrijk: per kenmerk 2-3 minuten, niet langer. Anders verzandt fase 1 en raakt fase 4 in de knel.
> - Spreek de drie kenmerken hardop en in dezelfde volgorde uit. Herhaling = verankering.
> - Vermijd termen als 'gradient descent', 'FedAvg', 'differential privacy' tenzij iemand ernaar vraagt — dan parkeren.

> **Valkuil — FL wordt verward met cloud-AI of edge-AI:**
> Als iemand zegt 'dat is toch gewoon edge?' — bevestig de verwarring. Schrijf op flip-over naast elkaar: edge-AI (lokaal infereren), cloud-AI (data + model centraal), FL (lokaal trainen, parameters delen). Pas dan vallen de definities op hun plek. Gebruik max 2 minuten — dan terug naar de drie kenmerken.

> **Valkuil — technische verdieping eist tijd:**
> Een MBO-4-er met IT-affiniteit vraagt naar het algoritme of differential privacy. Bevestig de vraag, parkeer op flip-over: 'verdieping voor later'. Houd het conceptueel — dit is een paradigma-LO.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de drie kenmerken groot op de flip-over en hou ze tijdens fase 2-4 zichtbaar.
> - **Teamleider sneller:** Vraag tussendoor: 'welke gespreksvraag stel jij aan IT na deze sessie?' — laat ze klein noteren.
> - **Gemengde groep:** Vraag bij kenmerk 1 eerst operator-MBO-4: 'wat zou jouw IT-collega hier zeggen?' Daarna teamleider — niet andersom.

---

### Blok 2: Drie scenario-kaarten — past FL hier?
**00:15 - 00:27** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer toetst het mentale model door drie scenario's te beoordelen op FL-geschiktheid en het doorslaggevende kenmerk per case te benoemen.

**Werkvorm:** Worked example (IK DOE) bij scenario A, daarna individueel B en C; trainer loopt rond en stelt verdiepende vragen.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Zeg: *"Drie scenario's. Per scenario kies je: past FL hier wel of niet, en welk van de drie kenmerken (privacy/data lokaal, bandbreedte, IP) is doorslaggevend. Vergelijkingsschema uit fase 1 mag op je tafel blijven liggen."*

2. **IK DOE — scenario A voor** (3 min) — toon slide 8. Zeg hardop: *"Scenario A: drie zusterfabrieken willen samen een PdM-model voor dezelfde lager-types. Mijn redenering: de drie fabrieken horen bij hetzelfde concern. Als ze elkaar al volledig vertrouwen en de data al delen via een gemeenschappelijke datalake — dan is centrale training simpeler. FL voegt dan vooral overhead toe. Maar..."* Pauze. *"...als de fabrieken in verschillende landen staan met verschillende GDPR-regimes, of als de productlijnen concurrentiegevoelig zijn naar elkaar, dán wordt FL relevant. A is bewust grijs — ik schrijf 'het hangt ervan af' op met als doorslaggevend kenmerk: 'data lokaal/privacy afhankelijk van situatie'."*

3. **Deelnemers werken aan B en C** (6 min) — toon slide 9. Zet timer op 6 min. Loop rond. Stel verdiepende vragen:
    - *"Welk van de drie kenmerken is hier doorslaggevend?"*
    - *"Stel je deelt deze data wél centraal — wat gaat er fout?"*
    - *"Heb je ooit van een klant gehoord: 'deze data verlaat onze muren niet'?"*

4. **Korte tussenstand** (1 min) — vraag: *"Wie heeft B al? Hand omhoog. C ook? Mooi — we lopen ze straks plenair door."*

5. **Tijd-check** (1 min 30) — als 80% klaar is, sluit af. Zeg: *"Pen neer. Niet bespreken — dat doen we straks samen. Houd je werkblad voor je."*

**Materiaal:**
- [ ] Slides 8-9
- [ ] wb-02-scenarios (1 per deelnemer, drie kaarten)
- [ ] Timer
- [ ] Pen

> **Tips voor de trainer:**
> - Bij twijfel: stuur niet bij. De twijfel is leerstof voor fase 3.
> - Loop wel langs trage starters — vraag hen hardop: 'wat staat er in scenario B?' Activeert de aandacht zonder voor te zeggen.
> - Schrijf zelf NIET mee. Je hoeft geen voorbeeld-antwoord op het bord — de plenaire bespreking moet uit de groep komen.

> **Valkuil — scenario A wordt te snel als FL-case afgedaan:**
> Als iedereen direct 'FL past' zegt, stel de tegenvraag: 'Stel jullie hebben al een gedeelde concern-database — heb je FL dan nog nodig?' Maak expliciet dat FL een antwoord is op een echt obstakel. Zonder obstakel is centrale training simpeler en goedkoper.

> **Valkuil — scenario C wordt onderschat:**
> Sommige deelnemers zien de lasrobot-IP-vraag niet als 'echte' privacy. Maak expliciet: productdata kan IP zijn (procesparameters, recepten, kwaliteitsmetingen). FL is niet alleen voor persoonsgegevens.

> **Differentiatie:**
> - **MBO-4 basis:** Vraag hen één kenmerk per keer af te lopen — 'is data lokaal-houden hier nodig? ja/nee. is bandbreedte een issue? ja/nee. is IP een issue? ja/nee.'
> - **Teamleider sneller:** Vraag bij snel klaar: 'welke organisatie-rol moet eerst akkoord op zo'n FL-voorstel — IT, juridisch, business?'

---

### Blok 3: Buurman-check + plenaire bespreking
**00:27 - 00:37** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander, hoort een ander perspectief op dezelfde casus, en herkent welk kenmerk voor de groep doorslaggevend is.

**Werkvorm:** 5 minuten in tweetallen vergelijken — daarna plenaire stemming en bespreking.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). Zeg: *"Vorm een tweetal met je buurman. Vergelijk je antwoorden op A, B en C. Bij verschillen: leg elkaar uit waarom. Vul aan het eind op het reflectiewerkblad in welk scenario je opnieuw zou beoordelen na de discussie."*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Luister mee. Verzamel 2-3 sterke verschillen voor de plenaire ronde. Bij stille tweetallen: stel een hardop-vraag aan beiden: *"Wie van jullie was het scherpst over scenario A?"*

3. **Plenair stemmen** (2 min) — toon slide 10. Per scenario: *"Hand omhoog wie 'FL past'. Hand omhoog wie 'FL past niet'. Wie twijfelt?"* Tel hardop, schrijf op flip-over de uitslag (bijv. A: 4-3-1, B: 8-0-0, C: 7-1-0).

4. **Bespreking — vooral A** (2 min 30) — toon slide 11. *"B was unaniem — scenario edge-device met beperkte bandbreedte. FL past omdat modelparameters veel kleiner zijn dan het ruwe vibration-signaal. C ook unaniem — IP-gevoelige lasrobotdata, klant wil dat data binnen blijft. A was verdeeld."* Vraag een 'ja-stemmer' op A: *"Waarom past FL volgens jou hier?"* Vang antwoord. Vraag een 'nee/twijfel-stemmer': *"En waarom niet, of waarom twijfel?"* Bevestig: *"A is bewust grijs. FL past als de data tussen de zusterfabrieken niet zomaar gedeeld mag worden — bijvoorbeeld door GDPR-regimes of concurrentie tussen plant managers. Maar als ze al delen via een datalake, voegt FL alleen overhead toe."*

**Materiaal:**
- [ ] Slides 10-11
- [ ] wb-03-reflectie
- [ ] Flip-over voor stemming-uitslag
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag in de plenaire ronde. Stilte van 5 seconden voelt lang maar haalt antwoorden op.
> - Veroordeel geen antwoord — ook 'verkeerde' antwoorden geven inzicht in waar het mentale model nog niet sluit.
> - Bij scenario B en C zonder discussie: een korte bevestiging van het doorslaggevende kenmerk is genoeg ('bandbreedte voor B, IP voor C'). Geen tijd verspillen aan het reeds-begrepene.

> **Valkuil — single-perspectief tweetal:**
> Twee deelnemers van dezelfde fabriek raken in eigen-bedrijfs-discussie. Bedank, zeg: *"Goeie discussie — bewaar het voor fase 4. Eerst de scenario's afronden."*

> **Valkuil — plenair wordt frontaal:**
> Trainer gaat zelf het 'goede antwoord' geven. Houd je in. De waarde zit in de twijfel die uit de groep komt.

> **Differentiatie:**
> - **Gemengde groep:** Vraag bij plenair eerst operators (B en C eerst) — daarna teamleiders bij A. Voorkomt dat strategisch perspectief operators de mond snoert.

---

### Blok 4: Eigen organisatie-scan — actieplan
**00:37 - 00:50** | 13 min | Kolb-fase: experimenteren

**Doel:** Deelnemer schrijft een concreet actieplan voor één situatie in de eigen organisatie of bij een klant waar FL relevant zou zijn.

**Werkvorm:** Individueel werkblad — trainer loopt rond en helpt bij concretisering.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Zeg: *"Laatste 13 minuten. Eén situatie in je eigen organisatie of bij een klant waar productiedata nu níet centraal verzameld wordt vanwege privacy, IP of bandbreedte. Vul vier velden in: welke data, met wie zou je samen willen leren, welk modeldoel, welk van de drie FL-kenmerken telt het zwaarst."*

2. **Inventarisatie-vraag** (1 min) — toon slide 12. *"Eerst even rondkijken: bij wie speelt dit type vraag op de eigen werkvloer? Multi-fabriek, OEM-leverancier, klant-relatie?"* Vang 4-5 antwoorden, niet bespreken — alleen verzamelen.

3. **Individueel werken** (8 min) — zet timer op 8 min. Loop rond. Stel concretiserende vragen:
    - *"Welke data krijg je nu niet uit de zusterfabriek of leverancier?"*
    - *"Heeft jouw klant ooit gezegd: deze data verlaat onze muren niet?"*
    - *"Met wie zou de samenwerking zinvol zijn — wie heeft vergelijkbare data?"*
    - *"Welk modeldoel — vision, vibration, kwaliteit, RUL?"*
    Bij vage antwoorden ('weet niet welke data'): help één concrete trio formuleren — data-type / partner / modeldoel. Bevestig dat een hypothetisch maar specifiek voorbeeld beter werkt dan een vaag generiek antwoord.

4. **Plenaire ronde** (2 min) — toon slide 13. *"Twee deelnemers — kort delen: één situatie, één partner, welk kenmerk telt het zwaarst."* Vang 2 voorbeelden — geen oordeel, alleen waardering.

5. **Afsluiting + transferopdracht** (1 min 30) — toon slide 14. *"Deze week: praat één keer met een collega van IT of data-afdeling. Open met: 'Ik leerde over federated learning — kennen jullie het concept, en zien jullie het in onze data-strategie?' Je krijgt vaak verrassend snel zicht op hoe je organisatie er nu over denkt. Volgende sessie bespreken we kort: wat heb je gehoord?"*

**Materiaal:**
- [ ] Slides 12-14
- [ ] wb-04-actieplan
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij 'ik werk niet in een multi-fabriek-omgeving' — bevestig: een hypothetische klant of toekomstig project mag ook. Het gaat om het denkraam.
> - De plenaire ronde van fase 4 is goud voor de volgende sessie. Schrijf 1 regel per voorbeeld in je trainersnotitieblok.
> - Houd 1 minuut over voor afsluiting — die transfergesprek-zin moet aankomen.

> **Valkuil — actieplan blijft hypothetisch en algemeen:**
> Help één concrete trio invullen: data-type / partner / modeldoel. Een specifiek hypothetisch voorbeeld werkt beter dan een vaag generiek antwoord.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 11 minuten door werkblad-tijd op 6 min te zetten. Sla afsluiting nooit over — het IT-gesprek is de transferactie.

> **Differentiatie:**
> - **MBO-4 basis:** Eén concrete situatie is genoeg. Niet vragen om vergelijking met klassieke ML.
> - **Teamleider sneller:** Vraag ook welke organisatie-rol (CISO, CTO, plant manager) als eerste op een FL-voorstel zou reageren — en hoe je het gesprek zou framen.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-vergelijkingsschema | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-scenarios (3 kaarten) | n + 2 | A4 dubbelzijdig |
| ☐ | wb-03-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-04-actieplan | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-ai-fund-fl-001.svg | 1 op A3 | Centraal vs. federated, zichtbaar in zaal |
| ☐ | Markeerstiften | n | Voor wb-01 en wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 2 | Parkeerlijst + drie kenmerken |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5-min en 6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 theoretiseren | Vergelijkingsschema invullen tijdens drie kenmerken | Mentaal model FL = data lokaal + parameters reizen + centrale aggregatie |
| 2 ervaren | Drie scenario-kaarten beoordelen | Per case: FL ja/nee + doorslaggevend kenmerk |
| 3 reflecteren | Buurman-check + plenaire stemming | Inzicht: A is grijs, B en C zijn duidelijk FL-cases |
| 4 experimenteren | Eigen organisatie-actieplan | Concreet trio: data / partner / modeldoel |

**Slagingscriterium:** drie kenmerken benoemen + minimaal 2 van 3 scenario's correct beoordelen + actieplan met herkenbare situatie.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met drie kenmerken gefotografeerd (voor consistentie volgende sessie)
- [ ] Genoteerd: stemming per scenario A/B/C (verdeling = indicatie groepsbegrip)
- [ ] Notitie voor volgende sessie: welke transfer-acties zijn aangekondigd? Wie ging IT spreken?
- [ ] xAPI-statements verstuurd: `experienced` (vergelijkingsschema), `completed` (scenario's + actieplan), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | Federated Learning*
*Bronnen: McMahan et al. (2017) Communication-Efficiënt Learning. | Kairouz et al. (2021) Advances and Open Problems in Federated Learning.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
