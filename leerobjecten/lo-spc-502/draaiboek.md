# Welke kaart, welke bovengrens, welk signaal? — Draaiboek
*SPC Module 2 (Train) | Workshop-blok 45 minuten | 6-10 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan bij telgegevens van een assemblage-inspectie (defecten per vaste eenheid) het c-kaarttype herkennen, de UCL berekenen met c̄ + 3√c̄, een punt boven UCL duiden als Nelson-regel-1, en minimaal 2 escalatiestappen in de juiste volgorde benoemen — in de oefening minimaal 3 van de 4 deelvragen correct. |
| **Doelgroep** | Operators MBO-3 en MBO-4 (primair, assemblage / kleinserie / inspectie), teamleiders MBO-4 (secundair), 6-10 personen |
| **Voorkennis** | ko-spc-108 (variatie: common vs special cause), ko-spc-201 (regelkaart-basis: centerlijn, UCL/LCL, één punt buiten limieten) doorlopen |
| **Stadium (H&B)** | Bewust onbekwaam — weet dat er meerdere regelkaarten zijn, kiest in de praktijk vaak intuïtief. Na ko-spc-108 en ko-spc-201 is het concept "één punt buiten UCL = signaal" bekend, maar de vertaling naar "welke kaart kies ik, wat is de formule, en durf ik nú te escaleren?" is nog niet gemaakt. |
| **Begeleidingsstijl** | Trainen — veel sturing én veel ondersteuning. Scaffolding via JIJ DOET → WIJ BESPREKEN → IK DUID: deelnemer probeert eerst zelfstandig (kaartkeuze, UCL-berekening, signaal-markering), trainer bespreekt plenair wat ze vonden, pas dan expliciete handout met de regels. De trainer demonstreert niet voor — de casus doet dat. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen module 2 (Train) — volgt op lo-spc-201 (Nelson-regels generiek), voorafgaand aan de groepsreflectie "welke kaart hoort bij mijn lijn?" |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | c-kaart oefening: kaartkeuze + UCL + signaal + eerste stap | 🟢 ervaren | 15 min |
| 00:15 - 00:30 | STARRT-reflectie op een late escalatie uit eigen werkvloer | 🟣 reflecteren | 15 min |
| 00:30 - 00:45 | Handout: c vs p vs np — Nelson-regel-1 — escalatieketen | 📘 theoretiseren | 15 min |

**Totaal:** 45 minuten — geen aparte pauze (dit blok komt direct na de module-pauze).
**Buffer:** elk blok bevat 1-2 minuten flexibele ruimte; gebruik die voor doorvragen of voor uitloop in fase 2 (reflectie).

---

## Voorbereiding

### De avond ervoor
- [ ] Print 3 werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 36 vellen bij 10 deelnemers.
- [ ] Print `diagram-lo-spc-502.svg` op A3 (in kleur indien mogelijk — de rode Nelson-regel-1 markering moet van achter in de zaal leesbaar zijn).
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer. Check slide 7 (A3-diagram ingesloten) op kleurweergave.
- [ ] Lees het antwoordmodel c-kaart oefening in dit draaiboek door en bedenk één extra eigen voorbeeld (soldeerfouten, krassen, foute labels, miswegingen) uit de productie-omgeving van de deelnemers.
- [ ] Check de doelgroeplijst: werken deelnemers in PCB/elektronica, assemblage, voedselverwerking, of verpakking? De casus blijft PCB (vastgelegd in ko-spc-502), maar de transferopdracht in blok 3 wordt overtuigender als jij één aangrenzend voorbeeld paraat hebt.
- [ ] Ga na of er teamleiders bij zijn. Zo ja, voorbereid op de extra discussie over materiaal-traceerbaarheid (batch-ID koppelen aan uur-inspectie, MES-systeem).

