# Cp en Cpk — wat zegt het cijfer écht? — Draaiboek
*SPC Module 2 (Train) | Workshop-blok 50 minuten | 6-10 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan een gegeven Cp- en Cpk-waarde interpreteren in operatorcontext, het probleem benoemen (centrering, spreiding, of stabiliteit), en een passende actie kiezen — in minimaal 3 van de 4 puzzelcasussen correct, met onderbouwing. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-10 personen |
| **Voorkennis** | ko-spc-101 (variatie), ko-spc-107 (specs vs control limits), lo-spc-201 (Nelson + stabiliteitscheck) doorlopen |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat Cp/Cpk bestaat na lo-spc-104 + lo-spc-201, maar kan het cijfer nog niet zelfstandig duiden. De puzzel activeert die ervaren onbekwaamheid bewust ('ik dacht dat ik dit kon, maar ik twijfel') als leerbrandstof. |
| **Begeleidingsstijl** | Trainen — veel sturing én veel ondersteuning. Scaffolding via IK DOE → WIJ DOEN → JIJ DOET: trainer modelleert eerst (worked example op het bord), werkt dan samen met de groep door (plenaire bespreking, hardop denken, flip-overtekening), pas dan zelfstandig oefenen op eigen lijn. Trainer demonstreert actief en bevestigt elke poging — geen coachen-stijl. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok 4 binnen module 2 (Train) — direct na pauze, vóór groepsreflectie configuratiebesluit |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Cpk-puzzel: 4 mini-casussen | 🟢 ervaren | 12 min |
| 00:12 - 00:25 | Plenaire bespreking + debrief | 🟣 reflecteren | 13 min |
| 00:25 - 00:38 | Handout: formules + interpretatietabel + spuitgiet-voorbeeld | 📘 theoretiseren | 13 min |
| 00:38 - 00:50 | Eigen-Cpk-analyse: één meetwaarde van mijn lijn | 🟢 experimenteren | 12 min |

**Totaal:** 50 minuten — geen aparte pauze (dit blok komt direct na de module-pauze).
**Buffer:** elk blok bevat 1-2 minuten flexibele ruimte; gebruik die voor doorvragen of voor uitloop in fase 2 (debrief).

---

## Voorbereiding

### De avond ervoor
- [ ] Print 4 werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 50 vellen bij 10 deelnemers.
- [ ] Print `diagram-lo-spc-301.svg` op A3 (in kleur indien mogelijk — twee verdelingen naast elkaar).
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer.
- [ ] Lees het antwoordmodel Cpk-puzzel in dit draaiboek door en bedenk per casus één extra voorbeeld uit jouw eigen ervaring (spuitgieten, CNC, verpakking, assemblage).
- [ ] Check of de doelgroeplijst klopt: zijn er teamleiders bij? Zo ja, voorbereid op de extra discussie over Ford PPAP en aanvullende capability studies.

### Het uur ervoor
- [ ] Leg per stoel: pen, stemkaartjes (4 kleuren of cijfers 1-4), wb-01-cpk-puzzel.
- [ ] Houd wb-02, wb-03, wb-04 apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Hang de A3-versie van het diagram zichtbaar achter in de zaal (nog afdekken — pas onthullen in blok 3).
- [ ] Schrijf op de flip-over alvast drie koppen: links **"Centrering?"**, midden **"Spreiding?"**, rechts **"Stabiliteit?"** — dit wordt je vangrail bij blok 2.
- [ ] Open slide 1 op het scherm.
- [ ] Optioneel: leg 2-3 rekenmachines klaar op de trainer-tafel voor wie zelf een Cpk wil narekenen — niet uitdelen, alleen op verzoek.

---

## Blok-details

### 🟢 Blok 1: Cpk-puzzel — 4 mini-casussen
**00:00 - 00:12** | 12 min | Kolb-fase: ervaren

**Doel:** De deelnemer ervaart aan den lijven dat een Cpk-cijfer alleen onvoldoende is — interpretatie vraagt om context (centrering, spreiding, stabiliteit). Verwarring wordt geactiveerd (= leerbrandstof voor het Cp/Cpk-onderscheid in fase 3).

