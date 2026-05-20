# RNN, LSTM en BiLSTM — neurale netwerken met geheugen — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 50 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan uitleggen waarom een RNN-familie nodig is voor tijdreeks-data, kan het verschil benoemen tussen vanilla RNN, LSTM en BiLSTM, en kan beoordelen welke variant past bij een gegeven scenario (online vs. offline, korte vs. lange sequentie). |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | data-lit-101 doorlopen + kent het begrip tijdreeks; bij voorkeur lo-ai-fund-cnn-001 doorlopen |
| **Stadium (H&B)** | Bewust bekwaam — kent neurale netwerken op hoog niveau, mist het mentaal model van geheugen |
| **Begeleidingsstijl** | Instrueren — sterk sturend op concept, ruimte voor eigen scenario-keuzes |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen AI Fundamentals Module 2 (Train) — naast FL, CNN, Ensemble, ML-leerklassen |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:18 | Mini-college: van RNN naar LSTM naar BiLSTM | theoretiseren | 18 min |
| 00:18 - 00:30 | Drie scenario-kaarten — welke variant past? | ervaren | 12 min |
| 00:30 - 00:40 | Buurman-check + plenaire bespreking | reflecteren | 10 min |
| 00:40 - 00:50 | Eigen tijdreeks-scan: actieplan | experimenteren | 10 min |

**Totaal:** 50 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel; gebruik bij voorkeur in fase 1 (LSTM-uitleg).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print `diagram-lo-ai-fund-rnn-001.svg` op A3 (LSTM-cel met drie gates). Hang in de zaal.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `RnnLstmVideo`, ~91s) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Inzet als visuele opening van fase 1 — tijds-animatie maakt het geheugen-mechanisme tastbaar.
- [ ] Pak een fysiek schrift / blocnote (rekwisiet voor schrift-analogie). Niet vergeten.
- [ ] Pak drie post-it-kleuren — rood, groen, geel (of andere drie kleuren). Voor de drie gates.
- [ ] Bereid op een flip-over voor: links **"Parkeerlijst — verdieping voor later"**, rechts **"Drie varianten"** met drie rijen (RNN / LSTM / BiLSTM).

### Het uur ervoor
- [ ] Hang het A3-diagram zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Leg het schrift en de drie post-its zichtbaar op de trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Mini-college — van RNN naar LSTM naar BiLSTM
**00:00 - 00:18** | 18 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer ontwikkelt een mentaal model van de drie varianten via een opbouwend verhaal: probleem → oplossing → nieuwe oplossing. Tijdens de uitleg vult de deelnemer een vergelijkingstabel in (RNN/LSTM/BiLSTM × probleem/use-case/online-offline).

**Werkvorm:** Trainer-geleid mini-college met diagram + schrift-analogie. Deelnemers vullen actief het werkblad in.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 50 minuten kijken we naar drie verwante AI-architecturen: RNN, LSTM en BiLSTM. Allemaal voor tijdreeks-data — vibration, temperatuur, druk, akoestiek. Tegen het eind kun je per variant uitleggen wat hij doet, en kun je drie scenario's beoordelen op welke variant past."*

2. **Trigger — een vraag** (1 min 30) — toon slide 2. Vraag: *"Wie heeft op zijn lijn een PdM-systeem dat een venster van bijvoorbeeld 50 of 200 samples bekijkt voordat het alarmeert?"* Vang 1-2 reacties. *"Waarom een venster en niet één meetwaarde?"* Antwoord: trends, patronen over tijd. Bevestig: *"Precies — voor die tijdreeksen heb je een ander type AI nodig dan een gewone classifier. Een AI met geheugen. En die geheugen-architecturen gaan we vandaag opentrekken."*

3. **Pak het schrift** (1 min) — pak fysiek het schrift. Zeg: *"Stel: dit is mijn aantekeningen-schrift. Elke pagina = één timestep. Wat ik schrijf, wat ik onthoud — daar gaan de drie varianten over. Drie soorten geheugen, drie pagineringsstrategieën."*

