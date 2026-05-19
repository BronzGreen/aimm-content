# Drie vormen van machine learning — welke past bij welke data? — Draaiboek
*AI Fundamentals Module 1B (Gebruik) | Workshop-blok 42 minuten | 6-12 deelnemers | Casus: Sanne op Lijn B*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan de drie basisvormen van machine learning herkennen (supervised, unsupervised, reinforcement), per vorm één signaalwoord noemen, en voor de eigen lijn de passende vorm onderbouwen. Centrale inzicht: leerprincipe ≠ data-vorm — InspectAI (foto's) en CycleAdvise (tabel) zijn allebei supervised. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1A (Wat is AI?) afgerond — kent Sanne, Van Daalen Plastics Lijn B, en weet dat er twee AI-systemen op de lijn hangen (InspectAI sinds najaar 2025, CycleAdvise sinds januari 2026) |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat AI iets met data doet, mist mentaal model van het verschil tussen leervormen |
| **Begeleidingsstijl** | Trainen — ervaringsgericht startend, contrast 1A↔1B als rode draad |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Module 1B in AI Fundamentals — onder de motorkap kijken bij beide Lijn-B-systemen. Verwijst vooruit naar 1D (drempelkeuzes op InspectAI) en 1C (kritisch denken bij CycleAdvise-bias) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Vier scenariokaarten — IK DOE op 1A + contrast 1B + zelf 2 en 3 | ervaren | 12 min |
| 00:12 - 00:22 | Buurman-check + plenaire bespreking met signaalwoorden + 1A↔1B-contrast | reflecteren | 10 min |
| 00:22 - 00:32 | Handout: drie vormen op één bladzijde + drie-stappen-vraag | theoretiseren | 10 min |
| 00:32 - 00:42 | Eigen lijn-verkenning + één-zin-rondje + transferopdracht | experimenteren | 10 min |

**Totaal:** 42 minuten — geen aparte pauze.
**Buffer:** 30 sec per blok flexibel; gebruik bij voorkeur in fase 2 (signaalwoorden) of fase 4 (lijn-verkenning).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bereid op flip-over voor: links **"Parkeerlijst — algoritmes / semi-supervised voor later"**, rechts vier kolommen voor **"Case 1A InspectAI / Case 1B CycleAdvise / Case 2 / Case 3"** met ruimte voor signaalwoorden.
- [ ] Optioneel: screenshot van een (fictieve) CycleAdvise-trainingstabel — versterkt 1B-herkenning.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Vier scenariokaarten — IK DOE op 1A + contrast 1B
**00:00 - 00:12** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer ondervindt aan vier scenario's dat de keuze van ML-vorm afhangt van wat voor data en feedback er is. Het contrastpaar 1A (InspectAI foto's) ↔ 1B (CycleAdvise tabel) maakt zichtbaar dat dezelfde vorm bij heel verschillende data-vormen past. Trainer doet 1A voor, leidt het contrast naar 1B in, deelnemers werken 1B, 2 en 3 zelfstandig.

**Werkvorm:** Plenaire opening + IK DOE op 1A, contrast-bridge naar 1B, daarna individueel op 1B, 2 en 3.

**Instructie:**

1. **Open de sessie** (1,5 min) — toon slide 1. *"Sanne werkt op Lijn B bij Van Daalen Plastics. Sinds vorig jaar hangen er twee AI-systemen aan haar lijn: InspectAI op het inspectiestation en CycleAdvise op het dashboard. Vandaag laat Joyce van kwaliteit haar zien hoe InspectAI heeft leren kijken. En Karim van onderhoud laat zien hoe CycleAdvise heeft leren adviseren. Wij kijken mee. De komende 42 minuten zie je dat er drie basisvormen van machine learning bestaan — en dat dezelfde vorm bij heel verschillende data kan werken."*

2. **IK DOE op Case 1A (InspectAI)** (2 min) — deel wb-01 uit. Toon slide 2 (vier kaarten, beginnen met 1A). Lees 1A hardop: *"InspectAI op Lijn B. Joyce van kwaliteit heeft 4.000 foto's van zijpanelen voor wasmachines vooraf gelabeld als GOED, TWIJFEL of AFGEKEURD. Het systeem moet leren bij welke klasse een nieuwe foto hoort."* Toon slide 3 (IK DOE-werkblad). Doe hardop voor: *"Joyce heeft bij elke foto een antwoord gezet. Dat is leren met voorbeelden — supervised learning. Ik schrijf op: 1A = supervised, argument = Joyce heeft 4.000 keer een label gezet."*

