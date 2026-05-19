# Van papieren kaart naar dashboard — Draaiboek
*SPC Module 1 (Gebruik) | Workshop-blok 40 minuten | 6-12 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | De MBO-3 operator kan na dit blok, gegeven een papieren X-bar-R-kaart en een MES/SCADA-dashboard-screenshot, minimaal 4 concrete overeenkomsten/verschillen benoemen tussen klassieke en Industry 4.0 SPC, én 1 voorbeeld van de eigen werkvloer geven. Onderbouwing: het Shewhart-principe blijft, meetfrequentie/drager/detectie/reactietijd/datavolume verschuiven. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | ko-spc-101 (basis variatiebegrip: common vs special cause) |
| **Stadium (H&B)** | Bewust onbekwaam — operator werkt dagelijks met schermen, maar heeft zelden expliciet stilgestaan bij wat het dashboard doet t.o.v. een regelkaart |
| **Begeleidingsstijl** | Trainen — veel sturing op de vergelijking, veel ondersteuning bij de eigen dashboard-inventarisatie |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, twee wandposities voor het diagram (A3 + A3), pen per deelnemer |
| **Plek in module** | Workshop-blok binnen module 1 (Gebruik) — direct na het basisblok variatie (lo-spc-101), vóór het herken-blok common/special cause (lo-spc-104) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Vergelijk papieren kaart en dashboard | 🟢 ervaren | 15 min |
| 00:15 - 00:30 | STARRT-reflectie: mijn dashboards en mijn reactietijd | 🟣 reflecteren | 15 min |
| 00:30 - 00:40 | Handout klassiek vs Industry 4.0 SPC | 📘 theoretiseren | 10 min |

**Totaal:** 40 minuten — geen aparte pauze binnen dit blok (pauze staat direct ná dit blok gepland).
**Buffer:** elk blok bevat 1-2 minuten flexibele ruimte; gebruik die voor doorvragen in blok 2 of voor uitloop in blok 3.

---

## Voorbereiding

### De avond ervoor
- [ ] Print 3 werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 45 vellen bij 12 deelnemers.
- [ ] Print het diagram `diagram-lo-spc-103.svg` op A3 (in kleur indien mogelijk) — hangt tijdens blok 3 zichtbaar.
- [ ] Print *Voorbeeld A* (papieren X-bar-R-kaart, fictief, 20 meetpunten ingevuld) op A4 — 1 per deelnemer.
- [ ] Print *Voorbeeld B* (screenshot MES/SCADA-dashboard, fictief, generieke stijl) op A4 — 1 per deelnemer.
- [ ] Open `presentatie.slidev.md` op je laptop en test de beamer-aansluiting.
- [ ] Lees het antwoordmodel vergelijkingstabel (onder dit draaiboek) door en bedenk per rij één extra voorbeeld uit jouw eigen ervaring (spuitgieten, CNC, verpakking).
- [ ] Markeer in je hoofd: welke rij in de tabel wil je als anker gebruiken voor het Shewhart-principe? (Advies: *detectie* — daar zie je de verschuiving van "operator scant" naar "regel alarmeert" het duidelijkst.)

### Het uur ervoor
- [ ] Leg per stoel: pen, wb-01, Voorbeeld A en Voorbeeld B naast elkaar.
- [ ] Houd wb-02 en wb-03 apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Hang de A3-versie van `diagram-lo-spc-103.svg` afgedekt achter in de zaal — pas onthullen in blok 3.
- [ ] Schrijf op de flip-over alvast twee kolommen: **VROEGER (papier)** | **NU (dashboard)** — leeg, vullen we tijdens blok 3 samen in.
- [ ] Schrijf op een apart hoekje: **"Shewhart-vraag: is dit signaal of ruis?"** — dat blijft staan tijdens het hele blok.
- [ ] Open slide 1 op het scherm.

---

## Blok-details

### 🟢 Blok 1: Vergelijk papieren kaart en dashboard
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** De deelnemer ziet twee beelden naast elkaar en ontdekt zélf wat gelijk is en wat anders is. Geen theorie vooraf — eerst kijken, dan benoemen. Dit activeert herkenning en maakt zichtbaar wat de operator al weet en wat nog niet.