### Het uur ervoor
- [ ] Leg per stoel: pen, rekenmachine of voorbereide vierkantswortel-tabel (√2,4 ≈ 1,549 — deelnemers mogen ook hun telefoon gebruiken), wb-01-oefening.
- [ ] Houd wb-02 en wb-03 apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Hang de A3-versie van `diagram-lo-spc-502.svg` zichtbaar achter in de zaal — nog afdekken, pas onthullen in blok 3.
- [ ] Schrijf op de flip-over alvast drie koppen: links **"Kaart?"**, midden **"UCL?"**, rechts **"Signaal?"** — dit wordt je vangrail bij blok 1 en 3.
- [ ] Open slide 1 op het scherm.
- [ ] Optioneel: leg 2-3 rekenmachines klaar op de trainer-tafel voor wie geen telefoon gebruikt.

---

## Blok-details

### 🟢 Blok 1: c-kaart oefening — kaartkeuze, UCL, signaal, eerste stap
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** De deelnemer ervaart dat drie dingen tegelijk spelen — het juiste kaarttype kiezen, de bovengrens uitrekenen, en een signaal herkennen — en dat dit in de praktijk in enkele minuten moet kunnen. De twijfel bij "is dit al een signaal of pech?" is de ingang voor blok 2 en 3.

**Werkvorm:** Individueel werkblad (JIJ DOET) — één fictieve PCB-casus met vier deelvragen. Geen formuleles vooraf — de formule staat op het werkblad.

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Stel je voor: je staat om 7 uur 's ochtends op een assemblagelijn. Er komt een nieuwe materiaalbatch binnen. Eerste uur na de wissel zie je 8 soldeerfouten op 50 boards. Normaal zijn het er 2 of 3. Is dit toeval? Of moet je nu aan de bel trekken?"* Wacht even. Laat 1-2 mensen kort knikken. Geen lange verhalen.

2. **Trigger** (1 min) — *"Wie op dit moment aan de bel trekt, beperkt de schade van zijn shift tot misschien 150 boards. Wie een uur afwacht, raakt er al snel 500. Wie een hele shift afwacht — duizenden. Dat is het verschil dat we vandaag maken. We gaan niet een nieuwe formule leren — we gaan leren om bij één punt boven de bovengrens te handelen, niet te wachten."*

3. **Korte ophaal voorkennis** (1 min) — toon slide 2. Vraag plenair: *"Snel rondje — wie kan in één zin zeggen wat 'één punt buiten UCL' betekende in de sessie van gisteren?"* Verwijs naar lo-spc-201. Vang 1-2 antwoorden, bevestig kort: *"Goed — Nelson-regel-1. Dat komt vandaag terug op een specifieke kaart: de c-kaart voor tellingen. Maar eerst gaan jullie het zelf proberen."*

4. **Deel wb-01-oefening uit** (30 sec). Zeg: *"Eén casus. Vier deelvragen. Op het werkblad staan alle getallen die je nodig hebt — en de formule. Jouw taak: kies de kaart, reken de UCL, markeer het signaal, en schrijf op wat je als eerste zou doen. Bij twijfel: zet een vraagteken — dat bespreken we zo."*

5. **Werkblad invullen** (11 min) — zet timer op 11 min. Loop rustig rond. Beantwoord praktische vragen (*"wat is √2,4?"*, *"wat betekent afkappen?"*) maar GEEN inhoudelijke (*"is c de goede kaart?"*) — verwijs door: *"Schrijf op wat jij denkt, ook als je twijfelt. We bespreken het zo plenair."*

6. **Buurman-check** (1 min) — *"Vergelijk met je buurman. Niet uitleggen — alleen noteren: waar verschillen jullie antwoorden?"* Dit is geen bespreking, alleen het zichtbaar maken van waar de twijfel zit. Dat is de opmaat naar blok 2.

7. **Verzamel-moment** (30 sec) — *"Bij welke deelvraag had je de meeste twijfel? Steek je hand op bij kaartkeuze... UCL-berekening... signaal-herkenning... eerste stap."* Tel hardop, schrijf de scores op de flip-over onder de drie koppen. Dit is je input voor blok 3: waar je de meeste aandacht op zet tijdens de handout.

