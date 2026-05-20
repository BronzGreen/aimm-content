# Gevoeligheid versus vals alarm — Draaiboek
*SPC Module 2 (Train) | Workshop-blok 40 minuten | 6-10 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan uitleggen waarom meer signaalregels niet automatisch een betere regelkaart opleveren, en kan op basis van ARL-getallen (371 / 91,75 / ~50) voor een lijn met 96 metingen per dag uitrekenen hoeveel vals alarm te verwachten is — in minimaal 2 van de 3 regelsets correct. |
| **Doelgroep** | Operators MBO-3 (primair), operators MBO-4 mogelijk aangehaakt, 6-10 personen |
| **Voorkennis** | ko-spc-201 doorlopen — kent ±3σ-band en het begrip 'signaal'. Heeft in Module 1 (Gebruik) regelkaart-basis geleerd. Het woord 'vals alarm' is uit praktijk bekend. |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat zijn lijn te vaak of te weinig alarm geeft, maar kent de afweging gevoeligheid vs vals alarm nog niet in getallen. De rekenoefening activeert die onbekwaamheid bewust ('mijn lijn krijgt elke dag alarm — past dat bij wat ik nu reken?'). |
| **Begeleidingsstijl** | Trainen — veel sturing én veel ondersteuning. Scaffolding via IK DOE → JIJ DOET: trainer modelleert de eerste rekensom plenair, deelnemers rekenen de andere twee zelf, daarna reflectie en theorie. De rekensom is eenvoudig; het besef is het leerdoel. Trainer demonstreert actief, bevestigt elke poging. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, rekenmachines beschikbaar |
| **Plek in module** | Workshop-blok binnen module 2 (Train) — bouwt voort op lo-spc-201 (Nelson + stabiliteit), leidt naar configuratiebesluit-reflectie voor eigen lijn |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Alarm-rekenoefening: vals alarm per dag op 3 regelsets | 🟢 ervaren | 15 min |
| 00:15 - 00:27 | STARRT-reflectie: mijn eigen ervaring met vals alarm | 🟣 reflecteren | 12 min |
| 00:27 - 00:40 | Handout: drie regelsets + ARL-tabel + gefaseerde aanpak | 📘 theoretiseren | 13 min |

**Totaal:** 40 minuten — geen aparte pauze (kort workshop-blok).
**Buffer:** elk blok bevat 1-2 minuten flexibele ruimte; gebruik die voor doorvragen of uitloop in fase 1 (rekenoefening).

---

## Voorbereiding

### De avond ervoor
- [ ] Print `wb-01-oefening.md`, `wb-02-reflectie.md`, `wb-03-handout.md` — elk n + 2 reserve (totaal ca. 36 vellen bij 10 deelnemers).
- [ ] Print `diagram-lo-spc-202.svg` op A3 (in kleur indien mogelijk — drie staafjes naast elkaar: kaal / WECO / Nelson).
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer.
- [ ] Lees het ARL-voorbeeld in dit draaiboek door. Herinner jezelf: het getal 91,75 komt uit **Champ & Woodall (1987, Technometrics)** — niet uit NIST.
- [ ] Check de doelgroeplijst: zijn er teamleiders bij? Zo ja, bereid je voor op de extra vraag over welke regelset zij zelf in hun lijn actief hebben staan.

### Het uur ervoor
- [ ] Leg per stoel: pen, rekenmachine (of vraag deelnemers hun telefoon te gebruiken), `wb-01-oefening.md`.
- [ ] Houd `wb-02` en `wb-03` apart op de trainer-tafel — uitdelen pas op het juiste moment in de sessie.
- [ ] Hang de A3-versie van het diagram zichtbaar achter in de zaal (nog afdekken — pas onthullen in blok 3).
- [ ] Schrijf op de flip-over alvast drie koppen: links **"Kaal — 371"**, midden **"WECO — 91,75"**, rechts **"Nelson — ~50"**. Dit wordt je structuur bij blok 3.
- [ ] Open slide 1 op het scherm.
- [ ] Leg 4-5 rekenmachines klaar op de trainer-tafel voor wie geen telefoon bij de hand heeft.