**Werkvorm:** Individueel werkblad. Operator vergelijkt Voorbeeld A (papieren X-bar-R-kaart) met Voorbeeld B (MES/SCADA-dashboard-screenshot) en vult de vergelijkingstabel + enkele open vragen in.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"In het vorige blok hebben we geleerd dat elk proces varieert — common cause en special cause. Vandaag kijken we: hoe zie je die variatie eigenlijk? Vroeger op een papieren kaart. Nu op een dashboard. In de komende 40 minuten ontdek je wat er echt verandert — en wat onder de motorkap exact hetzelfde blijft."*

2. **Introductie vergelijking** (1 min) — toon slide 2. *"Hier naast je stoel liggen twee beelden. Voorbeeld A is een papieren regelkaart van een spuitgietlijn uit 2010 — 20 meetpunten, met de hand ingevuld. Voorbeeld B is een screenshot van een MES-dashboard van een vergelijkbare lijn uit 2026. Allebei fictief, ter illustratie."*

3. **Deel wb-01-vergelijk-papieren-en-digitaal uit** (1 min, indien nog niet op stoel). Zeg: *"Pak het werkblad. 2 minuten rustig kijken naar beide beelden — geen pen op papier. Daarna vul je de vergelijkingstabel in. Je hebt in totaal 12 minuten."*

4. **Eerst 2 minuten rustig kijken** (2 min) — zet timer. Niet rondlopen — laat ze letterlijk even niks doen dan kijken. Dit is een doeners-groep, dus de neiging is direct schrijven. Hou de stilte.

5. **Individueel invullen** (10 min) — zet timer op 10 min. Loop nu rustig rond. Beantwoord praktische vragen (*"wat is UCL?"* — "dat is de bovengrens, upper control limit, staat in de handout zo") maar géén beoordelende vragen (*"is dit goed?"* — verwijs door: *"Schrijf op wat jij herkent. Bij twijfel een vraagteken. We kijken het straks samen."*).

6. **Mini-check** (1 min) — *"Pen neer. Onthoud: welk ding viel jou het meeste op dat je op het dashboard zag maar niet op papier? Dat ene ding — dat ga je straks in de reflectie gebruiken."*

**Materiaal:**
- [ ] wb-01-vergelijk-papieren-en-digitaal.md (1 per deelnemer + 2 reserve)
- [ ] Voorbeeld A — papieren X-bar-R-kaart (A4, ingevuld, fictief) × deelnemers + 2
- [ ] Voorbeeld B — screenshot MES/SCADA-dashboard (A4, fictief) × deelnemers + 2
- [ ] Pen per deelnemer
- [ ] Slide 1 (cover) en slide 2 (vergelijking intro)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Niet vooraf de vijf verschuivingen noemen (meten, drager, detectie, reactietijd, datavolume). Die ontdekken ze zelf in de tabel — dat is precies de leerwinst.
> - Loop tijdens het schrijven niet over schouders mee. Dat verhoogt prestatiedruk bij doeners-MBO-3 en zet hen op "juist antwoord zoeken" in plaats van eerlijk benoemen.
> - Bij iemand die vastloopt bij de checkboxen: wijs naar Voorbeeld A en stel één vraag — *"Zie je een bovenlijn op dit papier?"* — en laat hem zelf aankruisen.
> - De kolom "Alarmmelding" en "Kleurcodering" scoren bijna altijd: papier nee, dashboard ja. Dat is goud voor blok 3.

> **🔄 Differentiatie:**
> - **MBO-3 basis:** leesniveau van de checklist is B1. Indien iemand aangeeft het lastig te vinden: begin samen met de eerste drie rijen hardop.
> - **MBO-4 sneller:** vraag aan die deelnemer aanvullend: *"Wat mis je in beide beelden dat je zou verwachten in een volwassen SPC-systeem?"* (Antwoorden kunnen zijn: cp/cpk-waarde, capability-index, een runregel-overzicht.) Noteer voor blok 3.

> **🔴 Valkuil — deelnemer denkt "dashboard is gewoon beter":**
> Iemand zegt bij het neerleggen van de pen: *"Dat dashboard is gewoon veel slimmer hè."* Niet corrigeren, wel relativeren: *"Sneller, ja. Meer data, zeker. Maar of het slimmer is — dat is precies de vraag waar we straks op terugkomen. Een sensor die elke seconde meet stelt nog steeds dezelfde Shewhart-vraag: is dit signaal of ruis?"* Verwijs naar de flip-over-hoek met die zin.

