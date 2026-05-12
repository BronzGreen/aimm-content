# Vier ML-leerklassen — welke past bij welk PdM-probleem? — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 50 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan de vier ML-leerklassen benoemen (supervised, unsupervised, semi-supervised, reinforcement) en uitleggen welke past bij welke datasituatie en bij welk PdM-probleemtype (classification, regression, clustering). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | data-lit-101 doorlopen; weet dat AI/ML iets met data doet |
| **Stadium (H&B)** | Bewust bekwaam — kent AI op hoog niveau, mist mentaal model van leerklasse-onderscheid |
| **Begeleidingsstijl** | Trainen — sturend op concept, ervaringsgericht startend |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Foundational LO in AI Fundamentals — bij voorkeur eerst aanbieden, voor FL/CNN/RNN/Ensemble |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:14 | Vier scenario-kaarten — welke leerklasse past? | ervaren | 14 min |
| 00:14 - 00:25 | Buurman-check + plenaire bespreking | reflecteren | 11 min |
| 00:25 - 00:38 | Handout: vier leerklassen + drie PdM-probleemtypen | theoretiseren | 13 min |
| 00:38 - 00:50 | Actieplan: welke leerklasse past bij ons? | experimenteren | 12 min |

**Totaal:** 50 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (scenario-twijfels) of fase 3 (semi-supervised + reinforcement uitleg).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print `diagram-lo-ai-fund-ml-001.svg` op A3 (4 leerklassen × 3 probleemtypen). Hang in de zaal.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bereid stemkaartjes voor: 4 kleuren (rood/blauw/geel/groen — voor 4 leerklassen). Eén set per deelnemer.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst — verdieping voor later"**, rechts **"Vier leerklassen"** met vier rijen.

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01, set stemkaartjes.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Vier scenario-kaarten — welke leerklasse past?
**00:00 - 00:14** | 14 min | Kolb-fase: ervaren

**Doel:** Deelnemer ondervindt aan de hand van vier herkenbare PdM-scenario's dat de keuze van leerklasse direct afhangt van wat voor data je hebt. Deelnemers kiezen per scenario een leerklasse en motiveren — twijfel mag.

**Werkvorm:** Worked example (IK DOE) bij scenario A, daarna individueel B-D. Trainer loopt rond.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 50 minuten kijken we naar het belangrijkste keuzemodel uit ML: de vier leerklassen. Niet één AI — vier soorten. Tegen het eind weet je welke past bij welke data, en welke past bij welk type PdM-probleem."*

2. **Trigger — een leveranciersgesprek** (1 min 30) — toon slide 2. Vertel: *"Stel: een PdM-leverancier komt langs. Hij zegt 'wij doen supervised regression — geef ons jullie failure-data en wij voorspellen de RUL.' Of: 'wij doen unsupervised clustering — wij vinden de afwijkende patronen, jullie hoeven geen labels te leveren.' Twee verschillende aanbiedingen. Wat zegt dat over wat je nodig hebt?"* Pauze. *"Tegen het eind van deze sessie kun je dat gesprek leiden in plaats van ondergaan."*

3. **Deel wb-01 uit** (30 sec). *"Op het werkblad staan vier scenario-kaarten — vier verschillende fabrieken met vier verschillende data-realiteiten. Per kaart kies je een leerklasse en onderbouwt waarom. Twijfel mag — vraagteken zetten is welkom."*

4. **IK DOE — scenario A voor** (3 min) — toon slide 3. Lees scenario A hardop:
    - *"Fabriek met 5 jaar uitvalhistorie. Duidelijke failure-labels in het ERP. Wil RUL voorspellen — hoeveel cycli tot uitval per machine?"*
    - *"Mijn redenering: 5 jaar gelabelde data — supervised mogelijk. Voorspelling van een GETAL (cycli) — dat heet regression. Combinatie: supervised regression. Onderbouwing: gelabelde uitvalhistorie + voorspelling van getal. Schrijf op."*

5. **Deelnemers werken aan B, C, D** (7 min) — toon slide 4. Zet timer op 7 min. Loop rond. Stel verdiepende vragen:
    - *"Wat heb je aan data?"*
    - *"Wat moet er voorspeld worden — een getal, een klasse, een patroon, of een beslissing?"*
    - *"Heb je labels — gelabeld, niet gelabeld, beetje gelabeld?"*

6. **Korte tussenstand** (1 min) — vraag: *"Wie heeft alle drie? Twee? Eén? Mooi — plenair gaan we dadelijk."*

7. **Tijd-check** (1 min) — als 80% klaar is, sluit af.

**Materiaal:**
- [ ] Slides 1-4
- [ ] wb-01-scenarios (1 set per deelnemer, 4 kaarten)
- [ ] Timer
- [ ] Pen
- [ ] Stemkaartjes klaar voor fase 2

