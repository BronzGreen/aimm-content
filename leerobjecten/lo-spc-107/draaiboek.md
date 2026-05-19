# Control limits versus specificatiegrenzen — Draaiboek
*SPC Module 1 (Gebruik) | Workshop-blok 40 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan in eigen woorden het verschil benoemen tussen control limits (UCL/LCL, proces-grens) en specificatiegrenzen (product-grens), kan op drie voorbeeld-regelkaarten aanwijzen welke fout is opgezet, en kent globaal de 3σ-formule van Shewhart. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | ko-spc-101 (basis variatie). Deelnemers hebben regelkaarten gezien op de werkvloer maar weten meestal niet of de lijnen control limits of specs zijn. |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat er grenzen op de kaart staan, weet niet zeker wat ze betekenen of waar ze vandaan komen. |
| **Begeleidingsstijl** | Trainen — veel sturing op het onderscheid, veel ondersteuning bij de eerlijke "ik-weet-het-niet"-reflectie. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen. |
| **Plek in module** | Workshop-blok binnen module 1 (Gebruik) — bouwt voort op ko-spc-101, leidt naar lo-spc-108 (procesbekwaamheid) en lo-spc-203 (signaal-respons). |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Spot-the-fout: drie regelkaarten | ervaren | 15 min |
| 00:15 - 00:27 | STARRT-reflectie: jouw eigen kaart | reflecteren | 12 min |
| 00:27 - 00:40 | Handout: verschil + 3σ + NIST-waarschuwing | theoretiseren | 13 min |

**Totaal:** 40 minuten — geen aparte pauze (workshop-blok binnen een grotere module).
**Buffer:** elk blok heeft 1-2 minuten flexibele ruimte; gebruik die vooral in blok 3 voor doorvragen.

---

## Voorbereiding

### De avond ervoor
- [ ] Print de drie werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 45 vellen bij 12 deelnemers.
- [ ] Print `diagram-lo-spc-107.svg` op A3 (in kleur indien mogelijk). Dit diagram toont een regelkaart met UCL/LCL én USL/LSL duidelijk onderscheiden, plus de 4-scenario-matrix (stabiel/onstabiel × bekwaam/onbekwaam).
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer.
- [ ] Lees de antwoorden bij de drie voorbeeld-kaarten in dit draaiboek (blok 1 — bespreking) door. Zorg dat je de 3σ-berekening van kaart A en kaart C uit je hoofd kunt uitleggen zonder rekenmachine.
- [ ] Check of je weet wie op jouw locatie de SPC-coördinator is — handig om te noemen in blok 2 als deelnemers vragen wie de kaarten op hun lijn heeft gemaakt.

### Het uur ervoor
- [ ] Leg per stoel: pen, wb-01-spot-the-fout.
- [ ] Houd wb-02-reflectie en wb-03-handout apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Hang de A3-versie van het diagram zichtbaar achter in de zaal (nog afdekken met een vel papier — pas onthullen in blok 3).
- [ ] Schrijf op de flip-over alvast twee kolommen: **PROCES (UCL/LCL)** | **PRODUCT (USL/LSL)** — leeg, vullen we in blok 3 samen in.
- [ ] Schrijf op een tweede flip-over: **"Binnen specs ≠ onder controle"** — anker voor blok 3.
- [ ] Open slide 1 op het scherm.

---

## Blok-details

### Blok 1: Spot-the-fout — welke kaart is verkeerd opgezet?
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** De deelnemer ervaart dat het verschil tussen control limits en specs op het eerste oog klein lijkt, maar bij nadere inspectie groot is. Zonder theorie vooraf — eerst kijken, dan begrijpen. Dit activeert de leerbehoefte voor de vergelijkingstabel in blok 3.

**Werkvorm:** Trainer doet één kaart hardop voor (IK DOE), deelnemers beoordelen de andere twee zelf (JIJ DOET), korte buurman-check.

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Op veel werkvloeren hangen regelkaarten aan de wand. Er staan lijnen op — een bovengrens, een ondergrens. Maar wie heeft die lijnen getekend, en waarop zijn ze gebaseerd? Dat is de vraag van deze 40 minuten."*

