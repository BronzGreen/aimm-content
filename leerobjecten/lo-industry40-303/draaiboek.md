# Drempels instellen en alarm-rationalisatie — Draaiboek
*Industry 4.0 Module 2 (Train) | Sessie 45 minuten | 8-14 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Operator kan op een concrete alarm-stroom analyseren welke meldingen operator-grens (drempel voor handeling) zijn en welke alarm-grens (drempel voor stilstand), kan een eerste drempel beargumenteerd voorstellen uit historische data, en kan een onhandige alarm-stroom van 240 meldingen per dag teruglezen volgens drie EEMUA-principes (max-rate, relevantie, actiegerichtheid). |
| **Doelgroep** | Operators MBO-4 (primair), MBO-3 (secundair), 8-14 personen |
| **Voorkennis** | lo-industry40-302 doorlopen — data-pipeline vier knooppunten; lo-industry40-026 — mens beslist, AI adviseert |
| **Stadium (H&B)** | Bewust bekwaam — herkent alarm-vermoeidheid op eigen lijn, kent de regels nog niet |
| **Begeleidingsstijl** | Instrueren (S1) — regel-gebaseerd materiaal (EEMUA 191), expliciet voordoen |
| **Bloom** | Analyseren — principes herkennen en relateren op concrete meldingen |
| **Kirkpatrick** | Gedrag — transferopdracht op eigen werkvloer (drie stappen deze week) |
| **Ruimte** | U-opstelling of cabaretopstelling, beamer + scherm, whiteboard of flap-over voor grafiek + drie principes, voldoende tafelruimte voor A4-werkbladen |
| **Plek in module** | Tweede LO in module 2 (Train), direct na lo-industry40-302 (data-pipeline) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Een dag uit een spuitgieterij — 240 alarmen | 🟢 ervaren | 12 min |
| 00:12 - 00:22 | Twee soorten drempels en de tuning trade-off | 📘 theoretiseren | 10 min |
| 00:22 - 00:35 | Drempel-tuning op historische data — twee sensoren | 🟡 experimenteren | 13 min |
| 00:35 - 00:45 | 240 naar 24 — drie EEMUA-principes op fase-1-lijst | 🟣 reflecteren | 10 min |