> **Tips voor de trainer:**
> - Lees scenario A langzaam voor — je bent het rolmodel voor tempo en redeneerstijl.
> - Geef geen antwoorden. Bij twijfel: 'lekker — schrijf je twijfel op'.
> - Niet zelf duiden ('aha, dit is unsupervised!'). Die conclusies komen in fase 2-3.

> **Valkuil — 'Maar je moet toch labels hebben?':**
> Iemand zegt: 'Maar de AI weet toch niet of het klopt zonder labels?' Bevestig de logica: supervised is vaak het meest accuraat — ALS labels beschikbaar zijn. Maar 80% van fabrieken heeft die niet. Unsupervised, semi-supervised en reinforcement zijn dan geen 'minder' AI — ze zijn de enige optie. Houd kort, uitwerken in fase 3.

> **Valkuil — scenario D (continue beslissingen) wordt overgeslagen:**
> Reinforcement is onbekend bij MBO-4. Als iemand vastloopt: bevestig 'D is de meest abstracte — denk aan een AI die LEERT door beslissingen te nemen en feedback te krijgen of het goed of slecht uitviel'. Niet meer details — fase 3.

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopen op D — bied aan om die over te slaan en in fase 3 mee te nemen.
> - **Teamleider sneller:** Vraag bij snel klaar: 'Welk scenario is bij JOUW organisatie het meest realistisch?' Voorbereiding op fase 4.

---

### Blok 2: Buurman-check + plenaire bespreking
**00:14 - 00:25** | 11 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander, hoort een ander perspectief, en herkent waarom scenario C (semi-supervised) en D (reinforcement) de meest gemist worden.

**Werkvorm:** 5 minuten in tweetallen — daarna stemming met gekleurde stemkaartjes en bespreking.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Zeg: *"Tweetal met je buurman. Vergelijk je antwoorden op A t/m D. Bij verschillen: leg elkaar uit waarom. Welk woord uit de scenario-tekst was voor jou doorslaggevend?"*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Verzamel 2-3 sterke verschillen voor plenair.

3. **Plenair stemmen met kleurkaartjes** (2 min 30) — toon slide 5. *"Per scenario steek je een kleur omhoog: rood = supervised, blauw = unsupervised, geel = semi-supervised, groen = reinforcement."* Voor scenario A, B, C, D loop je af. Tel hardop, schrijf op flip-over.

4. **Bespreking — vooral C en D** (2 min 30) — toon slide 6. *"A is meestal supervised regression — gelabelde data + getal-voorspelling. B is unsupervised clustering — geen labels, zoek patronen. C en D zijn de tricky ones."* Pauze. *"C: 50 gelabeld + 5000 ongelabeld. Veel mensen kiezen unsupervised of supervised. Het juiste antwoord: semi-supervised — een COMBINATIE die het kleine gelabelde set gebruikt om iets te leren EN het grote ongelabelde set om patronen te versterken. Recent populair in PdM-onderzoek."*

   Pauze. *"D: continue beslissingen over onderhoud. Veel mensen denken 'reinforcement is voor robots'. Klopt voor de bekendste voorbeelden — maar reinforcement gaat over LEREN VAN BESLISSINGEN. Bij onderhoud: uitstellen vs. preventief vs. nu vervangen — elke beslissing heeft een uitkomst (kosten/baten). Reinforcement learnt die optimaliseren. Adaptief onderhoudsbeleid."*

5. **Brug naar fase 3** (30 sec) — *"Nu het framework — en hoe het verbindt aan PdM-probleemtypen."*

**Materiaal:**
- [ ] Slides 5-6
- [ ] wb-02-reflectie
- [ ] Stemkaartjes (4 kleuren per deelnemer)
- [ ] Flip-over voor stemming-uitslag
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag.
> - Bij stilte tijdens stemming: noem zelf de eerste 'hand omhoog' om het ijs te breken.
> - Bevestig zonder oordeel — fout antwoord op C is leerstof.

> **Valkuil — semi-supervised verwarring:**
> Bij C kiest meer dan helft 'unsupervised' of 'supervised'. Maak expliciet: semi-supervised gebruikt BEIDE. Niet alleen labels, niet alleen ongelabeld. Combinatie.

> **Valkuil — reinforcement = robot:**
> Bij D kiest niemand reinforcement. Bevestig de associatie maar verbreed naar 'leren van beslissingen met feedback'.

> **Differentiatie:**
> - **Gemengde groep:** Vraag bij C eerst operator (welk woord deed je twijfelen?), dan teamleider (welke leverancier biedt dit aan?).

---

