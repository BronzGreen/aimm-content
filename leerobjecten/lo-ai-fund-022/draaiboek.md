# Wat is een neuraal netwerk — patroonherkenning in lagen — Draaiboek
*AI Fundamentals Module 1 (Gebruik) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden uitleggen wat een neuraal netwerk is, op een schema input/lagen/output aanwijzen, en voor de eigen lijn benoemen waar zo'n model meekijkt. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | lo-ai-fund-101 (Wat is AI) afgerond — kent de twee kenmerken |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat AI iets met data doet, mist mentaal model van neurale netwerken |
| **Begeleidingsstijl** | Trainen — ervaringsgericht startend, structureel verdiepend |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, A3-print van lagen-diagram zichtbaar, flip-over |
| **Plek in module** | Tweede LO in AI Fundamentals Module 1 — na lo-ai-fund-101, vóór lo-ai-fund-117 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | Scene inspectiecamera — eigen gok op geel briefje | ervaren | 10 min |
| 00:10 - 00:20 | Buurman-check + 'in stapjes' op flipover | reflecteren | 10 min |
| 00:20 - 00:35 | Drie blokken: input — lagen — output (diagram) | theoretiseren | 15 min |
| 00:35 - 00:45 | Vier vragen over eigen lijn + plenair | experimenteren | 10 min |

**Totaal:** 45 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 3 (lagen-uitleg) bij IT-affiniteit-vragen.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-03 — n + 2 reserve (wb-03 met antwoordmodel achterop). **Of** kies digitaal voor wb-03: laad `model-lagen-verkennen.jsx` op een React-sandbox en test op één tablet.
- [ ] Print `diagram-lo-ai-fund-022.svg` op A3 — hang in de zaal.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bereid foto of korte video van inspectiecamera op lopende band voor (slide 2).
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `NeuraalNetwerkVideo`, ~90s) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Inzet in fase 3 ná de drie blokken.
- [ ] Schrijf op een flip-over: links **"Parkeerlijst — IT-detail voor later"**, rechts leeg veld voor **"In stapjes — wat als eerste?"**

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, geel briefje.
- [ ] Houd wb-01, wb-02 en wb-03 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Scene inspectiecamera — eigen gok op briefje
**00:00 - 00:10** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer ondervindt aan een herkenbare camera-inspectie-scene dat een AI-systeem 'op een bepaalde manier kijkt' en schrijft de eigen intuïtie op zonder oordeel. De groep maakt zelf de eerste stap naar 'in stapjes kijken'.

**Werkvorm:** Plenaire opening, daarna IK DOE-worked-example, daarna individueel.

**Instructie:**

1. **Open de sessie** (2 min) — toon slide 1. Zeg: *"Op steeds meer werkplekken hangt een camera die zelf goedkeurt of afkeurt. Voor velen voelt dat als magie of een black box. Het is geen van beide — het is wiskunde. De komende 45 minuten zie je hoe dat op hoofdlijnen werkt."*

2. **Scene tonen + opdracht** (2 min) — toon slide 2 (foto/video inspectiecamera boven een lopende band met metalen beugels, sommige met kras van 2mm). *"Hier hangt een camera boven de band. Hij wijst aan: deze beugel heeft een kras, deze niet. Vraag: hoe denk je dat hij dat doet? Hoe ziet hij het verschil?"* Deel gele briefjes uit. *"Schrijf één zin: 'volgens mij ziet de camera het zo: ...' Geen goede of foute antwoorden — je antwoord is een startpunt, geen toets."*

3. **IK DOE + individueel werken** (5 min) — doe hardop voor: *"Ik kijk naar deze foto en denk: zou de camera de hele foto in één keer beoordelen? Of zou hij eerst naar lijnen kijken, daarna naar vormen? Ik weet het eigenlijk niet zeker — laat ik dat opschrijven."* Schrijf zelf demonstratief op een briefje. *"Jouw beurt — schrijf jouw beste gok op. Twee minuten."* Zet timer. Loop rond na 1 min. Verzamel briefjes na 2-3 min.

4. **Briefjes voorlezen** (1 min) — schud de briefjes. Lees 3-4 voor zonder commentaar of oordeel. Bij elke briefje knik je en zeg je *"mooi, ik hoor je"*. Sluit af: *"Verschillende ideeën — dat is precies waar we hier voor zijn. We gaan ze straks vergelijken met je buurman."*