---

## Blok-details

### 🟢 Blok 1: Alarm-rekenoefening — hoeveel vals alarm per dag?
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** De deelnemer rekent voor drie regelsets op dezelfde fictieve lijn uit hoeveel vals alarm te verwachten is — en schrikt zichtbaar bij het verschil tussen kale Shewhart en volledige Nelson. Verwarring wordt geactiveerd ("zoveel vals alarm per dag? Echt?") als leerbrandstof voor fase 2 en 3.

**Werkvorm:** Individuele rekenoefening (JIJ DOET), voorafgegaan door een trainer-gedemonstreerd voorbeeld (IK DOE). Drie scenario's op dezelfde fictieve Verpakkingslijn B.

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Wie van jullie heeft deze week op de eigen lijn een alarm meegemaakt waarvan achteraf bleek dat er niks aan de hand was?"* Wacht. Laat 2-3 mensen kort knikken of een kort woord zeggen. Geen lange verhalen.

2. **Trigger** (1 min) — toon slide 2. *"Vandaag gaan we in 40 minuten het verschil begrijpen tussen 'gevoeligheid' en 'vals alarm'. En we doen dat niet met een theorie-verhaal — we beginnen met rekenen. Op een fictieve lijn, want rekenen is altijd makkelijker als iedereen met dezelfde getallen werkt."*

3. **Korte ophaal voorkennis** (1 min) — *"Snelle check: wat is een regelkaart? Wie kan in één zin zeggen wat die ±3σ-band op de kaart doet?"* Vang 1-2 antwoorden, bevestig kort. Dit is geen hertoetsing — alleen herinnering. Verwijs naar ko-spc-201.

4. **Deel wb-01-oefening uit** (30 sec). Zeg: *"Eén fictieve verpakkingslijn. 8 uur per dag. Meet elke 5 minuten. Dat zijn 96 metingen per dag. Het proces is in werkelijkheid stabiel — alle alarmen die afgaan zijn dus vals. De vraag: hoeveel krijg je er per dag bij drie verschillende regelsets? Rekensom: metingen per dag gedeeld door ARL."*

5. **IK DOE — demonstreer scenario A plenair** (2 min) — toon slide 3. Pak een markeerstift. Schrijf op de flip-over: **"Scenario A: ARL = 371"**. Zeg hardop: *"96 gedeeld door 371. 96 / 371. Dat is ongeveer 0,26. Dus 0,26 vals alarm per dag. Anders gezegd: je moet ongeveer 4 dagen wachten voor er 1 valsloos alarm-dag voorbij komt."* Schrijf op de flip-over: **"0,26/dag → ~1 per 4 dagen → goed te doen"**. *"Zo rekenen jullie straks zelf Scenario B en C uit. Scenario A heb ik nu voor jullie voorgerekend — als zekerheid."*

6. **JIJ DOET — individueel scenario B en C** (8 min) — zet timer op 8 min. Zeg: *"Pak je rekenmachine of telefoon. Scenario B is WECO, ARL = 91,75. Scenario C is volledige Nelson — we rekenen met een schatting ARL = 50, want het echte getal varieert per bron. Vul de tabel in, kies per scenario je oordeel (goed te doen / voelbaar / te veel), en schrijf onderin welk scenario je het meest schokte."* Loop rustig rond. Help alleen bij technische struikelingen (*"waar deel ik door?"*) — GEEN interpretatie-hints. Als iemand tussentijds vraagt 'klopt mijn antwoord?': *"Rond even af — straks bespreken we plenair."*

