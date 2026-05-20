# Ensemble learning — meerdere modellen die samen sterker zijn — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 48 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan uitleggen wat een ensemble is, kan het verschil benoemen tussen bagging (parallel, variance) en boosting (sequentieel, bias), en kan herkennen wanneer een ensemble passend is voor een PdM-probleem (onevenwichtige data, weinig failure-cases). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | data-lit-101 doorlopen; bij voorkeur lo-ai-fund-ml-001 (vier leerklassen) doorlopen |
| **Stadium (H&B)** | Bewust bekwaam — kent ML-modellen op hoog niveau, mist mentaal model van ensembles |
| **Begeleidingsstijl** | Trainen — sturend op concept, ervaringsgericht startend |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen AI Fundamentals Module 2 (Train) — naast FL, CNN, RNN, ML-leerklassen |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:13 | Diagnose-spel — één expert vs. drie experts | ervaren | 13 min |
| 00:13 - 00:22 | Buurman-check + plenaire reflectie | reflecteren | 9 min |
| 00:22 - 00:36 | Twee families: bagging en boosting | theoretiseren | 14 min |
| 00:36 - 00:48 | Actieplan: zou een ensemble onze PdM verbeteren? | experimenteren | 12 min |

**Totaal:** 48 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (diagnose-spel) of fase 3 (PdM-voorbeelden).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve. **Of** kies digitaal voor wb-01: laad `model-ensemble-stemming.jsx` op een React-sandbox en test op één tablet (slider 1-15 + diverse/identiek toggle).
- [ ] Print `diagram-lo-ai-fund-ensemble-001.svg` op A3 (bagging vs. boosting). Hang in de zaal.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Lees wb-01 zelf door en bereken de 'wins' per case voor case 1 — die doe je voor als IK DOE.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (~90s, 5 scenes) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Plan inzet als brug van fase 2 naar fase 3.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst — verdieping voor later"**, rechts **"Ensemble wins"** met vijf rijen voor de cases.

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Diagnose-spel — één expert vs. drie experts
**00:00 - 00:13** | 13 min | Kolb-fase: ervaren

**Doel:** Deelnemer ondervindt aan de hand van vijf mystery cases dat een 'meerderheid van drie experts' vaak een ander en beter antwoord geeft dan één expert alleen — vooral bij twijfelgevallen.

**Werkvorm:** Worked example (IK DOE) bij case 1, daarna individueel cases 2-5.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 48 minuten kijken we naar een ML-paradigma dat in PdM-onderzoek consequent betere voorspellingen geeft: ensemble learning. Maar we beginnen niet met theorie — we beginnen met een spel."*

2. **Trigger — drie experts** (1 min 30) — toon slide 2. Vertel: *"Stel: je laat een kapotte machine zien aan drie collega-monteurs. Ze stellen elk een diagnose. Soms zijn ze het eens. Soms niet. Wat doe jij — kies je voor expert A, omdat die het meest senior is? Of luister je naar alle drie?"* Pauze. *"Je gaat het zo zelf ervaren — vijf mystery cases met drie experts."*

3. **Deel wb-01 uit** (30 sec) — **OF** deel tablets uit met `model-ensemble-stemming.jsx` geopend. Zeg bij papier: *"Op het werkblad staan vijf cases — kort verhaaltje per machine, symptoom, sensorwaarden. Per case zijn er drie 'experts' (model A, B, C). Per case staat hun diagnose. Je gaat twee dingen doen: één — wat zou je doen als je alleen expert A had? Twee — wat als je alle drie meeneemt en stemt?"* Zeg bij digitaal: *"Op je tablet zie je een stem-experiment. Schuif het aantal modellen tussen 1 en 15 oneven, toggle tussen diverse en identieke modellen. Kijk wat er met de ensemble-accuracy gebeurt. Minimaal 3 verschillende instellingen."*