2. **Context klantopdracht** (1 min) — toon slide 2. *"We kijken naar een spuitgietlijn. De klant vraagt onderdeelgewicht 100 ± 1 g. Dus de specs zijn 99 tot 101 g. Dat is wat de klant wil. Vraag: zijn dat ook de lijnen die op de regelkaart horen te staan?"* Laat de vraag hangen.

3. **Deel wb-01-spot-the-fout uit** (30 sec). Zeg: *"Je krijgt drie regelkaarten van dezelfde klant. Eén daarvan is fout opgezet. De andere twee zijn goed. Jouw opdracht: vind welke fout is en leg in één zin uit waarom. Bij twijfel: zet een vraagteken. Dat is een eerlijk antwoord."*

4. **Trainer doet kaart A voor (IK DOE)** (3 min) — toon slide 3. Lees hardop: *"Kaart A: gemiddelde 99,9 g, σ is 0,12. UCL op 100,26 en LCL op 99,54. Specs staan apart aangegeven op 99 en 101."* Zeg: *"Wat valt op? De UCL/LCL liggen binnén de specs. Dat is geen toeval — die zijn berekend uit 100 metingen van de eigen lijn met de formule UCL = gemiddelde + 3σ. Deze kaart geeft antwoord op de vraag: loopt mijn proces stabiel? De specs staan er apart op voor de tweede vraag: mag dit naar de klant? Twee vragen, twee aparte grenzen. Deze kaart: goed opgezet."*

5. **Deelnemers beoordelen kaart B en C zelf (JIJ DOET)** (7 min) — zet timer op 7 min. Zeg: *"Nu jij. Kijk naar kaart B en kaart C. Welke is fout opgezet en waarom? Eén zin per kaart."* Loop rustig rond. Beantwoord praktische vragen, geen inhoudelijke: *"Dat is precies wat we straks plenair bespreken."*

6. **Korte buurman-check** (2 min) — *"Pen neer. Vergelijk met je buurman: welke kaart koos jij, welke hij? Verschillen jullie? Probeer niet elkaar te overtuigen — alleen zien waar je het oneens bent."* Loop rond, luister mee.

7. **Plenaire bespreking** (2 min) — *"Handen omhoog: wie zegt kaart B is fout?"* Tel. *"Wie zegt kaart C?"* Tel. *"Wie twijfelt tussen B en C?"* Tel. Bevestig: *"Kaart B is fout — de UCL en LCL staan op precies 99 en 101, dezelfde waarden als de specs. Die zijn niet berekend uit procesdata; iemand heeft de klantspecs gewoon gekopieerd naar de regelkaart. Kaart C is goed — UCL en LCL uit 3σ berekend (100,64 en 99,56), specs apart getoond. We komen straks precies terug op waarom dit zo'n grote fout is."*

**Materiaal:**
- [ ] wb-01-spot-the-fout.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Slides 1-3 (cover, klantspecs-intro, kaart A "IK DOE")
- [ ] Timer

> **Tips voor de trainer:**
> - Houd bij IK DOE het tempo rustig en wijs fysiek naar de waarden op de slide. Het gaat om zichtbaar maken: *"hier staat het gemiddelde, hier 3σ, dit is UCL."* Niet rekenen op het bord — dat duurt te lang en verliest de doeners.
> - Loop tijdens het zelfstandig werken niet over schouders mee. Dat verhoogt prestatiedruk en stuurt deelnemers naar "het juiste antwoord". Laat ze worstelen; twijfel is hier productief.
> - Bij iemand die heel snel "kaart B" roept: vraag *"Waarom niet kaart C? Noem één verschil."* Zo blijft ook de snelle denker aan de stof.