**Werkvorm:** Individuele puzzel (JIJ DOET) — 4 casussen waarin Cp en Cpk gegeven zijn, deelnemer interpreteert ZONDER theorie.

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Wie van jullie heeft wel eens 'Cpk = 1,2' gehoord en gedacht: wat zegt dat me eigenlijk? Of erger nog: 'Cpk = 0,9 — slecht', en daarna naar de machine gerend om iets te tweaken?"* Wacht. Laat 1-2 mensen kort knikken. Geen lange verhalen.

2. **Trigger** (1 min) — *"In de komende 50 minuten gaan we van 'het cijfer kennen' naar 'het cijfer begrijpen'. Want een Cpk-getal zonder interpretatie is een mooi getal zonder actie — en soms zelfs een gevaarlijk getal."*

3. **Korte ophaal voorkennis** (1 min) — toon slide 2. Vraag plenair: *"Snel rondje — wie kan in één zin zeggen wat 'het proces is stabiel' betekent? Verwijs naar gisteren — Nelson, common cause, special cause."* Vang 1-2 antwoorden, bevestig kort. Dit is geen hertoetsing — alleen herinnering. Sluit af: *"Onthou dit. Stabiliteit komt straks terug — op een vervelende manier."*

4. **Deel wb-01-cpk-puzzel uit** (30 sec). Zeg: *"Vier mini-casussen. Per casus krijg je: een Cp-waarde, een Cpk-waarde, en of het proces stabiel is. Geen formules. Geen berekeningen. Jouw vraag: wat is hier aan de hand, en wat zou jij doen? Per casus heb je drie velden — probleem, actie, twijfel."*

5. **Puzzel invullen** (8 min) — zet timer op 8 min. Loop rustig rond. Beantwoord praktische vragen (*"betekent dit getal..."*) maar GEEN inhoudelijke (*"is mijn antwoord goed?"*) — verwijs door: *"Dat gaan we straks samen ontdekken — schrijf vooral op wat jij denkt, ook als je twijfelt."*

6. **Verzamel-moment** (1 min) — *"Pen neer. Bij welke casus had je de meeste twijfel? Steek je hand op bij casus 1... 2... 3... 4."* Tel hardop, schrijf de scores op de flip-over. Dit is je input voor blok 2.

**Materiaal:**
- [ ] wb-01-cpk-puzzel.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Slide 1 (cover) en slide 2 (puzzel-intro)
- [ ] Flip-over met de drie koppen Centrering / Spreiding / Stabiliteit
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Loop tijdens de puzzel langs maar buig je niet over schouders — dat verhoogt prestatiedruk en maakt twijfel onzichtbaar.
> - Als iemand al na 4 minuten klaar is: vraag *"Heb je casus 4 ook echt afgewogen — wat denk jij dat een autobouwer van Cpk = 0,90 vindt?"* De PPAP-context van casus 4 is de toetssteen — wie snel klaar is, is waarschijnlijk over de klantcontext heengelopen.
> - Bewaak de tijd. 12 min is krap voor 4 casussen — maar dat is bewust. Twijfel is leerstof.

> **🔄 Differentiatie:**
> - **MBO-3 per ongeluk in zaal:** beperk tot casus 1, 2 en 4. Zeg er bij: *"Voor jou zijn de eerste drie het belangrijkst — casus 4 is een bonus."*
> - **MBO-4 standaard:** alle vier. Geen extra uitdaging nodig — de casussen zelf zijn de uitdaging.
> - **Teamleider erbij:** geef extra opdracht: *"Per casus: noteer ook wat jij als teamleider in een rapportage zou schrijven."*

> **🔴 Valkuil — operators willen formules leren:**
> Bij vraag *"hoe rekenen we Cp dan uit?"*: zeg *"De formule staat in de handout straks, en de software rekent het voor je. Wat de software niet doet is interpreteren — dat is wat we hier oefenen."* Niet opnieuw uitleggen.

---

### 🟣 Blok 2: Plenaire bespreking + debrief
**00:12 - 00:25** | 13 min | Kolb-fase: reflecteren

**Doel:** Twijfel verwoorden, antwoorden vergelijken, het kernonderscheid Cp vs Cpk vs stabiliteit uit eigen denken laten ontstaan (vóór de theorie). De aha-momenten landen.

**Werkvorm:** Plenaire bespreking per casus — eerst gokken (stemkaartjes), dan duiden (trainer + groep). Inclusief debrief van casus 4 (PPAP-context) als laatste klap.