7. **Korte plenaire check** (1 min 30) — *"Pen neer. Scenario B, WECO: wat kreeg je?"* Vang 2-3 antwoorden (verwachte antwoord: ~1 per dag, 5 per week). *"Scenario C, Nelson met ARL = 50: wat kreeg je?"* Vang 2-3 antwoorden (verwacht: ~2 per dag, 10 per week). *"Welk scenario schokte het meest?"* 2-3 korte antwoorden. Bevestig: *"Precies. Dit is de afweging waar het vandaag over gaat."*

**Materiaal:**
- [ ] wb-01-oefening.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Rekenmachine of telefoon (1 per deelnemer — leg 4-5 reserves klaar)
- [ ] Slide 1 (cover), slide 2 (trigger), slide 3 (rekenoefening-intro)
- [ ] Flip-over met drie koppen Kaal / WECO / Nelson
- [ ] Timer

> **Tips voor de trainer:**
> - Loop tijdens de oefening langs maar buig je niet over schouders — dat verhoogt prestatiedruk en maakt twijfel onzichtbaar.
> - Als iemand al na 3 minuten klaar is: vraag *"Heb je naast de rekensom ook je oordeel ingevuld — en de vraag 'welk scenario schokte je het meest'?"* Die open vragen zijn de aanloop naar fase 2.
> - De rekensom 96 / 91,75 ≈ 1,046 kan rare decimalen geven. Accepteer 'ongeveer 1 per dag' — het gaat om de orde van grootte.

> **Differentiatie:**
> - **MBO-3 die moeite heeft met de deling:** ga naast de deelnemer zitten, doe één rekensom voor. Daarna moedig aan: "nu reken jij de volgende zelf." Niet schaamtevol benaderen — de rekensom is bijzaak.
> - **MBO-4 of teamleider die snel klaar is:** geef extra vraag: *"Reken ook eens hoeveel vals alarm je op jullie eigen lijn zou verwachten bij WECO — weet jij hoeveel metingen per dag jullie lijn doet?"* Schrijf antwoord op losse post-it. Parkeer voor blok 2.

> **Valkuil — operators willen alle Nelson-regels uitgelegd krijgen:**
> Bij vraag *"wat zijn die 8 Nelson-regels precies?"*: zeg *"Een deel staat in de handout straks, met een korte uitleg per regel. Vandaag gaat het niet om de regels kennen — vandaag gaat het om de afweging begrijpen. De regels zelf komen terug in latere sessies."* Niet nu uitleggen.

> **Valkuil — rekensom-angst:**
> Een deelnemer zegt *"ik ben slecht in rekenen"* of blokkeert. Zeg rustig: *"De rekensom is delen — dat doet je rekenmachine voor je. Wat ik wil weten is wat je voelt bij de uitkomst. Reken eerst, voelen komt straks."* Geef indien nodig de getallen voor: *"96 / 91,75 = ongeveer 1. Dat is dus 1 vals alarm per dag. Wat vind je daarvan?"* Hou het klein.

---

### 🟣 Blok 2: STARRT-reflectie — mijn eigen ervaring met vals alarm
**00:15 - 00:27** | 12 min | Kolb-fase: reflecteren

**Doel:** De zojuist uitgerekende getallen koppelen aan een persoonlijke herinnering. Door de eigen ervaring met vals alarm bewust te maken, ervaart de deelnemer dat alarm-fatigue een reëel werkplekprobleem is — geen abstract concept. STARRT-structuur geeft houvast.

**Werkvorm:** Individueel invullen (8 min) + korte buurman-uitwisseling (3 min) + plenaire oogst (1 min).

**Instructie:**

1. **Overgang** (30 sec) — *"Die getallen die jullie net uitrekenden — waarschijnlijk herken je er iets in van je eigen werkdag. Nu gaan we kijken naar één concrete herinnering. Een moment dat op jouw lijn een alarm afging dat achteraf geen echt probleem bleek."*

