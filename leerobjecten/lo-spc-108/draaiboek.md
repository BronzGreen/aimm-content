# Welke regelkaart hoort bij welke meting? — Draaiboek
*SPC Module 2 (Train) | Workshop-blok 40 minuten | 6-10 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan voor een gegeven meetsituatie het passende regelkaart-type benoemen (X̄-R, X̄-S, I-MR, p, np, c, u) door eerst te bepalen of het om continue metingen of tellingen gaat, en daarna of de subgroep of steekproef vast of wisselend is — in minimaal 4 van de 5 puzzelcasussen correct, met onderbouwing in één zin. |
| **Doelgroep** | Operators MBO-3 (primair), operators MBO-4 (secundair), 6-10 personen |
| **Voorkennis** | ko-spc-101 (variatie) en ko-spc-107 (specs vs control limits) doorlopen. Weet wat tolerantie en steekproef betekenen. Heeft regelkaarten op de werkvloer gezien. |
| **Stadium (H&B)** | Bewust onbekwaam — heeft kaarten op de werkvloer gezien, weet dat er verschillende types zijn, maar kan er nog geen eentje koppelen aan een meting. De puzzel activeert die ervaren onbekwaamheid ('ik koos X̄-R, maar waarom?') als leerbrandstof. |
| **Begeleidingsstijl** | Trainen — veel sturing én veel ondersteuning. Scaffolding via IK DOE → WIJ DOEN → JIJ DOET: trainer modelleert casus 0 op het bord, werkt dan samen met de groep door de vijf casussen, laat pas daarna de beslis-stroom zien en vraagt tot slot één eigen meting op tafel. Geen coachen-stijl — die past bij een hoger stadium. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok 2 binnen module 2 (Train) — direct na ko-spc-107 (specs vs control limits), vóór het blok over stabiliteitscheck (lo-spc-201) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Kaart-kiezen puzzel: 5 meetcasussen | 🟢 ervaren | 12 min |
| 00:12 - 00:22 | Buurman-check + plenaire bespreking + STARRT | 🟣 reflecteren | 10 min |
| 00:22 - 00:35 | Handout + beslis-stroom + twee vuistregels | 📘 theoretiseren | 13 min |
| 00:35 - 00:40 | Rondvraag: één meting van mijn eigen lijn | 🟢 experimenteren | 5 min |

**Totaal:** 40 minuten.
**Buffer:** elk blok bevat 1 minuut flexibele ruimte; gebruik die voor doorvragen of voor uitloop in blok 2 (plenaire bespreking bij casus 4 of 5).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen × (aantal deelnemers + 2 reserve): `wb-01-oefening.md`, `wb-02-reflectie.md`, `wb-03-handout.md`. Totaal ca. 36 vellen bij 10 deelnemers.
- [ ] Print `diagram-lo-spc-108.svg` op A3 in kleur (decision tree — 7 kaart-types) en houd afgedekt achter in de zaal. Ontvouwen in blok 3.
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer. Slide 7 (A3-diagram) is de centrale slide van blok 3.
- [ ] Lees het antwoordmodel kaart-keuze in dit draaiboek door en bedenk per casus één extra voorbeeld uit jouw eigen ervaring (spuitgieten, CNC, verpakking, voeding/chemie, folie).
- [ ] Check de doelgroeplijst: is er een MBO-4 operator of teamleider bij? Zo ja, stem het differentiatieblok af (zie onderaan).

### Het uur ervoor
- [ ] Leg per stoel: pen, `wb-01-oefening.md`. Stemkaartjes voor deze sessie niet nodig — deelnemers omcirkelen op het werkblad zelf.
- [ ] Houd `wb-02-reflectie.md` en `wb-03-handout.md` apart op de trainer-tafel — uitdelen pas op het moment in de sessie (blok 2 en blok 3).
- [ ] Hang de A3-versie van het diagram zichtbaar achter in de zaal (nog afdekken — pas onthullen in blok 3).
- [ ] Schrijf op de flip-over alvast de **twee hoofdvragen** groot:
  > **1. Continue meting of telling?**
  > **2. Vaste of wisselende steekproef / eenheid?**

  Dit wordt je vangrail bij blok 2.
