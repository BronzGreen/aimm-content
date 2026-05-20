# CNN — hoe een neuraal netwerk patronen leert herkennen — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 50 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan de standaardarchitectuur van een CNN benoemen (input → convolutielagen → pooling → fully connected → output), kan uitleggen wat elke laag doet, en kan herkennen wanneer CNN passend is voor een werkvloerprobleem (lokale structuur in beeld of tijdreeks). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | data-lit-101 doorlopen; weet dat een AI-model getraind wordt en dat er 'lagen' in zitten |
| **Stadium (H&B)** | Bewust bekwaam — kent AI op hoog niveau, mist mentaal model van conv/pool/fc-lagen |
| **Begeleidingsstijl** | Instrueren — sterk sturend op concept, ruimte voor eigen plek-keuzes |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen AI Fundamentals Module 2 (Train) — naast FL, RNN, Ensemble, ML-leerklassen |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:17 | Mini-college: vier lagen van een CNN | theoretiseren | 17 min |
| 00:17 - 00:29 | Vier data-voorbeelden — past CNN hier? | ervaren | 12 min |
| 00:29 - 00:39 | Plenaire bespreking + buurman-check | reflecteren | 10 min |
| 00:39 - 00:50 | Eigen lijn-scan: actieplan | experimenteren | 11 min |

**Totaal:** 50 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (laag-vragen) of fase 4 (concretisering).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve. **Of** kies digitaal voor wb-02: laad `model-cnn-past-hier.jsx` op een React-sandbox (StackBlitz/CodeSandbox of lokale Vite-app) en test op één tablet.
- [ ] Print `diagram-lo-ai-fund-cnn-001.svg` op A3 (vier-lagen-architectuur). Hang in de zaal.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4 voor offline-inzet. Plan inzet na laag 4 in fase 1 (~90s extra; krap je dan in 14-min mini-college i.p.v. 17).
- [ ] Pak een fysiek vergrootglas (rekwisiet voor de speurder-analogie). Niet vergeten — dit is dé didactische ondersteuner van fase 1.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst — verdieping voor later"**, rechts **"Vier lagen"** met vier rijen (input / convolutie / pooling / fully connected).

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel — uitdelen pas op het moment.
- [ ] Leg het vergrootglas zichtbaar op de trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Mini-college — vier lagen van een CNN
**00:00 - 00:17** | 17 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer ontwikkelt een mentaal model van een CNN aan de hand van vier lagen (input, convolutie, pooling, fully connected) en twee kernconcepten (lokale connectiviteit, shared weights). Tijdens de uitleg vult de deelnemer een leeg architectuurdiagram in.

**Werkvorm:** Trainer-geleid mini-college met diagram + speurder-analogie. Deelnemers vullen actief het werkblad in.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 50 minuten kijken we onder de motorkap van een CNN — convolutional neural network. De magie van vision-AI en trillingsanalyse. Tegen het eind kun je per laag uitleggen wat hij doet, en kun je vier datavoorbeelden beoordelen op of CNN past."*

2. **Trigger — 'het werkt, maar wat doet het?'** (1 min 30) — toon slide 2. Vraag: *"Wie heeft op zijn lijn een vision-AI of trillingsanalyse-systeem zien werken?"* Vang 2-3 reacties. Vraag door: *"Weet je hoe het werkt?"* Antwoord is meestal 'nee'. Bevestig: *"Precies — die magie gaan we vandaag opentrekken. Niet de wiskunde, wel het idee."*

3. **Pak het vergrootglas — speurder-analogie** (2 min) — pak fysiek het vergrootglas. Loop voor de groep langs. Beweeg het over een denkbeeldige foto en spreek hardop: *"Krasje hier — krasje daar — randje — randje — kleurvlek — randje."* Leg uit: *"Een CNN is precies dit. Een speurder met een vergrootglas dat overal langsschuift en patronen markeert. Dat 'vergrootglas' heet een kernel. De gemarkeerde patronen samen heten een feature map."*

4. **Toon het diagram — vier lagen** (2 min) — toon slide 3. Wijs op het A3 en op het scherm. Loop de architectuur top-down af: input → convolutielaag → pooling → fully connected → output. Zeg: *"Vier lagen. Elk doet één ding. Samen herkennen ze patronen in beeld of tijdreeks. We gaan ze één voor één langs."*