3. **Contrast-brug naar 1B (CycleAdvise)** (1 min) — toon slide 4 (1B-kaart). Zeg: *"Op dezelfde lijn werkt nog een AI. Karim van onderhoud heeft zes maanden lang meegekeken bij de spuitgietmachine. Hij heeft 4.000 tabel-rijen gelabeld — geen foto's, maar meetwaarden: mal-temperatuur, druk, cyclustijd, uitvalpercentage. Bij elke rij staat zijn antwoord: BIJSTELLEN of NIET BIJSTELLEN. Vraag aan jullie: zelfde vorm als 1A, of een andere? Schrijf je gok op werkblad 1, in case 1B."* Geef GEEN antwoord. Geen lange uitleg over CycleAdvise — focus blijft op het contrast.

4. **Deelnemers werken 1B, 2 en 3** (6 min) — toon slide 5 (cases 2 en 3). *"Case 2: lasrobot bij een ander bedrijf, zes maanden 50.000 lasnaden, niemand heeft administratie van goed of fout. Productieleider wil weten of bepaalde dagen anders lopen. Case 3: verpakkingsrobot bij een ander bedrijf — probeert zelf zijn grijpkracht, ziet resultaat, past aan voor de volgende poging."* Zet timer op 6 min. Loop rond na 2 min. Stel vragen: *"Staat er bij elk voorbeeld een antwoord?"* *"Krijgt het systeem feedback na elke poging?"* *"Wat hebben Joyce en Karim gemeen? Wat is anders?"* Geef GEEN antwoord. PL-040 toegepast: scenariotekst noemt 'supervised'/'unsupervised' niet.

5. **Afsluiten + brug** (1,5 min) — vraag: *"Wie heeft een gok voor 1B in vergelijking met 1A — zelfde vorm of anders?"* Tel handen voor 'zelfde' en 'anders'. *"Mooi — niet delen welke vorm. Met je buurman vergelijken."*

**Materiaal:**
- [ ] Slides 1-5
- [ ] wb-01-scenarios-drie-vormen (1 set per deelnemer, 4 kaarten + vergelijktabel)
- [ ] Timer
- [ ] Pen

> **Tips voor de trainer:**
> - Houd 1A-IK-DOE en 1B-bridge samen onder 4 min — daarna individueel.
> - Bij 1B-bridge: noem Karim en de tabel kort. Geen technische uitleg over CycleAdvise — dat komt in 1D en 1C aan bod.
> - Tel innerlijk tot 7 na elke open vraag.

> **Valkuil — te lang stilstaan bij InspectAI of CycleAdvise als systeem:**
> Dit LO gaat over de drie leervormen — niet over hoe InspectAI of CycleAdvise werkt. Houd de uitleg per Lijn-B-systeem op wie labelt + wat de data is. Niet meer.

> **Valkuil — 1B-contrast laten verdampen:**
> Het kerninzicht van dit LO is dat 1A en 1B beide supervised zijn. Als je 1B als 'apart geval' presenteert, mist het contrast. Frame altijd: 'zelfde lijn, twee AI's, vraag is — zelfde vorm of anders?'

> **Valkuil — cognitive overload door twee systemen:**
> Twee AI's tegelijk is veel. Mitigatie: 1A volledig uitleggen (1 min), 1B alleen wat verschilt (30 sec). De rest van het LO benoemt InspectAI en CycleAdvise alleen bij naam als anker.

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers, vraag een eenvoudige binaire vraag: 'staat er een antwoord bij elk voorbeeld of niet?'
> - **Teamleider sneller:** Vraag bij snel klaar: *"Zou bij JULLIE iemand de Joyce-rol of de Karim-rol spelen? Wie zou kunnen labelen?"*

**Transitie naar blok 2:** *"Mooi — niet delen. Met je buurman vergelijken."*

---

### Blok 2: Buurman-check + plenaire bespreking met 1A↔1B-contrast
**00:12 - 00:22** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering, herkent het signaalwoord per case en ziet expliciet dat 1A en 1B beide supervised zijn ondanks andere data-vorm.

**Werkvorm:** 5 min duo's met focus op het contrast 1A↔1B, daarna 5 min plenair stemmen en bespreking.

**Instructie:**

1. **Duo-uitwisseling** (5 min) — toon slide 6. Deel wb-02 uit. *"Tweetal met je buurman. Vergelijk je keuzes op alle vier de cases. Extra: wat zei je over het contrast tussen 1A InspectAI en 1B CycleAdvise — zelfde vorm of anders? Welk woord uit de scenariotekst was doorslaggevend?"* Zet timer op 5 min. Loop rond, luister mee. Verzamel: welke woorden noemt de groep als signaal? ('Joyce heeft gelabeld', 'Karim heeft gelabeld', 'geen administratie', 'score per poging')