**Timing-note (na review-cyclus v3):** 13 min is krap voor 4 casussen plenair + buurman-check + volledig wb-02 invullen. Werkbare verdeling: 3 min buurman (alleen uitslag-vergelijking, niet de uitleg) + 9 min plenair (3+2+1+3 per casus) + 1 min uitloop. wb-02 wordt **parallel** ingevuld tijdens de plenaire bespreking (1 zin per casus) en thuis afgemaakt vóór de volgende sessie. Niet de volledige Korthagen-reflectie tijdens de sessie — dat past niet.

**Instructie:**

1. **Deel wb-02-reflectie uit** (30 sec). Zeg: *"Tijdens de bespreking vul je per casus 1 korte zin in: wat had je gedacht voordat we de casus bespraken, en wat denk je nu? Het verschil daartussen — dat is je leeropbrengst van vandaag. De volledige Korthagen-vragen maak je thuis af — neem het werkblad mee naar de volgende sessie."*

2. **Bespreek casus 1 — spuitgiet, centreer-puzzel** (3 min). Zeg: *"Eerst gokken. Wat is hier aan de hand? Steek je vinger op: 1 = niets, 2 = centrering, 3 = spreiding, 4 = stabiliteit."* Vang stemming. Bij verdeling tussen 'centrering' en 'twijfel/niets': *"Wie koos centrering — waarom?"* Laat uitleggen. Daarna: *"Cp = 1,39 — dat is boven 1,33, dus de spreiding past in potentie. Maar Cpk = 1,11 — lager dan Cp. Hoe kan dat?"*
    - Pak een markeerstift, teken op de flip-over snel twee verticale lijnen (LSL = 99,5 g en USL = 100,5 g) en daartussen een smalle klokvorm — maar verschoven naar de ondertolerantie (gemiddelde 99,9 g, niet 100,0 g).
    - *"De pers is smal genoeg in z'n spreiding — maar staat scheef tegen de ondergrens aan. Actie: centreren — gemiddelde naar 100,0 brengen. NIET aan de spreiding sleutelen — die is al goed. Dit is precies het patroon dat we straks in het spuitgiet-rekenvoorbeeld terugzien."*
    - Schrijf op de flip-over onder Centrering: ✅, onder Spreiding: ❌, onder Stabiliteit: ❌.

3. **Bespreek casus 2 — CNC-frees, spreiding te groot** (3 min). Vraag stemming. *"Cp = 0,85, Cpk = 0,85 — Cp en Cpk zijn gelijk. Wat zegt dat?"* Wacht. Eén iemand zegt 'gecentreerd'. *"Ja — als Cp en Cpk samenvallen, staat het proces gecentreerd. Maar beide onder 1,0. Wat is hier het probleem?"* Iemand: 'spreiding'. *"Precies. Het proces (boorgat 9,90–10,10 mm, gemiddelde 10,00 mm) staat netjes in het midden, maar de fles is te wijd voor het tolerantievak. Hier helpt centreren niets — je moet de spreiding zelf aanpakken: machine-onderhoud, beitelvervanging, betere materiaalspecificatie, of bij de klant terug om de tolerantie te heronderhandelen. Dit is een teamleider/engineering-gesprek."*

4. **Bespreek casus 3 — verpakking, alles goed** (2 min). Vraag stemming. Bij overgrote meerderheid 'niets': *"Goed gezien. Cp = 1,67 én Cpk = 1,67 — gelijk én ruim boven de Ford PPAP-grens. Vulgewicht 498–502 g, gemiddelde al maanden op 500,0 g. Dit proces is ruim capabel én gecentreerd. Actie: blij zijn. Niet tweaken — iedere instelling-aanpassing op een capabel proces verhoogt het risico op procesdrift. 'Goed laten zijn' is ook een vaardigheid."*