5. **Deel wb-01 uit** (30 sec). Zeg: *"Tijdens de vier lagen die ik nu uitleg vul je dit lege architectuurdiagram in. Per laag noteer je in eigen woorden wat hij doet. Geef ook een voorbeeld van wat hij zou kunnen 'zien' — bij vibration: een frequentie-band; bij beeld: een rand of textuur."*

6. **Laag 1 — Input** (1 min 30) — toon slide 4. *"Input. Niets bijzonders — alleen de ruwe getallen. Bij beeld: pixels (RGB). Bij tijdreeks: meetwaarden over tijd. Geen patronen, alleen data."*

7. **Laag 2 — Convolutielaag** (4 min) — toon slide 5. Pak het vergrootglas weer. *"Convolutielaag. Hier doet de speurder zijn werk. Het kernel — een klein venster van bijvoorbeeld 3 bij 3 pixels — schuift over de hele input. Op elke positie kijkt het: 'lijkt het hier op een rand? lijkt het op een streepje?' Het resultaat is een nieuwe afbeelding waarin gemarkeerd staat WAAR het patroon zit — de feature map."* Pauze 5 sec. *"Twee kernconcepten hier. Eén: lokale connectiviteit — een neuron kijkt alleen naar zijn lokale venster, niet naar de hele input. Twee: shared weights — hetzelfde kernel werkt links en rechts. Dezelfde randdetector werkt overal."*  Schrijf op flip-over: 'lokale connectiviteit' en 'shared weights'.

8. **Laag 3 — Pooling** (2 min 30) — toon slide 6. *"Pooling. Comprimeren. De feature map uit de convolutielaag wordt kleiner gemaakt — meestal max-pooling: per blokje van 2x2 alleen de hoogste waarde houden. Dat doet twee dingen: het netwerk wordt sneller, EN het wordt robuust voor kleine verschuivingen. Krasje een halve millimeter naar links — dezelfde feature."* Maak op flip-over scherp: convolutie ZOEKT, pooling COMPRIMEERT.

9. **Laag 4 — Fully connected + output** (3 min) — toon slide 7. *"Fully connected. Hier komen alle features samen. Geen lokaal venster meer — élk neuron in deze laag kijkt naar álle features uit de vorige laag. Dat is waar de uiteindelijke beslissing wordt gemaakt: kras of geen kras, klasse A of B, RUL is 30 cycli. De output is een probabiliteit per klasse of een numerieke voorspelling."*

10. **Optioneel — toon de video** (1 min 30) — als je in tempo zit, toon `video/composition.tsx` (~90s). Zeg: *"Voor wie het visueel wil zien gebeuren — kijk hoe het vergrootglas-kernel hier letterlijk over een lasergravure-beeld glijdt en per stap een feature-map vult. Dat is wat we net in woorden hebben uitgelegd, nu in beweging."* Geen bespreking achteraf — laat het bezinken.

11. **Brug naar fase 2** (1 min) — toon slide 8. *"Vier lagen samen. Werkt fantastisch op data met lokale structuur — beeld, tijdreeks. Werkt slecht op data zonder lokale structuur — denk aan een ERP-tabel waar de kolomvolgorde willekeurig is. Dat gaan jullie nu zelf beoordelen."*

**Materiaal:**
- [ ] Slides 1-8
- [ ] wb-01-architectuur-invullen (1 per deelnemer)
- [ ] Vergrootglas (rekwisiet)
- [ ] A3-diagram zichtbaar
- [ ] Flip-over met vier lagen klaar

> **Tips voor de trainer:**
> - Het vergrootglas is bewust theatrale ondersteuning. Pak het op bij convolutielaag, leg het neer bij pooling. Visueel onderscheid.
> - Tempo: 17 minuten is krap voor vier lagen. Houd convolutie + pooling + fully connected als kern (4-3-3 minuten); input mag 1-2.
> - Vermijd termen als 'feature extraction', 'receptive field', 'stride', 'padding', 'ReLU' tenzij iemand vraagt — dan parkeren.

> **Valkuil — 'het is wiskunde, ik snap het niet':**
> Bevestig direct: 'Je hoeft de wiskunde niet te kunnen — wel het idee.' Pak het vergrootglas. Demonstreer fysiek. Het idee is een venster dat overal langs gaat — dat is het. De wiskunde laten we aan de leverancier.