---

### 🟣 Blok 2: STARRT-reflectie — mijn dashboards en mijn reactietijd
**00:15 - 00:30** | 15 min | Kolb-fase: reflecteren

**Doel:** De abstracte vergelijking (papier vs dashboard) wordt persoonlijk. De operator brengt zijn eigen schermen in beeld, schat zijn eigen reactietijd in, en ontdekt wat hij eigenlijk weet (of niet weet) over wat er onder het scherm draait. Zo wordt de leervraag scherp: *"ben ik baas over het scherm of andersom?"*

**Werkvorm:** STARRT-werkblad individueel (10 min) → korte plenaire deel-ronde op één STARRT-vraag (5 min).

**Instructie:**

1. **Deel wb-02-reflectie uit** (30 sec). Zeg: *"Dit werkblad volgt de STARRT-structuur — Situatie, Taak, Actie, Resultaat, Reflectie, Transfer. Zes vragen. Je vult het in over jezelf en jouw werkvloer — niet meer over papier en Voorbeeld B. Welke schermen gebruik jij, wat gebeurde er bij het laatste alarm, hoe snel reageerde je, en — eerlijk — weet je wát er onder die alarmregel zit?"*

2. **Individueel STARRT-invullen** (10 min) — zet timer op 10 min. Loop rond. Help bij blokkades:
    - Bij vraag 1 (welke schermen?): *"Is er een scherm bij je machine? En eentje in de supervisor-kamer? En je mobiel met een trendapp?"* Drie schermen is standaard.
    - Bij vraag 4 (reactietijd): benadruk dat dit geen prestatiemeting is. *"Het gaat erom dat je het beseft — snel reageren hoeft niet per se goed te zijn."*
    - Bij vraag 5 (wat weet jij onder het scherm?): eerlijkheid stimuleren. *"'Ik weet alleen dat het rood wordt' is een prima antwoord — dan weet je tenminste waar je staat."*

3. **Plenaire deel-ronde op één vraag** (4 min) — *"Pen neer. We gaan rondbij vraag 5: wat weet jij onder het scherm? Drie keuzes — ik weet de regel, ik weet dat er een grens is maar niet welke, of ik weet alleen dat het rood wordt. Eerlijke antwoorden graag."* Laat 4-6 deelnemers snel hun keuze noemen (30 sec per persoon). Turf op de flip-over in drie kolommen.

4. **Korte plenaire duiding** (30 sec) — laat de cijfers zien. Zeg: *"Kijk eens. Het is heel normaal dat je niet weet wat er onder zit — dat heeft niemand jou geleerd. Maar zolang je het niet weet, ben je operator van het scherm in plaats van operator van het proces. Dat gaan we straks rechtzetten."*

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Flip-over met drie kolommen: *Ik weet de regel* | *Ik weet dat er een grens is* | *Ik weet alleen dat het rood wordt*
- [ ] Pen per deelnemer
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Stem zelf niet mee op vraag 5 — je bent facilitator, geen deelnemer.
> - Tel innerlijk tot 7 nadat je de ronde-vraag stelt. Vul stilte niet in. Doeners-MBO-3 hebben die tijd nodig om eerlijk te kiezen.
> - De derde kolom ("ik weet alleen dat het rood wordt") heeft vaak de meeste turfjes. Dat is *prima* — geen schaamte. Benoem het als vertrekpunt, niet als falen.
> - Bij deelnemer die alles zegt te weten: vraag *"En welke regel zit er onder het alarm van dat scherm bij de weegschaal?"* Vriendelijk doorvragen — vaak blijkt het een half antwoord.

> **🔴 Valkuil — deelnemer schaamt zich voor "ik weet het niet":**
> Iemand kiest de derde kolom en kijkt naar beneden. Zeg expliciet: *"Dat is de eerlijkste start. Iedereen die hier ooit is begonnen, begon daar. Het verschil tussen jou en iemand die het wél weet, is dat jij het nu gaat vragen — jouw transfervraag uit vraag 6."*