**Materiaal:**
- [ ] Slides 1-2
- [ ] Gele briefjes
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na de vraag — wachten geeft denkruimte.
> - Doe het IK DOE-voorbeeld kort — 30-45 sec, niet langer.
> - Demonstreer dat 'ik weet het niet zeker' een geldige uitkomst is.
> - Verzamel briefjes anoniem — geen namen erop.

> **Valkuil — hint geven richting 'lagen' of 'stapjes':**
> Wacht op blok 2 — daar laat je de groep het zelf bedenken.

> **Valkuil — commentaar bij voorlezen:**
> Lees neutraal voor. Geen 'goed idee' of 'klopt niet helemaal'.

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers, geef twee opties: 'in één keer' of 'in stapjes' — kies wat je denkt.
> - **Teamleider sneller:** Vraag bij snel klaar: *"En wat zou de camera als EERSTE moeten kunnen?"*

**Transitie naar blok 2:** *"Verschillende ideeën — dat is precies waar we hier voor zijn. We gaan ze straks vergelijken met je buurman."*

---

### Blok 2: Buurman-check + 'in stapjes' op flipover
**00:10 - 00:20** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander en herkent — samen met de groep — dat 'in stapjes kijken' het meest logische mentale model is. De flipover-verzameling vormt de brug naar de lagen-uitleg.

**Werkvorm:** 5 min duo's, daarna 4 min plenair stemmen + verzamelen, 1 min brug.

**Instructie:**

1. **Duo-uitwisseling** (5 min) — toon slide 3. Deel wb-01 uit. *"Tweetal met je buurman. Vergelijk jullie briefjes. Wat heb je opgeschreven? Wat heeft je buurman opgeschreven? Op het reflectiewerkblad schrijf je één zin: 'het meest verrassende voor mij was ...'"* Zet timer op 5 min. Loop rond, vang vastlopers binnen 2 min. Bij stilte: *"Wie begint? Lees voor wat je hebt opgeschreven."*

2. **Plenair stemmen** (2 min) — toon slide 4. Vraag: *"Wie dacht dat de camera in één keer naar het hele beeld kijkt? Steek je hand op."* Tel hardop. *"Wie dacht in stapjes — eerst lijnen, dan vormen?"* Tel.

3. **Flipover-verzameling** (2 min) — *"Bijna iedereen denkt aan 'in stapjes'. Welke stapjes zou de camera dan kunnen maken? Wat als eerste?"* Verzamel op flipover: schrijf antwoorden letterlijk op — 'lijnen', 'vormen', 'kleuren', 'krassen', wat de groep ook noemt.

4. **Brug naar fase 3** (1 min) — sluit af: *"Bijna iedereen denkt aan in stapjes kijken — en dat klopt. Dat is precies wat een neuraal netwerk doet. Nu zien we hoe dat eruitziet."*

**Materiaal:**
- [ ] Slides 3-4
- [ ] wb-01-buurman-reflectie
- [ ] Flipover + stiften
- [ ] Timer

> **Tips voor de trainer:**
> - Tel hardop bij elke stemming.
> - Bevestig 'in stapjes' als het juiste mentale model — daar gaan we straks dieper op in.
> - Schrijf antwoorden LETTERLIJK op — niet parafraseren.
> - Houd de flipover-lijst zichtbaar tijdens blok 3.

> **Valkuil — 'in één keer' bestempelen als fout:**
> Bevestig dat het ook een logische gedachte is. 'In stapjes' is wat een neuraal netwerk doet — maar 'in één keer' is geen domme gok.

> **Valkuil — definitie nu al geven:**
> Wacht op blok 3 — daar komt het diagram.

> **Differentiatie:**
> - **Gemengde groep:** Combineer in een duo een operator (werkvloer-kennis) met een teamleider (leverancier-perspectief).

**Transitie naar blok 3:** *"Nu zien we hoe dat eruitziet."*

---

### Blok 3: Drie blokken — input, lagen, output
**00:20 - 00:35** | 15 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer plaatst de eigen intuïtie ('in stapjes') in het structuur-schema van een neuraal netwerk: input, lagen met neuronen, output. Krijgt de twee belangrijkste misconcepties hardop benoemd: geen magie, geen brein. Concreet voorbeeld met cijfers uit Soldatos 2024.