### Blok 3: Handout — vier leerklassen + drie PdM-probleemtypen
**00:25 - 00:38** | 13 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer plaatst de eigen scenario-keuzes in een gestructureerd framework: 4 leerklassen × 3 PdM-probleemtypen. De handout wordt het naslagwerk voor het transfer-gesprek.

**Werkvorm:** Trainer-geleide handout-bespreking met directe verbinding naar de scenario's uit fase 1.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). Zeg: *"Pak je markeerstift. Tijdens het doorlopen markeer je wat voor jou nieuw is."*

2. **Toon de twee tabellen** (1 min) — toon slide 7. *"Twee tabellen op je handout. Eerst: vier leerklassen — welke datasituatie. Daarna: drie PdM-probleemtypen — welk type voorspelling. Beide moet je matchen."*

3. **Loop de vier leerklassen af** (5 min) — toon slide 8. Per leerklasse: kerngedachte + datasituatie + PdM-toepassing. Verbind expliciet aan een scenario:
    - **Supervised** (1 min 15): *"Met labels. Veel gelabelde failure-cases. PdM: classification (welke uitval) of regression (RUL). Scenario A — 5 jaar uitvalhistorie + RUL — past hier."*
    - **Unsupervised** (1 min 15): *"Zonder labels. Zoekt patronen, clusters, afwijkingen. PdM: clustering, anomaliedetectie. Scenario B — geen uitvalhistorie, wel sensordata — past hier."*
    - **Semi-supervised** (1 min 30): *"Combinatie. Klein gelabeld + groot ongelabeld. Recent populair omdat labelen DUUR is in praktijk. PdM: classificatie waar je 50 cases gelabeld hebt en 5000 ongelabeld. Scenario C — past hier."*
    - **Reinforcement** (1 min): *"Online leren via beslissingen + feedback. PdM: adaptief onderhoudsbeleid. Scenario D — past hier. Zeldzaam in deployment, vaak nog onderzoek."*

4. **Drie PdM-probleemtypen** (3 min 30) — toon slide 9. *"Drie typen voorspelling die je kunt willen:"*
    - *"Classification — welke klasse? Bv. 'normaal/uitval-type-A/uitval-type-B'. Past supervised."*
    - *"Regression — hoeveel? Bv. 'RUL = 23 cycli' of 'kostenschatting = 12.000 euro'. Past supervised."*
    - *"Clustering — welke groepen? Bv. 'machines die zich similar gedragen'. Past unsupervised."*
    Maak op flip-over de combinatie: PROBLEEM × LEERKLASSE.

5. **Praktische realiteit in PdM** (2 min) — toon slide 10. *"Belangrijk om te weten: 80% van fabrieken heeft GEEN systematische failure-data. Logboeken bevatten vaak waardevolle vrije tekst — labelen is verborgen werk. Voor de meeste organisaties is unsupervised of semi-supervised de meest realistische start. Reinforcement is zeldzaam — vooral academisch of in cloud-platformen."*

6. **Brug naar fase 4** (30 sec) — *"Nu jouw eigen organisatie. Welke leerklasse past bij wat jullie feitelijk in huis hebben?"*

**Materiaal:**
- [ ] Slides 7-10
- [ ] wb-03-handout-leerklassen
- [ ] A3-diagram zichtbaar
- [ ] Markeerstift per deelnemer
- [ ] Flip-over

> **Tips voor de trainer:**
> - Gebruik de scenario's als rode draad. Per leerklasse expliciet noemen welk scenario erbij hoorde.
> - Houd reinforcement-uitleg kort. Het is voor MBO-4 minder direct relevant; herkenning is genoeg.
> - Bij vragen over k-means, t-SNE, Q-learning — parkeer op flip-over.

> **Valkuil — supervised wordt 'best, anderen minder':**
> Maak expliciet: leerklasse moet aansluiten op DATA-realiteit, niet op een ideaal. Unsupervised bij geen labels = beste optie, niet inferieur.

> **Valkuil — algoritmen vs. leerklassen:**
> IT-affiniteit-vraag over algoritmes. Parkeer. Vandaag op leerklasse-niveau.

> **Differentiatie:**
> - **MBO-4 basis:** Per leerklasse één steekwoord: 'met labels / zonder labels / beetje labels / leren van beslissingen'.
> - **Teamleider sneller:** Vraag tussendoor: 'welke leverancier-claim doet alarmbellen rinkelen?' Antwoord: 'we kunnen alles' — geen leerklasse-keuze gemaakt = waarschijnlijk vaag.

---

### Blok 4: Actieplan — welke leerklasse past bij ons?
**00:38 - 00:50** | 12 min | Kolb-fase: experimenteren

**Doel:** Deelnemer noteert één concrete eigen toepassing, beoordeelt de huidige data-realiteit, en formuleert een gefundeerde leerklasse-keuze plus een concrete IT-vraag.