2. **Plenair stemmen + signaalwoord per case** (4 min) — toon slide 7. Per case stemmen:
    - **Case 1A** — *"Welke vorm hoort bij InspectAI? Handen omhoog voor supervised."* Tel. *"1A = supervised. Signaalwoord: Joyce HEEFT GELABELD — 4.000 foto's met een antwoord."*
    - **Case 1B** — *"Welke vorm hoort bij CycleAdvise? Zelfde als 1A of anders? Handen omhoog."* Tel. *"1B = óók supervised. Signaalwoord: Karim HEEFT GELABELD — 4.000 tabel-rijen met een antwoord."* Maak het kerninzicht expliciet: *"Twee verschillende data-vormen — foto's bij Joyce, een tabel bij Karim — maar zelfde leerprincipe. Dat is een belangrijk inzicht: leerprincipe ≠ data-vorm."*
    - **Case 2** — *"Welke vorm? Handen omhoog ..."* Tel. *"2 = unsupervised. Signaalwoord: GEEN ADMINISTRATIE. Geen labels. Het systeem moet zelf patronen vinden."*
    - **Case 3** — *"Welke vorm? ..."* Tel. *"3 = reinforcement. Signaalwoord: BIJ ELKE POGING EEN SCORE. Feedback per actie. Leren door proberen."*
   Schrijf op flipover de vier cases met hun signaalwoord. Maak expliciet: *"In de praktijk komen jullie als operator vooral supervised en unsupervised tegen. Reinforcement is bijzonder — vuistregel, te valideren per bedrijf."*

3. **Brug naar handout** (1 min) — sluit af: *"Vier cases, drie vormen. InspectAI én CycleAdvise zijn supervised — bewijs dat foto's en tabellen onder hetzelfde leerprincipe vallen. Nu zien we het op één bladzijde."*

**Materiaal:**
- [ ] Slides 6-7
- [ ] wb-02-reflectie-signaalwoorden
- [ ] Flipover voor signaalwoorden
- [ ] Stiften
- [ ] Timer

> **Tips voor de trainer:**
> - Tel hardop bij elke stemming.
> - Bij 1B-bevestiging EXPLICIET het kerninzicht uitspreken: *"leerprincipe ≠ data-vorm"*. Dit is de kern van het LO.
> - Schrijf 'Joyce labelt' en 'Karim labelt' letterlijk op de flipover bij 1A en 1B.

> **Valkuil — 1B als 'iets aparts' behandelen:**
> Als 1B niet expliciet met 1A wordt vergeleken, missen deelnemers het kerninzicht. Forceer de vergelijking: handen omhoog 'zelfde vorm' of 'andere vorm'.

> **Valkuil — supervised als 'echte AI':**
> Als grote meerderheid 'supervised' kiest voor case 2: maak expliciet dat 'geen labels = geen supervised, maar wel veel AI-mogelijkheden via unsupervised'.

> **Differentiatie:**
> - **Gemengde groep:** Bij 1A↔1B-vergelijking: vraag eerst operators wat er op de werkvloer anders is tussen foto's en tabel, dan teamleiders welk type leveranciersaanbieding daarbij past.

**Transitie naar blok 3:** *"Nu zien we het op één bladzijde."*

---

### Blok 3: Handout — drie vormen + drie-stappen-vraag
**00:22 - 00:32** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer plaatst de vier scenario-keuzes in een gestructureerd framework. De handout heeft het 1A↔1B-contrast als kernanker bij supervised.

**Werkvorm:** Trainer-geleide handout-bespreking met expliciete koppeling aan de vier cases. Drie-stappen-vraag op slide 11.

**Instructie:**

1. **Handout uitdelen + opdracht** (2 min) — deel wb-03 uit. Toon slide 8. *"Pak je markeerstift. Drie vormen op één bladzijde. Per vorm: kerngedachte, type data, maakindustrie-voorbeeld. Bij supervised staan beide Lijn-B-systemen als voorbeeld — InspectAI én CycleAdvise. Markeer wat voor jou nieuw is."*