2. **Deel wb-02-reflectie uit** (30 sec). Normaliseer meteen: *"Bijna iedereen heeft wel eens een alarm genegeerd dat achteraf niks was — of juist een alarm serieus genomen dat later vals bleek. Dat is alarm-fatigue in actie. Geen slechte mentaliteit — een reëel effect van een te gevoelige regelset. Dit werkblad laat je niet afgaan. Het laat je herkennen."*

3. **Individueel invullen** (8 min) — zet timer. Zeg: *"STARRT: Situatie, Taak, Actie, Resultaat, Reflectie, Transfer. Eén zin per stap. Niet een opstel — één zin. In de Transfer-stap gebruik je de ARL-getallen die je net hebt uitgerekend: wat zou je een volgende keer anders doen nu je weet dat WECO ongeveer 1 vals alarm per dag geeft?"* Loop rond. Help bij blokkades, vooral bij 'Taak' (want die is abstract) en 'Reflectie' (want die is zelfkritisch). Normaliseer: *"Je rol was misschien gewoon 'werk doorgaan' — dat mag."*

4. **Buurman-uitwisseling** (3 min) — *"Draai je stoel naar je buurman. Deel één ding: welke situatie heb je opgeschreven, en wat had je achteraf anders gedaan als je de ARL-getallen toen al had geweten? Twee mensen, 3 minuten — dus 90 seconden per persoon. Geen discussie, alleen delen en luisteren."* Loop langs. Bij vastgelopen duo's: *"Begin bij de Situatie. Wat was het alarm en wat bleek het?"*

5. **Plenaire oogst** (30 sec) — *"Wie wil er één zin delen: wat zou je een volgende keer anders doen of navragen?"* Vang 1-2 vrijwilligers. NIET iedereen laten delen — dan kost het te veel tijd en wordt het bespreking in plaats van oogst.

6. **Overgang naar blok 3** — *"Jullie hebben nu zelf gerekend, jullie hebben nu zelf teruggekeken. Nu gaan we naar de theorie. En je zult zien: de theorie bevestigt vooral wat jullie al vermoedden."*

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slide 4 (STARRT-intro)
- [ ] Timer

> **Tips voor de trainer:**
> - Laat de stilte tijdens het individueel invullen er zijn. Niet opvullen met muziek of extra uitleg — stilte is denktijd.
> - Tel innerlijk tot 7 na de plenaire vraag. Niet zelf invullen.
> - Als niemand vrijwillig wil delen: geef zelf een voorbeeld uit je eigen praktijk (1 zin). Daarna een open uitnodiging. Als het dan niet komt: parkeer het, ga door.

> **Differentiatie:**
> - **Deelnemer herinnert zich niks:** vraag door: *"Denk eens aan een verstorings-alarm waar je naartoe bent gelopen. Hoe bleek het aflopen?"* of: *"Denk aan een collega die wel eens 'ach, dat alarm hoor je altijd wel' heeft gezegd."* Herinneringen ontstaan vaak via dat soort aanhaakjes.
> - **Teamleider erbij:** vraag extra: *"Schrijf op je werkblad ook op: wanneer heb jij als teamleider beslist om een regelset aan of uit te zetten — en waarom?"*

> **Valkuil — reflectie wordt bespreking:**
> De buurman-uitwisseling loopt uit naar discussies ('en toen zei mijn teamleider...'). Stop kort. *"We zijn in reflectie-modus, niet in bespreking-modus. Elkaar horen is het doel — niet elkaars gelijk krijgen. Nog 1 minuut."* Bewaak de tijd.

> **Valkuil — iemand die 'ik negeer alarmen nooit' verdedigend zegt:**
> Niet in discussie gaan. Zeg: *"Je bent blijkbaar goed afgestemd op jouw lijn — dat is waardevol. Schrijf dan op: welke regelset staat bij jullie aan, en hoe heb je dat geleerd?"* Verplaats de energie van verdedigen naar reflectie op eigen competentie.

---