**Werkvorm:** Trainer-geleide handout-bespreking met A3-diagram en directe verbinding naar de scene uit fase 1.

**Instructie:**

1. **Handout uitdelen + diagram introduceren** (3 min) — deel wb-02 uit. Toon slide 5. Wijs het A3-diagram aan. *"Pak je markeerstift. Wat we straks gaan zien heeft een naam: een neuraal netwerk. Drie blokken op het diagram. Markeer in eigen woorden welk blok wat doet, terwijl ik het uitleg."*

2. **Drie blokken doorlopen** (8 min):
    - **Input** (2 min) — toon slide 5 ingezoomd op linker-blok. *"Dit is wat erin gaat — een foto van de metalen beugel op de lopende band. De camera maakt een foto en die wordt omgezet in pixels — getallen die het netwerk begrijpt."*
    - **Lagen** (4 min) — toon slide 5 ingezoomd op midden. *"Dit zijn de tussenlagen — hier zit het rekenwerk. Veel kleine eenheden — neuronen — kijken elk naar een stukje. EERSTE laag herkent lijnen en randen. VOLGENDE laag herkent vormen — een rond, een hoek. LAATSTE lagen herkennen complete patronen — een kras, een deuk, een ontbrekende schroef. Daarom dachten jullie net al aan 'in stapjes' — dat is precies wat hier gebeurt."*
    - **Output** (2 min) — toon slide 5 ingezoomd op rechter-blok. *"Het antwoord komt eraan — goed of kras op positie 3. Geen tussenvragen."*

3. **Optioneel — toon de video** (1 min 30) — als je in tempo zit (drie blokken in 6 min i.p.v. 8), toon `video/composition.tsx` (export id `NeuraalNetwerkVideo`, ~90s). Zeg: *"Voor wie het visueel wil zien gebeuren — kijk hoe het lagen-schema letterlijk doorstroomt: van tandwiel naar lijnen, naar vormen, naar 'kras' of 'goed'. En de heat-map laat zien WAAR het netwerk kijkt."* Geen bespreking achteraf — laat het bezinken.

4. **Twee misconcepties + Soldatos-cijfer** (3 min) — toon slide 6. *"Twee misverstanden om uit de weg te ruimen. EÉN: het is geen magie. Iemand heeft het gebouwd, getraind en getest. Elk antwoord komt uit rekenwerk. TWEE: het werkt niet precies zoals een brein. De naam komt van hersencellen — neuronen — maar de overeenkomst is oppervlakkig. Het is een rekenmodel, geen biologie."* Pauze. Toon slide 7. *"Een concreet voorbeeld: een producent van kunststof brandstoftanks gebruikte zo'n model voor inspectie. Het model leerde van 1.300 synthetische foto's en 295 echte foto's. Daarna herkende het 70% van de defecten correct, in real-time. Bron: Soldatos 2024. 70% klinkt niet zo hoog — maar het betekent: de camera vangt 70 van de 100 defecten meteen. De rest blijft mensenwerk. Het model neemt niet over — het helpt."*

5. **Brug naar fase 4** (1 min) — sluit af: *"Drie blokken — input, lagen, output. Hetzelfde patroon zit overal waar een camera of sensor meekijkt. Nu jouw lijn: waar staat dit ding bij jullie?"*

**Materiaal:**
- [ ] Slides 5-7
- [ ] wb-02-handout-lagen
- [ ] A3-diagram (zichtbaar)
- [ ] Markeerstift per deelnemer
- [ ] Optioneel: `video/composition.tsx` (Remotion `NeuraalNetwerkVideo`, ~90s) — pre-rendered MP4 of live preview

> **Tips voor de trainer:**
> - Houd het A3-diagram zichtbaar — wijs er steeds aan.
> - Verbind expliciet terug naar fase 1-2: *"Jullie 'lijnen' en 'vormen' zijn precies wat de eerste lagen herkennen."*
> - Houd cijfers concreet en uit de bron — niet zelf afronden.
> - Bevestig dat 70% genoeg is om waarde toe te voegen.

> **Valkuil — activatiefuncties/backpropagation uitleggen:**
> IT-affiniteit-vraag → parkeer op flipover. *"Vandaag blijven we op niveau input-lagen-output."*