4. **IK DOE — case 1 voor** (3 min) — toon slide 3. Lees case 1 hardop voor:
    - *"Machine: spuitgietpers. Symptoom: licht verhoogde cyclustijd. Sensoren: temperatuur 215°C (normaal), druk 42 bar (was 38), trillingen normaal."*
    - *"Expert A zegt: 'Lichte slijtage van plunjer — monitoren.' Expert B: 'Klinkt als drukvariatie — controleer hydrauliek.' Expert C: 'Klinkt als drukvariatie — controleer hydrauliek.'"*
    - *"Mijn antwoord met alleen A: lichte slijtage — monitoren. Met alle drie meegenomen: 2 op 3 zegt drukvariatie hydrauliek. Mijn antwoord verandert. Ik schrijf op: ja, mijn diagnose is anders met de drie experts."*
    - Plak op flip-over case 1: 1 win.

5. **Deelnemers werken aan cases 2-5** (6 min) — toon slide 4. Zet timer op 6 min. Loop rond. Stel verdiepende vragen:
    - *"Waar veranderde je antwoord, en waar niet?"*
    - *"Als alle drie hetzelfde zeggen — wat voegt het ensemble toe?"*
    - *"Als ze elkaar tegenspreken — hoe kies je?"*

6. **Kort afronden** (1 min) — *"Pen neer. Tel voor jezelf: bij hoeveel cases gaf het ensemble een ander antwoord dan expert A alleen?"*

**Materiaal:**
- [ ] Slides 1-4
- [ ] wb-01-diagnose-spel (1 per deelnemer, 5 cases) **OF** tablets/laptops met `model-ensemble-stemming.jsx` geopend
- [ ] Timer
- [ ] Pen
- [ ] Flip-over voor 'wins-tracker'

> **Tips voor de trainer:**
> - Lees case 1 langzaam voor. Het is je rolmodel — als je race-tempo gaat, doen deelnemers dat ook.
> - Loop tijdens de individuele 6 minuten rond, maar geef geen antwoorden. Bij twijfel zeg je: 'lekker — schrijf je twijfel op.'
> - Niet zelf duiden 'aha, jullie zien dat de meerderheid wint!' — die conclusie komt uit fase 2.

> **Valkuil — 'meerderheid wint altijd':**
> Iemand zegt: 'De meerderheid heeft toch altijd gelijk?' Reageer: 'Stel alle drie experts maken dezelfde fout — wint de meerderheid dan ook?' Hint: ensembles werken alleen als modellen DIVERS zijn — verschillende fouten maken. Pas die nuance plenair in fase 2 expliciet maken — niet hier.

> **Valkuil — sceptische deelnemer:**
> Iemand zegt: 'Onzin — bij ons werken we met één goede monteur.' Bevestig: 'Goed punt — een fantastische monteur kan een team verslaan. Het ensemble-idee is dat ALS je drie redelijk goede experts hebt, samen vaak beter dan elk apart.' Houd het kort.

> **Differentiatie:**
> - **MBO-4 basis:** Lees ook case 2 voor (extra IK DOE) als het bij case 1 nog moeilijk lijkt.
> - **Teamleider sneller:** Vraag bij snel klaar: 'wanneer voegde de meerderheid niets toe — bij eensgezinde experts of bij heel uiteenlopende?'

---

### Blok 2: Buurman-check + plenaire reflectie
**00:13 - 00:22** | 9 min | Kolb-fase: reflecteren

**Doel:** Deelnemer vergelijkt eigen wins-telling met een ander, ontdekt patronen in wanneer het ensemble waarde toevoegt en wanneer niet, en formuleert in eigen woorden welke 'stem-strategie' werkte.

**Werkvorm:** 5 minuten in tweetallen — daarna plenaire wins-telling op flip-over.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Zeg: *"Vorm een tweetal met je buurman. Vergelijk je wins. Vraag elkaar: bij welke case maakte het ensemble het grootste verschil? Bij welke voegde het niets toe?"*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Verzamel 2-3 sterke observaties voor plenair.