- [ ] Schrijf op een tweede flip-over-vel de **7 namen** op een rij, zonder uitleg:
  `X̄-R    X̄-S    I-MR    p    np    c    u`
  Hang deze zichtbaar vooraan — de puzzel verwijst er in blok 1 naar.
- [ ] Open slide 1 op het scherm.
- [ ] Optioneel: leg een markeerstift per deelnemer klaar voor blok 3 (handout markeren).

---

## Blok-details

### 🟢 Blok 1: Kaart-kiezen puzzel — 5 meetcasussen
**00:00 - 00:12** | 12 min | Kolb-fase: ervaren

**Doel:** De deelnemer ervaart dat kiezen tussen zeven kaart-types eerst verwarrend voelt — en ontdekt daarna dat twee vragen (continue vs tellen, vaste vs wisselende n) het terugbrengen tot iets doenlijks. Twijfel is leerbrandstof voor blok 2 en 3.

**Werkvorm:** Individuele puzzel (JIJ DOET) — 5 meetcasussen uit de maakindustrie, deelnemer kiest per casus één kaart uit de 7 namen op het bord, ZONDER de beslis-stroom gezien te hebben.

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Op jullie werkvloer hangen regelkaarten — soms één, soms verschillende naast elkaar. Wie van jullie heeft wel eens gedacht: waarom is het uitgerekend díe kaart die hier draait?"* Wacht. Laat 1-2 mensen knikken. Geen lange verhalen.

2. **Normaliseer** (30 sec) — slide 2. *"Engineering kiest die kaart, niet jij. Maar als je snapt waarom, lees je de kaart scherper af. Zeven kaart-types voelt eerst als veel, maar het zijn in wezen maar twee vragen: meet je een getal of tel je iets? En is je steekproef elke keer even groot? Meer heb je eerst niet nodig."*

3. **Doe casus 0 voor — IK DOE** (1 min) — slide 3. Teken op de flip-over en vertel hardop:
    > *"Operator meet elke 2 uur de diameter van 5 onderdelen op de spuitgietlijn. Diameter is een getal in millimeter. Vraag 1: continue of tellen? Continue — diameter is een getal. Vraag 2: vaste of wisselende steekproef? Vaste — elke keer 5 onderdelen. Continue plus kleine subgroep 5 — dat is X̄-R."*

    Schrijf het pad op de flip-over:
    `Continue → subgroep mogelijk → klein (5) → X̄-R`

    *"Straks leer je waarom; eerst doen we het op gevoel."*

4. **Deel wb-01-oefening.md uit** (30 sec). Zeg: *"Vijf casussen uit de maakindustrie. Per casus kies je één kaart door die te omcirkelen. Schrijf er in één zin bij waarom je die kiest. Twijfel je? Zet een vraagteken — dat is prima. Het doel is niet alles goed te hebben, maar te voelen welke vraag je jezelf moet stellen."*

5. **Puzzel invullen** (8 min) — zet timer op 8 min. Loop rustig rond. Beantwoord praktische vragen (*"betekent wisselende steekproef ..."*) maar GEEN inhoudelijke (*"is mijn antwoord goed?"*) — verwijs door: *"Dat bespreken we zo samen — schrijf vooral op wat jij denkt, ook als je twijfelt."*

6. **Verzamel-moment** (1 min 30) — *"Pen neer. Bij welke casus had je de meeste twijfel? Steek je hand op bij casus 1... 2... 3... 4... 5."* Tel hardop, schrijf de scores op de flip-over. Dit is je input voor blok 2: welke casus bespreek je het langst.