> **🔴 Valkuil — "bij ons hangen geen schermen":**
> Iemand zegt dat zijn werkplek nog volledig papier is. Mooi — gebruik die persoon: *"Dan word jij deze week onze verkenner. Welke schermen hangen er wél op andere lijnen in jouw fabriek? Ga er langs en beschrijf wat je ziet."* Zet die observatie in de transferopdracht.

> **🔄 Differentiatie:**
> - **Gemengde groep:** vraag bij de plenaire ronde eerst de MBO-3'ers, daarna de MBO-4'ers. Anders sturen MBO-4-stemmen het gesprek.

---

### 📘 Blok 3: Handout klassiek vs Industry 4.0 SPC
**00:30 - 00:40** | 10 min | Kolb-fase: theoretiseren

**Doel:** De waarnemingen uit blok 1 en de zelfkennis uit blok 2 krijgen een kader. Theorie als ordening — niet als nieuwe regelset. De operator ziet: *wat ik net noemde, heet officieel "detectie"; wat mij opviel aan snelheid, heet "reactietijd"*.

**Werkvorm:** Trainer-geleide handout-bespreking met live verwijzing naar de vergelijkingstabel uit blok 1 en de turfjes-flip-over uit blok 2. Deelnemers markeren wat nieuw is.

**Instructie:**

1. **Onthul het diagram** (30 sec) — verwijder de afdekking van de A3-versie van `diagram-lo-spc-103.svg` achter in de zaal. Toon slide 7. Zeg: *"Hier staan ze naast elkaar — links de papieren kaart, rechts het dashboard. Wat in het midden zit — het gele strookje — is het Shewhart-principe. Dat is de brug: onder beide gereedschappen dezelfde vraag."*

2. **Deel wb-03-handout-klassiek-vs-industry40 uit** (30 sec). Zeg: *"Pak je markeerstift. We gaan door de vijf verschuivingen. Markeer wat je in blok 1 ook al had opgeschreven, en zet een sterretje bij wat je nieuw vindt."*

3. **Vijf verschuivingen doorlopen** (6 min) — slides 8-10. Per rij van de tabel: definitie + één terugverwijzing naar wat er al was opgeschreven/gezegd.

    **Meten — handmatig/periodiek → continu sensor** (1 min):
    *"Voorbeeld A had één punt per uur — 20 punten totaal over de shift. Voorbeeld B had honderden punten per minuut. Dat is *meetfrequentie*."* Wijs naar flip-over VROEGER/NU en schrijf: VROEGER — "uur-steekproef" | NU — "elke seconde een punt".

    **Drager — papier → cloud/MES/SCADA** (1 min):
    *"Waar staan de getallen? Vroeger in een ordner. Nu op een scherm dat iedereen overal kan zien — ook de teamleider op een andere lijn, ook de kwaliteitsmanager op kantoor."* (Bron: recente literatuur Industry 4.0 SPC — zie ko-spc-103.yaml `metadata.source_ref`.)

    **Detectie — operator scant → regel alarmeert** (1 min):
    *"Wie ziet een trend? Vroeger jij, met je ogen over 20 punten. Nu een regel die automatisch telt. Soms aangevuld met een AI-model dat patronen herkent die je met je ogen zou missen."* Terugkoppeling blok 2: *"Die derde kolom van turfjes — 'ik weet alleen dat het rood wordt' — gaat over deze rij. De regel onder jouw alarm is wat jij hoort te kennen."*

    **Reactietijd — uren/dagen → seconden/minuten** (1 min):
    *"Vroeger zag je een afwijking pas na een paar uur. Nu piept het dashboard binnen 30 seconden. Belangrijk: sneller piepen betekent niet dat jij sneller moet handelen. Eerst de Shewhart-vraag — is dit signaal of ruis — dan pas iets doen."* Verwijs naar slide 11.

    **Datavolume — tientallen → miljoenen punten per dag** (1 min):
    *"Voorbeeld A had 20 punten op een shift. Een inline-sensor maakt 3,6 miljoen punten per dag. Dat is niet alleen méér — dat is fundamenteel een andere soort data. Zonder dashboard kun je dat niet lezen."*

    **Tempo-waarschuwing** (1 min): check of je nog op schema zit. Indien < 2 min over: sla rij "Datavolume" kort samen (*"je ziet in de tabel zelf het getal"*) en ga door.