3. **Plenair — wins per case** (2 min) — toon slide 5. Loop de cases af: *"Case 1 — wie heeft 'win'?"* Tel handen. Schrijf op flip-over. Idem voor cases 2-5. *"Tellen: gemiddeld bij hoeveel cases werkte het ensemble?"*

4. **Kerninzicht** (1 min 30) — toon slide 6. *"Twee patronen die jullie waarschijnlijk hebben gezien:* (1) als alle drie experts hetzelfde zeggen, voegt het ensemble niets toe — verspilde rekenkracht; (2) bij twijfelgevallen waar de experts uiteenlopen, wint het ensemble vaak — JUIST omdat ze verschillende fouten maken. *Dat tweede is hét principe achter ensembles in ML: diversiteit is voorwaarde."*

**Materiaal:**
- [ ] Slides 5-6
- [ ] wb-02-reflectie
- [ ] Flip-over voor wins-tracker
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag.
> - Bij stille tweetallen: stel een hardop-vraag: 'wie van jullie veranderde van mening op case 3?'
> - Het kerninzicht 'diversiteit is voorwaarde' is dé brug naar fase 3. Maak het expliciet — herhaal het steekwoord 2x.

> **Valkuil — discussie over 'wat is de juiste diagnose':**
> Twee deelnemers raken in technische discussie over wat de echte oorzaak is. Bedank, parkeer: 'Goeie discussie — bewaar voor straks. Voor nu: gaf het ensemble bij jou een ander antwoord?'

> **Differentiatie:**
> - **Gemengde groep:** Vraag eerst operator (welke case veranderde voor jou?), dan teamleider (wat zegt dat over modellen samenvoegen?).

---

### Blok 3: Twee families — bagging en boosting
**00:22 - 00:36** | 14 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert de twee hoofdfamilies van ensembles (bagging en boosting) kennen, kan ze onderscheiden, en koppelt elk aan een PdM-toepassing uit onderzoek.

**Werkvorm:** Trainer-geleide handout-bespreking met directe verbinding naar het diagnose-spel.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). Zeg: *"Pak je markeerstift. Tijdens het doorlopen markeer je wat voor jou nieuw is."*

2. **Brug van fase 2** (1 min) — toon slide 7. *"Wat jullie deden in het diagnose-spel — drie meningen middelen — was een vorm van bagging. Maar dat is niet de enige manier. Twee hoofdfamilies — die zien we nu."*

2b. **Optioneel — toon de video** (1 min 30) — als je in tempo zit, toon `video/composition.tsx` (~90s, 5 scenes). Zeg: *"Voor wie het visueel wil zien — eerst één expert op 75%, dan bagging met vijf modellen die stemmen, dan boosting als ketting. Dat is precies wat we nu in woorden gaan uitleggen, nu in beweging."* Geen bespreking achteraf — direct door naar bagging-uitleg.

3. **Familie 1 — Bagging** (4 min) — toon slide 8. *"Bagging — Bootstrap Aggregating. Train meerdere modellen ONAFHANKELIJK. Elk model krijgt een random subset van de data en de features. Daarna middel je hun voorspellingen — meerderheidsstem voor classificatie, gemiddelde voor regression. Verlaagt VARIANCE — als één model onstabiel was, het ensemble is stabieler."* Pauze. *"Beroemdste voorbeeld: Random Forest — een 'bos' van decision trees. Breiman, 2001."*

   Maak op flip-over scherp: **bagging = parallel + variance verlagen + Random Forest**.

4. **Familie 2 — Boosting** (4 min) — toon slide 9. *"Boosting — sequentieel werken. Eerste model traint op de data. Tweede model traint specifiek op WAT EERSTE FOUT DEED. Derde focust op de fouten van de tweede. Etc. Verlaagt BIAS — elke iteratie corrigeert systematische fouten."* Pauze. *"Beroemdste voorbeeld: Gradient Boosting — XGBoost, LightGBM. Wint heel veel Kaggle-competities. Friedman, 2001."*

   Maak op flip-over scherp: **boosting = sequentieel + bias verlagen + Gradient Boosting**.