> **Differentiatie:**
> - **MBO-3 basis:** lees bij kaart A de waarden langzaam voor en herhaal "UCL = gemiddelde + 3σ" twee keer. Geef desnoods 9 min schrijftijd in plaats van 7.
> - **MBO-4 sneller:** vraag extra: *"Bij kaart B — zou je met deze opzet een trend van 99,8 → 99,9 → 100,0 → 100,1 oppikken?"* Dit is een opmaat naar de NIST-waarschuwing in blok 3.

> **Valkuil — deelnemer vindt kaart B "wel handig":**
> Iemand zegt: *"Maar dan weet je toch gewoon wanneer het stuk afgekeurd wordt?"* Bevestig dat dit begrijpelijk voelt, maar parkeer: *"Dat klopt voor de afkeur-vraag. Maar de regelkaart is niet voor de afkeur-vraag. Daar komen we in blok 3 op terug — noteer je gedachte."*

> **Valkuil — niemand durft een kaart aan te wijzen:**
> Stilte na de buurman-check. Vraag gericht: *"Sandra, in welke kaart staan UCL en LCL op precies dezelfde waarden als de specs?"* De gesloten vraag helpt een voorzichtige deelnemer over de drempel.

---

### Blok 2: STARRT-reflectie — jouw eigen kaart
**00:15 - 00:27** | 12 min | Kolb-fase: reflecteren

**Doel:** De theorie uit blok 1 verbinden met de eigen werkplek. Veel deelnemers ontdekken nu dat ze niet zeker weten wat de lijnen op hun eigen kaart zijn — precies het moment waarop het onderscheid beklijft.

**Werkvorm:** Individueel STARRT-werkblad (7 min) → tweetallen uitwisselen (3 min) → kort plenair rondje (2 min).

**Instructie:**

1. **Deel wb-02-reflectie uit** (30 sec). Zeg: *"Dit werkblad volgt de STARRT-structuur: Situatie, Taak, Actie, Resultaat, Reflectie, Transfer. Je vult het in over je eigen werkplek. Niet-weten is een goed antwoord — dat is precies waarom deze sessie bestaat."*

2. **Individueel STARRT** (7 min) — zet timer op 7 min. Loop rustig rond. Help bij blokkades:
   - Bij *"ik weet het niet zeker"*: *"Schrijf dat op. 'Ik weet het niet zeker' is de eerlijke versie van het antwoord. Dat is goud waard."*
   - Bij *"er hangt geen kaart op mijn lijn"*: *"Denk aan een kaart die je wél ergens hebt gezien — een andere lijn, een collega. Of schrijf op: er hangt geen kaart, en wat dat betekent."*

3. **Tweetallen uitwisselen** (3 min) — *"Draai naar je buurman. Vraag aan elkaar: waar komen jullie UCL en LCL vandaan? Weet je het? Zo niet — aan wie ga je het vragen?"* Loop rond. Luister waar de verschillen zitten.

4. **Kort plenair rondje** (1 min 30) — *"Wie weet inmiddels zeker waar de lijnen op zijn lijn vandaan komen?"* Tel handen. *"Wie weet het niet zeker?"* Tel handen. *"Wie vermoedt dat het specs zijn die als control limits zijn ingevuld?"* Tel handen.

5. **Erkenning** (30 sec) — *"Kijk eens rond. Dit is normaal. De meeste operators weten het niet zeker. Dat komt niet door jullie — dat komt doordat die kaarten ooit zijn gemaakt zonder dat iemand jullie heeft uitgelegd waarop. Na blok 3 kun je zelf de juiste vraag stellen."*

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Timer

> **Tips voor de trainer:**
> - Stem zelf nooit mee in het handen-tellen. Je bent facilitator.
> - Bij iemand die zegt *"bij ons staan specs op de kaart"*: vraag *"Weet je dat zeker? Of heb je het altijd aangenomen?"* Meestal komt er dan *"ik heb het eigenlijk nooit gevraagd"* — en dat is precies het leermoment.
> - Tel innerlijk tot 7 na je vraag. Vul stilte niet in. Doeners-MBO-3 heeft denktijd nodig.