> **Valkuil — brein-vergelijking laten staan:**
> Bij *"dus de camera DENKT"* → bevestig de naam, maar maak verschil scherp: rekenmodel, geen biologie, geen begrip.

> **Valkuil — werkvloer-koppeling vergeten:**
> Maak ELKE laag-uitleg expliciet terug naar wat de groep in fase 2 zelf bedacht heeft.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de drie woorden — input, lagen, output — groot op flipover. Houd zichtbaar tijdens fase 4.
> - **Teamleider sneller:** Vraag tussendoor: *"Waarom zijn meer voorbeelden meestal beter?"* Antwoord-richting: het netwerk kan meer variatie zien.

**Transitie naar blok 4:** *"Nu jouw lijn: waar staat dit ding bij jullie?"*

---

### Blok 4: Vier vragen over eigen lijn + plenaire ronde
**00:35 - 00:45** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer past het input-lagen-output-schema toe op de eigen lijn (of een collega-lijn), benoemt input en output, en formuleert één vraag aan IT, leverancier of kwaliteit.

**Werkvorm:** Individueel werkblad met antwoordmodel-vangnet. Korte plenaire ronde: 3 deelnemers delen vraag 1.

**Instructie:**

1. **Werkblad uitdelen + opdracht** (2 min) — deel wb-03 uit **OF** deel tablets uit met `model-lagen-verkennen.jsx` geopend. Toon slide 8. Zeg bij papier: *"Vier vragen over jouw eigen lijn. (1) Op welke lijn of plek bij jou werkt een camera of sensor mee — of zou dat kunnen? (2) Wat is daar de input — een foto, een meting, een geluid? (3) Wat is daar de output — een goed/fout antwoord, een klasse, een getal? (4) Heeft jouw bedrijf voorbeelden om mee te trainen — denk je 100 of 1.000?"* Wijs het werkblad aan. *"Antwoordmodel staat achterop — kijk daar pas in als je echt vastloopt."* Maak duidelijk: *"'Weet ik niet zeker' is een geldig antwoord. Dat is precies de vraag voor IT."* Zeg bij digitaal: *"Op je tablet zie je drie inputs en vier lagen. Klik elke cel aan om te zien wat die laag voor die input oppikt. Verken eerst het mechanisme; pak daarna pen voor de eigen-lijn-vragen."*

2. **Individueel werken** (6 min) — zet timer op 6 min. Loop rond na 2 min. Stel doorvragen: *"Welke camera bedoel je? Boven welke band?"* *"Wie weet hoe vaak er een foto wordt opgeslagen?"* *"Wie zou de trainingsfoto's beoordeeld hebben?"* Bij vastlopers: bied antwoordmodel aan of geef een lijn-suggestie (spuitgieten met cameracontrole, lasrobot met afwijking-detectie, eindcontrole met camera). Bevestig 'ik weet het niet zeker' uitdrukkelijk.

3. **Plenaire ronde + transferopdracht** (2 min) — toon slide 9. *"Drie deelnemers — kort, één zin op vraag 1: waar staat jouw camera of sensor?"* Vang 3 voorbeelden, niet bespreken. Toon slide 10. *"Deze week loop je één keer langs de inspectiecamera of het sensorsysteem op jouw lijn. Drie dingen noteren: (1) waar hangt de camera precies — boven welke band, bij welke machine? (2) wat is de output — goed/fout, klasse, of getal? (3) waar komen de trainingsfoto's vandaan — wie maakt of beoordeelt die? Geen camera op je lijn? Vraag een collega van een andere lijn. Bonus: praat één keer met een kwaliteitscollega — 'wie bepaalt eigenlijk wat de camera ziet als goed of fout?'"*

**Materiaal:**
- [ ] Slides 8-10
- [ ] wb-03-eigen-lijn (met antwoordmodel achterop) **OF** tablets/laptops met `model-lagen-verkennen.jsx` geopend
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Vang precies 3 voorbeelden plenair — geen 5.
> - Eindig op tijd — transferopdracht moet helder overkomen.
> - Maak concreet: 'we hebben geen camera' is GEEN blokker — vraag collega-lijn of denk aan sensor.

> **Valkuil — eigen-lijn-werkblad blijft leeg:**
> Iemand: *"wij hebben geen camera"*. Twee uitwegen: (1) elders in het bedrijf? Eindcontrole, kwaliteitslab? (2) Welke SENSOR is wel aanwezig (temperatuur, druk, trilling)? Hetzelfde input-lagen-output-model geldt.