**Materiaal:**
- [ ] wb-01-oefening.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Rekenmachine of telefoon (minstens 1 per 2 deelnemers)
- [ ] Slide 1 (cover) en slide 2 (oefening-intro)
- [ ] Flip-over met de drie koppen Kaart / UCL / Signaal
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Loop tijdens de oefening langs, maar buig je niet over schouders — dat verhoogt prestatiedruk en maakt twijfel onzichtbaar.
> - Als iemand al na 5 minuten klaar is: vraag *"Heb je echt overwogen waarom het geen p of np is? Schrijf dat in één zin op."* De kaartkeuze is de diepste leerstof — wie snel klaar is, heeft vaak de formule gedaan zonder de keuze te onderbouwen.
> - Bij deelnemers die niet weten wat √2,4 is: laat ze een telefoon pakken. Dit is geen rekentoets — het is een keuzetoets.
> - Bewaak de tijd. 11 minuten is krap voor 4 deelvragen — maar de buurman-check en het verzamel-moment zijn de leeropbrengst, niet het volledig afwerken van het blad.

> **🔄 Differentiatie:**
> - **MBO-3 per ongeluk in zaal:** beperk tot deelvragen 1, 2 en 3 (kaart, UCL, signaal). Deelvraag 4 (eerste stap) is optioneel — dat komt uitgebreider in blok 3.
> - **MBO-4 standaard:** alle vier. Geen extra uitdaging nodig.
> - **Teamleider erbij:** geef extra opdracht: *"Schrijf ook in één zin: hoe zou jij in jouw rol bij signaal t=0 betrokken willen worden?"* — voorbereiding op de escalatiediscussie in blok 3.

> **🔴 Valkuil — deelnemer kiest p of np zonder onderbouwing:**
> Veel deelnemers grijpen naar p ("procent defecten — klinkt bekend") of np ("aantal defecten — lijkt logisch"). Niet meteen corrigeren. Laat ze in de buurman-check zelf ontdekken dat ze verschillen. Pas in blok 2/3 verduidelijken: c telt defecten per vaste eenheid, np telt defecte stuks. Eén board kan meerdere soldeerfouten hebben — daarom is het c, niet np.

> **🔴 Valkuil — deelnemer gaat rekenen met spec-grenzen in plaats van c̄:**
> Iemand vraagt "waar is USL?" of rekent met een tolerantie. Stop kort: *"Let op — bij een c-kaart komen de grenzen uit je eigen data, niet van de tekening. UCL is gebaseerd op historisch gemiddelde c̄, niet op een klantgrens. Die verwarring is precies wat lo-spc-107 adresseerde — specs versus control limits."*

---

### 🟣 Blok 2: STARRT-reflectie op een late escalatie
**00:15 - 00:30** | 15 min | Kolb-fase: reflecteren

**Doel:** De deelnemer koppelt de ko-spc-502-casus aan een eigen of waargenomen situatie waarin een materiaal- of kwaliteitsprobleem pas laat werd opgemerkt. De les "escalatie binnen 2 uur beperkt impact tot ~150 boards" landt dan niet als abstract getal maar als concrete eigen ervaring.

**Werkvorm:** Individuele STARRT-reflectie op wb-02 + korte plenaire deel-ronde (alleen de Transfer-stap). Andere stappen blijven persoonlijk — psychologische veiligheid is hier cruciaal.

**Timing-verdeling:** 10 min individueel invullen + 5 min plenair (alleen T — Transfer). De volledige Korthagen-achtige STARRT (S/T/A/R/R/T) mag niet plenair — dat leidt tot schaamte over niet-gehandeld hebben. Alleen de laatste T is vrijwillig plenair.

**Instructie:**

1. **Overgang markeren** (30 sec). Zeg: *"Jullie hebben net geoefend op een fictieve casus. Die is bewust simpel — één punt, 50 boards, duidelijke grens. In de praktijk is het zelden zo helder. We gaan nu één concreet moment terughalen waarop een materiaal- of kwaliteitsprobleem op jouw lijn of de lijn naast je pas laat werd opgemerkt. Geen incident zelf meegemaakt? Een situatie die je hoorde of zag telt ook."*

2. **Deel wb-02-reflectie uit** (30 sec). *"STARRT — zes korte stapjes. De eerste vijf (Situatie, Taak, Actie, Resultaat, Reflectie) blijven van jezelf. Alleen de laatste — de Transfer — mag je straks vrijwillig plenair delen. Als niemand wil delen, ook prima."*