5. **Bespreek casus 4 — automotive, centreer + PPAP-shock** (4 min). Dit is dé casus van de sessie — niet door een trick maar door de klantcontext. Vraag stemming.
    - Veel deelnemers zien Cp = 1,45 en Cpk = 0,90 en denken 'oh, lijkt op casus 1 — centreren'. Inhoudelijk klopt dat — maar de klantcontext maakt het zwaarder.
    - Onthul stap 1: *"Inhoudelijk hetzelfde patroon als casus 1: Cp boven 1,33, Cpk onder 1,0 — centreer-probleem. Gemiddelde 49,87 g zit te dicht tegen de ondergrens 49,80 g. Eerste actie: centreren naar 50,00 g."*
    - Stilte. Wijs op de eerste regel van de casus: *"Maar er staat één belangrijke extra zin: 'klant = autobouwer (PPAP-niveau)'. Wat denken jullie dat de autobouwer van Cpk = 0,90 vindt?"*
    - Tel innerlijk tot 5. Iemand: 'die accepteert dat niet'. *"Precies. PPAP-eis is Cpk ≥ 1,67. Een Cpk van 0,90 op een PPAP-onderdeel betekent: contractueel afgekeurd. Centreren alleen brengt je hooguit naar Cpk ≈ 1,4–1,5 — nog steeds onder 1,67. Voor PPAP-acceptatie is procesverbetering nodig — dat is engineering-territorium. Tot die tijd: lijn niet vrijgeven voor klantleveringen, of in overleg met kwaliteitsdienst."*
    - Verbreed: *"De les: dezelfde getallen kunnen totaal verschillende beslissingen vragen — afhankelijk van de klantcontext. Een operator die Cpk = 0,90 ziet zonder de klantcontext denkt 'centreren'. Een operator die de klantcontext kent, weet dat hij ook moet escaleren."*

6. **Sluit blok 2 af** (30 sec) — wijs naar de flip-over. Zeg: *"Drie verschillende patronen, drie verschillende acties — en één gemene gemeenschappelijke deler: zonder context (zowel proces-context: stabiliteit, als klant-context: PPAP-eis) zegt een Cpk-getal niets. We gaan nu kijken naar de formules — niet om te rekenen, maar om te zien waar dat verschil tussen Cp en Cpk vandaan komt. En in blok 3 komt stabiliteit terug als één van de drie veelgemaakte fouten — zodat je ook die laag straks paraat hebt."*

**Antwoordmodel — gebruik dit als basis voor de bespreking (exact gesynchroniseerd met wb-01):**

| Casus | Gegeven | Probleem | Actie | Pedagogische tip |
|-------|---------|----------|-------|------------------|
| 1 (spuitgiet) | Cp = 1,39 ; Cpk = 1,11 ; stabiel; spec 99,5–100,5 g; μ = 99,9 g | centrering | Centreren — gemiddelde van 99,9 → 100,0 g | Cp > Cpk = klassiek centreer-patroon; spreiding NIET aanpakken |
| 2 (CNC-frees) | Cp = 0,85 ; Cpk = 0,85 ; stabiel; spec 9,90–10,10 mm; μ = 10,00 mm | spreiding (intrinsiek) | Spreiding verkleinen (onderhoud, beitelvervanging) of tolerantie heronderhandelen | Cp = Cpk = gecentreerd; centreren helpt hier niets, vraagt teamleider/engineering |
| 3 (verpakking) | Cp = 1,67 ; Cpk = 1,67 ; stabiel; spec 498–502 g; μ = 500,0 g | geen | Blij zijn — ruim capabel, voldoet aan Ford PPAP (≥ 1,67) | Niet onnodig tweaken; iedere instelling-aanpassing verhoogt risico op procesdrift |
| 4 (automotive PPAP) | Cp = 1,45 ; Cpk = 0,90 ; stabiel; spec 49,80–50,20 g; μ = 49,87 g; klant = autobouwer | centrering + onacceptabel onder PPAP-eis (≥ 1,67) | Direct centreren naar 50,00 g, daarna ESCALEREN naar engineering — Cpk ≈ 1,4 nog steeds onder 1,67 | Klantcontext maakt het zwaarder; vraag plenair: 'wat vindt de autobouwer van Cpk = 0,90?' |

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Stemkaartjes 1-4 of 4 kleuren (1 set per deelnemer)
- [ ] Flip-over met centrering / spreiding / stabiliteit-koppen
- [ ] Markeerstift voor flip-over-tekening (klokvorm verschoven)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Stem zelf nooit mee. Je bent facilitator, geen deelnemer.
> - Bij casus 4: laat de stilte vallen. Niet invullen. Het ongemak ís het leereffect.
> - De flip-overtekening bij casus 2 (verschoven klokvorm tussen LSL en USL) is je belangrijkste visuele middel — twee lijnen + één klok kost 10 seconden en landt sterker dan elke slide.
> - Tel innerlijk tot 7 na elke vraag. Vul stilte niet in.