4. **Variant 1 — Vanilla RNN** (4 min) — toon slide 3. Zeg: *"RNN — Recurrent Neural Network. Idee: het netwerk gebruikt de output van de vorige timestep als input voor de volgende. Een terugkoppeling. In schrifttermen: ik schrijf alleen op wat er net gebeurde. Wat 50 pagina's geleden gebeurde? Vergeten."*

   Pauze. *"Probleem: long-term dependency. Stel: een trillingspiek nu wordt veroorzaakt door wrijving die 100 samples geleden ontstond. Vanilla RNN heeft die wrijving allang vergeten. Dat heet vanishing gradient — informatie van ver geleden 'zakt weg' tijdens trainen."*

   Schrijf op flip-over: 'RNN: kort geheugen — vergeet snel'.

5. **Variant 2 — LSTM** (6 min) — toon slide 4. Pak de drie post-its. Zeg: *"LSTM — Long Short-Term Memory. 1997, Hochreiter & Schmidhuber. Lost het probleem op met drie gates en een aparte cell-state. Geheugen dat overleeft over lange afstanden."*

   Houd elke post-it omhoog terwijl je hem benoemt:
   - **Rood (forget gate)**: *"Wat vergeten we uit het langetermijngeheugen? De forget gate beslist wat eruit gaat — wat irrelevant geworden is."*
   - **Groen (input gate)**: *"Wat voegen we toe? De input gate beslist welke nieuwe informatie het waard is om op te slaan."*
   - **Geel (output gate)**: *"Wat geven we door naar de volgende laag? De output gate beslist wat gedeeld wordt."*

   *"Drie gates, drie acties: doorstrepen, bijschrijven, voorlezen. Plus een cell-state — een rode draad die door alle timesteps loopt. LSTM is het werkpaard van realtime PdM."*

   Schrijf op flip-over: 'LSTM: lang geheugen — drie gates'.

6. **Variant 3 — BiLSTM** (4 min) — toon slide 5. *"BiLSTM — Bidirectional LSTM. Twee LSTM's. Eén leest de tijdreeks van begin naar eind, één leest hem omgekeerd. Beide outputs worden samengevoegd."*

   Pauze. *"Wat lost dit op? Toekomst-context. Bij offline batch-analyse — bijvoorbeeld RUL-prognose op een afgeronde dataset — heb je de hele reeks. De BiLSTM gebruikt zowel verleden als toekomst om elke timestep te beoordelen. Dat geeft veel hogere accuracy."*

   Pauze 5 sec. *"Maar... wat is de catch?"* Wacht. Antwoord: je hebt de toekomst nodig — kan dus alleen offline. Bevestig: *"Klopt. BiLSTM kan nooit online — je kunt geen alarm geven op iets wat over 50 samples gebeurt."*

   Schrijf op flip-over: 'BiLSTM: geheugen + toekomst — alleen offline'.

7. **Brug naar fase 2** (1 min 30) — toon slide 6. *"Drie varianten. Eén keuzecriterium: heb je geheugen nodig? Heb je toekomst beschikbaar? Of is je context kort? Op basis daarvan kies je. Dat gaan jullie nu zelf doen."*

**Materiaal:**
- [ ] Slides 1-6
- [ ] wb-01-vergelijkingstabel (1 per deelnemer)
- [ ] Schrift / blocnote (rekwisiet)
- [ ] Drie post-its in kleuren (rekwisiet)
- [ ] A3-diagram zichtbaar
- [ ] Flip-over met drie varianten klaar

> **Tips voor de trainer:**
> - De drie post-its zijn bewust theatrale ondersteuning. Houd ze omhoog terwijl je elke gate benoemt. Visueel verankerd.
> - Tempo: 18 minuten is krap voor drie varianten. Kern is LSTM (6 min); RNN en BiLSTM zijn 4 min elk.
> - Vermijd termen als 'sigmoid', 'tanh', 'cell-state als vector', 'hidden state' tenzij iemand vraagt — dan parkeren.

