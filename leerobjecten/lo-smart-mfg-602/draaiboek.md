# Het patroon van elk AI-camerasysteem — Draaiboek
*Module 1: Gebruik | 40 minuten | 6-16 deelnemers*

> Voor de trainer. Deze sessie bouwt voort op `lo-smart-mfg-601` (data als bottleneck). Deelnemers horen die te hebben gedaan; als dat niet zo is, besteed de eerste 3 minuten aan een samenvatting van die kernboodschap.

---

## Overzicht

| Blok | Titel | Kolb-fase | Scaffolding | Duur | Werkvorm |
|------|-------|-----------|-------------|------|----------|
| 1 | Het patroon meetekenen | theoretiseren | **IK DOE** | 10 min | trainer tekent, deelnemers schrijven mee |
| 2 | Case-diagnose | experimenteren | **WIJ DOEN** + **JIJ DOET** | 15 min | plenair case A + duo case B/C |
| 3 | Reflectie — wat viel op? | reflecteren | — | 10 min | duo (3) + plenair (7) |
| 4 | De 5-vragen-test op jouw werkvloer | experimenteren (transfer) | — | 5 min | individueel |
| | **Totaal** | | | **40 min** | |

---

## Voorbereiding

### Materialen checklist

- [ ] Werkblad 1 (patroon meetekenen): 1 per deelnemer
- [ ] Werkblad 2 (case-diagnose): 1 per duo, inclusief case B en case C geprint op half-A4
- [ ] Werkblad 3 (reflectie): 1 per deelnemer
- [ ] Werkblad 4 (5-vragen-test): 1 per deelnemer
- [ ] Case A (lopende band 3 — 3× meer afkeur): wordt mondeling gebracht, kaartje op flipover met de situatie is voldoende
- [ ] Flipover + dikke stift (zwart + rood)
- [ ] Pen per deelnemer
- [ ] Optioneel: beamer voor Slidev (`presentatie.slidev.md`) — maar flipover is primair

### Ruimte-inrichting

Duo-opstelling. Flipover vanaf elke plek zichtbaar. Voldoende schrijfruimte per persoon.

### Voorkennis trainer

- Je bent geen AI-expert en hoeft dat niet te zijn. Je moet het vijf-vakjes-patroon kunnen tekenen en voor elk vakje één faalpunt kunnen benoemen. Werkblad 1 en het diagram helpen je daarbij.
- Lees het kennisobject `ko-smart-mfg-602` (1 A4).
- Doorloop werkblad 2 — drie cases — vooraf zelf. Weten hoe jíj ze zou diagnosticeren maakt het begeleiden makkelijker.
- Je hoeft geen 'juiste' antwoorden paraat te hebben. De cases hebben geen éne correct antwoord — het gaat om de manier van kijken.

---

## Toon en aanpak

Deze sessie werkt het best als je:

- **Structuur voorziet en oplossingen terughoudt.** Je tekent het patroon — dat is het raamwerk. De invulling komt van de groep. Jouw beste zin: *"interessant — wat zou de volgende vraag zijn?"*.
- **Twijfel als kwaliteit behandelt.** Operators die vragen stellen in plaats van antwoorden geven, zijn goede diagnostici. Beloon dat gedrag expliciet.
- **Expliciet coacht, niet traint.** Deze doelgroep is bewust_onbekwaam — ze weten wat ze niet weten. Ze hebben geen behoefte aan instructie, wel aan begeleiding bij toepassing.
- **Case-keuze respecteert.** Duo's kiezen zelf tussen case B en C. Als ze beide willen doen: zeg dat dat niet in de tijd past, maar ze kunnen na de sessie de andere nog bekijken.
- **Aan de eigen werkvloer teruggeeft.** Elk blok eindigt in principe met één zin die terug koppelt naar hun dagelijkse praktijk. Ook als zij dat zelf nog niet zien.

Operators die dit leerobject volgen na KO-601 willen bewijs dat wat ze leren bruikbaar is. De 5-vragen-test (blok 4) is dat bewijs.