3. **Individueel invullen** (10 min) — zet timer op 10 min. Loop rustig rond. Blijf op afstand, buig je niet over schouders. Bij blokkades: zachte hints:
    - *"Eén moment is genoeg. Welk moment komt als eerste in je op als ik zeg: 'pas na een hele shift werd het opgepakt'?"*
    - *"Geen eigen incident? Iets wat een collega je vertelde, of iets wat je bij een andere ploeg zag — dat mag ook."*
    - *"De R van Reflectie: als er die dag een c-kaart had gehangen met een duidelijke UCL — wanneer had je eigenlijk kunnen handelen?"*
   Bij emotionele reacties (soms komt iemand bij een echte miskleun uit): *"Je hoeft het niet op te schrijven. De reflectie is voor jezelf. Misschien helpt het om de Transfer alvast te formuleren: wat neem je mee naar morgen?"*

4. **Plenaire deel-ronde — alleen T** (4 min) — *"Wie wil in één zin de Transfer delen? Welke concrete stap neem jij deze week op jouw lijn?"* 3-4 deelnemers, max 45 sec per persoon. Vraag niet door op de Situatie — dat was privé. Bevestig alleen: *"Concreet — dat helpt."* of *"Goed dat je aan de teamleider-kant begint."*

5. **Overgang naar blok 3** (30 sec). Wijs naar de flip-over met de drie koppen. *"Jullie hebben net zelf ervaren dat tussen 'iets voelt niet goed' en 'er wordt actie ondernomen' soms uren zitten. We gaan nu precies uittekenen wélke kaart, wélke formule, wélke regel daarbij hoort — en hoe de escalatieketen eruit ziet zodat die uren minuten worden."*

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slide 3 (sectie-slide reflecteren)
- [ ] Slide 4 (STARRT-stappen overzicht)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Stilte verdragen is hier belangrijker dan in de andere blokken. Sommige deelnemers hebben 3 minuten nodig om een moment op te halen. Niet opvullen met extra uitleg.
> - Noem de Transfer-stap in plenair "vrijwillig". Wie niet wil delen, deelt niet. Druk is gif in een reflectie-blok.
> - Deel zelf geen eigen verhaal tijdens dit blok — dat kan bij een intake-blok of afsluiting, niet hier. De reflectie hoort de deelnemer.
> - Schrijf hun Transfer-stappen niet op de flip-over. Die stappen zijn van hen, niet van de groep.

> **🔄 Differentiatie:**
> - **Nieuwe operator (< 6 maanden):** heeft vaak geen eigen incident. Maak expliciet: *"Een situatie die een ervaren collega je vertelde, telt ook. Kijk in de tweede persoon."*
> - **Teamleider:** koppel de R van Reflectie aan de escalatieketen. Vraag: *"Had jij op t=0 of op t=2 geïnformeerd willen worden?"*
> - **Deelnemer die niet wil reflecteren:** bied alternatief. *"Als een moment ophalen niet lukt: schrijf drie dingen op die jij als operator nodig hebt om bij het eerste signaal al door te geven."* Dat geeft dezelfde transferwaarde zonder de biografische laag.

> **🔴 Valkuil — reflectie wordt een klaagronde:**
> Als iemand uitgebreid begint te vertellen over "hoe slecht dit altijd gaat bij ons", stop vriendelijk: *"Goede observatie. Voor de reflectie: wat had jíj toen kunnen doen, en wat ga je deze week doen?"* Verplaats altijd naar eigen actie.

> **🔴 Valkuil — trainer krijgt de neiging tot analyse:**
> Bij een gedeelde Transfer-stap wil je misschien zeggen "maar dan zou ik ook aan batch-ID denken". Niet doen. De Transfer is van de deelnemer. Bevestigen en doorlaten.

---

### 📘 Blok 3: Handout — c vs p vs np, Nelson-regel-1, escalatieketen
**00:30 - 00:45** | 15 min | Kolb-fase: theoretiseren

**Doel:** Het kaartkeuze-schema, de c-kaart-formule, Nelson-regel-1 als statistisch begrip, en de escalatieketen worden expliciet gemaakt. Theorie als bevestiging van wat ze al hebben ervaren — en als naslagwerk voor de werkvloer.

**Werkvorm:** Trainer-geleide handout-bespreking met live koppeling terug naar de oefening van blok 1.