> **Valkuil — 'goed/fout' beoordelen bij rondlopen:**
> Alleen helpen formuleren — niet corrigeren.

> **Valkuil — plenair gaan discussiëren:**
> Alleen verzamelen. Anders loop je uit en mist de transferopdracht zijn doel.

> **Differentiatie:**
> - **MBO-4 basis:** Maak van vraag 4 een meerkeuze: 'minder dan 100' / '100-1.000' / 'meer dan 1.000' / 'weet ik niet'.
> - **Teamleider sneller:** Vraag óók: *"Wie zou bij jullie verantwoordelijk zijn voor de trainingsfoto's — onderhoud, kwaliteit of IT?"*

**Transitie naar afsluiting:** *"Mooi werk. Neem je notities mee — volgende sessie kijken we wat je hebt gevonden."*

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-buurman-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-handout-lagen | n + 2 | A4 dubbelzijdig (met diagram) |
| ☐ | wb-03-eigen-lijn | n + 2 | A4 dubbelzijdig (antwoordmodel achterop) — **OF** vervang/combineer met tablets met `model-lagen-verkennen.jsx` |
| ☐ | diagram-lo-ai-fund-022.svg | 1 op A3 | Input-lagen-output, zichtbaar in zaal |
| ☐ | Gele briefjes / Post-its | n + 5 | Voor fase 1 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Markeerstiften | n | Voor wb-02 |
| ☐ | Flip-over | 2 | 'In stapjes'-verzameling + parkeerlijst |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 2/5/6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |
| ☐ | Optioneel: `video/composition.tsx` (Remotion `NeuraalNetwerkVideo`) | 1 | ~90s, fase 3 |
| ☐ | Optioneel: tablets met `model-lagen-verkennen.jsx` | n | Vervangt of vult wb-03 aan in fase 4 |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| Geen beamer beschikbaar | Werk met A3-diagram en geprinte foto verpakkingslijn. Sla slides over, gebruik flipover. |
| IT-affiniteit-deelnemer trekt fase 3 abstract | Bevestig nieuwsgierigheid, parkeer activatiefuncties/backpropagation op flipover, blijf bij drie blokken. |
| Geen camera op iemands lijn | Bied sensor-alternatief: hetzelfde input-lagen-output-model geldt voor trillings-, temperatuur- of drukmetingen. |
| Groep loopt vast in fase 1 (niemand weet wat te schrijven) | Bied de twee opties expliciet aan: 'in één keer' of 'in stapjes' — kies + onderbouw met één zin. |
| Groep loopt uit in fase 3 (te veel vragen) | Vraag te parkeren. Behoud 5 min voor het Soldatos-cijfer + brug. |
| Plenaire ronde fase 4 lukt niet | Trainer noemt zelf 1 voorbeeld uit rondloop, zonder naam, daarna transferopdracht direct. |

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Scene inspectiecamera, gok op geel briefje | Eerste intuïtie op papier — twijfel mag |
| 2 reflecteren | Buurman-check + flipover 'in stapjes' | Groep heeft zelf bedacht: in stapjes kijken |
| 3 theoretiseren | Drie blokken + twee misconcepties + Soldatos-cijfer | Mentaal model: input → lagen → output, geen magie, geen brein |
| 4 experimenteren | Vier eigen-lijn vragen + IT-vraag | Concrete toepassing + transferopdracht |

**Slagingscriterium:** input/lagen/output benoemen + minimaal 3 van 4 eigen-lijn vragen ingevuld + één gerichte vraag voor IT, kwaliteit of leverancier.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Genoteerd: welke voorbeelden plenair gedeeld? (input voor volgende sessie)
- [ ] Flipover 'in stapjes' gefotografeerd (mentaal model van de groep)
- [ ] Parkeerlijst-vragen genoteerd (voor lo-ai-fund-117 of vervolg-LO)
- [ ] xAPI-statements verstuurd: `experienced` (scene), `completed` (handout + werkblad), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 1 (Gebruik) | Wat is een neuraal netwerk*
*Bronnen: Soldatos, J. (2024) Artificial Intelligence in Manufacturing Ch. 17-18 | Goodfellow et al. (2016) Deep Learning.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