**Materiaal:**
- [ ] `wb-01-oefening.md` (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Slide 1 (cover), slide 2 (twee hoofdvragen), slide 3 (worked example casus 0)
- [ ] Flip-over met de twee hoofdvragen + flip-over met de 7 kaart-namen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Loop rond maar buig je niet over schouders — dat verhoogt prestatiedruk en maakt twijfel onzichtbaar.
> - Als iemand al na 4 minuten klaar is: vraag *"Heb je bij casus 3 ook echt gecheckt of er een subgroep mogelijk is?"* Casus 3 (viscositeit per batch) is de toetssteen voor I-MR — wie snel klaar is, heeft die vaak te makkelijk op X̄-R gezet.
> - Bewaak de tijd. 8 minuten voor 5 casussen is krap — dat is bewust. Twijfel is leerstof.

> **🔄 Differentiatie:**
> - **Operator MBO-4 of teamleider erbij:** geef extra opdracht bij casus 5 (fouten per meter folie): *"Als de rollen wel elke keer even lang waren, welke kaart zou dan passen?"* Antwoord: c-kaart. Dit zet het verschil c versus u expliciet neer.
> - **Operator MBO-3 standaard:** alle vijf. Geen extra uitdaging nodig — de casussen zijn de uitdaging.

> **🔴 Valkuil — operator wil formules leren:**
> Bij vraag *"hoe bereken je de UCL op een X̄-R?"*: zeg *"De formules staan in je kwaliteitshandboek en de software rekent ze voor je. Wat de software niet doet, is kiezen welk kaart-type bij welke meting hoort — dat is wat we hier oefenen."* Niet opnieuw uitleggen.

> **🔴 Valkuil — deelnemer wil direct naar de beslis-stroom:**
> Bij *"staat er ergens een schema?"*: zeg *"Ja — en dat krijg je na deze puzzel. De puzzel eerst maakt het schema bruikbaar. Anders is het een papiertje dat je eenmalig leest en vergeet."*

---

### 🟣 Blok 2: Buurman-check + plenaire bespreking + STARRT
**00:12 - 00:22** | 10 min | Kolb-fase: reflecteren

**Doel:** Twijfel verwoorden, antwoorden vergelijken, het kernonderscheid (continue vs tellen, vaste vs wisselende n) uit eigen denken laten ontstaan — vóór de theorie. De twee hoofdvragen worden hier voor de deelnemer expliciet.

**Werkvorm:** Buurman-check (3 min) + plenaire bespreking per casus (6 min) + parallel invullen van `wb-02-reflectie.md` tijdens de bespreking. De STARRT-reflectie wordt thuis afgemaakt.

**Timing-note:** 10 min is krap voor 5 casussen plenair + buurman-check + starten met wb-02. Werkbare verdeling: 3 min buurman + 6 min plenair (1 min per casus met 1 min extra voor het lastigste geval) + 1 min uitloop. `wb-02` wordt **parallel** ingevuld tijdens de plenaire bespreking (één zin per blokje) en thuis afgemaakt vóór de volgende sessie. Niet de volledige STARRT tijdens de sessie — dat past niet.

**Instructie:**

1. **Buurman-check** (3 min) — slide 4. Zeg: *"Drie minuten met je buurman. Vergelijk je antwoorden. Leg per casus uit waarom je die kaart koos. Als jullie verschillen — zoek waar het verschil vandaan komt. Nog niet naar het goede antwoord zoeken — wel naar je eigen redenering."*

    Loop rond. Luister mee bij 2-3 duo's voor de plenaire bespreking — welke redenering komt terug, wie heeft iets scherps gezegd.

2. **Deel wb-02-reflectie.md uit** (30 sec). Zeg: *"Tijdens de plenaire bespreking vul je per blokje kort iets in — één zin per vraag. Niet een roman. De volledige STARRT maak je thuis af en neem je mee naar de volgende sessie."*

3. **Bespreek casus 1 — spuitgiet, onderdeelgewicht** (1 min). Vraag: *"Wie koos X̄-R? Wie iets anders?"* Laat stemmen. Bij overgrote meerderheid X̄-R: bevestig kort en schrijf op flip-over onder 'continue':
    `Casus 1 — continue, subgroep 5 → X̄-R ✅`
    *"Gewicht is een getal — continue. Steekproef van 5 — klein, dus R-kaart. Dit is de makkelijke als opening."*

4. **Bespreek casus 2 — foliedikte met lasersensor** (1 min). Vraag stemming. Hier splitst de groep vaak: X̄-R versus X̄-S. Bij X̄-R: *"Klopt dat de meting continue is — ja. Maar de subgroep is hier n = 30 per minuut. Dertig is niet klein meer. Wat gebeurt er met de range als je dertig metingen hebt?"* Wacht. Iemand: 'die wordt groot' of 'die wordt grof'. *"Precies — bij grotere subgroepen is de range te grof en gebruik je std. deviatie: X̄-S. Vuistregel uit NIST: zodra je subgroep groter wordt, wordt S efficiënter dan R."* Schrijf op flip-over:
    `Casus 2 — continue, subgroep 30 → X̄-S ✅`

5. **Bespreek casus 3 — viscositeit per batch** (1 min 30). Dit is de I-MR-casus. Vraag stemming. Deelnemers gokken soms X̄-R ('er staat toch één meting per batch'). *"Let op: hoeveel metingen doe je per moment?"* Iemand: 'één'. *"En kun je vlak erna nog een paar metingen doen?"* *'Nee, elke batch is uniek.'* *"Precies — geen subgroep mogelijk. Dat is precies de definitie van I-MR: individuele meting plus moving range. Vuistregel: I-MR pas als subgroeperen écht niet kan — zoals hier."* Schrijf op flip-over:
    `Casus 3 — continue, géén subgroep → I-MR ✅`

6. **Bespreek casus 4 — lekkende pakken, vaste steekproef 50** (1 min). Vraag stemming. Hier splitst de groep op p versus np. *"Meet je een getal of tel je iets?"* 'Tellen.' *"Is de steekproef elke keer even groot?"* 'Ja — 50.' *"Welke kaart past bij een telling met een vaste steekproef?"* 'np.' *"Waarom niet p?"* Iemand: 'omdat je het aantal opgeeft, niet het percentage'. *"Klopt — en bij een vaste steekproef is het aantal direct leesbaar. Bij wisselende steekproef moet je normaliseren naar percentage — dat is p."* Schrijf:
    `Casus 4 — tellen, vaste n → np ✅`

7. **Bespreek casus 5 — fouten per meter folie** (1 min 30). De lastigste van de vijf. Deelnemers gokken vaak c of p. *"Meet je een getal of tel je iets?"* 'Tellen — fouten.' *"Is de eenheid elke keer even groot?"* 'Nee — soms 80 meter, soms 120 meter.' *"Aantal defecten per **wisselende** eenheid — dat is u-kaart. Een c-kaart zou passen als je altijd exact dezelfde eenheid controleert — bijvoorbeeld altijd dezelfde plaat. Hier varieert de lengte, dus defectdichtheid per eenheid."* Schrijf:
    `Casus 5 — tellen, defecten per wisselende eenheid → u ✅`

8. **Sluit blok 2 af** (30 sec) — wijs naar de twee hoofdvragen op de flip-over. Zeg: *"Vijf casussen, vijf kaart-types, twee vragen. Dat is de logica die je vandaag meeneemt. In blok 3 gaan we dit verankeren met de handout en de beslis-stroom — als naslagwerk voor op de werkvloer."*

**Antwoordmodel — gebruik dit als basis voor de bespreking (exact gesynchroniseerd met wb-01-oefening.md):**

| Casus | Gegeven | Twee vragen | Kaart | Opmerking |
|-------|---------|-------------|-------|-----------|
| 1 | Elke 2 uur 5 onderdelen wegen op spuitgietlijn (gewicht in gram) | Continue + subgroep n=5 klein | **X̄-R** | Opener — makkelijkste casus |
| 2 | Lasersensor: 30 diktemetingen per minuut | Continue + subgroep n=30 groter | **X̄-S** | Toetssteen voor de R/S-vuistregel |
| 3 | Viscositeit per batch — één meting, elke batch uniek | Continue + géén subgroep mogelijk | **I-MR** | Vuistregel: I-MR alleen als laatste |
| 4 | Lekkende pakken, vaste steekproef 50 | Tellen + vaste n | **np** | Verschil p/np: aantal vs percentage |
| 5 | Fouten per rol folie — lengte varieert (80-120 m) | Tellen + defecten per wisselende eenheid | **u** | Verschil c/u: gelijke vs wisselende eenheid |

**Materiaal:**
- [ ] `wb-02-reflectie.md` (1 per deelnemer + 2 reserve)
- [ ] Flip-over met de twee hoofdvragen + 7 kaart-namen
- [ ] Markeerstift voor flip-over (antwoordpad per casus)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Stem zelf nooit mee. Je bent facilitator, geen deelnemer.
> - Tel innerlijk tot 5 na elke vraag. Vul stilte niet in — de groep moet zelf redeneren.
> - Bij casus 3 (I-MR): laat de redenering uit de groep komen. De vuistregel werkt alleen als ze zelf eerst voelen dat één meting per moment écht één meting is.
> - De flip-over met antwoord-paden (`Casus 1 — continue, subgroep 5 → X̄-R`) blijft hangen voor blok 3. Niet uitwissen.

> **🔴 Valkuil — p/np door elkaar:**
> Bij casus 4 zegt iemand 'p-kaart want percentage defecten'. Vraag: *"Wat staat er precies? 'Aantal lekkende pakken' of 'percentage lekkende pakken'?"* Laat de groep zien dat bij een vaste steekproef het aantal direct opgeschreven wordt — dat is np. Bij wisselende steekproef moet je normaliseren — dat is p.

> **🔴 Valkuil — c/u door elkaar:**
> Bij casus 5 zegt iemand 'c-kaart want aantal defecten'. Vraag: *"Is de eenheid elke keer even groot?"* Laat de groep ontdekken dat wisselende rollengte wisselende eenheid betekent — dus u (defectdichtheid per eenheid). c-kaart zou passen bij een vaste eenheid (altijd dezelfde plaat, altijd dezelfde tijdseenheid).

> **🔴 Valkuil — trainer gaat rekenen:**
> Verleidelijk om bij X̄-S de formule voor std. deviatie uit te leggen. Niet doen. De deelnemer hoeft niet te rekenen — alleen te kiezen. Eén zin: *"S staat voor standaarddeviatie — een nauwkeurigere spreidingsmaat dan de range, handig bij grotere subgroepen."* Meer niet.

> **🔄 Differentiatie:**
> - **Teamleider erbij:** voeg na casus 5 een korte vraag toe: *"Als je teamleider bent en je ziet een p-kaart terwijl jullie een vaste steekproef van 50 gebruiken — wat doe je?"* Antwoord: signaleren bij engineering dat np passender is. Parkeer verder — komt in module 3 terug.

---

### 📘 Blok 3: Handout + beslis-stroom + twee vuistregels
**00:22 - 00:35** | 13 min | Kolb-fase: theoretiseren

**Doel:** De twee hoofdvragen expliciet verankeren, de 7 kaart-types in een tabel vastleggen, de beslis-stroom als naslagwerk meegeven, en de twee vuistregels (R vs S, I-MR als laatste) expliciet markeren. Theorie als bevestiging van wat ze al hebben ervaren — niet als nieuw.

**Werkvorm:** Trainer-geleide handout-bespreking met live koppeling naar de puzzelcasussen + onthulling van het A3-diagram.

**Instructie:**

1. **Onthul het A3-diagram** (1 min) — verwijder de afdekking van `diagram-lo-spc-108.svg` achter in de zaal. Toon slide 7. Zeg: *"Hier is de beslis-stroom in beeld. Je ziet twee takken: links continue metingen, rechts tellingen van defecten. Elke tak splitst op basis van één vraag. Zes takjes, zeven bladeren — de zeven kaart-types die jullie net gekozen hebben."*

    Wijs kort naar elk blad: *"X̄-R, X̄-S, I-MR — aan de continue kant. p, np, c, u — aan de tellingen-kant. Allemaal op deze ene kaart."*

2. **Deel wb-03-handout.md uit** (30 sec). *"Pak een markeerstift. Markeer wat voor jou nieuw of verrassend is — dat zijn de stukken die je straks op de werkvloer nog eens naleest."*

3. **Loop door de handout — twee hoofdvragen** (1 min 30) — slide 8. *"Bovenaan staan de twee centrale vragen, en die wil ik dat jullie uit je hoofd kunnen opdreunen: Eén — meet je een getal (continue) of tel je defecten? Twee — is je steekproef elke keer even groot of varieert die? Dát is de sleutel tot de hele kaart."*

4. **Tabel doorlopen** (3 min) — slide 9. Loop de tabel met 7 rijen snel door. Per rij één zin:
    - *"X̄-R — continue, kleine subgroep, gemiddelde en range. Casus 1."*
    - *"X̄-S — continue, grotere subgroep, gemiddelde en std. deviatie. Casus 2."*
    - *"I-MR — één meting per moment of batch. Casus 3."*
    - *"p — tellen, percentage bij **wisselende** steekproef."*
    - *"np — tellen, aantal bij **vaste** steekproef. Casus 4."*
    - *"c — tellen, defecten per **gelijke** eenheid."*
    - *"u — tellen, defecten per **wisselende** eenheid. Casus 5."*

    Koppel bewust terug naar de puzzel — zo zijn de casussen ankers in het geheugen.

5. **Beslis-stroom als stroomschema** (2 min) — slide 10. Wijs naar de A3-poster. *"Dit is hetzelfde plaatje als in je handout, alleen uitvergroot. Je begint bovenaan bij 'Wat meet je?' en je volgt de takken. Elke vraag onderweg is één van de twee hoofdvragen — niets anders. Deze poster hangt straks waarschijnlijk op menig kantine-muur."*

6. **Twee vuistregels** (2 min) — slide 11. Loop expliciet langs beide:

    **Vuistregel 1 — R versus S.** *"Bij kleine subgroepen (2 tot 8) werkt R prima. Bij grotere subgroepen wordt de range te grof — dan gebruik je S. Dat was het verschil tussen casus 1 (n=5, R) en casus 2 (n=30, S). NIST/SEMATECH noemt dat expliciet: zodra je subgroep groter wordt, wordt S efficiënter dan R."*

    **Vuistregel 2 — I-MR als laatste keuze.** *"I-MR alleen als subgroeperen écht niet kan. Als je zelfs maar n=2 kunt nemen — twee metingen kort na elkaar — is X̄-R of X̄-S meestal informatiever. I-MR past vooral bij batch-, tank- of lotmetingen. Dat was casus 3."*

7. **Drie veelgemaakte fouten** (2 min) — slide 12. Dit staat in de handout — loop ze snel door voor wie ze thuis gaat herlezen:
    - *"Eén — I-MR gebruiken terwijl subgroeperen kan. Je verliest informatie."*
    - *"Twee — p en np door elkaar halen. p is percentage (wisselende n), np is aantal (vaste n)."*
    - *"Drie — c en u door elkaar halen. c bij gelijke eenheid, u bij wisselende eenheid."*

8. **Aha-moment vragen** (1 min) — *"Wie wil in één zin delen wat voor jou vandaag het aha-moment was?"* Vang 1-2 reacties. Bevestig kort. Geen lange uitwisseling — we gaan naar blok 4.

**Materiaal:**
- [ ] `wb-03-handout.md` (1 per deelnemer + 2 reserve, geprint A4 dubbelzijdig)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] `diagram-lo-spc-108.svg` — op A3 in de zaal én op slide 7
- [ ] Slides 7-12