**Instructie:**

1. **Onthul het diagram** (1 min) — verwijder de afdekking van de A3-versie achter in de zaal. Toon slide 7. Zeg: *"Drie dingen op één plaat. Links: de regelkaart die jullie net hebben uitgerekend — c̄ van 2,4, UCL op 7,1, meetreeks 8/6/9. De rode stip op t=0 is Nelson-regel-1. Rechts: de keuzehulp c/p/np/u. Onder: de escalatieketen in vijf stappen. Dit diagram neem je straks mee."*

2. **Deel wb-03-handout uit** (30 sec). *"Pak je markeerstift. Markeer één aha-moment — iets wat voor jou vandaag klikt of dat je niet wist."*

3. **Blok 1 — kaartkeuze c/p/np/u** (4 min) — slide 5. Verwijs direct naar de oefening. *"Jullie moesten kiezen uit c, p, np, u. Wie koos c? Wie koos iets anders?"* Vang de stemming. Als 70%+ c koos: *"Mooi. Laten we vastleggen waarom."* Als < 50% c koos: *"Dat is juist het vakmanschap. Kijk mee."*
    - Gebruik slide 5 met de 2-vraags-beslistabel:
    - **Vraag 1:** tel je *defecten* (een item kan er meerdere hebben) of *defecte stuks* (elk stuk telt 1×)?
    - **Vraag 2:** is je *eenheid* constant (altijd 50 boards) of variabel (soms 30, soms 80)?
    - Schrijf op de flip-over: *"Defecten + constant = c. Defecten + variabel = u. Stuks + constant = np. Fractie + variabel = p."*
    - Koppel terug: *"In onze casus telden jullie soldeerfouten (een board kan er meerdere hebben) per vaste eenheid (50 boards). Dat is c. Niet np, want np zou defecte boards tellen — en dan had één board met vier fouten één defect opgeleverd, niet vier."*
    - Benoem dat de keuze (niet de formule) het vakmanschap is.

4. **Blok 2 — de c-kaart formule + Nelson-regel-1** (4 min) — slide 6. *"De formule is ongemakkelijk eenvoudig. Dat is bewust — want de c-kaart gaat uit van een Poisson-verdeling, en daarin is de standaardafwijking gewoon de wortel van het gemiddelde."*
    - Schrijf op flip-over: **UCL = c̄ + 3√c̄** en **LCL = c̄ − 3√c̄ (bij negatief: 0)**.
    - Werk de casus-getallen uit: *"c̄ = 2,4. √2,4 ≈ 1,549. Drie keer 1,549 is 4,65. UCL = 2,4 + 4,65 ≈ 7,1. LCL = 2,4 − 4,65 = −2,25 — wordt 0."*
    - Leg Nelson-regel-1 uit: *"Eén punt buiten de ±3σ-grenzen. Bij een stabiel Poisson-proces is de kans daarop door puur toeval ongeveer 0,3%. Als je het tóch ziet, is de kans dat er écht iets bijzonders gebeurt vele malen groter dan de kans op pech. Dat is waarom één punt genoeg is om te handelen — je hoeft niet te wachten op een tweede bevestiging."*
    - Verwijs naar bron: *"Dit is de eerste van acht regels uit Nelson's artikel uit 1984 in de Journal of Quality Technology. De andere zeven behandelen we niet vandaag — die gaan over patronen over meerdere punten. Regel 1 is de krachtigste én de makkelijkste."*

5. **Blok 3 — de escalatieketen** (4 min) — slide 8. Wijs op het onderste deel van het A3-diagram. *"Vijf stappen, elk met een tijdsdoel. Dit is geen theorie — dit is de reden dat we vandaag hier staan."*
    - Loop de stappen door:
    - **Stap 1 — teamleider direct (t=0).** *"Direct na het eerste signaal. Niet na het tweede, niet bij de koffiepauze. Direct."*
    - **Stap 2 — boards apart (< 15 min).** *"Jouw rol. Gebeurt op de werkvloer, niet in het kantoor."*
    - **Stap 3 — kwaliteit/engineering + quarantaine (< 1 uur).** *"Teamleider regelt dit. Materiaal gaat fysiek apart."*
    - **Stap 4 — leverancier informeren / batch terugroepen (< 2 uur).** *"Inkoop of kwaliteit. Maar het signaal begon bij jou."*
    - **Stap 5 — productie hervatten met vorige batch (zodra OK).** *"Niet doorgaan met het verdachte materiaal — ook al lijkt het te werken."*
    - Schrijf op de flip-over: **"2 uur = ~150 boards. Hele shift = duizenden."**