> **🔴 Valkuil — Cpk = goed/slecht zonder klantcontext:**
> Bij casus 4 zegt iemand 'Cpk = 0,90 dus centreren — klaar'. Niet meteen corrigeren. Vraag: *"Wie is hier de klant, en wat eist die contractueel?"* Laat hen zelf de PPAP-context vinden. Verbreed: *"Een Cpk-getal hangt altijd af van de klantcontext — voor één klant is 1,33 prima, voor een autobouwer is 1,67 het minimum."*

> **🔴 Valkuil — centrering en spreiding worden niet onderscheiden:**
> Bij casus 2 zegt iemand 'centreren' bij Cp = 0,85 en Cpk = 0,85. Vraag: *"Cp en Cpk zijn allebei 0,85 — wat zegt dat over de positie van het gemiddelde?"* Laat de groep ontdekken dat gelijke Cp en Cpk = gecentreerd. Pas dan duiden: spreiding is hier het probleem, niet centrering.

> **🔴 Valkuil — instabiliteit niet besproken in wb-01:**
> wb-01 bevat geen instabiele casus (de eerdere 'trick'-versie is vervangen door een PPAP-context). Compenseer: noem in blok 3 bij 'drie veelgemaakte fouten' de instabiliteit expliciet als #1, en verwijs terug naar lo-spc-201 (Nelson). Wie wil testen of de groep dit echt heeft begrepen, kan plenair vragen: *"Stel: in casus 4 was de regelkaart instabiel geweest — wat had je dan met de getallen Cp = 1,45 en Cpk = 0,90 gedaan?"* Antwoord: niets — je mag geen capability uitspraak doen op een instabiel proces.

> **🔴 Valkuil — specs vs control limits:**
> Iemand zegt 'we zitten binnen de UCL/LCL dus capabel'. Stop kort. *"Belangrijk verschil: Cp en Cpk vergelijken klantgrenzen (USL/LSL — staan op de tekening) met procesgedrag. UCL/LCL zijn proceslimieten — die berekent SPC uit jouw data zelf. Andere meting, andere doel."* Verwijs naar ko-spc-107.

> **🔄 Differentiatie:**
> - **Teamleider erbij:** voeg na casus 4 een korte vraag toe: *"Wanneer is op jouw lijn een aanvullende capability study nodig? Bij elke procesverandering, bij klantklacht, bij PPAP-aanvraag?"* Vang 1-2 antwoorden — niet uitdiepen, parkeren voor groepsreflectie straks.

---

### 📘 Blok 3: Handout — formules + interpretatietabel + spuitgiet-voorbeeld
**00:25 - 00:38** | 13 min | Kolb-fase: theoretiseren

**Doel:** Het Cp/Cpk-onderscheid expliciet maken, formules en interpretatietabel verankeren, en de spuitgiet-casus laten dienen als geïntegreerd voorbeeld dat alles samenbrengt. Theorie als bevestiging van wat ze al hebben ervaren.

**Werkvorm:** Trainer-geleide handout-bespreking met live koppeling naar de puzzelcasussen + één geïntegreerd rekenvoorbeeld.

**Instructie:**

1. **Onthul het diagram** (1 min) — verwijder de afdekking van de A3-versie achter in de zaal. Toon slide 7. Zeg: *"Twee verdelingen. Links: smal en gecentreerd — Cp hoog, Cpk hoog. Rechts: even smal, maar verschoven — Cp hetzelfde, Cpk laag. Dat is precies casus 2 uit jullie puzzel. Cp vraagt: is de fles smal genoeg? Cpk vraagt: staat hij ook midden op de tafel?"*

2. **Deel wb-03-cpk-handout uit** (30 sec). *"Pak je markeerstift. Markeer wat voor jou nieuw of verrassend is."*

3. **Behandel Cp** (2 min) — slide 5. Schrijf op flip-over: **Cp = (USL − LSL) / 6σ**. *"Bovenkant min onderkant van de tolerantie, gedeeld door zes keer de procesvariatie. Of in operator-taal: hoe vaak past de spreiding van mijn proces in het tolerantievak? Cp = 1 betekent: precies één keer — het past nipt. Cp = 1,33 betekent: het past met 33% marge. Cp = 1,67 betekent: het past ruim — Ford-niveau."* Geen berekening hier — alleen de leesregel.