> **💡 Tips voor de trainer:**
> - Houd het tempo. 13 min is krap voor tabel + beslis-stroom + twee vuistregels + drie fouten. Niet vertragen met eigen anekdotes — die passen beter in blok 4.
> - De A3-poster is je krachtigste visuele middel. Laat hem hangen gedurende de rest van de module — nieuwe sessies verwijzen ernaar terug.
> - Bij elke rij van de tabel: verwijs expliciet naar de puzzelcasus. Zo koppelen deelnemers 'X̄-S' aan 'de foliedikte van casus 2' — dat is veel sterker dan een losse definitie.

> **🔴 Valkuil — trainer gaat formules behandelen:**
> Bij *"hoe bereken je nu precies die range of die std. deviatie?"*: zeg *"De formules staan in je kwaliteitshandboek, en de SPC-software rekent ze voor je. Wat de software niet doet: kiezen welk kaart-type bij welke meting past — dat is wat je hier geleerd hebt."* Park verder. Formules horen bij module 3 (Op Maat) als de deelnemer zelf kaarten wil opzetten.

> **🔴 Valkuil — trainer gaat Western Electric of Nelson-rules uitleggen:**
> *"Hoe lees je op een X̄-R-kaart een 'special cause' af?"* — park het. *"Goede vraag — patronen herkennen op regelkaarten komt in lo-spc-201 (volgende blok in deze module) uitgebreid aan bod. Vandaag hebben we de kaart-keuze."* Schrijf op parkeerflip.