6. **Voorwaarde traceerbaarheid** (1 min 30) — slide 9. *"De hele keten werkt alleen als materiaal-traceerbaarheid geregeld is: welke batch is wanneer op welke lijn gegaan, in welke boards verwerkt. Zonder die registratie: Nelson-regel-1 zie je nog steeds, boards apart zetten werkt — maar terugroepen lukt niet, en de leverancier kan niet gericht onderzoeken."*
    - Praktische check: *"Wordt op jouw lijn de batch-ID gekoppeld aan de uur-inspectie? Staat dat in het MES, op papier, of nergens? Vraag dit deze week aan je teamleider — dat is de bonus-transferopdracht."*

7. **Afsluiting + transferopdracht** (1 min) — slide 10. *"Eén opdracht voor deze week. Zoek op jouw eigen lijn één kwaliteitsgrootheid die je per vaste eenheid telt — soldeerfouten per 50 boards, krassen per 100 stuks, foute labels per pallet. Vraag je teamleider naar het gemiddelde over de laatste weken. Reken zelf de UCL uit met c̄ + 3√c̄. Neem dit mee naar de volgende sessie — we bespreken per persoon kort of je UCL realistisch is."*

**Materiaal:**
- [ ] wb-03-handout.md (1 per deelnemer)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] diagram-lo-spc-502.svg — op A3 achter in de zaal én op slide 7
- [ ] Slides 5-10
- [ ] Flip-over voor kaartkeuze-schema en escalatie-tijdsgrenzen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Houd het tempo. 15 minuten is krap voor drie blokken + transfer. Niet vertragen met eigen anekdotes — die bewaar je voor het einde als er tijd over is.
> - Schrijf de UCL-uitkomst (≈ 7,1) groot op de flip-over. Laat staan tot het einde van de sessie — het is het ankergetal.
> - Bij een deelnemer die zegt "wij hebben geen c-kaart op onze lijn": *"Precies de reden dat je dit meeneemt. De UCL bestaat of je hem nu tekent of niet — je kunt hem vandaag zelf uitrekenen."*

> **🔴 Valkuil — trainer gaat dieper op Poisson-statistiek:**
> Een deelnemer vraagt *"waarom precies 3σ, niet 2σ?"* of *"wat is een Poisson-verdeling eigenlijk?"*. Houd het op één zin: *"Drie sigma is de gangbare keuze bij Shewhart-kaarten — dat is wat AIAG, NIST en de meeste kwaliteitsstandaarden volgen. De statistische onderbouwing komt in module 3, of vraag het je kwaliteitsdienst."* Niet dieper. 3σ-onderbouwing is HBO-niveau.

> **🔴 Valkuil — trainer springt naar p- of u-kaart formules:**
> Iemand vraagt *"hoe zit het dan met p of u?"*. Reactie: *"Goede vraag voor module 3. Vandaag blijven we bij c — want dat is de kaart voor de situatie die jullie hebben geoefend. De keuze-beslisregel heb je — de formule voor u of p is een volgende stap."* Schrijf op parkeerflip.

> **🔴 Valkuil — escalatie wordt abstract:**
> Als een deelnemer zegt *"wij kunnen niet zomaar de leverancier bellen"*: niet uitpraten. Vraag: *"Wie kan dat op jouw lijn wel? Noteer die naam op wb-03 onder stap 4."* De keten moet concreet worden voor de eigen werkvloer, niet generiek besproken blijven.