### 📘 Blok 3: Handout — drie regelsets, ARL-tabel, gefaseerde aanpak
**00:27 - 00:40** | 13 min | Kolb-fase: theoretiseren

**Doel:** De ervaring (fase 1) en de reflectie (fase 2) worden verankerd in het theoretisch kader. De deelnemer ziet de getallen die hij zelf heeft uitgerekend terug in een officiële tabel, snapt waar ze vandaan komen, en begrijpt waarom AIMM signaalregels gefaseerd opbouwt. Theorie als bevestiging, niet als last.

**Werkvorm:** Trainer-geleide handout-bespreking met markering van aha-momenten. Onthulling van het A3-diagram.

**Instructie:**

1. **Onthul het diagram** (1 min) — verwijder de afdekking van de A3-versie achter in de zaal. Toon slide 8. Zeg: *"Drie staafjes. Kaal, WECO, Nelson. Let op de verhouding. Dat is precies wat jullie net hebben uitgerekend."*

2. **Deel wb-03-handout uit** (30 sec). *"Pak je markeerstift. Markeer wat voor jou nieuw of verrassend is. Ik ga de handout plenair doorlopen — jij mag op elk moment een vraag stellen."*

3. **Bespreek de centrale zin** (1 min) — slide 5. Lees hardop voor: *"Elke extra signaalregel maakt je regelkaart gevoeliger — maar ook vaker vals. Te veel regels = alarm-fatigue. Operators gaan signalen negeren."* Stilte. *"Deze zin is de hele sessie in twee regels. Schrijf hem over of markeer hem."*

4. **Bespreek de ARL-tabel** (3 min) — slide 6. Loop door:
    - *"Kale Shewhart — alleen één punt buiten ±3σ. Robuust. ARL = 371. Dit is de klassieke regel van Walter Shewhart, de grondlegger van SPC — 1924."*
    - *"WECO — Western Electric Company Rules. 1956. Vier extra regels: 2-van-3 buiten ±2σ, 4-van-5 buiten ±1σ, 8 opeenvolgende aan één kant, en trends. ARL gaat naar 91,75."*
    - **Bronverantwoording** (30 sec): *"Dat getal 91,75 — onthoud waar het vandaan komt. Het is berekend door Champ en Woodall in 1987, in het tijdschrift Technometrics. Niet door NIST, zoals vaak foutief wordt doorgegeven op internet. Als iemand je ernaar vraagt: noem Champ & Woodall."*
    - *"Volledige Nelson — 8 regels, Lloyd Nelson publiceerde die in 1984 in Journal of Quality Technology. Strenger dan WECO. ARL aanzienlijk lager — in de buurt van 40-60, afhankelijk van de exacte configuratie. Meer vals alarm dus."*

5. **Bespreek waarom 'meer' een val is** (2 min) — slide 9. Loop snel door de drie redenen:
    - **Alarm-fatigue** — *"Psychologisch effect. Als het alarm vaker vals is dan echt, gaan mensen het niet meer checken. De échte verstoring mist zijn kans om opgemerkt te worden."*
    - **Verloren productietijd** — *"Elk alarm = lijn stil of operator ernaartoe. Vals alarm is niet 'gratis ruis' — het is echt geld. Reken maar even: 2 valse alarmen per dag, 5 minuten per stuk, 20 werkdagen... dat is 3+ uur productie per maand."*
    - **Verloren vertrouwen in de kaart** — *"Als operators het systeem niet meer geloven, is de kaart als instrument kwijt. Dat is erger dan geen kaart — want een kapotte vertrouwensrelatie is moeilijk te repareren."*
    - Citeer: *"Minitab-stelregel: liever drie regels die je begrijpt, dan acht die je negeert."*