> **🔴 Valkuil — trainer gaat ISO 7870 in detail citeren:**
> ISO 7870-1 en 7870-2 zijn de normatieve documenten achter deze kaarten, maar de details (UCL-formules, steekproefregels) zijn HBO-terrein. Eén zin volstaat: *"De zeven kaart-types zijn genormeerd in ISO 7870-1 en 7870-2 — dat is de internationale standaard waar jullie kwaliteitshandboek waarschijnlijk aan refereert."* Meer niet.

> **🔄 Differentiatie:**
> - **Operator MBO-4 of teamleider:** noem ook de term **ARL (Average Run Length)** als concept dat verschilt per kaart-type — niet uitleggen, alleen noemen. MBO-3 negeert, MBO-4 onthoudt.
> - **Operator MBO-3 basis:** sla de term ARL over. Blijf bij de twee hoofdvragen en de beslis-stroom.

---

### 🟢 Blok 4: Rondvraag — één meting van mijn eigen lijn
**00:35 - 00:40** | 5 min | Kolb-fase: experimenteren

**Doel:** De deelnemer formuleert een concrete transferopdracht. Autonomie (zelf kiezen welke meting) staat centraal. De stap naar de eigen werkvloer is daarmee gezet.

**Werkvorm:** Korte plenaire rondvraag + transferopdracht. Geen werkblad — dit blok is oraal.

