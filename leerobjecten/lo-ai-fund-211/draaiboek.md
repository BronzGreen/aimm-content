# No-code AI-tools voor de werkvloer — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden uitleggen wat een no-code AI-tool is, kent de drie standaard-stappen (data uploaden, model trainen, model testen), kiest voor minimaal 4 van 6 werkvloer-scenario's beargumenteerd WEL of NIET, en benoemt voor zijn eigen vraagstuk één AVG-overweging (cloud versus offline). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 (Gebruik) afgerond + lo-ai-fund-205 (data labelen) + lo-ai-fund-022 (neuraal netwerk in grote lijnen) + lo-ai-fund-132 (trainingsdata-kwaliteit) |
| **Stadium (Hersey & Blanchard)** | Bewust bekwaam — theorie van AI bekend (Module 1), drie stappen van no-code-tool nog niet zelf gezien |
| **Begeleidingsstijl (manier van begeleiden)** | Coachen — hoge relatiegerichtheid, lagere taakgerichtheid; vragen-stellen i.p.v. antwoord-geven |
| **Ruimte** | U-opstelling of clusters van 2-4 (buurman moet naast deelnemer kunnen zitten), beamer + scherm, **demo-laptop met Teachable Machine vooraf getest**, flip-over of bord, **stabiele internetverbinding** |
| **Plek in module** | Tweede hands-on LO van Module 2 (Train). Brengt Module-1-theorie en lo-205-labelwerk samen in een echte tool — én introduceert AVG als operator-vraagstuk. |
| **Bloom-niveau** | Toepassen — drie stappen benoemen + scenario-keuze + AVG-overweging |
| **Kirkpatrick-niveau** | Gedrag — concrete actie deze week (Teachable Machine thuis + twee vragen voor IT) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type (Kolb-fase / leerfase) | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | LIVE-demo Teachable Machine — drie stappen | 🟢 ervaren | 10 min |
| 00:10 - 00:20 | Zes scenario's — WEL / NIET / TWIJFEL | 🟣 reflecteren | 10 min |
| 00:20 - 00:35 | Handout — WEL / NIET / AVG | 📘 theoretiseren | 15 min |
| 00:35 - 00:45 | Eigen werkvloer-keuze + actie deze week | 🟠 experimenteren | 10 min |

**Totaal:** 45 minuten.
**Buffer:** 1 min per blok flexibel (kan opgenomen worden in fase 3).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve per werkblad.
- [ ] Test de Slidev-presentatie (`lo-ai-fund-211-presentatie.slidev.md`) op de beamer.
- [ ] Verzamel fictieve dataset: 20 foto's schroeven mét kop + 20 schroeven zonder kop (alternatief: 20 fietsen + 20 auto's). **Geen werkvloer-data — dat triggert AVG-discussie te vroeg.**
- [ ] Lees blok 3 van de handout (wb-03) één keer hardop voor jezelf — drie blokken vlot achter elkaar.