---

## Blok 1: Het patroon meetekenen — IK DOE *(10 min)*

### Wat je doet

1. Open met: *"Vorige sessie hebben we het gehad over waarom data de bottleneck is. Nu gaan we kijken naar hoe het systeem als geheel werkt — zodat je zelf kunt zien waar het stuk kan."*
2. Deel werkblad 1 uit.
3. Teken op de flipover de vier hoofdvakjes: **CAMERA → BEELD → MODEL → BESLISSING**. Tussen elk vakje een dikke pijl.
4. Per vakje benoem je in één zin wat het doet. Operators schrijven mee op hun werkblad.
5. Teken dan naast de lijn — onder het model — een gestippelde pijl van een extra vakje **TRAININGSDATA** richting het model. Zeg: *"dit is de onzichtbare vijfde stap — die is al gebeurd voordat het systeem live ging. Maar het bepaalt alles."*
6. Tenslotte: maak een tabel onder het patroon met vijf rijen — één per component — en per rij één voorbeeld-faalpunt. Operators noteren het in hun tabel.

### Wat je zegt

> **Opening:** *"Jullie gaan een patroon leren dat past op elk AI-camerasysteem. Dat is bruikbaar voor morgen en over tien jaar."*

> **Per vakje:** *"De camera... maakt een foto."* (simpel, niet te lang)

> **Bij trainingsdata:** *"Dit is de vijfde stap die je niet ziet als het systeem draait — maar die bepaalt hoe goed het werkt."*

### Waar je op let

- Deelnemers die al willen diagnosticeren tijdens blok 1 ("bij ons gaat het mis bij..."). Goed signaal, maar parkeer het: *"Hou dat vast voor blok 2 — we gaan zo met concrete cases werken."*.
- Deelnemers die nog niet meetekenen. Dat is een stille barrière. *"Doe maar gewoon mee met tekenen, ook als het scheef wordt."*.

### Veelgemaakte fouten

- **Techniek uitleggen.** Verleidelijk om te vertellen wat het model precies doet (neural network, convolutional layers). Doe dat niet — het breekt het niveau. Blijf bij "het model kijkt en beslist".
- **Alle vijf faalpunten uitwerken.** Dat kan niet binnen 10 minuten en het is ook niet nodig — blok 2 gaat daar dieper op in.
- **Projecteren in plaats van tekenen.** Schrijvend uitleggen werkt beter. Slidev is aanvullend, niet primair.

### Differentiatie

- **Sterkere groep:** Laat hen het patroon eerst zelf tekenen in duo's (3 min) — dan check jij plenair. Werkblad 1 fungeert dan als antwoord-blad.
- **Zwakkere groep:** Voeg een minuut toe voor de trainingsdata-pijl. Dat is het concept dat het lastigst landt.

### Kernboodschap

Vier zichtbare vakjes + één onzichtbare. Samen vormen ze het patroon van elk AI-camerasysteem. Het patroon is universeel.

### Suggestie

Als iemand in blok 1 al een voorbeeld van faalpunt aandraagt uit eigen ervaring — schrijf het bij de juiste rij in de tabel. Gebruik het citaat in blok 2 bij de cases: *"Eva noemde net al een voorbeeld van een vuile lens — dit is wat je toen bedoelde."*.

### Overgang naar blok 2

> *"Nu gaan we dit patroon gebruiken. Ik geef jullie een situatie, en samen stellen we de diagnose."*

---

## Blok 2: Case-diagnose — WIJ DOEN + JIJ DOET *(15 min)*

### Wat je doet

**WIJ DOEN (5 min) — plenair case A:**
1. Schrijf op de flipover: *"Lopende band 3. Sinds vanochtend 3× zoveel afkeur. Producten lijken voor het oog goed. Wat check je?"*.
2. Ga met de groep systematisch door de vakjes: camera → beeld → model → beslissing → trainingsdata.
3. Vraag per vakje: *"wat zou hier stuk kunnen zijn?"*. Noteer op de flipover bij het vakje.
4. Rond af: *"Welk vakje gaan we als eerste checken? Waarom dat?"*. Laat de groep beslissen.