2. **Drie vormen doorlopen** (6 min) — per vorm 2 min:
    - **Supervised** (slide 9) — *"Gelabelde data — een mens heeft goed of fout aangegeven. Voorspelt klasse of getal. Twee voorbeelden van Lijn B die we al kennen: InspectAI — 4.000 gelabelde foto's, Joyce heeft gelabeld. CycleAdvise — 4.000 gelabelde tabel-rijen, Karim heeft gelabeld. Twee data-vormen, één leerprincipe. Dat is de kern: leerprincipe ≠ data-vorm. Andere voorbeelden in de maakindustrie: camera-inspectie met 150 voorbeeldfoto's per klasse, voorspellen wanneer een onderdeel slijt."*
    - **Unsupervised** (slide 10) — *"Geen labels. Computer zoekt zelf patronen of groepen. Voorbeelden: afwijkende dagen op de CNC-frees ontdekken. Case 2 — 50.000 ongelabelde lasnaden — past hier."*
    - **Reinforcement** (slide 11) — *"Beloning per actie. Voorbeelden: lasersnijder die zelf snijsnelheid optimaliseert. Case 3 — verpakkingsrobot met score per poging — past hier. Vuistregel: in praktijk zeldzaam."*

3. **Drie-stappen-vraag + brug** (2 min) — toon slide 12. *"Hoe herken je welke vorm past? Drie vragen over de data: (1) staat er bij elk voorbeeld een antwoord? Ja → supervised — zoals bij Joyce en Karim. Nee → vraag 2. (2) Krijgt het systeem feedback na elke poging? Ja → reinforcement. Nee → vraag 3. (3) Zoeken we patronen of groepen? Ja → unsupervised."* Sluit af: *"Onthoud deze drie vragen. Nu jouw lijn."*

**Materiaal:**
- [ ] Slides 8-12
- [ ] wb-03-handout-drie-vormen
- [ ] Markeerstift per deelnemer

> **Tips voor de trainer:**
> - Bij supervised-slide: NOEM ALTIJD beide Lijn-B-systemen. Dat is de ankering van het kerninzicht.
> - Vermijd algoritmen (k-means, deep learning, Q-learning).

> **Valkuil — alleen InspectAI bij supervised noemen:**
> Het LO ontwerpt expliciet voor het contrastpaar. Vergeet niet CycleAdvise mee te nemen — anders mist de groep dat 'tabel = óók supervised'.

> **Valkuil — semi-supervised noemen:**
> Parkeer naar lo-ai-fund-ml-001.

**Transitie naar blok 4:** *"Nu jouw lijn."*

---

### Blok 4: Eigen lijn-verkenning + één-zin-rondje
**00:32 - 00:42** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer past de drie vormen toe op een eigen lijn-toepassing en formuleert één gerichte vraag. Plus contrast: lijkt de toepassing meer op InspectAI of CycleAdvise?

**Werkvorm:** Individueel verkenningsblad, daarna één-zin-rondje plenair en transferopdracht.

**Instructie:**

1. **Werkblad uitdelen + opdracht** (2 min) — deel wb-04 uit. Toon slide 13. *"Laatste 10 minuten. Eén AI-toepassing of monitoring-vraag op je eigen lijn. Vier vragen plus een contrastvraag: lijkt jouw toepassing meer op InspectAI (foto's) of op CycleAdvise (tabel)? Of iets compleet anders?"* Wijs op slide 12: *"Gebruik de drie-stappen-vraag. 'Weet ik niet' is geldig."*

2. **Individueel werken** (6 min) — zet timer op 6 min. Loop rond na 2 min. Doorvragen: *"Wie zou bij jullie de Joyce-rol kunnen spelen — wie weet wat goed of fout is?"* *"Of de Karim-rol — wie kent de meetdata?"* *"Is jullie data meer als foto's of meer als tabel?"* Bij vastlopers, geef suggesties: *"Inspectiecamera = lijkt op InspectAI. Sensordata-dashboard = lijkt op CycleAdvise."* Bevestig 'we weten het nog niet' uitdrukkelijk.

3. **Één-zin-rondje + transferopdracht** (2 min) — toon slide 14. *"Elk om de beurt, één zin: welke vorm past bij jouw lijn, en lijkt het meer op InspectAI of CycleAdvise?"* Loop rond. NIET bespreken. Sluit af: *"Deze week: kies één plek op Lijn B of op je eigen lijn waar AI nuttig zou zijn. Drie dingen noteren: (1) welke data hebben we — foto's, tabel of iets anders? (2) heeft iemand goed of fout aangegeven? (3) welke vorm past? Plus: meer op InspectAI of CycleAdvise? Bonus: praat met een collega van kwaliteit of onderhoud."*