> **Valkuil — convolutie en pooling worden door elkaar gehaald:**
> Maak op flip-over scherp: convolutie ZOEKT (vergrootglas), pooling COMPRIMEERT (uitzoomen). Eén zoekt, één vat samen. Twee verschillende werkstappen — niet één.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de vier lagen onder elkaar op flip-over en hou ze tijdens fase 2-4 zichtbaar. Per laag één steekwoord (zoeken / comprimeren / oordelen / classificeren).
> - **Teamleider sneller:** Bij fully connected: vraag 'waarom heet die laag fully connected?' — laat ze het zelf afleiden uit 'élk neuron kijkt naar álle features'.
> - **Gemengde groep:** Bij vraag uit groep: vraag een operator als eerste te reageren. Voorkomt dat strategisch perspectief operators de mond snoert.

---

### Blok 2: Vier data-voorbeelden — past CNN hier?
**00:17 - 00:29** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer toetst het mentale model door vier data-voorbeelden te beoordelen op CNN-geschiktheid en het doorslaggevende kernconcept (lokale structuur) te benoemen.

**Werkvorm:** Worked example (IK DOE) bij scenario A, daarna individueel B-D; trainer loopt rond.

**Instructie:**

1. **Deel wb-02 uit** (30 sec) — **OF** deel tablets uit met `model-cnn-past-hier.jsx` geopend. Zeg bij papier: *"Vier data-voorbeelden. Per voorbeeld kies je: past CNN hier wel of niet, en welk woord uit de uitleg is doorslaggevend — lokale structuur, kernel, feature map, of shared weights."* Zeg bij digitaal: *"Zes data-voorbeelden op je tablet. Per voorbeeld klik je 'CNN past' of 'CNN past niet' — je krijgt direct feedback met uitleg. Streef naar minimaal 4 van 6 correct."*

2. **IK DOE — voorbeeld A voor** (3 min) — toon slide 9. Zeg hardop: *"Voorbeeld A: lasergravure-beeld van een metalen plaat. We willen krassen detecteren. Mijn redenering: een kras is een lokaal patroon — een streepje, ergens op het beeld. Het kernel uit de convolutielaag is precies daarvoor gemaakt. En shared weights helpen: dezelfde kras-detector werkt linksboven en rechtsonder. Dus: CNN past sterk. Doorslaggevend: lokale ruimtelijke structuur."*

3. **Deelnemers werken aan B, C, D** (6 min) — toon slide 10. Zet timer op 6 min. Loop rond. Stel verdiepende vragen:
    - *"Heeft deze data een ruimtelijke ordening?"*
    - *"Zit het patroon op een specifieke plek of overal?"*
    - *"Zou shared weights hier voordeel geven?"*

4. **Korte tussenstand** (1 min) — vraag: *"Wie heeft alle drie? Hand omhoog. Twee? Eén? Mooi — we lopen ze straks plenair door."*

5. **Tijd-check** (1 min 30) — als 80% klaar is, sluit af. Zeg: *"Pen neer. Houd je werkblad voor je. Plenaire bespreking volgt."*

**Materiaal:**
- [ ] Slides 9-10
- [ ] wb-02-data-voorbeelden (4 kaarten per deelnemer) **OF** tablets/laptops met `model-cnn-past-hier.jsx` geopend (1 per deelnemer)
- [ ] Timer
- [ ] Pen

> **Tips voor de trainer:**
> - Bij twijfel: stuur niet bij. De twijfel is leerstof voor fase 3.
> - Loop wel langs trage starters — vraag hen hardop: 'wat zie je in voorbeeld B?' Activeert de aandacht zonder voor te zeggen.
> - Schrijf zelf NIET mee. De plenaire bespreking moet uit de groep komen.

> **Valkuil — scenario D (ERP-tabel) als CNN-case beoordeeld:**
> Iemand kiest 'CNN past' bij ERP omdat 'het toch ook data is'. Stel de tegenvraag: 'Heeft de volgorde van kolommen betekenis? Als ik onderdeelnummer en leverdatum verwissel — verandert er iets?' Antwoord: nee. Maak expliciet: CNN heeft ruimtelijke of volgordelijke structuur nodig.

> **Valkuil — vibration-signaal (C) wordt onterecht 'past niet':**
> Iemand denkt: vibration is een 1D-signaal, niet een 2D-beeld. Klopt half — maar 1D-CNN bestaat. Het kernel schuift dan over de tijdas en vindt frequentiebanden. CNN past dus, maar in 1D-vorm. Maak die nuance expliciet.