**Instructie:**

1. **Introduceer het blok** (30 sec) — slide 13. Zeg: *"Vijf puzzelcasussen, vijf kaarten — nu jullie eigen lijn. Denk 30 seconden na: één meting op jouw werkplek — wat is het, hoe meet je het, en welk kaart-type hoort daarbij volgens de beslis-stroom?"* Laat even stilte.

2. **Rondvraag** (3 min) — *"We gaan rond. Je noemt: de meting, de steekproef of eenheid, en het kaart-type dat erbij hoort."*

    Loop de groep langs. Per persoon max 30 sec. Bevestig of stel één corrigerende vraag:
    - Correct: *"Goed — en in de beslis-stroom ga je dan..."* of gewoon *"Klopt — volgende."*
    - Onzeker of verkeerd: *"Hoe groot is je steekproef? Vast of wisselend?"* Laat de deelnemer zelf corrigeren.

    Parkeer lastige gevallen (bijv. 'ik weet het eigenlijk niet'): *"Prima — die neem je mee als transferopdracht. Ga deze week kijken en kom volgende keer terug."*

3. **Transferopdracht** (1 min 30) — slide 14. *"Deze week ga je op je werkplek kijken: welke kaart(en) hangen of draaien er? Neem drie dingen mee voor de volgende sessie:"*
    - Welk type kaart is het? (kijk naar de as-titels, subgroep-info, naam)
    - Welke meting staat erop?
    - Klopt de keuze met de beslis-stroom — of twijfel je?

    *"En de bonus: vraag deze week één keer aan je teamleider of engineer: 'Waarom hebben we op deze lijn een X̄-R / p-kaart / I-MR gekozen?' Je krijgt vaak een verhelderend antwoord en je laat tegelijk zien dat je meedenkt."*