6. **Bespreek de gefaseerde AIMM-aanpak** (2 min) — slide 10. *"Dit is waarom wij de regels gefaseerd leren. Niet alles tegelijk aanzetten."*
    - *"Module 1 (Gebruik) — regels 1 en 2. Basisstabiliteit. Je leert de kaart lezen."*
    - *"Module 2 (Train) — deze module. Regels 3-6. Trend- en mixsignalen. Je leert wat ze toevoegen en wat ze kosten."*
    - *"Module 3 (Op Maat) — regels 7 en 8. Diagnostische verdieping. Alleen als je subgroepering begrijpt."*
    - *"Die volgorde is geen toeval. Het voorkomt dat je te snel te veel tegelijk aan zet — en dat de kaart onbetrouwbaar wordt voor jouw collega's."*

7. **Operator-implicatie** (1 min 30) — slide 11. Loop door de praktijktabel uit de handout: *"Meerdere alarmen per dag? Vraag teamleider welke regelset actief is. Engineering stelt voor om regels aan te zetten? Vraag om de afweging. Collega's negeren alarmen? Dat is alarm-fatigue — meld het als productierisico, niet als mentaliteitsprobleem. Je weet niet welke regelset actief is? Vraag het na — als niemand het weet, is dat ook informatie."*

8. **Aha-oogst** (1 min 30) — *"Wie wil één aha-moment delen uit de handout? Iets wat je gemarkeerd hebt en waarom."* Vang 1-2 vrijwilligers. Bevestig kort. Niet uitdiepen.

9. **Afsluiting + transferopdracht** (1 min) — slide 12. *"Deze week — één opdracht. Ga op je eigen lijn na welke signaalregels actief zijn. Vraag teamleider, kijk in het dashboard, of vraag engineering. Noteer: welke regels staan aan? Hoeveel alarm krijg je ongeveer per dag? Klopt dat met wat je nu weet over ARL? Neem je antwoorden mee naar de volgende sessie."*

**Materiaal:**
- [ ] wb-03-handout.md (1 per deelnemer)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] diagram-lo-spc-202.svg — op A3 én op slide 8
- [ ] Slides 5-12
- [ ] Flip-over met de drie koppen Kaal / WECO / Nelson

> **Tips voor de trainer:**
> - Houd het tempo. 13 minuten voor 7 onderdelen is krap. Niet vertragen door eigen anekdotes — bewaar die voor na afloop.
> - Het onthullen van het A3-diagram is een theatrale moment. Doe het met aandacht — even stil, laat het landen.
> - De bronverantwoording Champ & Woodall (1987) is een moment van inhoudelijke precisie. Een paar seconden langzaam spreken hier geeft gewicht. Operators waarderen dat er eerlijk over bronnen gepraat wordt.

> **Differentiatie:**
> - **MBO-3 standaard:** sla de exacte jaartallen en auteursnamen over in je mondelinge uitleg — ze staan in de handout voor wie later terugkijkt. Focus op de drie cijfers (371, 91,75, ~50) en de implicatie.
> - **MBO-4 / teamleider:** noem de jaartallen (WECO 1956, Nelson 1984, Champ & Woodall 1987). Benadruk dat het 'geen internetmening' is — het zijn peer-reviewed getallen. Dat geeft hen gereedschap om het in hun eigen organisatie te verdedigen.

> **Valkuil — trainer gaat te diep op Nelson-regels:**
> Verleidelijk om alle 8 Nelson-regels uit te leggen. Niet doen. De handout bevat een korte uitleg voor wie thuis terugleest. Vandaag volstaat: *"8 regels, strenger dan WECO, meer vals alarm. De regels zelf komen in latere sessies terug."*

> **Valkuil — trainer gaat over op CUSUM / EWMA:**
> Een voorbereide deelnemer vraagt naar 'moderne' kaarttypes (CUSUM, EWMA). *"Goede vraag — dat zijn andere typen regelkaarten die een heel ander gevoeligheids-profiel hebben. Die komen eventueel in module 3 of in een verdiepingstraject. Vandaag blijven we bij Shewhart-kaarten, want dat is wat 90% van de lijnen gebruikt."* Schrijf op parkeerflip.