**JIJ DOET (10 min) — duo's case B of C:**
1. Deel werkblad 2 uit. Zeg: *"Kies samen met je buurman één case — B of C. Je hebt 7 minuten om het patroon toe te passen op jullie case. Voor elk vakje: wat zou stuk kunnen zijn, en welke vraag zou je stellen."*.
2. Loop rond. Stel diagnostische vragen (niet antwoorden geven): *"waar begin jullie?"*, *"welke vraag lijkt jullie het eerste zinnig?"*.
3. Na 7 minuten: 2-3 duo's presenteren hun diagnose. Max 1 minuut per duo. Vraag aan de groep: *"wie heeft dezelfde case gedaan en is het eens of oneens?"*.

### Wat je zegt

> **Start WIJ DOEN:** *"Stel je bent opgeroepen. Lopende band 3. Wat zou jij als eerste checken?"*

> **Overgang naar JIJ DOET:** *"Nu jullie. Case B of C — kies samen. Zeven minuten."*

> **Bij rondlopen:** *"Waar zijn jullie nu? Welke vraag staat al?"*

### Waar je op let

- Duo's die alleen invullen zonder te praten. Onderbreek: *"Wat denken jullie — praat eens even hardop."*.
- Duo's die alle vijf vakjes hetzelfde antwoord geven. Dat is een red flag — het patroon is dan niet gebruikt. *"Probeer eens een ander vakje dan het eerste."*.
- Dominante stem in plenaire diagnose. *"Dank, andere kant — wat zie jij?"*.

### Veelgemaakte fouten

- **Zelf oplossen.** Je weet (hopelijk) het 'juiste' antwoord bij case B en C. Niet zeggen. Laat hen zoeken — foute richtingen leveren de beste leerervaring.
- **Te weinig tijd voor JIJ DOET.** Als WIJ DOEN uitloopt naar 8 minuten, heb je voor de duo's maar 7 minuten. Die duo's moeten de meeste tijd krijgen.
- **Alle duo's presenteren.** Dat kost 15 min. Twee tot drie is genoeg. Laat vrijwilligers opstaan, niet elk duo.

### Differentiatie

- **Sterkere groep:** Geef duo's toegang tot beide cases maar met beperkte tijd. *"Kies: diep op één, of ondiep op twee."*. Laat hen kiezen.
- **Zwakkere groep:** Doe WIJ DOEN langzamer (7 minuten in plaats van 5). Geef duo's maar één case — wijs het toe, laat ze niet kiezen.

### Kernboodschap

Het patroon is een denkgereedschap. Toepassing is de vaardigheid. Oefening is hoe je 'm leert.

### Suggestie

Als een duo in hun diagnose uitkomt op trainingsdata als oorzaak (zoals in case C bij de donkerder kapjes) — laat hen dat expliciet koppelen aan KO-601. *"Vorige sessie ging over data als bottleneck. Dit is wat dat in de praktijk betekent."*.

### Overgang naar blok 3

> *"Oké. Nu even niet aan diagnoses denken. Alleen: hoe was dat?"*

---

## Blok 3: Reflectie — wat viel op? *(10 min)*

### Wat je doet

1. Duo-gesprek (3 min): *"Met je buurman — welk vakje was het lastigst om een vraag bij te bedenken? Waar twijfelden jullie?"*.
2. Plenair (7 min): trek antwoorden uit de groep. Zet op de flipover de vakjes en turf welke het vaakst worden genoemd als 'lastig'.
3. Reflecteer: *"Het vakje dat jullie lastig vinden is vaak het vakje waar in de praktijk ook de meeste fouten zitten. Vuile lens wordt altijd vergeten — niemand denkt daaraan. Dat maakt het 'saaie' vakje ironisch het belangrijkste."*.
4. Laat werkblad 3 invullen tijdens het plenaire deel (niet na).

### Wat je zegt

> **Openingsvraag duo:** *"Welk vakje was het lastigst? Waar twijfelden jullie?"*