> **Differentiatie:**
> - **MBO-4 basis:** Vraag hen één vraag per voorbeeld: 'is er lokale structuur — ja/nee?' Laat de rest komen.
> - **Teamleider sneller:** Vraag bij snel klaar: 'voor welke van de vier zou je de leverancier vragen waarom ze deze architectuur kozen?'

---

### Blok 3: Plenaire bespreking + buurman-check
**00:29 - 00:39** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander, hoort een ander perspectief op dezelfde casus, en herkent waarom CNN bij D (ERP) niet past — als contrast op A-C.

**Werkvorm:** 5 minuten in tweetallen vergelijken — daarna plenaire stemming en bespreking.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). Zeg: *"Vorm een tweetal met je buurman. Vergelijk je antwoorden op A t/m D. Bij verschillen: leg elkaar uit waarom. Vul aan het eind in welke laag van de architectuur voor jou nu het duidelijkst is, en welke nog vragen oproept."*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Luister mee. Verzamel 2-3 sterke verschillen voor de plenaire ronde.

3. **Plenair stemmen** (2 min) — toon slide 11. Per voorbeeld: *"Hand omhoog wie 'CNN past'. Hand omhoog wie 'CNN past niet'. Wie twijfelt?"* Tel hardop, schrijf op flip-over de uitslag.

4. **Bespreking — vooral D als contrast** (2 min 30) — toon slide 12. *"A, B en C waren waarschijnlijk grotendeels CNN-passend — krassen, vlekken, frequentiebanden zijn allemaal lokale patronen. D is het contrast: ERP-tabel met onderdeelnummer en leverdatum. Verwissel de kolommen — verandert er iets? Nee. Geen ruimtelijke of volgordelijke structuur. Voor tabular data zoals deze past random forest of gradient boosting beter — dat zien jullie in een volgende sessie over ensembles."* Pauze. *"De truc: voordat je een CNN inzet, vraag je: zit er lokale structuur in mijn data? Zo nee — kies iets anders."*

**Materiaal:**
- [ ] Slides 11-12
- [ ] wb-03-reflectie
- [ ] Flip-over voor stemming-uitslag
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag in de plenaire ronde.
> - Bevestig D als kerncase. Het contrast is belangrijker dan dat A/B/C overtuigend zijn.
> - Verwijs kort naar lo-ai-fund-ensemble-001 voor het alternatief bij tabular data — niet uitweiden.

> **Valkuil — discussie over kernel-grootte of ReLU:**
> Een MBO-4-er met IT-affiniteit duikt in details. Bedank, parkeer op flip-over. Houd de bespreking conceptueel.

> **Differentiatie:**
> - **Gemengde groep:** Vraag eerst operator-MBO-4: 'wat zag je bij voorbeeld C (vibration)?' Daarna teamleider: 'wat zou je vragen aan de leverancier?'

---

### Blok 4: Eigen lijn-scan — actieplan
**00:39 - 00:50** | 11 min | Kolb-fase: experimenteren

**Doel:** Deelnemer kiest één concrete plek op de eigen lijn (visuele inspectie of trillingsmeting), beschrijft welk patroon erin zit, en koppelt aan een passende laag van de CNN.

**Werkvorm:** Individueel werkblad — trainer loopt rond en helpt bij concretisering.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Zeg: *"Laatste 11 minuten. Eén plek op je eigen lijn (of bij een klant) waar visuele inspectie of trillingsmeting plaatsvindt. Vul vier velden in: welk type data (beeld of tijdreeks), welk patroon herken jij nu zelf, welke laag (convolutielaag, pooling, fully connected) zou dat patroon waarschijnlijk oppikken."*

2. **Inventarisatie-vraag** (1 min) — toon slide 13. *"Eerst rondkijken: bij wie speelt vision of vibration op de eigen werkvloer? CNC, spuitgieten, verpakking, lakken?"* Vang 4-5 antwoorden, niet bespreken.

3. **Individueel werken** (6 min 30) — zet timer op 6 min 30. Loop rond. Stel concretiserende vragen:
    - *"Welk patroon herken jij nu zelf met je oog of oor?"*
    - *"Zit dat patroon op een specifieke plek of overal?"*
    - *"Welke laag doet het werk — convolutielaag (lokaal patroon), pooling (robuust), fully connected (eindoordeel)?"*
    Bij twijfel: bevestig dat de keuze niet hoeft te kloppen met een bestaand AI-systeem — het gaat om het denkraam.