4. **Behandel Cpk** (2 min) — slide 6. Schrijf op flip-over: **Cpk = min[(USL−μ)/3σ, (μ−LSL)/3σ]**. *"Twee afstanden: van het gemiddelde naar de bovengrens, en van het gemiddelde naar de ondergrens — beide gedeeld door 3σ. Het kleinste van die twee is je Cpk. Cpk vertelt dus: hoe ver zit ik van de dichtstbijzijnde tolerantiegrens, gemeten in spreidingseenheden? Hoe groter het verschil tussen Cp en Cpk, hoe schever het proces staat."*

5. **Interpretatietabel** (2 min) — slide 8. Loop snel door:
    - *"Onder 1,0 — niet capabel, structureel afkeur waarschijnlijk."*
    - *"Precies 1,0 — theoretisch passend, maar één procesdrift en je bent buiten."*
    - *"1,33 — veelgebruikte industriële ondergrens. De minimum die meeste klanten accepteren."*
    - *"1,67 — Ford PPAP, automotive, kritische karakteristieken."*
    - *"2,0 — gecentreerd zes-sigma proces — luxepositie."*

6. **Spuitgiet-voorbeeld** (4 min) — slide 9. *"Concrete casus. Spuitgietlijn, onderdeelgewicht moet tussen 99,5 en 100,5 gram liggen. Stabiele lijn — regelkaart zegt: alleen common cause. Gemiddelde van 50 metingen: 99,9 gram. σ van die metingen: 0,12 gram."*
    - Toon Cp-berekening: *"Cp = (100,5 − 99,5) / (6 × 0,12) = 1,00 / 0,72 ≈ 1,39. Cp boven 1,33 — spreiding zit goed."*
    - Toon Cpk-berekening: *"Cpk = min[(100,5 − 99,9)/0,36 ; (99,9 − 99,5)/0,36] = min[1,67 ; 1,11] = 1,11. Cpk boven 1,0 maar onder 1,33."*
    - Stilte. *"Wat zien we? Cp is mooi, maar Cpk lager — verschil zit in centrering. De pers staat te dicht tegen de ondertolerantie aan. Schiet de pers te wijd? Nee. Staat hij scheef? Ja."*
    - *"Operatorles: de juiste actie is centreren — gemiddelde naar 100,0 brengen, niet harder proberen de spreiding te verkleinen. Dat is de hele les van vandaag in één voorbeeld."*

7. **Drie veelgemaakte fouten** (1 min 30) — slide 10. Loop snel door:
    - *"Eén: capability op een instabiel proces — casus 4 uit jullie puzzel. Verboden."*
    - *"Twee: slechte subgroepering — kortetermijn- en langetermijnvariatie door elkaar. Komt in module 3 terug."*
    - *"Drie: slecht meetsysteem — Cpk zegt evenveel over de meter als over de machine. Hoe je je meter checkt heet MSA of Gage R&R. Onderwerp voor jullie kwaliteitsdienst, of voor module 3."*

8. **Overgang naar blok 4**: *"Nu is het bekend. Tijd om het op je eigen lijn los te laten — maar wel met de stabiliteits-vraag erbij."*

**Materiaal:**
- [ ] wb-03-cpk-handout.md (1 per deelnemer)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] diagram-lo-spc-301.svg — op A3 én op slide 7
- [ ] Slides 5-10
- [ ] Flip-over voor Cp- en Cpk-formules

> **💡 Tips voor de trainer:**
> - Houd het tempo. 13 min is krap voor formules + tabel + voorbeeld + drie fouten. Niet vertragen door eigen anekdotes — bewaar die voor blok 4.
> - Het spuitgiet-voorbeeld is je krachtigste moment. Schrijf de uitkomsten op de flip-over zodat ze blijven staan voor blok 4.
> - Vermijd symmetrische voorbeelden waar Cpk = Cp toevallig samenvalt — dat creëert verwarring. Het asymmetrische spuitgiet-voorbeeld (μ = 99,9, niet 100,0) is bewust gekozen.

> **🔴 Valkuil — trainer gaat te diep op MSA:**
> Verleidelijk om hier de Gage R&R-procedure uit te leggen. Niet doen. Eén zin: *"Cpk zegt evenveel over de meter als over de machine — hoe je je meter checkt is een onderwerp voor je kwaliteitsdienst of voor module 3."* Verder niets. MSA is HBO-niveau en zuigt 10 minuten op.

> **🔴 Valkuil — trainer gaat over op Pp/Ppk:**
> Een MBO-4'er met voorkennis vraagt naar Pp/Ppk of long-term capability. *"Goede vraag — Pp en Ppk komen in module 3 (Op Maat) uitgebreid terug. Vandaag houden we het bij Cp en Cpk."* Schrijf op parkeerflip.