**Werkvorm:** Individueel werkblad — trainer loopt rond.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Zeg: *"Laatste 12 minuten. Eén PdM- of monitoring-toepassing op je eigen lijn. Vier vragen: (1) heb je gelabelde uitvalhistorie? (2) wat wil je voorspellen — getal, klasse, patroon, beslissing? (3) welke leerklasse past? (4) welke vraag stel je aan IT?"*

2. **Inventarisatie-vraag** (1 min) — toon slide 11. *"Bij wie speelt PdM of monitoring op de werkvloer? Spuitgieten, CNC, verpakking?"* Vang 4-5 antwoorden, niet bespreken.

3. **Individueel werken** (8 min) — zet timer op 8 min. Loop rond. Stel concretiserende vragen:
    - *"Hoe vaak houden jullie systematisch uitval bij?"*
    - *"Heeft jullie ERP een uitval-categorie-veld?"*
    - *"Wat is het primaire iets dat je zou willen voorspellen?"*
    Bij 'we weten het niet zeker': bevestig — DAT is waardevol. Het is de eerste IT-vraag.

4. **Plenaire ronde** (1 min 30) — toon slide 12. *"Twee deelnemers — kort: jouw toepassing + welke leerklasse + welke IT-vraag."* Vang 2 voorbeelden.

5. **Afsluiting + transferopdracht** (1 min) — toon slide 13. *"Deze week: onderzoek bij IT, onderhoud of kwaliteit: (1) registreren we systematisch failures? (2) hoeveel cases? (3) zijn oorzaken gecategoriseerd? Drie concrete vragen. Bonus-praatje: vraag een onderhoudscollega 'houden wij systematisch bij waarom een machine stuk gaat?' — de informatie zit vaak in logboeken maar niet bruikbaar gestructureerd. Dat ontdekken is goud waard voor elk AI-project."*

**Materiaal:**
- [ ] Slides 11-13
- [ ] wb-04-actieplan
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij 'ik werk niet rechtstreeks met PdM': hypothetische klant of toekomstig project mag.
> - De plenaire ronde is goud voor volgende sessie.
> - Maak concreet dat 'we hebben het niet bijgehouden' GEEN blokker is — het is precies de waardevolle ontdekking.

> **Valkuil — actieplan blijft 'ik weet niet hoeveel data':**
> Bevestig: 'weet ik niet' is een GELDIGE uitkomst. Help formuleren als 3 concrete IT-vragen.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 10 min door werkblad-tijd op 6 min te zetten. Sla afsluiting nooit over.

> **Differentiatie:**
> - **MBO-4 basis:** Eén concrete toepassing + één leerklasse-keuze is genoeg.
> - **Teamleider sneller:** Vraag ook: welke leverancier-claim zou bij JULLIE data-realiteit verdacht zijn? Voorbeeld: 'wij doen supervised RUL' bij een fabriek zonder failure-historie = mismatch.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-scenarios (4 kaarten) | n + 2 | A4 dubbelzijdig |
| ☐ | wb-02-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-leerklassen | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-actieplan | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-ai-fund-ml-001.svg | 1 op A3 | 4 leerklassen × 3 PdM-probleemtypen |
| ☐ | Stemkaartjes 4 kleuren | n sets | Rood / blauw / geel / groen |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 2 | Parkeerlijst + 4 leerklassen |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5/7/8-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Vier scenario-kaarten | Per scenario: leerklasse-keuze + onderbouwing (twijfel mag) |
| 2 reflecteren | Buurman + plenair stemmen met kleuren | Inzicht: C (semi-supervised) en D (reinforcement) zijn vaak gemist |
| 3 theoretiseren | Handout 4 leerklassen × 3 probleemtypen | Mentaal model: data-realiteit → leerklasse → probleemtype |
| 4 experimenteren | Eigen actieplan + IT-vragen | Concrete toepassing + gefundeerde leerklasse + 3 IT-vragen |

**Slagingscriterium:** vier leerklassen benoemen + minimaal 3 van 4 scenario's correct + actieplan met concrete data-inschatting.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met stemming-uitslag gefotografeerd (verdeling = indicatie groepsbegrip)
- [ ] Genoteerd: hoe scoorde de groep op C en D? (vaak gemist = leerwinst)
- [ ] Notitie voor volgende sessie: welke IT-vragen zijn aangekondigd? Wie ging onderhoud bevragen?
- [ ] xAPI-statements verstuurd: `experienced` (scenario's), `completed` (handout + actieplan), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | Vier ML-leerklassen*
*Bronnen: Russell & Norvig (2020) AI: A Modern Approach. | Mitchell (1997) Machine Learning. | Recent PdM-onderzoek 2025-2026 over semi-supervised pseudo-labeling.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