4. **Afsluiting** (30 sec) — slide 15. *"Twee vragen. Zeven kaarten. Eén beslis-stroom. Volgende sessie bespreken we wat jullie hebben gezien op je eigen lijn — neem je notities mee. Bedankt voor jullie oplettendheid."*

**Materiaal:**
- [ ] Slide 13 (rondvraag), slide 14 (transferopdracht), slide 15 (afsluiting)
- [ ] `wb-03-handout.md` als referentie voor wie nog iets wil checken
- [ ] A3-diagram blijft hangen

> **💡 Tips voor de trainer:**
> - Verleidelijk om 'mee te denken' bij iemand die twijfelt over de eigen lijn. Niet doen. *"Dat ga je deze week uitzoeken — zo leer je het te gebruiken"* is het juiste antwoord. De autonomie is de werkende component voor transfer.
> - Als iemand drie metingen wil noemen: *"Eén — de meest interessante. Die levert het meest op als je deze week gaat kijken."*
> - Eindig op tijd. Blok 4 overslaan is GEEN optie — dat is de brug naar de werkvloer.

> **🔄 Differentiatie:**
> - **Operator MBO-3:** één meting + één kaart-type is genoeg. Geen tijdpad, geen extra actie.
> - **Operator MBO-4 of teamleider:** vraag om naast de meting ook te noemen of er nu de **juiste** kaart draait. *"Zou jij er een andere kiezen? Waarom?"* Dat is teamleider-denken.