### 30 min ervoor — niet-onderhandelbaar
- [ ] Open Teachable Machine (https://teachablemachine.withgoogle.com) in je browser.
- [ ] **Doorloop zelf de drie stappen één keer** met de voorbereide fictieve dataset. Train één model van begin tot eind. Test met een twijfelgeval (halve schroef, ongebruikelijke hoek).
- [ ] Noteer waar elke knop *vandaag* staat (UI kan zonder waarschuwing zijn veranderd).
- [ ] **Maak backup-screenshots** van stap 1 (drag-and-drop), stap 2 (voortgangs-balk), stap 3 (testen + twijfelgeval). Sla op als losse slides die je via presenter-modus kunt openen als de live-tool faalt.
- [ ] Check internetverbinding op locatie. Plan B als WiFi onbetrouwbaar: hotspot van je telefoon.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `NoCodeAiVideo`, ~90s, 5 scenes) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Plan B voor fase 1 als LIVE-demo écht niet werkt.
- [ ] **Optioneel — interactief klaarzetten:** als je in fase 2 digitaal wilt: laad `model-no-code-scenario-sorteer.jsx` (8 scenario's, drempel 6/8) op een React-sandbox en test op één tablet. Het AVG-werknemer-scenario bewaar je voor plenaire bespreking aan eind fase 2.

### Het uur ervoor
- [ ] Leg per stoel klaar: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel — deel je per fase opnieuw uit.
- [ ] Bord of flip-over voorbereiden — twee zichtbare velden klaar (nog niet ingevuld, pas onthullen tijdens fase 2):
  - Veld 1: *"Snelheid = knelpunt"* (komt bij scenario 4)
  - Veld 2: *"AVG = mogen, niet kunnen"* (komt bij scenario 6 + blok 3)
- [ ] Open Slidev in presenter-modus, slide 1.
- [ ] Open Teachable Machine in een aparte tab — klaar voor stap 1.
- [ ] Zet stoelen zo dat elke deelnemer een buurman naast zich heeft.

---

## Blok-details

### 🟢 Blok 1: LIVE-demo Teachable Machine — drie stappen in 90 seconden
**00:00 - 00:10** | 10 min | Kolb-fase (leerfase): ervaren

**Doel:** Deelnemer ziet voor het eerst een no-code AI-tool LIVE in actie. Begrijpt zonder uitleg vooraf dat dit dezelfde labels uit lo-ai-fund-205 zijn, alleen nu als drag-and-drop. Ervaart dat accuratesse geen vaste waarde is.

**Werkvorm:** Plenaire opening (1 min), LIVE-demo van de tool met drie stappen (8 min), brug naar fase 2 (1 min). Trainer IK DOE; deelnemers kijken mee + vullen wb-01 in.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 45 minuten zien jullie hoe een AI-model wordt gemaakt zonder dat je een regel code schrijft. Vorige week labelden jullie op papier. Vandaag zien jullie diezelfde labels als drag-and-drop in een echte tool — en leren wanneer no-code wel én niet past."* Pauze 5 seconden.

2. **Werkblad uitdelen + tool tonen** (1 min) — deel wb-01 uit. Schakel over naar de Teachable Machine browser-tab. Toon het scherm. Zeg: *"Dit is Teachable Machine van Google. Gratis, geen account nodig. Op dit lege scherm bouwen wij in 90 seconden een AI-model. Jullie kijken. Per stap noteer je één observatie op wb-01."*

3. **LIVE — Stap 1: data uploaden** (2 min) — toon op het scherm de twee lege klasse-vakken. Hernoem ze: *"Klasse 1 — schroef MET kop"* en *"Klasse 2 — schroef ZONDER kop"* (of jouw gekozen dataset). Sleep nu de 20 + 20 foto's per klasse in. Zeg hardop: *"Stap 1 — data. Ik sleep 20 foto's in elke klasse. Dit zijn jullie labels van vorige week — alleen nu sleep ik ze in plaats van schrijf ik ze."*

4. **LIVE — Stap 2: model trainen** (2 min) — druk op de train-knop. De voortgangs-balk loopt 20-40 seconden. Wijs aan: *"Stap 2 — trainen. Dit is dezelfde wiskunde als in een neuraal netwerk uit Module 1 — alleen jij ziet alleen de balk."* Wacht stil tot de balk vol is. Niet pratend de tijd vullen.

5. **LIVE — Stap 3: model testen** (2 min) — houd een nieuwe foto voor de webcam (of upload). Het model geeft een label + accuratesse-percentage. Lees voor: *"Stap 3 — testen. Het model zegt: 'schroef met kop — 92 procent'."* Toon **bewust een twijfelgeval**: een halve schroef of ongebruikelijke hoek. Wijs aan: *"Kijk — bij dit voorbeeld daalt het percentage. Het model is hier minder zeker. Dat is wat precision (precisie) betekent."*

6. **Alternatief — video i.p.v. LIVE** (vervangend, alleen als LIVE-demo niet kan) — als WiFi écht uitvalt of UI onherkenbaar is veranderd: speel `video/composition.tsx` (Remotion `NoCodeAiVideo`, ~90s) af op de beamer. Benoem hardop wat je *zou* doen tijdens scene 2 (drie-stappen-workflow): *"Hier zou ik nu 20 foto's slepen, dan op trainen drukken, dan een nieuw beeld voor de camera houden."* Sla scene 5 (transfer) over — die komt in fase 4.

7. **Open vraag + brug** (2 min) — sluit de tool-tab niet, laat hem zichtbaar. Toon slide met de open vraag: *"Welke knop heb ik echt zelf bedacht — en welke deed de tool?"* Wacht 5-7 seconden in stilte. Verzamel 2-3 antwoorden zonder zelf het 'juiste' antwoord te geven. Sluit af: *"Vul nu kort wb-01 in. Drie observaties — één per stap. En één vraag die je nog hebt."* Geef 1-2 minuten om af te ronden tijdens de overgang.

**Materiaal:**
- [ ] Slide 1-3
- [ ] wb-01-observatie-demo.md (1 per deelnemer)
- [ ] Demo-laptop met Teachable Machine **vooraf getest**
- [ ] Internetverbinding (cloud-tool)
- [ ] **Backup-screenshots** klaar in presenter-modus
- [ ] **Optioneel:** `video/composition.tsx` (Remotion `NoCodeAiVideo`, ~90s) — als alternatief voor LIVE-demo
- [ ] Pen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke open vraag. Stilte is je vriend — vooral bij de slot-vraag *"welke knop heb ik echt zelf bedacht?"*
> - Vermijd jargon. Zeg 'het model' (niet 'classifier'), 'accuratesse-percentage' (niet 'confidence score'), 'data uploaden' (niet 'dataset ingest'). Eén uitzondering: *precision (precisie)* — die mag, met NL-haakje, omdat het in latere LOs terugkomt.
> - Toon de voortgangs-balk volledig. Geen knip. Stilte tijdens het trainen is OK — het maakt zichtbaar dat je niet weet wat er onder de motorkap gebeurt.

> **🔴 Valkuil — demo wordt theoretisch in plaats van LIVE:**
> WiFi haperde, of UI is sinds je voorbereiding net veranderd. **LIVE is niet-onderhandelbaar.** Als de tool écht niet werkt: open de backup-screenshots, klik er één voor één doorheen en benoem wat je normaal zou doen — *"Hier zou ik nu 20 foto's slepen."* Niet doen alsof het 'ook wel theoretisch kan'. Voorbereiding 30 min vooraf voorkomt dit in 90 procent van de gevallen.

> **🔴 Valkuil — Teachable Machine UI is veranderd:**
> Google update zonder waarschuwing. Benoem het als het anders is dan je had verwacht: *"Normaal staat deze knop links; vandaag staat hij rechtsboven. Het principe blijft hetzelfde — data, trainen, testen."* Maakt het juist concreter dat de drie stappen het echte anker zijn, niet de bediening.

> **🔴 Valkuil — accuratesse als magie tonen:**
> Sla nooit het twijfelgeval over. Een tool die altijd 92 procent zegt, lijkt magisch. Een tool die bij een halve schroef naar 51 procent zakt, laat zien wat het model wel en niet kan.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Doe stap 2 (trainen) extra langzaam — laat de voortgangs-balk volledig zien, geen knip. Bij stap 3 nog één extra twijfelgeval om zichtbaar te maken dat accuratesse varieert.
> - **Teamleider sneller:** Bij snel klaar: vraag *"Welke van de drie stappen lijkt het meest op iets wat al op jullie lijn gebeurt?"* — activeert transferdenken vóór fase 2.

**Antwoordmodel werkblad 1:**

Bewust geen sluitende sleutel. De drie observaties zijn vrij beschrijvend. Typische uitkomsten per stap:

| Stap | Verwachte observatie | Toets |
|---|---|---|
| 1 — Data | "Trainer sleept foto's per klasse"; "twee groepen op het scherm" | Concreet zien — geen abstract 'data inladen' |
| 2 — Trainen | "Voortgangs-balk loopt 20-40 sec"; "er gebeurt iets, maar je ziet niet wat" | Tijd genoteerd + erkenning van de zwarte doos |
| 3 — Testen | "Tool zegt label + percentage"; "bij twijfelgeval daalt het percentage" | Percentage gezien + variatie opgemerkt |
| Vraag | "Waar gaan mijn foto's heen?" / "Werkt dit op een productielijn?" / "Hoeveel foto's heb ik nodig?" | Eén vraag is genoeg — wordt anker voor fase 3 |

Vragen die opduiken zijn de brug naar fase 3 — verzamel ze op de flip-over voordat je verder gaat.

**Transitie naar blok 2:** *"Jullie zien nu wat de tool kan in drie stappen. De vraag is: past dit bij élk werkvloer-vraagstuk? Tweetal met je buurman — zes scenario's."*

---

### 🟣 Blok 2: Zes scenario's — WEL / NIET / TWIJFEL
**00:10 - 00:20** | 10 min | Kolb-fase (leerfase): reflecteren

**Doel:** Deelnemer ontdekt door duo-werk dat no-code niet voor élk vraagstuk geschikt is. Ervaart dat AVG (mogen) een aparte vraag is naast technisch kunnen. Drie verschillen tussen duo's worden plenair geoogst.

**Werkvorm:** Werkblad uitleg (1 min), duo-werk zes scenario's (5 min), plenair scenario 4 (snelheid) + scenario 6 (AVG) (4 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-02 uit. **OF** deel tablets uit met `model-no-code-scenario-sorteer.jsx` geopend. Zeg bij papier: *"Tweetal met je buurman. Zes werkvloer-scenario's. Per scenario kruis je aan: WEL passend, NIET passend, of TWIJFEL. Plus één reden in maximaal acht woorden. TWIJFEL is een legitieme keuze als je twee dimensies ziet."* Zeg bij digitaal: *"Acht werkvloer-scenario's op je tablet. Per scenario klik je WEL of NIET — je krijgt direct feedback op vier criteria: dataset-grootte, retraining-frequentie, complexiteit, kritikaliteit. Streef naar minimaal 6 van 8 correct. Eén scenario gaat over werknemer-foto's — daar komen we plenair op terug."*

2. **Duo-werk** (5 min) — zet timer op 5 minuten. Zeg expliciet: *"Vergelijk niet wie gelijk heeft. Bespreek samen waarom jullie kiezen wat jullie kiezen."* Loop rond na 2 minuten. Coach bij vastlopers met grens-vragen:
   - *"Kijk naar de demo van net — werkt dat hier ook in drie stappen?"*
   - *"Of zit er iets in dit scenario dat je niet kunt slepen in een tool?"*
   - *"Wat is hier het knelpunt — de hoeveelheid data, de snelheid, of iets anders?"*

3. **Plenair scenario 4 — snelheid** (2 min) — toon slide met scenario 4 (real-time afkeur 600 producten/min). Vraag twee duo's: *"Wat hebben jullie gekozen — en waarom?"* Verzamel hun redenering OP HET BORD voordat je zelf iets zegt. Pas dan onthul je veld 1: **"Snelheid = knelpunt"**. Zeg: *"Een no-code tool kan dit type model wel maken — maar niet draaien op 10 voorspellingen per seconde. Voor productie heb je een productie-versie nodig die door IT of een leverancier wordt gebouwd."*

4. **Plenair scenario 6 — AVG** (2 min) — toon slide met scenario 6 (HR-camera werknemer-gezichten). Vraag twee duo's: *"Wat hebben jullie gekozen — en waarom?"* Wacht op hun antwoord. Pas dan onthul je veld 2: **"AVG = mogen, niet kunnen"**. Zeg: *"Technisch kun je dit in drie stappen bouwen. Maar onder AVG mag je werknemer-gezichten niet zomaar door een cloud-AI laten herkennen. Hier gaat het niet over kunnen — het gaat over mogen. Dat is de derde dimensie."* Pauze 5-7 seconden. Markeer: *"De andere scenario's bewaren we voor de handout."*

**Materiaal:**
- [ ] Slides scenario-overzicht + scenario 4 + scenario 6
- [ ] wb-02-zes-scenarios.md **OF** tablets/laptops met `model-no-code-scenario-sorteer.jsx` geopend (8 scenario's incl. AVG-werknemer-foto's)
- [ ] Bord of flip-over met twee voorbereide velden (nog niet ingevuld)
- [ ] Stiften
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Onthul de twee bord-velden ("Snelheid = knelpunt", "AVG = mogen, niet kunnen") pas NA de duo-redenering. Onthul je ze te vroeg, dan kalibreren alle duo's stiekem op jouw antwoord.
> - Bij stilte op de kernvraag *"Wat hebben jullie gekozen — en waarom?"* — tel tot 7. Daarna een hint: *"Was het de snelheid die jullie zorgen baarde? Of iets anders?"*
> - TWIJFEL is geen zwakte. Reframen: *"TWIJFEL met onderbouwing is een volwassen antwoord — het zegt dat je twee dimensies zag."*

> **🔴 Valkuil — plenaire scenario-bespreking wordt eindoordeel:**
> Trainer geeft direct het 'juiste' antwoord (real-time = NIET, HR-camera = AVG-NIET) zonder eerst twee duo's te bevragen. Daarmee leert de groep 'het antwoord' i.p.v. de redenering. Op een nieuw scenario op de eigen lijn kunnen ze dan niets. Vraag dus EERST. Markeer pas DAARNA.

> **🔴 Valkuil — alle zes scenario's plenair willen oogsten:**
> Houd het op twee (4 en 6). De andere vier scenario's (1, 2, 3, 5) komen terug bij de handout. *"Houd je andere redenering vast — daar komen we bij blok 3 op terug."*

> **🔴 Valkuil — AVG bagatelliseren:**
> Iemand zegt *"AVG is gezeur van privacy-mensen"*. Niet meegaan. Reframen kort: *"AVG is geen formaliteit — het is een werkvloer-vraag. Werknemer-foto's zijn van die werknemers. Hoe zou jij het vinden als jouw gezicht in een cloud-AI in de VS belandde zonder dat iemand het je vroeg?"* Daarna door.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Doe één scenario eerst plenair voor (bv. scenario 1 — visuele afkeur inpaklijn) — modelleer hoe je tot WEL/NIET komt. Dan pas duo-werk op scenario 2-6.
> - **Teamleider sneller:** Bij snel klaar: *"Welk scenario lijkt het meest op een vraagstuk uit jouw team? En wat zou jij als teamleider als eerste vraag aan IT stellen?"*
> - **Gemengde groep:** Combineer in duo's operator (past dit in drie stappen?) met teamleider (wie zou dit beheren?).

**Antwoordmodel werkblad 2:**

| Scenario | Verwacht | Reden |
|---|---|---|
| 1 — Visuele afkeur inpaklijn | WEL | Visie + eenvoudig label + kleine dataset |
| 2 — Voorspellen pomp-uitval (20 kolommen × 6 mnd) | NIET | Ingewikkelde tabel-data — meerdere bronnen, transformaties nodig |
| 3 — Sorteren schroeven prototype | WEL | Visie + prototype + klein team |
| 4 — Real-time 600/min | NIET | Snelheid — productie-versie nodig |
| 5 — Klein team prototype, geen budget | WEL | Prototype + klein team — exact waar no-code voor is |
| 6 — HR-camera werknemer-gezichten | NIET (op AVG-gronden) | Kunnen WEL, mogen NIET zonder wettelijke basis |

Succescriterium: minimaal 4 van 6 beargumenteerd. TWIJFEL is OK indien onderbouwd (bv. scenario 5 kan TWIJFEL zijn omdat "geen budget" organisatorisch is).

**Transitie naar blok 3:** *"Jullie hebben net zelf de WEL/NIET-grens gevoeld. En jullie zagen dat AVG een aparte vraag is. Tijd om er taal op te zetten — vier WEL-criteria, vier NIET-criteria, en het AVG-blok."*

---

### 📘 Blok 3: Handout — WEL / NIET / AVG
**00:20 - 00:35** | 15 min | Kolb-fase (leerfase): theoretiseren

**Doel:** Deelnemer kent vier WEL-criteria (visie, audio, eenvoudige tabel-data, prototype) plus aanvulling klein team, kent vier NIET-criteria (ingewikkelde tabel-data, real-time, grote datasets, streng gereguleerd), en herkent het AVG-onderscheid tussen voorbeelddata (cloud meestal OK) en eigen werkvloer-data (offline of bewuste afweging).

**Werkvorm:** Handout uitdelen (1 min), blok 1 — WEL passend (4 min), blok 2 — NIET passend (4 min), blok 3 — AVG-impact (5 min), markeer-moment (1 min).

**Instructie:**

1. **Handout uitdelen + markeerstift** (1 min) — deel wb-03 uit. Zeg: *"Drie blokken op de handout. Eerst WEL — wanneer past no-code wél. Dan NIET — wanneer past het niet. Dan AVG — een aparte vraag. Pak je markeerstift — aan het eind markeer je wat voor jouw werkvloer geldt."*

2. **Blok 1 — WEL passend, met terugkoppeling** (4 min) — toon slide blok 1. Doorloop één voor één, koppel aan scenario's uit fase 2:
   - **Visie** — *"Foto's of camera-beelden labelen. Voorbeeld: afkeur op de inpaklijn. Jullie hebben dit net als scenario 1 als WEL aangekruist."*
   - **Audio** — *"Geluid-patronen herkennen. Voorbeeld: tikkende pomp."*
   - **Eenvoudige tabel-data** — *"Twee of drie kolommen, minder dan 1000 rijen. Voorbeeld: temperatuur + druk → goedkeur/afkeur."*
   - **Prototype** — *"Een snelle test of AI eigenlijk kan helpen. Voorbeeld: scenario 3 en scenario 5 uit fase 2 — sorteer-prototype en klein team."*
   - **Klein team zonder data-scientist** — *"Een operator met één dag training kan dit zelf. Dat is precies wat no-code uniek maakt."*

3. **Blok 2 — NIET passend, met terugkoppeling** (4 min) — toon slide blok 2. Doorloop één voor één:
   - **Ingewikkelde tabel-data** — *"Vele kolommen, meerdere bronnen, transformaties. Scenario 2 uit fase 2 — pomp-uitval met 20 kolommen sensor-data — viel hieronder."* Wijs naar bord-veld 1 (snelheid is een andere reden).
   - **Real-time productie** — *"Honderden voorspellingen per seconde. Scenario 4 — 600 producten per minuut — viel hieronder. Wijs naar bord: 'Snelheid = knelpunt'."*
   - **Grote datasets** — *"Vanaf 100.000 voorbeelden hebben no-code tools limieten. Een heel jaar productiedata over alle ploegen is meestal te groot."*
   - **Streng gereguleerd** — *"AVG-strict of ISO-gecertificeerd. Medische diagnose, financiële kredietbeoordeling. Daar moet meer onder de motorkap zichtbaar zijn."*

4. **Blok 3 — AVG-impact** (5 min) — toon slide blok 3. Onthul nu de kernvraag op het bord: **"Voorbeelddata of eigen werkvloer-data?"** Zeg langzaam:

   - *"Veel no-code tools sturen je trainings-data naar cloud-servers. Vaak in de VS. Of dat OK is, hangt af van WAT je uploadt."*
   - *"**Voorbeelddata** — fictieve sets, fietsen, schroeven, openbare datasets — geen persoonsgegevens, geen bedrijfsgeheimen. Cloud is meestal prima. Dat is precies waarom ik vandaag schroeven gebruikte voor de demo en geen werknemer-foto's."*
   - *"**Eigen werkvloer-data** — werknemer-gezichten, productiedata met bedrijfsgeheimen. Cloud is onder AVG NIET acceptabel zonder uitdrukkelijke wettelijke basis. Scenario 6 uit fase 2 — HR-camera — viel hieronder."* Wijs naar bord-veld 2: *"AVG = mogen, niet kunnen."*
   - *"**Alternatief** — kies een tool die offline kan draaien. Microsoft Lobe heeft een offline-modus. Of vraag IT om een lokale variant. Het hoeft geen dealbreaker te zijn — alleen een bewuste keuze."*
   - **Werkvloer-voorbeeld als afsluiter:** *"MKB-fabriek, 40 medewerkers, geen IT-afdeling. Operator wil weten of de sticker recht op het product zit. Verzamelt 200 foto's 'label correct' en 200 foto's 'scheef of ontbreekt'. Sleept ze in Teachable Machine. Drukt op trainen. Krijgt 88 procent accuratesse. Geen perfect model — maar genoeg om de eigenaar te overtuigen om verder te investeren in een productie-versie met IT. Eén week werk. Zonder no-code was dit prototype nooit gebouwd."*

5. **Markeer-moment** (1 min) — zeg: *"Pak je markeerstift. Markeer één WEL-criterium dat voor jouw werkvloer het meest relevant is. Markeer één NIET-criterium dat voor jou het grootste risico is. En markeer bij AVG of jouw werkvloer-data dichter bij 'voorbeelddata' of bij 'identificeerbare info' zit."*

**Materiaal:**
- [ ] Slides blok 1 + blok 2 + blok 3 + werkvloer-voorbeeld
- [ ] wb-03-handout-wel-niet-avg.md
- [ ] Markeerstift per deelnemer
- [ ] Bord (twee velden zichtbaar uit fase 2 + kernvraag blok 3)

> **💡 Tips voor de trainer:**
> - Bij elk criterium één directe terugkoppeling naar fase 2 of fase 1. Anders blijft het lijstjes-kennis.
> - De AVG-kernzin (*"mogen, niet kunnen"*) en de scheidslijn voorbeelddata/eigen werkvloer-data zijn de twee anker-uitspraken — herhaal ze in fase 4.
> - Werkvloer-voorbeeld aan het eind nooit overslaan. Het is wat een operator concreet meeneemt — *"dit is wat één week werk oplevert"*.

> **🔴 Valkuil — AVG-blok behandelen als formaliteit:**
> Trainer leest blok 3 voor zonder expliciet aan scenario 6 te koppelen, of zegt *"AVG is een formaliteit voor IT"*. AVG is een operator-vraagstuk. Stel expliciet de plenaire vraag: *"Wie van jullie heeft op de eigen lijn al eens een AI-tool zien waarbij niemand wist waar de data heen ging?"* Tel tot 7. Het gesprek dat dan ontstaat is het hart van blok 3.

> **🔴 Valkuil — handout in één lap voorlezen:**
> Drie blokken — niet één. Tussen WEL en NIET: ademhalen, vraag *"Welk WEL-criterium pas jij het meeste tegen?"* Tussen NIET en AVG: *"Wie heeft op de eigen lijn een AVG-vraag zien spelen die niemand stelde?"* Adempauzes maken de overgang concreet.

> **🔴 Valkuil — vier WEL-criteria als losse begrippen:**
> Bij elk criterium terug naar fase 2: *"Jullie hebben dit net als scenario X als WEL aangekruist."* Niet *"visie betekent..."*. De ervaring komt eerst, de naam erbij.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Schrijf vier WEL- en vier NIET-criteria groot op het bord — laat ze staan voor fase 4. Bij blok 3: extra tijd voor het werkvloer-voorbeeld, met de cijfers (200+200, 88%, één week) op een aparte slide.
> - **Teamleider sneller:** Vraag: *"Welk WEL-criterium hebben jullie op de werkvloer al, maar wordt nog niet voor AI benut? Welk NIET-criterium is bij jullie de grootste struikel?"* Activeert systeem-blik.
> - **Bij weinig tijd:** Houd vier WEL- en vier NIET-criteria vast plus AVG-kernzin; werkvloer-voorbeeld kun je inkorten tot één zin — maar niet weglaten.

**Antwoordmodel werkblad 3:**

| Element | Verwacht | Toets |
|---|---|---|
| Eén WEL-criterium gemarkeerd | Markeerstift-aanstreping | Geen 'goed/fout' — keuze is persoonlijk |
| Eén NIET-criterium gemarkeerd | Markeerstift-aanstreping | Idem |
| AVG-zelfinschatting | "Voorbeelddata" / "identificeerbare info" / "grijs gebied" | Eén van drie aangekruist |
| Veelgekozen WEL | Visie + klein team | Logisch want demo + scenario 1, 3, 5 net beleefd |
| Veelgekozen NIET | Real-time + streng gereguleerd | Logisch want scenario 4 net besproken + AVG-blok |

**Transitie naar blok 4:** *"Vier WEL-criteria ken je nu. Vier NIET-criteria herken je. AVG snap je als 'mogen, niet kunnen'. Nu jouw beurt — één werkvloer-vraagstuk."*

---

### 🟠 Blok 4: Eigen werkvloer-keuze + actie deze week
**00:35 - 00:45** | 10 min | Kolb-fase (leerfase): experimenteren

**Doel:** Deelnemer kiest één concreet werkvloer-vraagstuk, doorloopt zelf de beslis-checklist (datatype, volume, real-time/prototype, AVG), maakt een onderbouwde keuze WEL / NIET / TWIJFEL, en formuleert één concrete eerste stap voor deze week.

**Werkvorm:** Werkblad-uitleg (1 min), individueel werken (6 min), plenaire ronde één-zin-per-persoon (2 min), transferopdracht (1 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit. Toon slide met de vier stappen. Zeg: *"Laatste 10 minuten. Vier stappen op het verkenningsblad. Stap 1 — kies één concreet werkvloer-vraagstuk waar AI mogelijk kan helpen. Stap 2 — beantwoord vier vragen op het blad. Stap 3 — kruis WEL / NIET / TWIJFEL aan. Stap 4 — schrijf één concrete eerste stap voor deze week. Geen IT-kennis nodig."*

2. **Individueel werken** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. CAR (competentie/autonomie/relatedness): bij vastlopers coach door met grens-vragen:
   - *"Welk werkvloer-moment gaat nu handmatig dat AI mogelijk zou kunnen ondersteunen — een visuele check, een sortering, een afkeur-moment?"*
   - *"Is dit beeld, geluid, of tabel-data? Kun je het in drie stappen zien — data uploaden, model trainen, model testen?"*
   - *"Hoeveel voorbeelden heb je? Minder dan 1000, of veel meer?"*
   - *"Bevat de data persoonsgegevens of bedrijfsgeheimen? Of zijn het neutrale productfoto's?"*
   - *"Wat zou jij als eerste in een cloud zetten — en wat juist niet?"*

3. **Plenaire ronde** (2 min) — toon slide. Zeg: *"Eén ronde — iedereen één zin: welk vraagstuk heb je gekozen, en welke keuze (WEL / NIET / TWIJFEL)?"* Houd kort — max 15 seconden per persoon. Bevestig TWIJFEL: *"Twijfel + IT raadplegen is een volwassen antwoord — het zegt dat je twee dimensies hebt gezien."* Begin zelf met een voorbeeld als de stilte te lang duurt: *"Bij mij zou het zijn: 'inspectiecamera op de inpaklijn' — WEL, want visie + prototype. Actie deze week: vragen aan IT welke camera-data al beschikbaar is."*

4. **Transferopdracht + afsluiting** (1 min) — toon slide met de transferopdracht. Zeg: *"Deze week drie stappen op je eigen lijn. Eén — zoek één werkvloer-moment waar AI mogelijk kan helpen, beschrijf in drie zinnen. Twee — open thuis Teachable Machine in een browser, doe de drie stappen zelf met een eenvoudige dataset. Bewust GEEN bedrijfsdata of werknemer-foto's — kies fietsen, koffiekopjes of schroeven. Drie — bedenk twee vragen voor IT of kwaliteit. Bijvoorbeeld: 'welke camera-data hebben we al?' En: 'mogen productiefoto's in een cloud-tool — of moet het offline?' Neem alle drie de uitkomsten mee naar de volgende sessie. Bonus: praat deze week met een collega over wat jullie als team van AI verwachten op de lijn."*

**Materiaal:**
- [ ] Slides werkblad-overzicht + transferopdracht
- [ ] wb-04-eigen-keuze-no-code.md
- [ ] Pen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Plenair: max 15 seconden per persoon. Eindig op tijd. Een goede afsluiting is beter dan uitlopen.
> - Bij iemand die geen werkvloer-vraagstuk kan bedenken: geef twee suggesties (inspectiecamera, sortering, afkeur-moment) en laat deelnemer kiezen.
> - Bij TWIJFEL: reframen actief — *"TWIJFEL met onderbouwing is sterker dan een gokje WEL of NIET. Je hebt twee dimensies gezien."*

> **🔴 Valkuil — bedienings-instructies geven i.p.v. de keuze coachen:**
> Een deelnemer vraagt *"maar HOE upload ik die foto's"*. Niet uitleggen. Reframen: *"De drie stappen ken je nu uit fase 1 — data, trainen, testen. De vraag in dit LO is niet HOE maar OF — past dit type vraagstuk in drie stappen? Welk scenario uit fase 2 lijkt het meest op jouw vraagstuk?"* Tool-bediening komt in een vervolg-LO.

> **🔴 Valkuil — actie deze week te abstract:**
> *"Ik ga erop letten"* of *"Ik ga er eens naar kijken"* is geen actie. Begrens: *"Wat doe je precies, wanneer, met wie?"* Voorbeeld: *"Donderdagmiddag vraag ik aan IT-Esra welke camera-data we al hebben."*

> **🔴 Valkuil — werkvloer-vraagstuk te abstract:**
> *"AI-implementatie in mijn afdeling"* is te groot. Begrens: *"Eén concreet moment — een visuele check, een sorteer-beslissing, een afkeur-moment. Wat zie jij iemand nu handmatig doen wat AI mogelijk zou kunnen ondersteunen?"*

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers — geef twee voorbeelden van werkvloer-vraagstukken (inspectiecamera, sortering) en laat deelnemer kiezen. Help met de eerste vraag (datatype) — daarna kan de deelnemer zelf verder.
> - **Teamleider sneller:** Bij snel klaar: *"Hoe ga jij in jouw team systematisch in beeld brengen welke processen kandidaat zijn voor een no-code prototype?"* Strategische blik.
> - **Bij niet-werkvloer-deelnemer (zeldzaam):** Laat hem een hypothetisch vraagstuk kiezen uit de zes scenario's van fase 2 en doorloop daarmee de vier stappen.

**Antwoordmodel werkblad 4:**

| Stap | Verwacht | Toets |
|---|---|---|
| 1 — Werkvloer-vraagstuk | Concreet benoemd (inspectiecamera, sortering, afkeur, visuele eindcontrole) | Niet abstract ('kwaliteit') |
| 2 — Vier vragen | (a) beeld/audio/tabel (b) <1000 / 1000-100k / >100k (c) real-time of prototype (d) persoonsgegevens of bedrijfsgeheimen | Concreet antwoord per vraag |
| 3 — Keuze | WEL / NIET / TWIJFEL aangekruist | TWIJFEL legitiem bij twee dimensies |
| 4 — Actie deze week | Wat-wanneer-met-wie | Niet *"ik ga erop letten"* |

**Veelvoorkomende werkvloer-vraagstukken:**
- Inspectiecamera op visuele kwaliteitslijn
- Sorteersysteem op formaat of kleur
- Visuele eindcontrole bij assemblage
- Afkeur-systeem op spuitgietproducten

**Veelvoorkomende acties voor deze week:**
- Open Teachable Machine thuis met fictieve dataset, doorloop de drie stappen
- Vraag aan IT of kwaliteit: *"Welke camera-data hebben we al beschikbaar?"*
- Vraag aan IT of kwaliteit: *"Mogen productiefoto's in een cloud-tool — of moet het offline?"*

**Transitie naar afsluiting:** *"Mooi werk. Drie stappen deze week — Teachable Machine zelf openen, twee vragen voor IT, en een gesprek met een collega. Volgende sessie hoor ik graag welk werkvloer-moment ieder van jullie heeft gekozen — en welk antwoord IT gaf over jullie productiedata."*

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-observatie-demo | n + 2 | A4 enkelzijdig (drie observatie-velden + één vraag) |
| ☐ | wb-02-zes-scenarios | n + 2 | A4 enkelzijdig (zes scenario's + WEL/NIET/TWIJFEL + redenenveld) — **OF** vervang door tablets met `model-no-code-scenario-sorteer.jsx` (8 scenario's, drempel 6/8, AVG-werknemer-scenario inbegrepen) |
| ☐ | wb-03-handout-wel-niet-avg | n + 2 | A4 dubbelzijdig (drie blokken WEL/NIET/AVG + markeer-veld) |
| ☐ | wb-04-eigen-keuze-no-code | n + 2 | A4 enkelzijdig (vier stappen + actie) |
| ☐ | Pennen | n + 5 | Reserve |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Flip-over of bord | 1 | Twee velden: 'Snelheid = knelpunt' + 'AVG = mogen, niet kunnen' |
| ☐ | Dikke stiften | 2-3 | |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Demo-laptop met webcam | 1 | Voor live-test in stap 3 |
| ☐ | Internetverbinding | 1 | Stabiel — cloud-tool, hotspot als backup |
| ☐ | Teachable Machine vooraf getest | 1 | 30 min van tevoren één model doorlopen |
| ☐ | Backup-screenshots stap 1-2-3 | 1 set | Klaar in presenter-modus voor noodgeval |
| ☐ | Fictieve dataset (20+20 foto's) | 1 set | Schroeven met/zonder kop, of fietsen/auto's — bewust GEEN werkvloer-data |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | Presenter-modus |
| ☐ | Optioneel: `video/composition.tsx` (Remotion `NoCodeAiVideo`) | 1 | ~90s, alternatief voor LIVE-demo |
| ☐ | Optioneel: tablets met `model-no-code-scenario-sorteer.jsx` | n | Vervangt wb-02 in fase 2, incl. AVG-werknemer-foto's |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| WiFi werkt niet tijdens demo (fase 1) | Schakel naar backup-screenshots; benoem expliciet wat je *zou* doen ("hier zou ik nu 20 foto's slepen"). Niet doen alsof het 'ook wel theoretisch kan'. Plan B: hotspot van je telefoon. |
| Teachable Machine UI is veranderd | Benoem het: "Normaal staat deze knop links; vandaag rechts. Principe blijft: data, trainen, testen." Maakt het juist concreter. |
| Demo levert hoge accuratesse (>95%) zonder twijfelgeval | Forceer een twijfelgeval — een halve schroef, ongebruikelijke hoek, of een product dat niet in de trainingsset zat. Zonder twijfelgeval lijkt accuratesse magie. |
| Duo-werk fase 2 levert overal WEL op | Reframen: "Jullie zien overal kansen — mooi. Welk scenario zou ook een NIET kunnen zijn als je goed kijkt? Welke heeft een ander knelpunt — snelheid, volume, of AVG?" |
| AVG-discussie loopt uit in fase 2 of fase 3 | Begrens: "Goede vraag — parkeer op de flip-over. We komen er in blok 3 op terug. Voor nu: het knelpunt bij scenario 6 is mogen, niet kunnen." |
| Een deelnemer wil tool-bediening leren in fase 4 | Reframen: "Bediening komt in een vervolg-LO. Vandaag gaat het over de KEUZE — past dit type vraagstuk in drie stappen?" |
| Plenaire ronde fase 4 dreigt uit te lopen | Begrens tot 15 sec per persoon. Bij grote groep: laat 4 deelnemers delen, anderen schrijven op een sticky en plakken die voor je weggaan. |
| Groep is te klein (4 of minder) | Duo-werk fase 2 wordt drietal of plenair. Plenaire ronde fase 4 versmelt met individueel delen. |

---

## Snel-overzicht

| Fase (leerfase) | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | LIVE-demo drie stappen (max 8 min) + twijfelgeval | Drie observaties op wb-01 + één vraag genoteerd |
| 2 reflecteren | Zes scenario's duo + plenair scenario 4 (snelheid) en 6 (AVG) | WEL/NIET/TWIJFEL + reden voor min 4 van 6 |
| 3 theoretiseren | Handout drie blokken (WEL / NIET / AVG) + werkvloer-voorbeeld | Eén WEL + één NIET gemarkeerd + AVG-zelfinschatting |
| 4 experimenteren | Eigen werkvloer-keuze + vier vragen + actie deze week | Vraagstuk + keuze + concrete actie wat-wanneer-met-wie |

**Slagingscriterium:** drie observaties bij demo + min 4 van 6 scenario's beargumenteerd + eigen vraagstuk + één AVG-overweging + één concrete actie deze week.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor reflectie op de groep)
- [ ] Genoteerd: welke werkvloer-vraagstukken zijn gekozen (input voor volgende sessie)
- [ ] Genoteerd: welke AVG-vragen plenair zijn opgekomen (input voor curriculum-niveau)
- [ ] Genoteerd: heeft Teachable Machine UI gewerkt zoals verwacht, of moeten backup-screenshots geüpdatet?
- [ ] xAPI-statements verstuurd: `experienced`, `attempted`, `performed`, `completed`

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | No-code AI-tools voor de werkvloer*
*Bron: ko-ai-fund-211 + ko-ai-fund-022 + ko-ai-fund-210 + praktijklessen no-code prototyping RLC Oost/Zuid 2025-2026.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