**Totaal:** 45 minuten — geen aparte pauze (één-blok sessie binnen module 2).
**Buffer:** 1 minuut per fase flexibel; gebruik in fase 3 voor extra duo-rondgang als histogrammen lastig leesbaar zijn.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — 1 per deelnemer + 2 reserve. wb-03 dubbelzijdig (twee histogrammen op één blad).
- [ ] Open `lo-industry40-303-presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Lees de antwoordmodellen in `lo-industry40-303-trainer.yaml` (ankerinformatie) — niet om voor te zeggen, wel om te herkennen wat een goede onderbouwing is.
- [ ] Check rekenmachine-toegang — meeste operators hebben telefoon, anders 4-5 calculators meenemen.

### Het uur ervoor
- [ ] Leg per stoel: pen en markeerstift. Werkbladen op trainer-tafel — uitdelen pas op het moment van de fase.
- [ ] Teken op whiteboard alvast een leeg assenstelsel: horizontaal 'tijd', verticaal 'meetwaarde'. NIET de drempels invullen — die teken je tijdens fase 2 live.
- [ ] Reserveer rechterhelft van whiteboard voor de drie EEMUA-principes (vul je in fase 4 in).
- [ ] Open slide 1.

---

## Blok-details

### 🟢 Blok 1: Een dag uit een spuitgieterij — 240 alarmen
**00:00 - 00:12** | 12 min | Kolb-fase: ervaren

**Doel:** Deelnemer ervaart op een concrete alarm-lijst dat sommige meldingen vragen om handeling, andere om stilstand en weer andere om niets — zonder dat de termen 'operator-grens' en 'alarm-grens' al gevallen zijn. De spreiding in keuzes is het materiaal voor fase 2.

**Werkvorm:** Individueel werk op werkblad (7 min) → plenaire vergelijking (4 min) → overgang (1 min).

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 45 minuten kijken we naar drempels en alarmen. Tegen het eind heb je drie principes om elk alarm op jouw lijn te wegen. We beginnen met een echte werkvloer: spuitgietmachine, één dag, 240 meldingen."*

2. **Deel werkblad wb-01 uit** (1 min) — wb-01-dagelijkse-alarm-lijst. Toon slide 2. Zeg: *"Boven aan staat: 24-uurs overzicht, 8 sensoren, 240 meldingen. In de tabel staan 10 voorbeelden uit die dag. Per melding: type sensor, gemeten waarde, tijd, en wat de operator deed."*

3. **Instructie taak** (1 min) — *"Per melding kruis je één van drie opties aan: (a) operator moet iets doen, (b) machine moet stoppen, of (c) had nooit als alarm hoeven binnenkomen. Bij twee meldingen schrijf je in één zin waarom. Eerste indruk telt — twijfel mag."* Geen termen geven.

4. **Individueel werk** (7 min) — zet timer op 7 min. Loop rond. Stel verdiepende vragen aan vastlopers:
    - *"Lees de actie-kolom — wat deed de operator?"*
    - *"Als de operator iets noteerde maar de machine draaide door — wat zegt dat?"*
    - *"Een melding die genegeerd werd — wat denk je dat de operator daarvan vond?"*
    - **Geef geen termen.** Bevestig elke poging.

5. **Plenaire vergelijking** (2 min) — *"Pen neer. Wie heeft bij de melding 'temperatuur 65 graden, 07:12, ingevuld in logboek' optie (a) gekruist? Wie (b)? Wie (c)?"* Tel snel op. Vraag 1-2 deelnemers waarom. Schrijf hun zin op het bord zonder oordeel.

6. **Doe hetzelfde voor één lastige melding** (1 min) — bijvoorbeeld 'materiaal-laag 02:34 tijdens shift-wissel, genegeerd'. Zelfde rondje. Laat zien dat de groep verdeeld is.

7. **Bevestig spreiding** (1 min) — *"Verschillende antwoorden, oké. Die spreiding is precies wat we vandaag leren. Er zijn twee soorten drempels en je kunt niet zomaar zien welke wat is. Dat gaan we nu uit elkaar trekken."*

**Materiaal:**
- [ ] wb-01-dagelijkse-alarm-lijst (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Houd je in. Het is verleidelijk om al uit te leggen dat 65 graden 'operator-grens' is. Niet doen — anders wordt fase 2 een dubbeling.
> - Stilte tijdens individueel lezen is goed. Laat het.
> - Als een deelnemer zegt 'wat is het juiste antwoord?' — antwoord: *"Jouw onderbouwing is wat telt, niet het ene antwoord."*

> **🔄 Differentiatie:**
> - **MBO-3 basis:** geef een voorbeeld op het bord: 'temperatuur 80 graden — automatische stilstand — dit is een melding die zegt machine stop'. Eén voorbeeld, geen term.
> - **MBO-4 sneller:** vraag bij plenair: *"Welke melding had volgens jou nooit binnenmoeten komen, en waarom?"* Hint naar fase 4.

> **🔴 Valkuil — termen te vroeg:** als je hoort 'die 65 is dus een operator-grens?' — antwoord: *"De naam komt in het volgende blok. Eerst je eigen denken."*

> **Overgang:** *"Jullie zien al: sommige meldingen vragen iets, andere stoppen de machine, sommige doen niets. Tijd om die drie groepen netjes uit elkaar te halen — met namen."*

---

### 📘 Blok 2: Twee soorten drempels en de tuning trade-off
**00:12 - 00:22** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert de twee drempel-soorten benoemen en herkent ze in zijn eigen fase-1-keuzes. Trade-off tussen te laag en te hoog wordt visueel verankerd.

**Werkvorm:** Trainer-geleide uitleg in twee blokken met live tekening op whiteboard, deelnemer markeert op fase-1-werkblad.

**Instructie:**

1. **Deel handout wb-02 uit** (1 min) — wb-02-twee-drempels-handout. Toon slide 3.

2. **Blok 1 — Twee soorten drempels** (3 min) — toon slide 4. Schrijf op het bord:
    - **Operator-grens** = drempel voor handeling. Operator MOET iets doen. Machine blijft draaien.
    - **Alarm-grens** = drempel voor stilstand. Machine stopt of leidinggevende wordt gebeld.

    Geef voorbeeld: *"Temperatuur 65 graden — controleer koeling, geen stilstand: operator-grens. Temperatuur 80 graden — automatische stilstand en onderhoud bellen: alarm-grens."* Wijs terug naar fase 1: *"65 was operator-grens. 80 was alarm-grens. Iedereen die anders had gekruist — geen fout, dat verschil is wat we nu leren."*

3. **Vraag eigen werkvloer-voorbeeld** (1 min) — *"Wat is bij jullie op de werkvloer een typische operator-grens? Iets waar je bij ingrijpt maar de machine niet stopt."* Vang 1-2 antwoorden. Bevestig.

4. **Blok 2 — Drempel-tuning trade-off** (3 min) — toon slide 5. Teken nu op het assenstelsel:
    - Wolkje 'normaal gedrag' in het midden.
    - Lijn 'operator-grens' net boven de wolk — label 'handeling'.
    - Lijn 'alarm-grens' boven de operator-grens — label 'stilstand'.

    Vertel: *"Te laag (drempel onder normale werking) — constante meldingen, alarm-vermoeidheid (overdaad aan meldingen). Operator raakt afgestompt. Te hoog (drempel boven probleem-gedrag) — issue pas zichtbaar als hij al kostbaar is. Voorspellend voordeel weg."*

5. **Markeren fase-1-werkblad** (1 min) — *"Pak je werkblad van fase 1. Markeer met je markeerstift: bij welke meldingen had je operator-grens, bij welke alarm-grens? Vergelijk met je eerste keuze."*

6. **Overgang naar fase 3** (1 min) — *"Als je niet weet welke waarde een goede drempel is — waar zou je beginnen met zoeken?"* Vang antwoord. Brug: *"Bij historische data. Dat is wat we nu gaan doen."* Bron-vermelding: *"De principes komen uit EEMUA 191 — de industrie-standaard voor alarm-systemen. Niet onthouden, wel weten dat het bestaat."*

**Materiaal:**
- [ ] wb-02-twee-drempels-handout (1 per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 3-5
- [ ] Whiteboard met assenstelsel + drempel-grafiek (live tekenen)

> **💡 Tips voor de trainer:**
> - Teken de grafiek tijdens je verhaal — niet vooraf. Live tekenen werkt beter dan kant-en-klare slide.
> - Gebruik bij eerste introductie altijd én jargon én vertaling: *"operator-grens (drempel voor handeling)"*. Na drie keer mag je alleen 'operator-grens'.
> - Het 'wolkje normaal' is bewust onscherp — drempel-design is geen exacte wiskunde.

> **🔄 Differentiatie:**
> - **MBO-3 basis:** schrijf de twee termen ook in B1-vertaling op het bord: 'handeling-grens' / 'stop-grens'. Naast de officiële termen.
> - **MBO-4 sneller:** vraag bij wolkje: *"Wat als de wolk verandert — nieuwe charge materiaal, andere matrijs?"* Hint naar fase 3 scenario's.

> **🔴 Valkuil — te lang theoretiseren:** als je voelt dat je over 5 minuten heen gaat — sla het tweede voorbeeld over. Trade-off is belangrijker dan tweede operator-grens-voorbeeld.

> **Overgang:** *"We weten nu wat we zoeken: een operator-grens en een alarm-grens per sensor. Hoe vind je daar in de data een goede waarde voor? Twee sensoren — een temperatuur, een druk — op historische data. Aan de slag."*

---

### 🟡 Blok 3: Drempel-tuning op historische data — twee sensoren
**00:22 - 00:35** | 13 min | Kolb-fase: experimenteren

**Doel:** Duo's stellen voor twee sensoren een operator-grens en een alarm-grens voor, met onderbouwing uit historische data. Daarna toetsen ze hun voorstel op drie scenario's (warme zomer, nieuwe leverancier, nieuwe operator).

**Werkvorm:** Duo's op werkblad (9 min: 6 voor drempel-voorstel + 3 voor scenario-toets) → plenaire bespreking (4 min).

**Instructie:**

1. **Deel werkblad wb-03 uit + vorm duo's** (1 min) — wb-03-drempel-tuning-twee-sensoren. Toon slide 6. *"Zoek een buurman. Twee histogrammen op het werkblad: temperatuur op een spuitgietmal, druk op de spuit-cilinder. Vier kerngetallen per histogram: gemiddelde, hoogste, laagste, en hoeveel procent boven een 'verdachte zone'."*

2. **Instructie drempel-voorstel** (1 min) — *"Per sensor stellen jullie TWEE drempels voor: operator-grens (handeling) en alarm-grens (stilstand). Bij elk een zin onderbouwing uit de data. Eén iemand leest de getallen voor, één schrijft het voorstel."* Geef expliciet de regel: *"Eerste drempel rond de bovengrens van normaal. Daarna bijstellen na 2 tot 4 weken op basis van operator-feedback."*

3. **Duo's stellen drempels voor** (6 min) — zet timer op 6 min. Loop rond. Stel doorvragen:
    - *"Kijk naar het histogram — waar zit het meeste van de tijd? Wat ligt daarboven?"*
    - *"Welke waarde komt zelden voor — kan dat je alarm-grens worden?"*
    - *"Schrijf de onderbouwing — niet het exacte getal."*
    - Bij rekenen: *"Het exacte getal maakt minder uit. Onderbouwing is belangrijker."*

4. **Scenario-toets** (3 min) — toon slide 7. Lees de drie scenario's voor:
    - (a) De zomer wordt heet — werkruimte 5 graden warmer.
    - (b) Nieuwe materiaalleverancier — andere stroom-eigenschappen.
    - (c) Een nieuwe operator zit aan deze machine.

    *"Past jullie voorstel nog? Schrijf bij elk scenario in één zin: ja-blijft / aanpassen-naar / niet-aanpassen-want."*

5. **Plenaire bespreking** (2 min) — toon slide 8. *"Eén duo per sensor: wat is jullie operator-grens en alarm-grens, en wat is de zin onderbouwing? Niet het hele scenario-rijtje — alleen de onderbouwing."* Hak na 1 minuut af. Markeer op het bord: 'goede aanpak: data → eerste drempel → bijstellen → operator-feedback'.

**Materiaal:**
- [ ] wb-03-drempel-tuning-twee-sensoren (1 per deelnemer, dubbelzijdig)
- [ ] Pen per deelnemer
- [ ] Rekenmachine (telefoon mag)
- [ ] Slides 6-8
- [ ] Whiteboard met aanpak-pijl (data → drempel → bijstellen → feedback)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Hou de tijd strak. 6 minuten voor drempel-voorstel is genoeg — perfectie is niet het doel.
> - Bij duo's die niet op gang komen: stel voor temperatuur direct de regel — eerste drempel net boven 80 procent-zone. Geef de regel, geen getal.
> - Bevestig elke onderbouwing uit historische data. Corrigeer geen getal — wel een onderbouwing zonder data ('ik denk dat dit goed is').

> **🔄 Differentiatie:**
> - **MBO-3 basis:** verlaag eis van twee zinnen onderbouwing naar één. Help duo's expliciet door de eerste sensor heen, laat de tweede zelf.
> - **MBO-4 sneller:** geef een vierde scenario: *"De drempel is uit een naburige lijn overgenomen — past die hier nog?"*
> - **Gemengde groep:** vorm duo's gemengd. MBO-3 leest, MBO-4 schrijft onderbouwing.

> **🔴 Valkuil — rekenfanaat:** bij duo dat 5 minuten doorrekent op één getal: onderbreek — *"Schrijf je voorstel op. Onderbouwing is wat telt."*

> **🔴 Valkuil — drempel als wet:** als iemand schrijft 'de drempel is 65 graden, klaar' — vraag: *"En als de zomer warmer wordt — past hij dan nog? En na 4 weken?"* Drempel leeft.

> **Overgang:** *"Twee drempels per sensor — operator-grens en alarm-grens. Werkt voor twee sensoren. Maar wat als je er acht hebt en de teller staat op 240 alarmen per dag? Dan ben je er nog niet. Dat is rationalisatie — de hele alarm-stroom logisch maken."*

---

### 🟣 Blok 4: 240 naar 24 — drie EEMUA-principes op fase-1-lijst
**00:35 - 00:45** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer past drie EEMUA-principes toe op zijn eigen fase-1-werkblad (10 meldingen). Hij ziet hoe een autoleverancier van 240 naar 24 alarmen ging — geen wonder, gewoon systematisch toepassen.

**Werkvorm:** Trainer-presentatie casus (3 min) → individueel werk op fase-1-werkblad (5 min) → plenair (2 min).

**Instructie:**

1. **Presenteer de casus** (3 min) — toon slide 9. Schrijf op de rechterhelft van het whiteboard de drie principes (één regel per principe):
    - **Principe 1 — max-rate** = max circa 10 alarmen per uur per operator
    - **Principe 2 — relevantie** = relevant voor DEZE operator op DIT moment
    - **Principe 3 — actiegerichtheid** = concrete actie verbonden

    Vertel de casus: *"Autoleverancier, spuitgietmachine, 8 sensoren. Eerste maand: 240 alarmen per dag. 80 procent niet-actionabel. Na alarm-rationalisatie (rationalisatie = logisch maken): 24 alarmen per dag, allemaal actiegericht. Operator-tevredenheid steeg. Kritische alarmen 12 minuten sneller opgepakt."*

    Wat veranderde:
    - Opstartmeldingen verwijderd — verwacht gedrag, geen actie (principe 3 hersteld).
    - Materiaal-detectie naar shift-leiders — verkeerde ontvanger voor operator (principe 2 hersteld).
    - Temperatuur-overschrijdingen kregen specifieker actie-advies: *'temperatuur 75 graden — controleer koelsysteem klep 3'* in plaats van alleen *'temperatuur 75 graden'* (principe 3 versterkt).

    *"Geen nieuwe sensoren. Geen ander systeem. Gewoon principes toepassen."*

2. **Deel werkblad wb-04 uit** (1 min) — wb-04-drie-principes-toepassen. Toon slide 10. *"Pak je werkblad uit fase 1 ernaast. Voor elke melding: schendt hij principe 1 (te veel), principe 2 (verkeerde ontvanger) of principe 3 (geen actie)? Mag combineren, maar kies welk principe het sterkst speelt."*

3. **Individueel werk** (5 min) — zet timer op 5 min. Loop rond. Stel doorvragen:
    - *"Wat deed de operator met deze melding? Niets? Dan welk principe?"*
    - *"Komt deze melding 30 keer per dag? Dan welk principe?"*
    - *"Hoort hij eigenlijk bij onderhoud? Dan welk principe?"*
    - Bij 'alles principe 3': *"Wijs me een melding die niet principe 3 is — kijk naar relevantie en max-rate."*

4. **Plenair + transferopdracht** (1 min) — toon slide 11. *"Eén deelnemer: welke melding, welk principe geschonden, in één zin?"* Vang 1-2 antwoorden. Maak de transferopdracht expliciet: drie stappen deze week op de eigen lijn. (1) Tel je alarmen in één dienst. (2) Kies één dat je negeert — bepaal welk principe. (3) Stel één concrete vraag aan teamleider of IT: *"Waarom staat deze drempel zo — is hij ooit aangepast aan deze lijn?"* of *"Wie beheert de alarm-instellingen?"*

5. **Afsluiting** (1 min) — *"Drempels en alarmen zijn niet vast — ze leven met de productie mee. Wie ze niet bijhoudt, krijgt na een jaar dezelfde 240. Wie ze maandelijks bespreekt, houdt het op 24. Tot volgende week."*

**Materiaal:**
- [ ] wb-04-drie-principes-toepassen (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 9-11
- [ ] Whiteboard met drie principes (zichtbaar tot eind sessie)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Schrijf de drie principes zelf op het bord — niet alleen op slide. De tactiele act helpt opname.
> - De casus is 3 minuten max. Niet meer. Het is gereedschap voor de oefening, geen verhaal.
> - Bij plenair: laat 1-2 antwoorden, niet meer. Tijd is krap.

> **🔄 Differentiatie:**
> - **MBO-3 basis:** doe de eerste 3 meldingen plenair. Daarna individueel verder.
> - **MBO-4 sneller:** vraag een tweede ronde — welke meldingen schenden meer dan één principe?

> **🔴 Valkuil — casus als magie:** bij 'wow, 240 naar 24!' — antwoord: *"Geen magie. Drie principes naast de lijst. Daarom doe je het nu zelf met tien."*

> **🔴 Valkuil — sceptische operator:** als iemand zegt 'op onze lijn besluit IT alles' — *"Klopt. De transferopdracht is geen drempel veranderen, maar de juiste vraag stellen. Wie weet welke alarmen onzin zijn? Jij."*

> **🔴 Valkuil — alles principe 3:** *"Komt deze melding te vaak? Principe 1. Hoort hij bij een ander? Principe 2. Geen actie? Principe 3. Kies de sterkste."*

> **Geen overgang — afsluiting:** *"Drie principes. Drie stappen deze week. Volgende sessie deel je in één minuut: hoeveel alarmen, welk principe, welk antwoord van IT of teamleider. Tot dan."*

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-dagelijkse-alarm-lijst | n + 2 | A4 — 10 meldingen met drie-keuze-veld |
| ☐ | wb-02-twee-drempels-handout | n + 2 | A4 — twee blokken plus grafiek-schets |
| ☐ | wb-03-drempel-tuning-twee-sensoren | n + 2 | A4 dubbelzijdig — twee histogrammen + drie scenario's |
| ☐ | wb-04-drie-principes-toepassen | n + 2 | A4 — drie principes + terugkoppeling 10 meldingen |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften (geel of oranje) | n | Voor fase 2 — markeren fase-1-werkblad |
| ☐ | Rekenmachine | 4-5 stuks | Of telefoon van deelnemer — voor histogram fase 3 |
| ☐ | Whiteboard of flap-over | 1 | Voor drempel-grafiek + drie principes |
| ☐ | Whiteboard-stiften zwart/rood/groen | 1 set | Voor live tekenen fase 2 + drie principes fase 4 |
| ☐ | Timer / mobiel met geluid | 1 | Voor 7-min, 6-min, 5-min momenten |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | lo-industry40-303-presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 10 meldingen indelen — geen termen | Spreiding zichtbaar; eigen denken op tafel |
| 2 theoretiseren | Twee drempel-soorten + grafiek + trade-off | Operator-grens en alarm-grens herkend in fase-1-keuzes |
| 3 experimenteren | Duo's drempel-voorstel op twee histogrammen + drie scenario's | Onderbouwing uit data + besef dat drempel leeft |
| 4 reflecteren | Drie EEMUA-principes op fase-1-lijst + casus 240→24 | Principe-schending kunnen toewijzen; transferopdracht in handen |

**Slagingscriterium:** minimaal 6 van 10 meldingen correct ingedeeld, twee drempel-voorstellen met onderbouwing uit data, minimaal twee principe-schendingen geïdentificeerd op fase-1-lijst.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (voor learning analytics)
- [ ] Whiteboard gefotografeerd (drempel-grafiek + drie principes — voor follow-up)
- [ ] Genoteerd: welke melding gaf de meeste spreiding in fase 1? Welk principe werd het vaakst geschonden in fase 4?
- [ ] Notitie voor volgende sessie: welke transferopdracht-vragen heb ik gehoord ('Wie beheert onze drempels?' / 'Hoe vaak worden ze aangepast?') — daar haken we volgende keer op aan
- [ ] xAPI-statements verstuurd: `experienced` (wb-01), `analyzed` (wb-04), `completed` (vier werkbladen), `performed` (transferopdracht)

---

*AIMM Curriculum | Industry 4.0 Module 2 (Train) | Drempels en alarm-rationalisatie*
*Bronnen: EEMUA Publication 191 — Alarm Systems: A Guide to Design, Management and Procurement. | Bakopoulos et al. (2024). Digital-Twin-Enabled Framework, Ch. 7.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