> **Reflectie:** *"Wat jullie lastig vinden, is vaak waar het in de praktijk misgaat."*

### Waar je op let

- Een deelnemer die zegt "niets was lastig". Dat kan. Doorvragen: *"dat is fijn — wat maakte het helder?"*. Vaak volgt dan wel iets.
- Stilte bij de plenaire vraag. Wachten is oké. Niet invullen.

### Veelgemaakte fouten

- **Te snel conclusies trekken.** Laat de groep het werk doen. Je synthese kan pas aan het eind.
- **Persoonlijk worden.** *"Wat vind jij van...?"* — dat klinkt als examen. Vraag liever naar observaties: *"wat was lastig?"*.

### Differentiatie

- **Introverte groep:** Voeg een extra minuut toe voor individueel opschrijven in het duo-deel vóór het gesprek begint.
- **Spraakzame groep:** Beperk plenaire reacties tot 2-3 en ga over naar de reflectie-conclusie.

### Kernboodschap

Je voelt waar je mentaal nog geen ankers hebt. Dat is waardevolle informatie — het wijst precies aan waar je meer wilt leren.

### Suggestie

Als de groep alle vakjes 'lastig' vindt (in plaats van één specifiek): daag hen uit. *"Alle vijf? Oké — welke zou je als eerste onder de knie willen krijgen?"*. Dat prioriteren is ook reflectie.

### Overgang naar blok 4

> *"Laatste blok. Nu gaat het over jullie eigen werkvloer."*

---

## Blok 4: De 5-vragen-test *(5 min)*

### Wat je doet

1. Deel werkblad 4 uit. Zeg: *"Kies één AI-camerasysteem dat je kent. Formuleer voor elk vakje één vraag die je zou stellen aan de beheerder. Vijf vragen, vijf minuten."*.
2. Loop rond. Help deelnemers die geen systeem kunnen noemen — verwijs naar eerder genoemde voorbeelden uit de groep.
3. Benoem de vervolgopdracht expliciet: *"Deze week stel je één van die vragen. Kies de vraag bij het vakje waar jij het minste over weet."*.
4. Afsluiting: laat twee of drie deelnemers één vraag hardop delen.

### Wat je zegt

> **Opening:** *"Niet een verzonnen systeem. Iets wat je kent — bij jezelf of bij een bedrijf."*

> **Bij rondlopen:** *"Welke vraag is voor jou het spannendst om te stellen?"*

> **Afsluitende kernvraag:** *"Bij welke vraag verwacht jij het meest interessante antwoord?"*

### Waar je op let

- Deelnemers die "alle vijf vakjes werken vast wel" opschrijven. Dat is geen diagnose, dat is blind vertrouwen. *"Je weet toch niet welk model er draait? Hoe check je dat?"*.
- Deelnemers zonder systeem voor ogen. *"Kijk eens rond op je telefoon — video over Philips Drachten, Waymo, CAPTCHA — daar zit het patroon ook in."*.

### Veelgemaakte fouten

- **Generieke vragen accepteren.** *"Werkt de camera goed?"* — nee, dat is geen vraag. *"Wanneer is de lens voor het laatst schoongemaakt?"* — dát is een vraag.
- **Afsluiten zonder kernvraag.** De sessie moet een haak hebben voor de week die komt.

### Differentiatie

- **Deelnemers zonder directe werkvloer-toegang:** Laat hen een publiek systeem kiezen (zelfrijdende auto, CAPTCHA, gezichtsherkenning bij de luchthaven) en die vragen formuleren.
- **Deelnemers die snel klaar zijn:** Vraag om één vraag per vakje te ranken op 'hoe spannend is dit antwoord voor mij' — dat maakt prioritering zichtbaar.

### Kernboodschap

Het patroon is nu jouw denkgereedschap. De 5-vragen-test is jouw gebruiksaanwijzing.

### Suggestie