> **Valkuil — long-term dependency = lange tijdreeks:**
> Iemand zegt 'LSTM is voor lange tijdreeksen, RNN voor korte'. Maak scherp: het gaat om afstand tussen gerelateerde gebeurtenissen, niet tussen het totale aantal samples. Voorbeeld: trillingspiek nu door wrijving 100 samples geleden.

> **Valkuil — drie gates door elkaar:**
> Pak schrift en post-its. Forget = rood = doorstrepen. Input = groen = bijschrijven. Output = geel = voorlezen. Drie gates, drie acties — fysieke koppeling helpt.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de drie varianten onder elkaar op flip-over. Per variant één steekwoord (kort geheugen / lang geheugen / toekomst kennen).
> - **Teamleider sneller:** Vraag 'hoe verschilt LSTM van een 1D-CNN op tijdreeksen?' Antwoord: CNN ziet patronen binnen vast venster, LSTM houdt geheugen over willekeurige afstand.
> - **Gemengde groep:** Vraag bij gates eerst operator: 'als je een ouderwets schrift had — wat zou jij doorstrepen?' Daarna teamleider.

---

### Blok 2: Drie scenario-kaarten — welke variant past?
**00:18 - 00:30** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer toetst het mentale model door drie scenario's te beoordelen op variant-keuze (RNN/LSTM/BiLSTM) en het doorslaggevende criterium (sequentielengte, online/offline) per case te benoemen.

**Werkvorm:** Worked example (IK DOE) bij scenario A, daarna individueel B en C; trainer loopt rond.

**Instructie:**

1. **Deel wb-02 uit** (30 sec). Zeg: *"Drie scenario's. Per scenario kies je: RNN, LSTM of BiLSTM, en welk criterium is doorslaggevend — sequentielengte of online/offline. Vergelijkingstabel uit fase 1 mag op je tafel."*

2. **IK DOE — scenario A voor** (3 min) — toon slide 7. Zeg hardop: *"Scenario A: online vibration-monitoring op een actieve machine. Signaal van afgelopen 50 samples. Alarm binnen seconden gewenst. Mijn redenering: online — dus geen toekomstdata beschikbaar — BiLSTM valt af. Sequentielengte 50 samples is niet kort, niet super lang. Long-term dependency kan optreden — wrijving van 30 samples geleden kan nu een effect hebben. Vanilla RNN is dus risicovol — vergeet te snel. Mijn keuze: LSTM. Doorslaggevend: online + middellange context."*

3. **Deelnemers werken aan B en C** (6 min) — toon slide 8. Zet timer op 6 min. Loop rond. Stel verdiepende vragen:
    - *"Heb je de toekomst beschikbaar?"*
    - *"Hoe lang is je context-venster?"*
    - *"Speelt long-term dependency hier?"*

4. **Korte tussenstand** (1 min) — vraag: *"Wie heeft B al? C ook? Mooi — plenair gaan we dadelijk."*

5. **Tijd-check** (1 min 30) — als 80% klaar is, sluit af.

**Materiaal:**
- [ ] Slides 7-8
- [ ] wb-02-scenarios (1 set per deelnemer, 3 kaarten)
- [ ] Timer
- [ ] Pen

> **Tips voor de trainer:**
> - Bij twijfel: stuur niet bij. Twijfel is leerstof voor fase 3.
> - Loop langs trage starters — vraag hardop: 'wat staat er in scenario B?'
> - Schrijf zelf NIET mee. De plenaire bespreking moet uit de groep komen.

> **Valkuil — BiLSTM voor online scenario:**
> Iemand kiest BiLSTM voor scenario A. Stel de vraag: 'Heb je de toekomst beschikbaar?' Online = nee. BiLSTM heeft toekomstdata nodig. Dus alléén offline. Online = LSTM.

> **Valkuil — scenario C overschat:**
> Iemand kiest LSTM voor scenario C (20 samples, geen lange context). Vraag: 'Speelt long-term dependency hier?' 20 samples = nauwelijks. Vanilla RNN is voldoende — LSTM is overkill. Beide antwoorden mogen, maar ken het verschil.