4. **Shewhart-principe expliciet** (1 min) — toon slide 11. Zeg: *"Wat verandert niet? Dit."* Wijs naar het gele strookje in het diagram en naar de zin op de flip-over. *"Shewhart bedacht in 1931: is dit signaal, of is dit ruis? Die vraag zit onder elke regelkaart én onder elk dashboard. Bron: Shewhart 1931, vandaag nog de basis van ISO 7870-2."*

5. **Eén-zins-afsluiter** (1 min 30) — *"Iedereen — één zin: wat verandert volgens jou het meest, én wat blijft exact hetzelfde?"* Laat 3-4 deelnemers kort delen. Slagingscriterium: minstens één noemt "detectie" of "reactietijd" als verandering, en minstens één noemt "Shewhart" of "signaal/ruis" als gelijkblijvend.

6. **Transferopdracht + afsluiting** (30 sec) — toon slide 12. *"Deze week één keer bewust langs de schermen op je werkvloer. Per scherm: welke meting zie ik? Welke grens of alarm zit eronder? Als je het niet weet, schrijf op wat je ziet en wat je je afvraagt. In module 2 ga je hier zelf een regel op instellen — begin dus met jouw lijstje. Neem je werkblad mee."*

**Materiaal:**
- [ ] wb-03-handout-klassiek-vs-industry40.md (1 per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] diagram-lo-spc-103.svg — op A3 zichtbaar én op slide 7
- [ ] Slides 7-12
- [ ] Flip-over met VROEGER/NU-kolommen (wordt tijdens dit blok ingevuld)

> **💡 Tips voor de trainer:**
> - Houd het tempo hoog. 10 min voor 5 verschuivingen + Shewhart + afsluiter is krap — niet afdwalen met eigen anekdotes. Eén korte terugkoppeling naar wat de groep noemde, geen tweede.
> - De visuele brug — *tabel links/rechts, Shewhart in het midden* — is wat operators onthouden. Refereer er twee, drie keer aan.
> - De eenvoudige zin "Shewhart-vraag: is dit signaal of ruis?" op de flip-over is meer waard dan een uitleg over common/special cause. Dat komt bij lo-spc-104.
> - Bij de MES/SCADA-uitleg: gebruik één zin. Niet in de verleiding komen om cloud-architectuur uit te leggen — daar hebben we data literacy-blokken voor.

> **🔄 Differentiatie:**
> - **MBO-3 basis:** laat de rijen "Meten" en "Reactietijd" het zwaarst wegen — die zijn het meest concreet. "Datavolume" mag op één zin ("veel meer data") zonder de miljoenen-berekening.
> - **MBO-4 sneller:** voeg in bij "Detectie" de vraag: *"En wat is het verschil tussen een alarmregel en een AI-model? Een regel is een formule die jij kunt lezen; een model is getraind op data en niet altijd uitlegbaar."* Verwijs naar ko-spc-601 (AI in SPC) voor wie verder wil.

> **🔴 Valkuil — Shewhart-principe klinkt als "oud en achterhaald":**
> Iemand zegt: *"Shewhart — dat is toch van 100 jaar geleden?"* Antwoord: *"Precies — en daar is-ie nog steeds. Bron: ISO 7870-2, internationale norm van 2013, bevestigt letterlijk wat hij in 1931 opschreef. Het gereedschap verandert, de vraag niet."*