5. **PdM-voorbeelden** (3 min 30) — toon slide 10. Loop drie cases af:
    - *"Wu et al. — Random Forest voor tool wear in dry milling. Bagging-stijl. Werkt goed omdat verschillende sensors verschillende patronen oppikken — diversiteit ontstaat vanzelf."*
    - *"Boosted decision tree voor pipe failure prediction. Boosting-stijl. Werkt goed bij onevenwichtige data: weinig failure-cases, veel normale. Boosting kan zich op die zeldzame failures focussen."*
    - *"Li, 2026 — ensemble RUL-prognose voor aircraft engines. Combinatie. Toont dat in PdM ensembles consequent betere voorspellingen geven dan losse modellen."*

6. **Brug naar fase 4** (1 min) — toon slide 11. *"Drie redenen waarom ensembles bij PdM zo vaak passen: (1) onevenwichtige data — weinig failures, veel normaal; (2) sensor-heterogeniteit — verschillende sensors zien verschillende patronen; (3) robuustheid — uitvalmodi variëren. Nu naar je eigen situatie."*

**Materiaal:**
- [ ] Slides 7-11
- [ ] wb-03-handout-bagging-boosting
- [ ] A3-diagram zichtbaar
- [ ] Markeerstift per deelnemer
- [ ] Flip-over

> **Tips voor de trainer:**
> - Maak op flip-over twee aparte rijen tegenover elkaar. Bagging en boosting moeten visueel anders staan — anders verwarren ze.
> - Gebruik de PdM-voorbeelden om concreet te maken — niet om te impressioneren met namen. Wu, Li blijven kort.
> - Vermijd XGBoost-internals tenzij iemand vraagt — parkeer dan.

> **Valkuil — bagging en boosting verwisseld:**
> Iemand zegt 'random forest is sequentieel'. Corrigeer met de twee axes op flip-over: parallel/sequentieel én variance/bias. Twee verschillende families.

> **Valkuil — 'altijd ensemble is beter':**
> Bevestig de neiging maar nuanceer: ensembles zijn duurder en moeilijker uit te leggen. Bij grote dataset + goed afgesteld model wint één model soms al genoeg. Trade-off.

> **Differentiatie:**
> - **MBO-4 basis:** Per familie één steekwoord (samen / na elkaar). Niet uitweiden over variance vs. bias — dat is onthoudbaar zonder de wiskunde.
> - **Teamleider sneller:** Vraag tussendoor: 'random forest vs. een 1D-CNN op vibration?' Antwoord: random forest werkt op handmatige features (RMS, kurtosis), CNN leert features zelf. Bridge naar lo-ai-fund-cnn-001.

---

### Blok 4: Actieplan — zou een ensemble onze PdM verbeteren?
**00:36 - 00:48** | 12 min | Kolb-fase: experimenteren

**Doel:** Deelnemer kiest één PdM-toepassing op de eigen lijn (of bij klant), beoordeelt of een ensemble passend zou zijn, en formuleert een vraag voor IT of leverancier.

**Werkvorm:** Individueel werkblad — trainer loopt rond.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Zeg: *"Laatste 12 minuten. Eén PdM-toepassing op je eigen lijn. Vier vragen op je werkblad: hoeveel failure-cases beschikbaar, is de data heterogeen (meerdere sensors), zou een ensemble passen, en zo ja welke familie — bagging of boosting?"*

2. **Inventarisatie-vraag** (1 min) — toon slide 12. *"Bij wie loopt PdM op de lijn? RUL-voorspelling, classificatie van uitvalmodes, anomaliedetectie? Spuitgieten, CNC, verpakking?"* Vang 4-5 antwoorden.