> **Differentiatie:**
> - **MBO-4 basis:** Vraag hen één criterium per keer: 'online of offline?' eerst. Daarna sequentielengte.
> - **Teamleider sneller:** Vraag: 'wat als de leverancier zegt "we gebruiken LSTM" — welke vraag stel jij om te verifiëren of dat past?' Antwoord: vraag of het systeem online of offline is.

---

### Blok 3: Buurman-check + plenaire bespreking
**00:30 - 00:40** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer toetst eigen redenering aan een ander, hoort een ander perspectief, en herkent waarom scenario B (BiLSTM) een offline-only-oplossing is.

**Werkvorm:** 5 minuten in tweetallen vergelijken — daarna plenaire stemming en bespreking.

**Instructie:**

1. **Deel wb-03 uit** (30 sec). Zeg: *"Tweetal met je buurman. Vergelijk je antwoorden op A, B, C. Bij verschillen: leg elkaar uit waarom. Vul aan het eind in welk criterium voor jou doorslaggevend was."*

2. **Tweetallen werken** (5 min) — zet timer op 5 min. Loop rond. Verzamel 2-3 sterke verschillen voor plenair.

3. **Plenair stemmen** (2 min) — toon slide 9. Per scenario: *"Stem voor RNN. Voor LSTM. Voor BiLSTM."* Tel hardop, schrijf op flip-over.

4. **Bespreking — vooral B als kerncase** (2 min 30) — toon slide 10. *"A is meestal LSTM — online + middellange context. C is vaak vanilla RNN — korte context, long-term dependency speelt nauwelijks. B is de kerncase: 24 uur opgenomen vibration-data, RUL-prognose. Offline + lange sequentie + complete reeks beschikbaar. Hier komt BiLSTM tot zijn recht — beide kanten lezen, hogere accuracy. Maar nooit live inzetbaar."* Pauze. *"In PdM-onderzoek (Li 2026) is BiLSTM precies daarom een kern-keuze voor RUL-prognose op vibration-data."*

**Materiaal:**
- [ ] Slides 9-10
- [ ] wb-03-reflectie
- [ ] Flip-over voor stemming-uitslag
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7. Stilte haalt antwoorden op.
> - Bevestig B als kern. De waarde zit in het inzicht 'offline + accuracy = BiLSTM'.
> - Bij vragen over autoencoder of Isolation Forest als alternatieven: parkeer op flip-over, verwijs naar lo-smart-mfg-092 en lo-smart-mfg-107 voor self-study.

> **Valkuil — discussie over LSTM-formules:**
> IT-affiniteit-vraag over wiskunde van gates. Bedank, parkeer.

> **Differentiatie:**
> - **Gemengde groep:** Vraag eerst operator over scenario A, daarna teamleider over scenario B. Operator brengt werkvloer-realisme, teamleider brengt accuracy-vs-latency-perspectief.

---

### Blok 4: Eigen tijdreeks-scan — actieplan
**00:40 - 00:50** | 10 min | Kolb-fase: experimenteren

**Doel:** Deelnemer kiest één concrete tijdreeks-meting van de eigen lijn (vibration, temperatuur, druk), beschrijft online/offline en context-venster, en koppelt aan een passende variant.

**Werkvorm:** Individueel werkblad — trainer loopt rond en helpt bij concretisering.

**Instructie:**

1. **Deel wb-04 uit** (30 sec). Zeg: *"Laatste 10 minuten. Eén tijdreeks-meting van je eigen lijn (of bij een klant). Vier velden: welke meting, online of offline, hoe lang context-venster, welke variant."*

2. **Inventarisatie-vraag** (1 min) — toon slide 11. *"Eerst rondkijken: bij wie speelt vibration, temperatuur, druk, akoestiek of stroomverbruik? Spuitgieten, CNC, verpakking?"* Vang 4-5 antwoorden.