4. **Plenaire ronde** (2 min) — toon slide 14. *"Twee deelnemers — kort delen: één plek, één patroon, welke laag doet het werk."* Vang 2 voorbeelden — geen oordeel, alleen waardering.

5. **Afsluiting + transferopdracht** (1 min) — toon slide 15. *"Deze week: kijk op je eigen lijn waar vision-AI of trillingsanalyse actief is. Vraag aan de leverancier of IT: gebruikt het systeem een CNN? Wat is de input — beeld of tijdreeks? Welk type defect herkent het — en welk juist niet? Noteer en koppel aan de architectuur. Bonus: zoek op YouTube 'CNN feature map visualization' — je ziet dan letterlijk wat de convolutielaag oppikt."*

**Materiaal:**
- [ ] Slides 13-15
- [ ] wb-04-actieplan
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij 'we hebben geen vision-AI op onze werkvloer': bevestig dat een hypothetische klant of toekomstig project mag.
> - De plenaire ronde van fase 4 is goud voor de volgende sessie. Schrijf 1 regel per voorbeeld in je trainersnotitieblok.
> - Bonus-tip (feature-map-video): noem alleen als er tijd over is. Anders glipt de kerntransfer weg.

> **Valkuil — actieplan blijft hangen op 'we hebben al een vision-AI':**
> Stel vervolgvragen: 'Welk patroon herkent dat systeem? Een streepje? Een kleur? Een vlek?' Help één concrete koppeling maken: patroon ↔ laag.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 9 minuten door werkblad-tijd op 5 min te zetten. Sla afsluiting nooit over.

> **Differentiatie:**
> - **MBO-4 basis:** Eén concrete plek + één laag is genoeg.
> - **Teamleider sneller:** Vraag ook 'wat als het systeem morgen een nieuw defecttype moet leren — welke laag gaat dan opnieuw trainen?' Antwoord: alle, maar fully connected verandert het meest.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-architectuur-invullen | n + 2 | A4 enkelzijdig, leeg architectuurdiagram |
| ☐ | wb-02-data-voorbeelden | n + 2 | A4 dubbelzijdig, 4 kaarten — **OF** vervang door tablets met `model-cnn-past-hier.jsx` (6 cases, directe feedback) |
| ☐ | wb-03-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-04-actieplan | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-ai-fund-cnn-001.svg | 1 op A3 | Vier-lagen-architectuur, zichtbaar in zaal |
| ☐ | Vergrootglas | 1 | Rekwisiet voor speurder-analogie |
| ☐ | Markeerstiften | n | Voor wb-01 en wb-03 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 2 | Parkeerlijst + vier lagen |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5-min en 6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |
| ☐ | Optioneel: `video/composition.tsx` (Remotion) | 1 | ~90s, na laag 4 in fase 1; pre-rendered MP4 of live preview |
| ☐ | Optioneel: tablets met `model-cnn-past-hier.jsx` | n | Vervangt wb-02 in fase 2 als digitaal gekozen wordt |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 theoretiseren | Architectuurdiagram invullen tijdens vier lagen | Mentaal model: input → conv → pool → fc → output |
| 2 ervaren | Vier data-voorbeelden beoordelen | Per case: CNN ja/nee + doorslaggevend concept |
| 3 reflecteren | Buurman-check + plenair | Inzicht: D (ERP) is contrast — geen lokale structuur |
| 4 experimenteren | Eigen lijn-actieplan | Concrete plek + patroon + laag-koppeling |

**Slagingscriterium:** vier lagen plaatsen op het schema + minimaal 3 van 4 voorbeelden correct + actieplan met concrete plek.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met vier lagen gefotografeerd
- [ ] Genoteerd: stemming per voorbeeld (verdeling = indicatie groepsbegrip)
- [ ] Notitie voor volgende sessie: wie ging leverancier bevragen? Wie zoekt feature-map-video op?
- [ ] xAPI-statements verstuurd: `experienced` (architectuurdiagram), `completed` (voorbeelden + actieplan), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | CNN-architectuur*
*Bronnen: LeCun et al. (1998) Gradient-Based Learning. | Krizhevsky et al. (2012) ImageNet/AlexNet. | Olah (2014) Conv Nets — Modular Perspective.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