> **Valkuil — deelnemer wil getallen in twijfel trekken:**
> Iemand zegt *"91,75 bij ons is nooit zo — wij hebben veel minder vals alarm"*. Bevestig de observatie. Zeg: *"Dat kan heel goed — die 91,75 is theoretisch, bij een proces dat in werkelijkheid stabiel is én bij exact deze WECO-configuratie. In de praktijk variëren processen. De bedoeling van het getal is de orde van grootte: veel meer vals alarm dan bij kale Shewhart, veel minder dan bij Nelson. Jouw lijn kan daar een eigen plek in hebben — dat ga je deze week opzoeken."*

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-oefening.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout.md | n + 2 | A4 dubbelzijdig (handout) |
| ☐ | diagram-lo-spc-202.svg | 1 | Print A3 in kleur, hang achter in zaal (drie staafjes: kaal / WECO / Nelson) |
| ☐ | Rekenmachines | 4-5 reserve | Plus verzoek aan deelnemers om telefoon te gebruiken |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Voor drie koppen Kaal / WECO / Nelson + plenaire rekensom-demonstratie |
| ☐ | Timer / mobiel met geluid | 1 | Voor 8-min rekenoefening + 8-min STARRT |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 8 (SVG-diagram) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel rekenoefening

| Scenario | ARL | 96 metingen / ARL | Per dag | Per week (5 werkdagen) | Oordeel |
|----------|-----|-------------------|---------|------------------------|---------|
| A — Kale Shewhart | 371 | 96 / 371 ≈ 0,26 | ~0,26 vals alarm | ~1,3 — dus **~1 per week** | Goed te doen |
| B — + WECO | 91,75 | 96 / 91,75 ≈ 1,05 | ~1 vals alarm | ~5 — dus **~1 per dag** | Voelbaar |
| C — + Volledige Nelson | ~50 (schatting) | 96 / 50 ≈ 1,9 | ~2 vals alarm | ~10 | Te veel (alarm-fatigue) |

**Slagingscriterium:** 2 of meer scenario's correct berekend = leerdoel behaald (ABCD-degree). Plus: kan in eigen woorden benoemen waarom alarm-fatigue een productierisico is.

**Bron-herinneringen:**
- **Shewhart (1924)** — grondlegger regelkaart, basisregel ±3σ
- **WECO (1956)** — Western Electric Company, Statistical Quality Control Handbook
- **Nelson (1984)** — Lloyd Nelson, *Journal of Quality Technology* 16(4): 237-239
- **Champ & Woodall (1987)** — *Technometrics* 29(4): 393-399, berekening ARL voor WECO-set
- **NIST/SEMATECH e-Handbook** — open-access referentie, sectie 6.3 (regelkaarten)
- **Minitab documentation** — Tests for Special Causes, Capability Analysis

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Plenair genoteerd: welke regelsets staan bij welke deelnemers op hun eigen lijn? (Input voor volgende sessie.)
- [ ] Flip-over met Kaal / WECO / Nelson gefotografeerd
- [ ] xAPI-statements verstuurd: `experienced` (rekenoefening), `attempted` (STARRT-reflectie), `completed` (handout doorgenomen)
- [ ] Notitie voor volgende workshop: bij welke deelnemers weet niemand welke regelset actief is? Dat is een signaal voor de gefaseerde-aanpak-discussie.

---

*AIMM Curriculum | SPC Module 2 (Train) | Gevoeligheid versus vals alarm — ARL en signaalregels*
*Bronnen: NIST/SEMATECH Engineering Statistics Handbook, sectie 6.3 | Champ & Woodall (1987) Technometrics 29(4) | Nelson (1984) JQT 16(4) | Western Electric Statistical Quality Control Handbook (1956) | Minitab Tests for Special Causes documentation*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