> **Valkuil — deelnemer schaamt zich voor "ik weet het niet":**
> Iemand zegt: *"Eigenlijk weet ik het niet — ik had het wel moeten weten."* Reageer ontspannen: *"Je had het niet moeten weten, want niemand heeft het je verteld. Wat je nu wel weet is dat je de vraag kunt stellen — en dat is het verschil."* Dit raakt de R van CAR: de relatiebasis houdt deelnemers open.

> **Valkuil — lange discussie over één specifieke machine:**
> Twee deelnemers van dezelfde lijn beginnen te discussiëren over hun eigen kaart. Bedank: *"Dit is het perfecte gesprek voor na de sessie — noteer het kort op je werkblad. We gaan terug naar het algemene principe."*

> **Differentiatie:**
> - **Gemengde groep:** bij de plenaire turf-ronde: vraag eerst de MBO-3'ers en daarna de MBO-4'ers. Anders sturen de MBO-4-stemmen het gesprek.

---

### Blok 3: Handout — het verschil, de 3σ-formule, de NIST-waarschuwing
**00:27 - 00:40** | 13 min | Kolb-fase: theoretiseren

**Doel:** De theorie expliciet maken als ordening van wat de deelnemers in blok 1 en 2 hebben ervaren. Geen nieuwe regelset — een bevestiging. Vergelijkingstabel, 3σ-formule, en de scenariomatrix staan centraal.

**Werkvorm:** Trainer-geleide handout-bespreking met live verwijzing naar de foute kaart B en de reflectie-uitkomsten.

**Instructie:**

1. **Onthul het diagram** (1 min) — verwijder de afdekking van de A3-versie achter in de zaal. Toon slide 4 (diagram op scherm). Zeg: *"Dit is waar we naartoe werken. Links zie je een regelkaart — zo hoort het. UCL en LCL uit de procesdata, specs apart getoond. Rechts zie je vier mogelijke situaties die je kaart kan laten zien. We lopen ze zo langs."*

2. **Deel wb-03-handout-verschil-control-vs-specs uit** (30 sec). Zeg: *"Pak je markeerstift. Markeer wat voor jou een aha-moment is. Dit werkblad neem je mee — het is je naslagwerk."*

3. **Vergelijkingstabel** (3 min) — toon slide 5. Lees de vier regels hardop langs, per regel: *"Welke vraag beantwoordt elke grens? Waar komen ze vandaan? Waar staan ze op de kaart? Welke beslissing volgt?"* Wijs terug naar kaart B uit blok 1: *"Op die foute kaart stond één lijn die twee vragen tegelijk moest beantwoorden. Dat kan niet."*
    Schrijf op de flip-over onder **PROCES (UCL/LCL)**: *"uit data, 3σ, is proces stabiel?"* en onder **PRODUCT (USL/LSL)**: *"van klant, mag dit naar klant?"*.

4. **De 3σ-formule van Shewhart** (3 min) — toon slide 6. *"Deze formule komt van Walter A. Shewhart. Hij werkte bij Bell Labs en schreef in 1931 het boek waarin de regelkaart werd uitgevonden. De formule: UCL = gemiddelde + 3σ, LCL = gemiddelde − 3σ. Die 3σ is niet willekeurig — bij een stabiel normaal proces zit 99,7% van je metingen binnen die grenzen. Dus als er iets buiten komt, is dat bijna zeker een echt signaal en geen toeval."*
    Reken hardop voor: *"Bij kaart A: gemiddelde 99,9, σ is 0,12. 3 × 0,12 is 0,36. 99,9 + 0,36 = 100,26. 99,9 − 0,36 = 99,54. Dat zijn de control limits die op kaart A staan."*