> **🔄 Differentiatie:**
> - **MBO-4 sneller / teamleider:** noem ook kort de term **PPAP** (Production Part Approval Process — Ford) bij ≥ 1,67. Operators negeren de term, teamleiders onthouden hem.
> - **Operator basis:** sla de exacte formules over op flip-over — vertel alleen de leesregel ("hoe vaak past de spreiding").

---

### 🟢 Blok 4: Eigen-Cpk-analyse — één meetwaarde van mijn lijn
**00:38 - 00:50** | 12 min | Kolb-fase: experimenteren

**Doel:** De deelnemer formuleert een concrete transferopdracht voor de eigen werkvloer. Eigenaarschap (autonomie) staat centraal — ze kiezen zelf welke meetwaarde ze gaan analyseren. Stabiliteits-vraag is verplicht onderdeel.

**Werkvorm:** Individueel werkblad invullen + korte plenaire afsluiting + transferopdracht.

**Instructie:**

1. **Deel wb-04-eigen-cpk-analyse uit** (30 sec). Zeg: *"De afgelopen 38 minuten waren oefenen met casussen. Nu kijk je naar je eigen lijn. Kies één meetwaarde waarvan je weet of vermoedt dat de tolerantie bekend is — onderdeelgewicht, diameter, vulhoogte, druk, temperatuur. Iets waar USL en LSL voor bestaan."*

2. **Inventarisatie-vraag** (1 min) — *"Even rondkijken: noem in één zin welke meetwaarde je kiest, en wat de tolerantie is — als je die uit je hoofd weet."* Vang 4-5 voorbeelden op (gewicht, diameter, vulvolume, lengte). Niet bespreken — alleen verzamelen. Helpt deelnemers die niet weten wat ze moeten kiezen.

3. **Individueel invullen** (8 min) — zet timer op 8 min. Loop rond. Het werkblad heeft 4 secties:
    - Welke meetwaarde + USL en LSL?
    - Is je proces stabiel? Hoe weet je dat? (Verwijs naar lo-spc-201 — Nelson, regelkaart van gisteren.)
    - Welke Cp- en Cpk-waarde verwacht je / heb je beschikbaar / ga je opvragen?
    - Wat is jouw interpretatie en welke actie gaat daaruit volgen?
    Help bij blokkades met deze vragen:
    - *"Welke meetwaarde controleren jullie sowieso al elke shift?"*
    - *"Heb je een idee waar het gemiddelde zit ten opzichte van de specs?"*
    - *"Wat zou je gaan doen als je hoort: Cpk = 1,0?"*
    Bevestig dat 'ik moet dit eerst opvragen' een geldig antwoord is — sterker nog: vaak het juiste.

4. **Korte deel-ronde** (2 min) — *"Wie wil in één zin vertellen welke meetwaarde je gaat onderzoeken, en welke actie je verwacht dat eruit komt?"* 3-4 deelnemers, max 30 sec per persoon.

5. **Afsluiting + transfer** (30 sec) — slide 12. *"Deze week: vraag bij je teamleider of kwaliteitsdienst de Cp- en Cpk-waarden op van jouw gekozen meetwaarde, plus de stabiliteits-status. Beantwoord drie vragen: is het stabiel? Wat is het probleem (centrering, spreiding, beide, geen)? Welke actie is passend? Bonus: praat er één keer met een collega over — 'wat zou jij doen bij Cpk = 1,1 met Cp = 1,4?'. Volgende workshop bespreken we per persoon."*

**Materiaal:**
- [ ] wb-04-eigen-cpk-analyse.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slide 11 (eigen-lijn-actieplan)
- [ ] Slide 12 (transferopdracht)
- [ ] Slide 13 (afsluiting)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Het is verleidelijk om in deze fase 'mee te denken' over instellingen of acties. Niet doen. De deelnemer moet zelf de keuze maken — dat is de autonomie-component die het werkbaar maakt op de werkvloer.
> - Als iemand drie meetwaardes wil kiezen: zeg *"Ik daag je uit om er één te kiezen waarvan je het meeste vermoeden hebt dat er iets te ontdekken valt. Die levert in week 1 het meeste op."*
> - Bonusvraag voor wie snel klaar is: *"Wat zou je doen als je teamleider zegt 'Cpk hoeft hier niet boven 1,33'? Hoe ga je dat gesprek voeren?"*