3. **Individueel werken** (6 min) — zet timer op 6 min. Loop rond. Stel concretiserende vragen:
    - *"Wil je realtime alarmeren of achteraf inzicht?"*
    - *"Hoeveel samples heb je per beslissing nodig?"*
    - *"Speelt long-term dependency — heb je trends die zich opbouwen?"*
    Bij twijfel: 'weet ik niet' is óók waardevol — dat is de eerste vraag aan IT.

4. **Plenaire ronde** (1 min 30) — toon slide 12. *"Twee deelnemers — kort delen: meting, online of offline, gekozen variant."* Vang 2 voorbeelden.

5. **Afsluiting + transferopdracht** (1 min) — toon slide 13. *"Deze week: kijk of er op je lijn een tijdreeks-PdM actief is. Vraag bij IT of leverancier: hoe lang is het context-venster? Online of offline? Welke modelfamilie? Noteer en koppel aan vergelijkingstabel. Volgende sessie bespreken we kort wat je vond."*

**Materiaal:**
- [ ] Slides 11-13
- [ ] wb-04-actieplan
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Bij 'we hebben geen PdM-systeem': hypothetische klant of toekomstig project mag.
> - De plenaire ronde is goud voor volgende sessie. Schrijf 1 regel per voorbeeld.

> **Valkuil — actieplan blijft bij 'we monitoren al vibration':**
> Help één concreet trio: meting / context-venster / online-of-offline. 'Weet ik niet' is óók waardevol.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 8 minuten door werkblad-tijd op 5 min te zetten. Sla afsluiting nooit over.

> **Differentiatie:**
> - **MBO-4 basis:** Eén meting + één variant is genoeg.
> - **Teamleider sneller:** Vraag ook welke organisatorische trade-off (alarm-snelheid vs. accuracy) bij hun productie speelt.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-vergelijkingstabel | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-scenarios (3 kaarten) | n + 2 | A4 dubbelzijdig |
| ☐ | wb-03-reflectie | n + 2 | A4 enkelzijdig |
| ☐ | wb-04-actieplan | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-ai-fund-rnn-001.svg | 1 op A3 | LSTM-cel met drie gates, zichtbaar in zaal |
| ☐ | Schrift / blocnote | 1 | Rekwisiet voor schrift-analogie |
| ☐ | Post-its in 3 kleuren | 1 set | Voor de drie gates |
| ☐ | Markeerstiften | n | Voor wb-01 |
| ☐ | Pennen | n + 5 | Reserve op trainertafel |
| ☐ | Flip-over | 2 | Parkeerlijst + drie varianten |
| ☐ | Dikke stiften | 3 | Voor flip-over |
| ☐ | Timer / mobiel met geluid | 1 | Voor 5-min en 6-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 theoretiseren | Vergelijkingstabel invullen tijdens drie varianten | Mentaal model: kort / lang / lang+toekomst |
| 2 ervaren | Drie scenario-kaarten beoordelen | Per case: variant + doorslaggevend criterium |
| 3 reflecteren | Buurman-check + plenair | Inzicht: B (RUL offline) is BiLSTM-kerncase |
| 4 experimenteren | Eigen tijdreeks-actieplan | Concrete meting + venster + online/offline + variant |

**Slagingscriterium:** drie varianten benoemen + minimaal 2 van 3 scenario's correct + actieplan met concrete tijdreeks.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Flip-over met drie varianten gefotografeerd
- [ ] Genoteerd: stemming per scenario (verdeling = indicatie groepsbegrip)
- [ ] Notitie voor volgende sessie: wie ging IT bevragen?
- [ ] xAPI-statements verstuurd: `experienced` (vergelijkingstabel), `completed` (scenario's + actieplan), `attempted` (transferopdracht)

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | RNN/LSTM/BiLSTM*
*Bronnen: Hochreiter & Schmidhuber (1997) LSTM. | Schuster & Paliwal (1997) Bidirectional RNN. | Olah (2015) Understanding LSTM Networks. | Li (2026) BiLSTM voor RUL-prognose.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