5. **NIST-waarschuwing** (3 min) — toon slide 7. *"Dit is een waarschuwing uit het NIST/SEMATECH e-Handbook of Statistical Methods — een referentiewerk voor proces- en meetbeheersing. Twee scenario's."*
    Lees voor: *"Een proces kan stabiel zijn én toch te dicht bij de specificatiegrens zitten. Omgekeerd: een proces kan incidenteel binnen specs produceren terwijl het al uit controle is."*
    Wijs naar de flip-over *"Binnen specs ≠ onder controle"*. *"Dat is de kern. Binnen specs zegt niets over het proces. Uit controle zegt niets over afkeur. Twee aparte dingen. De vier-scenario-matrix rechts op je handout laat precies zien wat je doet in welke situatie."*

6. **De 4-scenario-matrix kort** (2 min) — toon slide 8 (matrix uit het diagram). Per vak één zin:
    - *"Proces stabiel én binnen specs: laat lopen."*
    - *"Proces stabiel, maar vlak tegen de specs: capability verbeteren, minder spreiding."*
    - *"Proces niet meer stabiel, producten toevallig nog binnen specs: ingrijpen — dit is het scenario waar SPC zijn waarde bewijst."*
    - *"Proces stabiel, maar producten buiten specs: centreren — je proces draait op een verkeerde instelling."*

7. **Korte vraagronde** (30 sec) — *"Welke regel op de vergelijkingstabel had je niet zo scherp?"* Laat 1-2 mensen delen.

8. **Afsluiting en transfer** (1 min) — toon slide 9. *"Deze week: ga naar één regelkaart op jouw lijn. Kijk welke lijnen erop staan. Noteer de waarden. Vraag aan je teamleider of SPC-coördinator: komen deze uit de klantspecs of uit 3σ-berekening? Noteer het antwoord. Bonus: kijk of er kaarten hangen met specs én control limits allebei — dat is juist goede praktijk. Neem je notitie mee naar de volgende sessie."*

**Materiaal:**
- [ ] wb-03-handout-verschil-control-vs-specs.md (1 per deelnemer)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] diagram-lo-spc-107.svg — op A3 én op slides 4 en 8
- [ ] Slides 4-9
- [ ] Flip-over met twee kolommen PROCES / PRODUCT (voorbereid leeg, in dit blok ingevuld)
- [ ] Flip-over "Binnen specs ≠ onder controle"

> **Tips voor de trainer:**
> - Houd het tempo. 13 min is krap voor tabel + formule + NIST + matrix + transfer. Niet vertragen door eigen anekdotes — die kun je in de evaluatie kwijt.
> - Bij de 3σ-uitleg: niet in de statistische diepte duiken (geen normaalverdeling-grafiek, geen confidence intervals). De 99,7%-vuistregel is genoeg voor dit niveau. Verwijs MBO-4-deelnemers die meer willen naar ISO 7870-2.
> - De terugkoppeling naar kaart B in blok 1 is de belangrijkste interventie van dit blok. Daar landt het onderscheid persoonlijk: *"dat wat je net zag, die fout — hier zie je waaróm het een fout is."*

> **Differentiatie:**
> - **MBO-4 sneller:** voeg bij de NIST-waarschuwing een opmerking toe: *"Dit is precies waarom SPC en capability-analyse (Cp, Cpk) aparte disciplines zijn. Daar komen we in lo-spc-108 op terug."* Wie verder wil, verwijs naar ISO 7870-2.
> - **MBO-3 basis:** bij de 3σ-formule: laat de berekening achterwege, focus op *"UCL en LCL komen uit metingen op jouw eigen lijn, niet van de klant"*. Dat is de kern die moet blijven hangen.

> **Valkuil — deelnemer raakt in statistiek-overload:**
> Iemand fronst bij σ. Zeg: *"σ is alleen maar een maat voor hoeveel je metingen normaal heen en weer springen. Als je metingen dicht bij elkaar liggen, is σ klein. Als ze ver uit elkaar liggen, is σ groot. Excel of je SPC-software rekent het voor je uit — je hoeft zelf nooit die formule te doen. Maar je moet wel weten wat UCL en LCL zíjn."*