3. **Individueel werken** (8 min) — zet timer op 8 min. Loop rond. Stel concretiserende vragen:
    - *"Hoe vaak per jaar gaat deze machine echt stuk? 1, 5, 50?"*
    - *"Hoeveel sensors meten mee?"*
    - *"Heb je gelijke uitvalmodi of wisselt het?"*
    Bij 'we hebben weinig failure-data': bevestig — DAT is juist een argument voor ensembles. Help formuleren als vraag voor leverancier, niet als blokker.

4. **Plenaire ronde** (1 min 30) — toon slide 13. *"Twee deelnemers — kort: situatie + welke familie zou je vragen aan leverancier."* Vang 2 voorbeelden.

5. **Afsluiting + transferopdracht** (1 min) — toon slide 14. *"Deze week: kijk of er PdM op je lijn loopt. Vraag aan IT of leverancier: gebruikt het systeem een ensemble? Bagging-stijl (random forest) of boosting-stijl (gradient boosting)? Hoeveel failure-cases voor training? Bonus: bekijk een korte clip 'random forest explained simple' op YouTube — je ziet letterlijk hoe meerdere bomen samen stemmen."*

**Materiaal:**
- [ ] Slides 12-14
- [ ] wb-04-actieplan
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij 'we hebben geen PdM': hypothetisch project mag.
> - De plenaire ronde is goud voor volgende sessie.
> - Verwijs ook naar Isolation Forest video (lo-smart-mfg-107) voor wie unsupervised wil verkennen — dat is een ensemble in unsupervised territory.

> **Valkuil — actieplan blijft 'we hebben weinig data, dus niets':**
> Draai om: weinig failure-data is JUIST argument voor ensemble. Help formuleren als vraag, niet als blokker.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 10 min door werkblad-tijd op 7 min te zetten. Sla afsluiting nooit over.

> **Differentiatie:**
> - **MBO-4 basis:** Eén concrete situatie + één familie is genoeg.
> - **Teamleider sneller:** Vraag ook hoe ze ensemble vs. één model zouden uitleggen aan productie-manager. Houvast voor strategisch gesprek.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-diagnose-spel | n + 2 | A4 dubbelzijdig, 5 cases + tabel — **OF** vervang met tablets met `model-ensemble-stemming.jsx` |
| ☐ | wb-02-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-bagging-boosting | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-actieplan | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-ai-fund-ensemble-001.svg | 1 op A3 | Bagging vs. boosting, zichtbaar in zaal |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 2 | Parkeerlijst + wins-tracker / families |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5/6/8-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |
| ☐ | Optioneel: `video/composition.tsx` (Remotion `EnsembleVideo`) | 1 | ~90s, brug fase 2 → fase 3 |
| ☐ | Optioneel: tablets met `model-ensemble-stemming.jsx` | n | Parallel aan/vervangend voor wb-01 in fase 1 |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Diagnose-spel: 1 expert vs. 3 experts | Bij sommige cases verandert het antwoord |
| 2 reflecteren | Buurman + plenair wins-tracker | Inzicht: diversiteit is voorwaarde voor ensemble-winst |
| 3 theoretiseren | Handout bagging vs. boosting | Twee families, twee mechanismen, drie PdM-cases |
| 4 experimenteren | Eigen PdM-actieplan | Concrete situatie + gekozen familie + IT-vraag |

**Slagingscriterium:** ensemble in eigen woorden uitleggen + bagging vs. boosting onderscheiden + actieplan met PdM-koppeling.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met wins-tracker en families gefotografeerd
- [ ] Genoteerd: gemiddelde wins per case (verdeling = indicatie groepsbegrip)
- [ ] Notitie voor volgende sessie: wie ging IT bevragen?
- [ ] xAPI-statements verstuurd: `experienced` (diagnose-spel), `completed` (handout + actieplan), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | Ensemble Learning*
*Bronnen: Breiman (2001) Random Forests. | Schapire (1990) Strength of Weak Learnability. | Friedman (2001) Gradient Boosting. | Wu et al. — Random Forest tool wear. | Li (2026) ensemble RUL aircraft engines.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