**Materiaal:**
- [ ] Slides 13-14
- [ ] wb-04-eigen-lijn-verkenning
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Het InspectAI-vs-CycleAdvise-contrast helpt deelnemers de eigen data sneller te plaatsen.
> - 'Weet ik niet' is GEEN blokker — het is de eerste vraag.
> - Eindig op tijd.

> **Valkuil — verkenning blijft 'weet ik niet wat we hebben':**
> Bevestig dat het OK is. Help formuleren als 3 vragen: (1) waar gaat de data heen? (2) heeft iemand goed/fout aangevinkt? (3) hoe lang bewaren we de data?

> **Differentiatie:**
> - **MBO-4 basis:** Eén toepassing + één vorm-keuze is genoeg.
> - **Teamleider sneller:** Vraag *"Welk woord uit een leveranciersaanbieding zou bij JULLIE data-realiteit een alarmbel laten rinkelen?"*

**Transitie naar afsluiting:** *"Mooi werk. Neem je notities mee — volgende sessie kijken we wat je hebt gevonden. Wil je verder met PdM-leerklassen? lo-ai-fund-ml-001 in Module 2 Train."*

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-scenarios-drie-vormen (4 kaarten + vergelijktabel) | n + 2 | A4 dubbelzijdig |
| ☐ | wb-02-reflectie-signaalwoorden | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-drie-vormen | n + 2 | A4 enkelzijdig |
| ☐ | wb-04-eigen-lijn-verkenning | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Flip-over | 1-2 | Parkeerlijst + vier kolommen voor cases |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5/6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |
| ☐ | CycleAdvise-trainingstabel-screenshot (optioneel) | 1 | Versterkt 1B-herkenning |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| IT-affiniteit-deelnemer vraagt naar algoritmen | Parkeer op flipover. Verwijs naar lo-ai-fund-cnn-001, lo-ai-fund-rnn-001, lo-ai-fund-ensemble-001. |
| Iemand noemt semi-supervised | Parkeer expliciet. Verwijs naar lo-ai-fund-ml-001. |
| Groep loopt vast in fase 1 bij 1B | Geef een binaire vraag: 'staat er bij elke rij een antwoord van Karim — ja of nee?' Daarna komt 'supervised of niet' eerst. |
| Te veel discussie over CycleAdvise-techniek | Parkeer: 'CycleAdvise zelf komt in 1D en 1C. Hier gaat het om wie labelt en wat de data is — niets meer.' |
| Geen beamer | Werk vanaf flipover en geprinte werkbladen. Vier kolommen op flipover schrijven. |
| Plenair-rondje fase 4 lukt niet | Trainer noemt eigen voorbeeld eerst. |
| Groep is te klein (4 of minder) | Buurman-check wordt groepsrondje. Plenaire afsluiting in fase 4 versmelt met transferopdracht. |
| Cognitive load te hoog (groep verzuipt in twee systemen) | Maak 1B kort: 'Karim heeft gelabeld, klaar — wat denk je: zelfde vorm als Joyce?' Skip data-detail. |

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Vier scenariokaarten + IK DOE 1A + contrast naar 1B | Per case: vorm-keuze + onderbouwing; expliciet contrast 1A↔1B genoteerd |
| 2 reflecteren | Buurman-check + plenair stemmen | Signaalwoord per case + kerninzicht 'leerprincipe ≠ data-vorm' |
| 3 theoretiseren | Handout drie vormen + drie-stappen-vraag | Beslissingshulp: antwoord-bij-elk-voorbeeld? feedback? patronen? |
| 4 experimenteren | Eigen lijn + IT-vraag + plenair-rondje | Concrete toepassing + meer-op-InspectAI-of-CycleAdvise + transferopdracht |

**Slagingscriterium:** drie vormen benoemen + minimaal 3 van 4 scenario's correct met signaalwoord + 1A↔1B beide als supervised + eigen-lijn-verkenning met passende vorm en IT-vraag.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flipover signaalwoorden gefotografeerd
- [ ] Genoteerd: hoeveel deelnemers herkenden 1A↔1B-contrast direct? (kerninzicht-indicator)
- [ ] Parkeerlijst-vragen genoteerd
- [ ] xAPI-statements verstuurd: `experienced` (scenario's), `completed` (handout + verkenningsblad), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 1B (Gebruik) | Drie vormen van machine learning | Casus: Sanne op Lijn B*
*Bronnen: Russell & Norvig (2020) AI: A Modern Approach. | Mitchell (1997) Machine Learning. | Goodfellow et al. (2016) Deep Learning Ch. 5.*
*Casus-bron: docs/casus-ai-fundamentals.md (v2).*
*© BronzGreen × AIMM, 2026 | Draaiboek v2.0*