> **🔴 Valkuil — deelnemer concludeert "dus alarmen moet ik altijd vertrouwen":**
> Dat is een tampering-reflex avant la lettre. Zeg: *"Andersom — een alarm van een dashboard dat te streng staat piept ook zonder dat er iets aan de hand is. Dat heet 'valse alarmen'. Daarom blijft de Shewhart-vraag: is dit *echt* signaal of is dit ruis — óók bij een dashboard-alarm. In module 2 ga je zelf aan de knoppen van zo'n regel."*

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-vergelijk-papieren-en-digitaal.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-klassiek-vs-industry40.md | n + 2 | A4 dubbelzijdig (handout — komt mee) |
| ☐ | Voorbeeld A — papieren X-bar-R-kaart (fictief) | n + 2 | A4, kleur indien mogelijk |
| ☐ | Voorbeeld B — screenshot MES/SCADA-dashboard (fictief) | n + 2 | A4, kleur indien mogelijk |
| ☐ | diagram-lo-spc-103.svg | 1 | A3 in kleur, hang afgedekt achter in zaal tot blok 3 |
| ☐ | Markeerstiften | n | Voor handout-blok (geel of roze) |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Twee vellen: VROEGER/NU-kolommen (blok 3) + turfjes vraag 5 (blok 2) |
| ☐ | Timer / mobiel met geluid | 1 | Voor 2-min, 10-min, 6-min blokken |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 7 (SVG) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel vergelijkingstabel

*Gebruik bij blok 1 als ruggengraat — niet uitdelen aan deelnemers.*

| Aspect uit wb-01 | Papieren kaart | Dashboard | Opmerking voor trainer |
|------------------|----------------|-----------|------------------------|
| Meetwaardes (getallen) | Ja (20 punten) | Ja (honderden-miljoenen) | Aantal is het grote verschil |
| Lijn in de tijd (grafiek) | Ja | Ja | Beide hebben een tijdgrafiek — overeenkomst |
| UCL / LCL | Ja | Ja (meestal) | Overeenkomst — Shewhart-principe |
| Gemiddelde-lijn | Ja | Ja | Overeenkomst |
| Datum / tijd | Ja | Ja (automatisch) | Overeenkomst — maar op dashboard rijker |
| Operator-naam / paraaf | Ja (handgeschreven) | Soms (login-stempel) | Verschuiving: automatische audit trail |
| Alarmmelding | Nee | Ja | Alleen dashboard — dit is *detectie*-verschuiving |
| Kleurcodering rood/geel/groen | Nee (of potlood) | Ja | Alleen dashboard |
| Meerdere grafieken tegelijk | Nee | Ja | Alleen dashboard |
| Aanbeveling ("check X") | Nee | Soms (AI) | Alleen dashboard — raakt ko-spc-601 |

**Slagingscriterium leerdoel:** Deelnemer benoemt minimaal 4 concrete overeenkomsten/verschillen én 1 voorbeeld van eigen werkvloer (in wb-02). Bij plenaire afsluiter (blok 3, stap 5): minstens één deelnemer noemt een verandering (detectie/reactietijd/datavolume), minstens één noemt het Shewhart-principe als gelijkblijvend.

**De vijf rij-verschuivingen uit de handout:** meten, drager, detectie, reactietijd, datavolume. Bron: recente literatuur Industry 4.0 SPC (zie ko-spc-103.yaml `metadata.source_ref`). Klassiek principe: Shewhart (1931) *Economic Control of Quality of Manufactured Product*, herbevestigd in ISO 7870-2.

---

## Checklist na de sessie

- [ ] Werkbladen 1 en 2 ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Werkblad 3 (handout) — operators nemen mee naar werkvloer (niet innemen!)
- [ ] Turfjes-flip-over van blok 2 vraag 5 gefotografeerd (hoeveel mensen wisten de regel?)
- [ ] VROEGER/NU-flip-over van blok 3 gefotografeerd als bewijs van gezamenlijke ordening
- [ ] Notitie voor volgende sessie: welke verschuiving herkenden deelnemers het snelst? Welk voorbeeld van eigen werkvloer kwam vaak terug?
- [ ] xAPI-statements verstuurd: `experienced` (vergelijking), `completed` (STARRT + handout), `attempted` (transferopdracht)
- [ ] Check 1 week later met de groep: hoeveel dashboards hebben jullie geïnventariseerd? Welke vraag heb je gesteld?

---

*AIMM Curriculum | SPC Module 1 (Gebruik) | Van papieren kaart naar dashboard*
*Bronnen: Shewhart, W.A. (1931) *Economic Control of Quality of Manufactured Product*; ISO 7870-2 voor Shewhart-regelkaarten; recente literatuur Industry 4.0 SPC (zie ko-spc-103.yaml `metadata.source_ref`). Verwijzing kennisbank: ko-spc-101 (basis variatie), ko-spc-104 (common/special cause), ko-spc-601 (AI in SPC).*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