> **🔄 Differentiatie:**
> - **MBO-3:** sla de Poisson-achtergrond volledig over. Leesregel: "De c-kaart-formule is UCL = gemiddelde + 3 × wortel-gemiddelde. Dat is alles."
> - **MBO-4 sneller / teamleider:** noem expliciet de bronnen (AIAG SPC, NIST/SEMATECH sectie 6.3, Nelson 1984). Operators negeren de verwijzingen; teamleiders vinden ze later terug.
> - **Teamleider erbij:** voeg bij de escalatieketen één extra vraag: *"Op jouw lijn — wie is stap 3 en wie is stap 4? Staat dat ergens vast?"* Parkeer voor de groepsreflectie die volgt in module 2.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-oefening.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout.md | n + 2 | A4 dubbelzijdig (3 blokken passen op 1 vel dubbelzijdig) |
| ☐ | diagram-lo-spc-502.svg | 1 | Print A3 in kleur, hang achter in zaal (regelkaart + keuzehulp + escalatieketen) |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Rekenmachine of telefoon | ≥ n/2 | Voor √2,4 ≈ 1,549 — deelnemers mogen eigen telefoon gebruiken |
| ☐ | Flip-over + dikke stiften | 1 set | Voor Kaart/UCL/Signaal-koppen + kaartkeuze-schema |
| ☐ | Timer / mobiel met geluid | 1 | Voor 11-min oefening + 10-min reflectie |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 7 (SVG ingesloten) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel c-kaart oefening

| Deelvraag | Antwoord | Toelichting |
|-----------|----------|-------------|
| 1 — Kaartkeuze | **c-kaart** | Defecten (niet defecte stuks — één board kan meerdere soldeerfouten hebben) per vaste eenheid (50 boards). Niet p (fractie, variabele steekproef), niet np (stuks, constante steekproef), niet u (variabele eenheid). |
| 2 — UCL | **≈ 7,1** | UCL = c̄ + 3√c̄ = 2,4 + 3 × √2,4 = 2,4 + 3 × 1,549 = 2,4 + 4,65 ≈ 7,1. LCL = 2,4 − 4,65 = −2,25 → **afkappen op 0**. |
| 3 — Signaal | **t=0 (8 fouten) ligt boven UCL — Nelson-regel-1. t=1 (6) onder UCL. t=2 (9) opnieuw boven UCL — bevestiging.** | Eén punt buiten ±3σ-grenzen = signaal. Bij stabiel Poisson-proces kans ≈ 0,3% op toeval. |
| 4 — Eerste stap | **Teamleider informeren + boards apart zetten** (in die volgorde, beide binnen 15 min). | NIET: leverancier zelf bellen (stap 4, door inkoop/kwaliteit). NIET: afwachten tot t=1 — Nelson-regel-1 is al op t=0 compleet. |

**Slagingscriterium:** 3 of meer correct = leerdoel behaald (ABCD-degree). Deelvraag 1 (kaartkeuze) is de toetssteen voor het echte vakmanschap — de andere drie volgen uit de formule en de handout.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics — wb-01 en wb-03; wb-02 blijft bij de deelnemer)
- [ ] Twijfel-statistiek genoteerd (bij welke deelvraag was de meeste twijfel?)
- [ ] Kaart-keuze flip-over gefotografeerd (voor module-evaluatie)
- [ ] Notitie voor volgende workshop: welke kwaliteitsgrootheid heeft elke deelnemer gekozen voor de eigen UCL-berekening?
- [ ] xAPI-statements verstuurd: `experienced` (c-kaart oefening), `attempted` (UCL-berekening), `completed` (handout + transfer)
- [ ] Bij teamleider-deelnemers: korte handover naar de groepsreflectie traceerbaarheid en escalatie-verantwoordelijkheid (volgend blok in module 2)
- [ ] Bij emotionele momenten in blok 2: even informeel napraten met deelnemer — zonder inhoudelijk door te vragen

---

*AIMM Curriculum | SPC Module 2 (Train) | Welke kaart, welke bovengrens, welk signaal?*
*Bronnen: AIAG SPC Reference Manual (2nd ed.) — attribuutkaarten en 3σ-conventie | NIST/SEMATECH e-Handbook of Statistical Methods, sectie 6.3.3 (c-chart en Poisson-aanname) | Nelson, L.S. (1984). "The Shewhart Control Chart — Tests for Special Causes." Journal of Quality Technology, 16(4), 237-239. | Fictieve PCB-assemblagecasus, geïllustreerd uit operator-praktijk (ko-spc-502).*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