> **Valkuil — deelnemer vraagt "maar welke moet ik dan gebruiken?":**
> Dit verraadt dat het onderscheid niet geland is. Antwoord: *"Allebei, maar voor verschillende vragen. UCL/LCL gebruik je om te beoordelen of je moet ingrijpen in het proces. Specs gebruik je om te beoordelen of een stuk naar de klant mag. Nooit één lijn voor beide vragen."* Wijs naar de flip-over PROCES / PRODUCT.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-spot-the-fout.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-verschil-control-vs-specs.md | n + 2 | A4 dubbelzijdig — naslagwerk, mee naar werkvloer |
| ☐ | diagram-lo-spc-107.svg | 1 | Print A3 in kleur, hang achter in de zaal (eerst afdekken) |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Twee vellen: PROCES/PRODUCT-kolommen + "Binnen specs ≠ onder controle" |
| ☐ | Timer / mobiel met geluid | 1 | Voor 7-min en 9-min metingen |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slides 4 en 8 (SVG) zijn cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel drie regelkaarten

| Kaart | Gemiddelde | σ | UCL op kaart | LCL op kaart | 3σ-berekening UCL | 3σ-berekening LCL | Opzet | Waarom |
|-------|-----------|---|--------------|--------------|-------------------|-------------------|-------|--------|
| A | 99,9 g | 0,12 | 100,26 | 99,54 | 99,9 + 3×0,12 = 100,26 | 99,9 − 3×0,12 = 99,54 | **Goed** | UCL/LCL uit 3σ, specs (99-101) apart getoond |
| B | 100,0 g | 0,15 | 101,00 | 99,00 | 100,0 + 3×0,15 = 100,45 (niet op kaart) | 100,0 − 3×0,15 = 99,55 (niet op kaart) | **Fout** | UCL/LCL zijn gelijk aan de specs — klanttoleranties als control limits ingevuld |
| C | 100,1 g | 0,18 | 100,64 | 99,56 | 100,1 + 3×0,18 = 100,64 | 100,1 − 3×0,18 = 99,56 | **Goed** | UCL/LCL uit 3σ, specs (99-101) apart getoond |

**Kernverschil kaart B:** de berekende 3σ-grenzen zouden 99,55-100,45 zijn geweest. Op de kaart staan echter 99,00-101,00, precies de klantspecs. Een trend van 99,8 → 99,9 → 100,0 → 100,1 geeft op kaart B nooit een signaal, terwijl het proces wel degelijk opschuift. Dit is het signaalverlies dat NIST beschrijft.

**Slagingscriterium:** deelnemer wijst kaart B correct aan én noemt minimaal één reden die aansluit op "UCL/LCL zijn klantspecs, niet uit procesdata berekend" of "trend zou niet opgemerkt worden".

---

## Checklist na de sessie

- [ ] Werkbladen 1 en 2 ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Werkblad 3 (handout) — deelnemers nemen mee naar werkvloer (niet innemen!)
- [ ] Flip-over PROCES / PRODUCT gefotografeerd
- [ ] Notitie voor volgende sessie: bij hoeveel deelnemers stond "ik weet het niet zeker" als antwoord op vraag 2 van wb-02? (Indicatie voor hoeveel transfer-opvolging nodig is.)
- [ ] xAPI-statements verstuurd: `experienced` (spot-the-fout), `completed` (reflectie + handout gelezen)
- [ ] Check 1-2 weken later met de groep: wie is naar zijn eigen kaart gaan kijken en wat bleek?

---

*AIMM Curriculum | SPC Module 1 (Gebruik) | Control limits versus specificatiegrenzen*
*Bronnen: NIST/SEMATECH e-Handbook of Statistical Methods (Control Charts vs Specification Limits). | Shewhart, W.A. (1931) Economic Control of Quality of Manufactured Product. | ISO 7870-2 (Shewhart-regelkaarten). | Verwijzing kennisbank: ko-spc-101 (variatiebegrip), ko-spc-108 (procesbekwaamheid), ko-spc-203 (signaal-respons).*
*De getoonde regelkaarten in wb-01 zijn fictieve voorbeelden, bedoeld voor oefening.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