> **🔄 Differentiatie:**
> - **MBO-3 per ongeluk in zaal:** één meetwaarde opvragen + één interpretatie noteren is genoeg. Geen tijdspad, geen actie.
> - **MBO-4 standaard:** vraag om naast de actie ook een tijdpad ('wanneer ga ik dit voorstellen aan mijn teamleider?').
> - **Teamleider:** dubbele rol — eigen analyse + één opdracht voor zijn team ('mijn operator X gaat meting Y opvragen, ik bespreek het op vrijdag').

> **🔴 Valkuil — geen tijd voor de afsluiting:**
> Als blok 3 is uitgelopen: kort blok 4 in tot 10 minuten door de inventarisatie naar 30 sec te brengen en de deel-ronde naar 1 minuut. Sla de afsluiting / transferopdracht NOOIT over — dat is wat de workshop verbindt met de werkvloer.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-cpk-puzzel.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-cpk-handout.md | n + 2 | A4 dubbelzijdig (handout) |
| ☐ | wb-04-eigen-cpk-analyse.md | n + 2 | A4 enkelzijdig |
| ☐ | diagram-lo-spc-301.svg | 1 | Print A3 in kleur, hang achter in zaal (twee verdelingen) |
| ☐ | Stemkaartjes 1-4 (of 4 kleuren) | n sets | 1 set per deelnemer voor casus-stemming |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Voor centrering/spreiding/stabiliteit-koppen + flip-over-tekening (verschoven klokvorm) |
| ☐ | Timer / mobiel met geluid | 1 | Voor 8-min puzzel + 8-min eigen-analyse |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 7 (SVG) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |
| ☐ | Rekenmachine of telefoon | 2-3 | Optioneel — alleen op verzoek, voor wie zelf wil narekenen |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel Cpk-puzzel

| Casus | Gegeven (uit wb-01) | Probleem | Actie |
|-------|---------------------|----------|-------|
| 1 (spuitgiet) | Cp = 1,39 ; Cpk = 1,11 ; stabiel; 99,5–100,5 g; μ = 99,9 g | centrering | Centreren naar 100,0 g — spreiding niet aanpakken |
| 2 (CNC-frees) | Cp = 0,85 ; Cpk = 0,85 ; stabiel; 9,90–10,10 mm; μ = 10,00 mm | spreiding (intrinsiek) | Spreiding verkleinen of tolerantie heronderhandelen — centreren helpt niet |
| 3 (verpakking) | Cp = 1,67 ; Cpk = 1,67 ; stabiel; 498–502 g; μ = 500,0 g | geen | Blij zijn — ruim capabel, voldoet aan Ford PPAP |
| 4 (automotive PPAP) | Cp = 1,45 ; Cpk = 0,90 ; stabiel; 49,80–50,20 g; μ = 49,87 g; klant = autobouwer | centrering + onacceptabel onder PPAP-eis | Direct centreren naar 50,00 g + ESCALEREN naar engineering — Cpk ≈ 1,4 nog steeds < 1,67 |

**Slagingscriterium:** 3 of meer correct = leerdoel behaald (ABCD-degree). Casus 4 is de toetssteen voor diepere interpretatie (klantcontext meewegen). Stabiliteit komt aan bod in blok 3 als één van de drie veelgemaakte fouten — wb-01 bevat in deze versie geen instabiele casus.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Twijfel-statistiek genoteerd (welke casussen waren het lastigst)
- [ ] Centrering/spreiding/stabiliteit-flip-over gefotografeerd
- [ ] Notitie voor volgende workshop: welke meetwaardes hebben deelnemers gekozen voor de eigen analyse?
- [ ] xAPI-statements verstuurd: `experienced` (Cpk-puzzel), `completed` (reflectie + eigen-analyse)
- [ ] Bij teamleider-deelnemers: korte handover naar de groepsreflectie configuratiebesluit (volgend blok in module 2)

---

*AIMM Curriculum | SPC Module 2 (Train) | Cp en Cpk — wat zegt het cijfer écht?*
*Bronnen: NIST/SEMATECH e-Handbook, sectie 6.1.6 | Ford PPAP, 4th ed. | Minitab Capability Analysis docs | Wheeler, D.J. (1999). Beyond Capability Confusion. SPC Press.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