> **🔴 Valkuil — uitloop blok 3:**
> Als blok 3 is uitgelopen: nooit blok 4 overslaan. Kort het af: schrap de rondvraag tot 3 deelnemers en breng de transferopdracht naar 30 seconden. Eindig stipt — transfer is wat de workshop verbindt met de werkvloer.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | `wb-01-oefening.md` | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | `wb-02-reflectie.md` | n + 2 | A4 enkelzijdig |
| ☐ | `wb-03-handout.md` | n + 2 | A4 dubbelzijdig (handout — naslagwerk) |
| ☐ | `diagram-lo-spc-108.svg` | 1 | Print A3 in kleur, hang achter in de zaal (decision tree 7 kaart-types) |
| ☐ | Markeerstiften | n | Voor handout-blok 3 |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Voor twee hoofdvragen + 7 kaart-namen + antwoordpaden per casus |
| ☐ | Timer / mobiel met geluid | 1 | Voor 8-min puzzel |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 7 (SVG) is cruciaal |
| ☐ | `presentatie.slidev.md` geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel kaart-keuze

| Casus | Gegeven (uit wb-01) | Continue of telling? | Subgroep / eenheid | Kaart |
|-------|---------------------|----------------------|---------------------|-------|
| 1 (spuitgietlijn) | Elke 2 uur 5 onderdelen wegen; gewicht in gram | Continue | Vaste subgroep n=5 (klein) | **X̄-R** |
| 2 (lasersensor folie) | Elke seconde 1 meting, n=30 per minuut; dikte in mm | Continue | Vaste subgroep n=30 (groter) | **X̄-S** |
| 3 (viscositeit batch) | Eén meting per batch, geen vlak-na-elkaar-metingen mogelijk; viscositeit in mPa·s | Continue | Geen subgroep mogelijk | **I-MR** |
| 4 (lekkende pakken) | Elk uur steekproef van **precies 50** pakken; telling defecten | Telling | Vaste steekproef n=50 | **np** |
| 5 (fouten per rol folie) | Rol varieert in lengte (80-120 m); telling defecten per rol | Telling | **Wisselende** eenheid | **u** |

**Slagingscriterium:** 4 of meer van de 5 correct = leerdoel behaald (ABCD-degree). Casus 2 (X̄-S versus X̄-R) en casus 5 (u versus c) zijn de toetsstenen voor de twee vuistregels (R/S, gelijke/wisselende eenheid). Casus 3 (I-MR) toetst de tweede vuistregel.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Twijfel-statistiek genoteerd (welke casussen waren het lastigst voor deze groep)
- [ ] Flip-over met antwoordpaden gefotografeerd
- [ ] Notitie voor volgende workshop: welke kaart-types hebben deelnemers op hun eigen lijn gezien?
- [ ] xAPI-statements verstuurd: `experienced` (kaart-kiezen puzzel), `completed` (reflectie + handout-markering), `attempted` (transferopdracht)
- [ ] Bij teamleider-deelnemers: korte handover naar de volgende sessie (lo-spc-201 — Nelson-rules op regelkaarten)

---

*AIMM Curriculum | SPC Module 2 (Train) | Welke regelkaart hoort bij welke meting?*
*Bronnen: NIST/SEMATECH Engineering Statistics Handbook, sectie 6.3.2 (Control Charts) | ISO 7870-1:2019 en ISO 7870-2:2023 | ASQ Statistics Division, Control Chart Selection Guide | Minitab Support, Choose a Control Chart.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