Als je op de flipover nog ruimte hebt: noteer de vijf systemen die deelnemers kiezen. Een week later (volgende sessie) vraag je: *"wie heeft welke vraag gesteld, en wat was het antwoord?"*. Dat maakt de leerlijn zichtbaar.

---

## Afsluiting *(laatste minuut)*

Vat samen in één zin: *"Vier zichtbare stappen, één onzichtbare, vijf faalpunten, vijf vragen. Dat is alles."*.

Bedank kort. Verwijs naar de volgende sessie: *"Module 2 — Train. Daar gaan we niet meer naar systemen kíjken, maar er zelf mee werken."*.

---

## Veelgestelde vragen van deelnemers

**"Wat als mijn systeem meer dan één camera heeft, of meerdere modellen?"**
Het patroon herhaalt zich dan per camera of per model. Je tekent het dan vijf keer parallel, of als een keten. De kernvragen blijven hetzelfde.

**"Is het model dat we in de les noemen hetzelfde als wat Google gebruikt?"**
Hetzelfde idee, andere schaal. De architectuur (neural network) lijkt op elkaar. Het verschil zit in hoeveelheid trainingsdata en rekenkracht — daar werken we aan in Module 2 en 3.

**"Kunnen we het patroon ook gebruiken bij sensordata-systemen, bijvoorbeeld bij trillingen?"**
Ja. Vervang 'camera' door 'sensor' en 'beeld' door 'datapunt'. De rest (model, beslissing, trainingsdata) is identiek. Predictive maintenance werkt volgens dit patroon.

**"Wie beslist eigenlijk wanneer een model moet worden bijgetraind?"**
In theorie: de beheerder van het systeem, op basis van signalen (meer afkeur, meer gemiste defecten). In praktijk: vaak niemand, tot er een probleem ontstaat. Dat is precies waarom operators die het patroon herkennen waardevol zijn — zij kunnen het signaal als eerste geven.

**"Wat als wij dit patroon willen gebruiken om een systeem te koppen, en de leverancier is nog niet eens geselecteerd?"**
Nog beter. Stel de vijf vragen vóór de aanschaf, niet erna. Als een leverancier er niet op kan antwoorden, weet je dat het een dure pilot gaat worden in plaats van een product.

---

## Alternatieve tijdsverdeling

### Als je maar 25-30 minuten hebt

- Blok 1 in 7 min. Laat de vijf-faalpunten-tabel weg in de sessie; hij staat op werkblad 1 en ze zien hem tijdens blok 2.
- Blok 2 in 10 min — alleen case A plenair, geen duo-werk.
- Blok 3 plenair in 5 min (geen duo-gesprek).
- Blok 4 als huiswerk — geef werkblad 4 mee.

### Als je 60 minuten hebt

- Blok 2 uitgebreid: plenair case A + alle duo's zowel case B als case C. 20 min in plaats van 15.
- Voeg een blok 5 toe (10 min): **ethische dimensie**. *"Stel jullie systeem keurt structureel producten van leverancier X af. Is dat een technisch probleem of een ethische keuze? Wie beslist wat acceptabel is?"*.
- Blok 4 met peer-check: duo's wisselen werkblad 4 en bekritiseren elkaars vragen.

---

## Reserve-materiaal

**Vierde case (als je tijd over hebt in blok 2):** *"Systeem X werkt goed op één productielijn maar is nu gekoppeld aan een tweede lijn — daar werkt het slechter. Waar zit het probleem?"*. Hint: trainingsdata + beeld-kwaliteit.

**Quote-bank voor afsluiting:** *"Een patroon dat je eenmaal herkent, zie je overal. Die herkenning is jouw voorsprong."* — niet elke trainer zal dit uitspreken, maar voor groepen die meer contextueel gestimuleerd moeten worden, is het een nuttige afsluitzin.

---

*Onderdeel van de AIMM × BronzGreen curriculum-pipeline. Gegenereerd uit `lo-smart-mfg-602-trainee.yaml`, structuur conform blueprint `docenthandleiding-w00.md` + patronen uit `lo-smart-mfg-601` (zelfde pipeline, andere didactische keuzes).*
