# Capability-valkuilen — drie voorwaarden vóór het getal telt — Draaiboek
*SPC Module 3 (Op Maat) | Workshop-blok 45 minuten | 4-8 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer (teamleider MBO-4/HBO) toetst één gerapporteerd capability-getal (Cp/Cpk/Pp/Ppk) uit de eigen werkpraktijk aan de drie voorwaarden (meetsysteem geschikt via Gage R&R/MSA, proces stabiel via SPC-regelkaart, rationele subgroepering), formuleert drie concrete vragen aan de rapporteur en benoemt één maandag-actie. |
| **Bloom-niveau** | Evalueren — een getal kritisch beoordelen aan normen (AIAG MSA, NIST/SEMATECH, Ford PPAP) en onderbouwen of het een beslissing mag sturen. |
| **Doelgroep** | Teamleiders MBO-4 (secundair), teamleiders HBO (primair), 4-8 personen (optimaal 6) |
| **Voorkennis** | ko-spc-301 + ko-spc-302 (Cp/Cpk op hoofdlijnen), ko-spc-109 (rationele subgroepen via voorafgaande module). Deelnemer neemt één gerapporteerd capability-getal mee. |
| **Stadium (H&B)** | Bewust bekwaam — kent Cp/Cpk, heeft getallen gezien, mist kritische toetsings-checklist. |
| **Begeleidingsstijl** | **Coachen** — weinig sturing, veel ondersteuning. Trainer stelt doorvragen, vermijdt formule-college, laat stiltes vallen. |
| **Ruimte** | U-opstelling of tafels voor individueel werk, beamer + scherm, wand voor A3-diagram, ruimte voor eigen kwaliteitsrapporten op tafel |
| **Plek in module** | Workshop content_block 'Capability-getallen kritisch toetsen' — module 3 (Op Maat), ná DMAIC-skeleton (lo-spc-402) en vóór Six Sigma belt-rollen (ko-spc-403) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Theoretiseren — handout drie valkuilen + juiste volgorde | 📘 theoretiseren | 12 min |
| 00:12 - 00:32 | Experimenteren — eigen Cpk-getal toetsen op wb-01 | 🟢 experimenteren | 20 min |
| 00:32 - 00:45 | Reflecteren — STARRT op wb-02 + één-zin deelronde | 🟣 reflecteren | 13 min |

**Totaal:** 45 minuten — geen aparte pauze (dit blok volgt direct op modulepauze).
**Buffer per blok:** 1 min transitie meegerekend; netto activiteitstijd 11/19/12 min. Strakke timing — gong/bel bij elke overgang.
**Plan-B bij tijdsdruk in blok 2:** zie de gele box bij blok 2 — focus op één voorwaarde (de voorwaarde die onbekend is) in plaats van alle drie.

---

## Voorbereiding

### De avond ervoor
- [ ] Print 3 werkbladen × (aantal deelnemers + 2-3 reserve). **wb-01 op A3** (of A4 dubbelzijdig) — wb-02 en wb-03 op A4. Bestandslocatie: `output/learning_objects/trainee/lo-spc-303/werkbladen/`.
- [ ] Print `diagram-lo-spc-303.svg` op A3 in kleur (drie voorwaarden-check + %GRR-drempels). **Check dat het bestand bestaat in `output/learning_objects/trainee/lo-spc-303/`.**
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer.
- [ ] Vraag deelnemers 48 uur vooraf via e-mail om **één gerapporteerd capability-getal mee te nemen** (kwaliteitsrapport, MES-export, klantaudit-dossier, teamdashboard). Stuur één zin mee: *"Fysiek op papier of digitaal maakt niet uit — het moet een echt getal zijn dat nu ergens een beslissing kan sturen."*
- [ ] Lees de **fictieve case** uit het kennisobject nog één keer door (lijnmanager claimt Cpk = 1,5; drie vragen onthullen drie onbekenden) — dit is je enige toegestane illustratie. Vermijd bewust andere voorbeelden.
- [ ] Markeer voor jezelf in wb-03 welke passages je wilt aanhalen tijdens blok 1 (centrale zin, %GRR-tabel, fictieve case).
- [ ] Check de doelgroep: zijn er deelnemers met een automotive-achtergrond (Ford PPAP-ervaring)? Dat wordt je doorverwijs-anker bij vragen over audit-eisen.

### Het uur ervoor
- [ ] Hang de A3-versie van `diagram-lo-spc-303.svg` zichtbaar achter in de zaal.
- [ ] Leg per stoel: pen, markeerstift, `wb-03-handout.md` (bovenop), `wb-01-eigen-analyse.md` eronder, `wb-02-reflectie.md` eronder. De volgorde = de volgorde waarin ze worden gebruikt.
- [ ] Houd een stapel blanco A4 apart voor deelnemers die geen eigen getal bij zich hebben (plan-B: dan gebruiken ze de fictieve case uit wb-03).
- [ ] Open slide 1 op het scherm.
- [ ] Zet een 'parkeerflip' klaar voor vragen over formules, statistische details, meetsysteem-implementatie — alles wat buiten de toetsings-scope valt.

---

## Blok-details

### 📘 Blok 1: Theoretiseren — handout drie valkuilen + juiste volgorde
**00:00 - 00:12** | 12 min (incl. transitie) — netto 11 min | Kolb-fase: theoretiseren

**Doel:** De drie valkuilen (meetsysteem / stabiliteit / subgroepering) en de juiste volgorde (MSA → stabiliteit → verdeling → capability) herkenbaar maken. Deelnemers markeren in de handout welke valkuil zij herkennen van eigen lijn. Klaar om eigen getal tegen de drie voorwaarden te leggen.

**Werkvorm:** **Coachend doorlopen** van wb-03-handout.md. Jij stelt per valkuil één herkennings-vraag; deelnemers markeren. Diagram op A3 + slide 3 als anker. Maximaal 4 slides — de handout doet het werk.

**Pedagogische lijn:** dit is de eerste 12 min van een 45-min coaching-blok. Vermijd de instrueerstijl ('ik leg de formules uit'). De doelgroep (teamleider MBO-4/HBO, bewust bekwaam) kent Cp/Cpk al — jouw rol is de drie voorwaarden blootleggen en eigen ervaring mobiliseren. Geen formules op het bord.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1 (cover). Zeg: *"Welkom. In module 3 werken jullie aan eigen lijnen. Vorig blok de DMAIC-skeleton — vandaag één scherpe vraag: als er straks op jouw bureau 'Cpk = 1,5' verschijnt, weet je dan of dat getal een beslissing mag sturen? Ik ga jullie vandaag weinig vertellen — de meeste vragen zijn aan jullie."*

2. **Trigger — de drie valkuilen** (1,5 min) — toon slide 2 (Cpk = 1,5 — klinkt goed. Maar…). Stel coachende vraag: *"Wie heeft ooit een Cpk-getal gezien waarvan je achteraf dacht: dat klopte niet?"* Wacht. Tel innerlijk tot 7. Vang 1-2 antwoorden. Bevestig: *"Precies — de vraag vandaag is hoe je dat ontdekt vóór de beslissing valt, niet erna."* Niet meer.

3. **Deel wb-03-handout uit** (30 sec). *"Pak je markeerstift. Markeer wat je herkent van je eigen lijn, markeer ook wat nieuw voor je is. We lopen samen door de drie valkuilen en de volgorde. Niets uit je hoofd leren — dit is naslag."*

4. **Drie valkuilen samen doorlopen** (6 min — ~2 min per valkuil) — toon slide 3 (drie-voorwaarden-overzicht, verwijst naar A3-diagram achter in zaal). **Coachende werkvorm:** per valkuil begint de groep met herkenning.

    - **Valkuil 1 — Instabiel proces** (~2 min). Vraag: *"Wanneer werd op jouw lijn een capability berekend zonder eerst de regelkaart te checken?"* Wacht 5-7 sec. Vang één antwoord. Bevestig en noem de bron: *"NIST/SEMATECH: capability-formules zijn alleen geldig op een statistisch stabiel proces."* Wijs naar de handout.

    - **Valkuil 2 — Slechte subgroepering** (~2 min). Vraag: *"Op jouw lijn — hoe waren de subgroepen samengesteld toen de laatste Cpk werd berekend?"* Als niemand het weet: *"Precies het punt. Als de subgroep-strategie onbekend is, is Cpk ook onbekend."* Noem kort: *"AIAG: rationele subgroepen — zelfde omstandigheden, dicht in tijd, één bron. Terug naar ko-spc-109."*

    - **Valkuil 3 — Slecht meetsysteem** (~2 min). Toon slide 4 (%GRR-drempels). Vraag: *"Wie weet hier de laatste Gage R&R-datum van het meetsysteem op zijn lijn?"* Houd de stilte. Bevestig het ongemak: *"Dit is het punt. Ford PPAP eist Gage R&R expliciet vóór capability — geen suggestie, automotive-audit-vereiste. %GRR < 10 % is geschikt, 10–30 % marginaal, > 30 % niet bruikbaar. AIAG MSA 4e editie."*

5. **De juiste volgorde** (2 min) — toon slide 5 (stroomschema). Verwijs naar A3-diagram achter in zaal. *"Vier poortjes: MSA → stabiliteit → verdeling → capability. Elke poort overgeslagen = elke beslissing daarna minder onderbouwd. De fictieve case in je handout: iemand claimt Cpk = 1,5 — drie vragen onthullen dat alle drie de poortjes niet gecheckt zijn. Je gaat zo hetzelfde doen met jouw eigen getal."*

6. **Overgang naar blok 2** (1 min) — toon slide 6. *"Tot zover de structuur. Nu de echte vraag: jouw eigen getal. Pak wb-01 uit je stapeltje. Laat wb-03 open op tafel als naslag."*

**Materiaal:**
- [ ] `wb-03-handout.md` (1 per deelnemer + 2 reserve)
- [ ] Markeerstift per deelnemer
- [ ] `diagram-lo-spc-303.svg` op A3 (achter in zaal) + op slide 3 en 4
- [ ] Slides 1-6 (max 6 — geen aparte formule-slides; de handout doet dat werk)
- [ ] Timer (innerlijk — 2 min per valkuil)

> **💡 Tips voor de trainer:**
> - Houd het tempo. 11 min netto is krap voor drie valkuilen + volgorde — daarom samen doorlopen, niet doceren. De groep doet het herkennings-werk, jij bevestigt en noemt de bron.
> - De fictieve case is je enige toegestane illustratie. Markeer als je hem aanhaalt: *"Dit is een fictieve case ter illustratie — niet uit één specifiek bedrijf."* Consistent met hoe hij in wb-03 staat.
> - Stiltes zijn je vriend. Tel innerlijk tot 7 na elke vraag. Teamleiders die geen Gage R&R-datum weten vinden het ongemakkelijk — laat dat ongemak werken. Het ongemak = het leermoment.
> - Vermijd formule-college. Geen herleidingen van σ_binnen vs σ_totaal op het bord. Wie dat wil: verwijs naar wb-03 "Vakjargon kort uitgelegd" voor zelfstudie.

> **🔴 Valkuil — trainer schiet in formule-modus:**
> Iemand vraagt *"Hoe bereken je eigenlijk %GRR?"* of *"Wat is het verschil tussen Pp en Cp precies?"*. Verleidelijk om dat uit te leggen. Niet doen. *"Goede vraag — de formule staat in wb-03 onder Vakjargon. Vandaag gaan we het beoordelings-denken trainen, niet de rekenkunde. AIAG MSA 4e editie is je naslag voor de formule."* Parkeerflip.

> **🔴 Valkuil — deelnemer zegt: "Wij doen altijd Gage R&R, dit is niet van toepassing":**
> Vraag door: *"Wanneer was de laatste studie op de meter die dit getal heeft geproduceerd? En wat was het %GRR?"* Negen van de tien keer is het antwoord onbekend. Bevestig zonder schaamte: *"Dat is precies het punt — 'wij doen altijd' betekent niets als je het niet per studie kunt aantonen."*

> **🔄 Differentiatie:**
> - **Teamleider MBO-4 zonder audit-ervaring:** noem expliciet dat 'onbekend' een geldig en veilig antwoord is. Onbekend = iets om uit te zoeken, geen tekortkoming.
> - **Deelnemer met automotive-achtergrond (Ford PPAP-ervaring):** gebruik deze persoon als resource. *"Hoe werkt dit in jouw PPAP-dossiers?"* — maar houd het kort (30 sec), geen uitwijding.

---

### 🟢 Blok 2: Experimenteren — eigen Cpk-getal toetsen
**00:12 - 00:32** | 20 min (incl. transitie) — netto 19 min | Kolb-fase: experimenteren

**Doel:** De deelnemer past de drie voorwaarden toe op één concreet gerapporteerd capability-getal uit de eigen werkpraktijk. Per voorwaarde: ja / nee / onbekend + bron + kritische vraag aan de rapporteur. Aan het eind: drie concrete vragen + één maandag-actie.

**Werkvorm:** Individueel werk op wb-01-eigen-analyse (A3 of A4 dubbelzijdig). Trainer loopt rond, stelt **doorvragen** (geen instructies, geen oplossingen). Drie-zinnen-aanpak bij blokkades.

> **🟡 Plan-B bij tijdsdruk of bij deelnemer zonder eigen getal**
>
> **Scenario A — tijdsdruk:** na 10 min visuele check. Als meer dan de helft nog bij voorwaarde 1 hangt, kondig aan: *"Even bijschakelen. Focus op de voorwaarde die voor jouw getal het meest onbekend is — de andere twee kun je na de sessie afmaken. Liever één voorwaarde scherp dan drie vaag."* Dat scheelt 4-5 min.
> **Scenario B — geen eigen getal meegebracht:** zeg individueel: *"Pak de fictieve case uit wb-03 als werkmateriaal. Zelfde stappen, maar op papier. Je neemt de leer-beweging mee, niet het concrete antwoord."* Werkt ook als fallback voor deelnemer die later aanschuift.

**Instructie:**

1. **Deel wb-01-eigen-analyse uit** (30 sec) — of bevestig dat het al op tafel ligt. Zeg: *"Eén capability-getal. Drie voorwaarden. Per voorwaarde: wat weet ik, wat weet ik niet, welke bron bevestigt het, welke vraag stel ik aan de rapporteur. Onbekend invullen mag — dat is zelfs de hele les."*

2. **Kies-moment** (1 min) — toon slide 7 (wb-01-instructie). *"Eerste keuze: welk getal? Het getal dat je hebt meegebracht. Als je meerdere hebt — kies het getal waar de belangrijkste beslissing van afhangt. Schrijf bovenaan: welk getal, uit welke bron, welke beslissing."* Wacht 45 sec.

3. **Analyse invullen** (15 min) — zet timer op 15 min. *"Werk top-down: voorwaarde 1 (meetsysteem), dan 2 (stabiliteit), dan 3 (subgroepering). Per voorwaarde: kruis aan, bron, vraag aan rapporteur. Eindig met de samenvatting en de maandag-actie. Pen niet stilleggen."* Loop rond.

   **Wat je doet als trainer (kerntaak van dit blok):**
   - Loop rond. Buig je niet over schouders — dat verhoogt prestatiedruk.
   - Lees stiekem mee. Bij stagnatie: stel **één doorvraag** uit de bibliotheek hieronder per voorwaarde. Niet meer dan één per bezoek.
   - **Geef geen oplossingen.** Geen 'in mijn praktijk doen we...'. Geen 'de vuistregel is...'. Vervang elke neiging tot voorbeeld door een vraag.
   - Bij blokkades — drie-zinnen-aanpak: één doorvraag → wacht 5 sec → bevestig wat de deelnemer al heeft → stilte.

4. **Halverwege-signaal** (30 sec) — bij 7,5 min, sla zachtjes op de tafel. *"Halverwege. Even kijken: heb je alle drie de voorwaarden aangeraakt — ook al staat er 'onbekend' bij twee? Als voorwaarde 3 (subgroepering) nog leeg is, ga er nu naartoe. Voorwaarde 3 wordt het vaakst vergeten."*

5. **Eindsignaal** (30 sec) — bij timer-stop. *"Pen neer. Check: heb je drie vragen voor de rapporteur geformuleerd, en één maandag-actie? Die twee dingen zijn het harde resultaat van dit blok. Laat wb-01 open liggen — je hebt het zo bij de reflectie nodig."*

**Materiaal:**
- [ ] `wb-01-eigen-analyse.md` (A3 of A4 dubbelzijdig, 1 per deelnemer + 3 reserve)
- [ ] `wb-03-handout.md` als referentie (al bij deelnemer, blijft open)
- [ ] Eigen gerapporteerd capability-getal (meegebracht — fysiek of digitaal)
- [ ] Pen + markeerstift per deelnemer
- [ ] Slide 7 (wb-01-instructie)
- [ ] Timer (15 min, halverwege-signaal bij 7,5 min)
- [ ] A3-diagram achter in zaal (blijft hangen)

**Doorvragen-bibliotheek per voorwaarde** *(kies er één per bezoek — niet opstapelen)*

- **Voorwaarde 1 (Meetsysteem) — blokkade onbekend %GRR:**
  - *"Wie heeft de meter die dit getal heeft geproduceerd voor het laatst gekalibreerd of geValideerd?"*
  - *"Als ik je morgen vraag: laat het Gage R&R-rapport zien — waar moet je zijn?"*
  - *"Is het systeem veranderd sinds de laatste studie — andere meter, andere operator, andere software?"*

- **Voorwaarde 2 (Stabiliteit) — blokkade geen regelkaart:**
  - *"Over welke periode is dit getal berekend? En: was er over dezelfde periode een SPC-kaart draaiend?"*
  - *"Stel je kijkt de regelkaart terug over die periode — ga je runs zien? Trends? Punten buiten de grenzen?"*
  - *"Als het proces wél instabiel was: wat zou dat betekenen voor dit getal?"*

- **Voorwaarde 3 (Subgroepering) — blokkade subgroepen onbekend:**
  - *"Hoeveel metingen per subgroep, hoe vaak per dag, over welke bron (één machine, één caviteit)?"*
  - *"Als je vier caviteiten door elkaar hebt gemeten: wat zit er dan in σ_binnen dat er eigenlijk niet thuishoort?"*
  - *"Waar staat de subgroep-definitie gedocumenteerd — SPC-plan, control plan, nergens?"*

> **💡 Tips voor de trainer:**
> - Dit is je belangrijkste blok als coach. Het verschil tussen een trainer-die-formules-uitlegt en een coach-die-vragen-stelt wordt hier zichtbaar. Hou jezelf in.
> - Wat doe je als een wb-01 leeg blijft na 5 min? Loop ernaartoe. Vraag: *"Welke voorwaarde is voor jouw getal het meest onduidelijk — meet, stabiliteit of subgroep?"* Dat is altijd één van de drie. Werk 1 minuut samen, geef de pen terug.
> - Wat doe je als iemand alle drie op "ja" zet binnen 5 min? Vraag: *"Bron per voorwaarde — waar staat het Gage R&R-rapport, waar ligt de regelkaart-uitdraai, waar staat de subgroep-definitie gedocumenteerd?"* Dat is de bron-check. Negen van de tien keer verschuift minstens één "ja" naar "onbekend".
> - Wat doe je als iemand vraagt "is dit %GRR oké?"? Verwijs naar slide 4 of wb-03 tabel. *"AIAG zegt: < 10 % geschikt, 10-30 % marginaal, > 30 % niet geschikt. Wat zegt het over jouw getal?"* Laat de deelnemer het oordeel vellen.

> **🔴 Valkuil — deelnemer schrijft overal "ja" zonder bron:**
> Op het werkblad staan drie vinkjes bij "ja", geen enkele bron ingevuld. Vraag: *"Waar zou je naartoe moeten om elk 'ja' hard te maken?"* Maak onderscheid tussen 'ik geloof dat het goed zit' en 'ik kan het aantonen'. Niet beoordelen — laat de deelnemer zelf het verschil voelen.

> **🔴 Valkuil — deelnemer weigert "onbekend" in te vullen:**
> Je ziet aarzeling, uiteindelijk vinkt deelnemer "ja" aan zonder overtuiging. Vraag: *"Als je het zeker weet, welke bron bewijst het? Als die er niet is, is 'onbekend' het eerlijke antwoord. Dat is geen tekortkoming — dat is het startpunt voor de maandag-actie."*

> **🔴 Valkuil — deelnemer springt naar "nieuwe meter kopen":**
> Bij twijfel meetsysteem roept iemand *"Dan moeten we een nieuwe schuifmaat"*. Vraag: *"Wacht — weet je zeker dat het de meter is? Wat zou een Gage R&R-studie eerst onthullen? Is het Repeatability of Reproducibility?"* Verwijs kort naar wb-03 en naar ko-spc-303-kernpunt: investering naar de verkeerde plek is precies het gevaar van capability-zonder-MSA.

> **🔴 Valkuil — deelnemer wil alleen formule-antwoord:**
> *"Geef me gewoon de formule voor %GRR dan reken ik het zelf uit."* Vriendelijk: *"De formule staat in wb-03 en in de AIAG MSA-manual. Vandaag trainen we het beoordelings-denken, niet de rekenkunde. Is het rapport dat je meebracht berekend volgens AIAG MSA 4e? Dat is de vraag."*

> **🔄 Differentiatie:**
> - **Teamleider MBO-4:** loop bewust eerst langs in de eerste 5 min. Drie doorvragen achter elkaar bij voorwaarde 1: *"Welke meter heeft dit getal geproduceerd?"*, *"Wie is de meter-eigenaar?"*, *"Waar zou een Gage R&R-rapport liggen als het bestaat?"* Drie zinnen. Dan weglopen.
> - **Deelnemer met automotive-achtergrond:** vraag bij de samenvatting of zijn getal PPAP-klaar zou zijn. Als antwoord "nee" is: *"Welke voorwaarde zou een auditor als eerste aankaarten?"* Dat maakt het realistisch.

---

### 🟣 Blok 3: Reflecteren — STARRT + één-zin deelronde
**00:32 - 00:45** | 13 min (incl. transitie) — netto 12 min | Kolb-fase: reflecteren

**Doel:** Individuele STARRT-reflectie op wat de analyse opleverde (welke voorwaarde bleek onbekend, welke beslissing stond op het spel, wat verandert structureel). Afsluitend: één zin plenair per deelnemer — de maandag-actie.

**Werkvorm:** Individueel wb-02-reflectie invullen (STARRT-structuur). Daarna plenaire deel-ronde van één zin per persoon. Trainer modelleert door zelf te beginnen.

**Instructie:**

1. **Deel wb-02-reflectie uit** (30 sec) — of bevestig dat het op tafel ligt. *"STARRT — zes velden. Situatie, Taak, Actie, Resultaat, Reflectie, Transfer. Kort en concreet. Eindig met de maandag-actie op de laatste pagina. Dat is de zin die je zo plenair uitspreekt."*

2. **Individueel schrijven** (9 min) — zet timer op 9 min. *"Individueel werk, geen gesprek. De kernvragen op het werkblad zijn je gids. Belangrijkste vragen: welke voorwaarde bleek 'onbekend', welke beslissing hing af van dit getal, en wat ga je maandag anders doen. Pen niet stilleggen."* Loop rustig rond, kijk niet mee — geef rust.

3. **Plenaire één-zin-ronde** (3 min bij 6 deelnemers, 4 min bij 8) — bel/gong. *"Pen neer. Plenair rondje. Eén zin per persoon: wat ga je maandag anders doen — concreet, met naam en datum. Ik begin."*
    - Trainer eerst, één zin als voorbeeld: *"Maandag stuur ik één collega een bericht: 'kun jij het Gage R&R-rapport opsturen van de meter waar Cpk X op is berekend?' — dat is mijn maandag-actie als ik hier was."*
    - Dan kring rond. Knik naar volgende. Bij twijfelaar: *"Wie volgt vrijwillig?"* — niet aanwijzen.
    - Strak: 15 sec per persoon, geen reactie, geen vervolgvraag.

4. **Afsluiting** (30 sec) — slide 10. *"Wat jullie net hebben gedaan: één echt getal langs drie voorwaarden leggen. Dat is het verschil tussen getallen napraten en er grip op hebben. Neem wb-01 mee — maandag-actie onderaan is het werkdocument voor deze week. Volgende blok in module 3: Six Sigma belt-rollen — wie heb je nodig om een MSA of DMAIC goed uit te voeren."*

**Materiaal:**
- [ ] `wb-02-reflectie.md` (A4, 1 per deelnemer + 2 reserve)
- [ ] `wb-01-eigen-analyse.md` (ingevuld, blijft bij deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 8-10 (reflectie-overgang + maandag-actie + afsluiter)
- [ ] Timer + bel/gong (9 min schrijven + 15 sec per persoon in deel-ronde)

> **💡 Tips voor de trainer:**
> - Bewaak rust tijdens het schrijven. STARRT is individueel — weersta de neiging om te coachen tijdens dit blok. Coaching was blok 2.
> - De één-zin-deelronde is geen feedback-ronde. De waarde zit in commitment (uitspreken = vasthouden) en exposure (horen wat anderen doen). Geen reacties op elkaar — dat is volgende-sessie-materiaal.
> - Je begint zelf. Modelleert de kortheid. Eén zin, niet drie. Als jij uitwijdt, wijdt de groep uit.
> - De maandag-actie mag "klein" zijn. *"Maandag bel ik X"* is prima. *"Maandag lanceer ik een kwaliteitssysteem-revisie"* is vermoedelijk te groot voor een maandag-actie.

> **🔴 Valkuil — STARRT wordt een feedbackronde:**
> Iemand begint hardop na te denken, een ander reageert, een gesprek ontstaat. Onderbreek vriendelijk: *"STARRT is individueel schrijven — straks één zin plenair. Nu even rust voor de pen."*

> **🔴 Valkuil — één-zin-ronde wordt drie-zinnen-ronde:**
> Deelnemer begint uit te leggen waarom de maandag-actie is wat het is. Zacht handgebaar bij 15 sec. *"Dank — volgende."* Niet onderbreken mid-zin, wel strak na de zin. Ritme = boodschap: één zin is genoeg.

> **🔴 Valkuil — deelnemer heeft geen maandag-actie:**
> *"Ik weet het nog niet."* Vraag: *"Wat is de kleinste stap die je morgen nog kunt zetten? Bellen, mailen, vragen, opvragen — niet oplossen, één stap."* Accepteer een hele kleine actie. Kleine actie die gebeurt > grote actie die niet gebeurt.

> **🔄 Differentiatie:**
> - **Onzeker / nieuw:** bevestig vooraf dat 'ik vraag het Gage R&R-rapport op bij kwaliteit' een perfecte maandag-actie is — juist omdat het klein en concreet is.
> - **Deelnemer met automotive-achtergrond:** vraag of de maandag-actie PPAP-proof is. Dat legt een hogere lat zonder hem expliciet op te leggen aan de anderen.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | `wb-03-handout.md` | n + 2 | A4 dubbelzijdig — drie valkuilen + volgorde + %GRR-tabel + fictieve case |
| ☐ | `wb-01-eigen-analyse.md` | n + 3 | **A3 enkelzijdig of A4 dubbelzijdig** — drie voorwaarden + vragen + maandag-actie |
| ☐ | `wb-02-reflectie.md` | n + 2 | A4 — STARRT-format |
| ☐ | `diagram-lo-spc-303.svg` | 1 | **Print A3 in kleur**, hang achter in zaal (drie voorwaarden + %GRR-drempels) |
| ☐ | Markeerstiften | n | Voor wb-03-markeren + wb-01-invullen |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Timer / mobiel met geluid | 1 | Voor 15 min wb-01 + 9 min wb-02 + 15 sec per persoon deelronde |
| ☐ | Bel of gong | 1 | Voor halverwege-signaal + deel-ronde-signaal |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 3 (drie voorwaarden) en slide 4 (%GRR) zijn centraal |
| ☐ | `presentatie.slidev.md` geopend | 1 | In presenter-modus voor speaker notes |
| ☐ | Parkeerflip + dikke stift | 1 | Voor formule-vragen, implementatie-vragen, audit-detailvragen |
| ☐ | Stapel blanco A4 | 5 | Voor deelnemers zonder eigen getal — fallback op fictieve case |
| ☐ | Naamkaartjes (indien vreemd aan elkaar) | n | Coaching per naam werkt beter |

n = aantal deelnemers

---

## Snel-overzicht drie voorwaarden + doorvragen

> Dit is je vangrail. Geen 'goed/fout antwoord' — wel: welke vraag stel je aan een teamleider die hier blijft hangen?

| Voorwaarde | Norm | Belangrijkste valkuil | Eerste doorvraag |
|-----------|------|----------------------|------------------|
| **1. Meetsysteem** | AIAG MSA: %GRR < 10 % geschikt, 10-30 % marginaal, > 30 % niet geschikt. Ford PPAP eist MSA vóór capability. | Geen recent Gage R&R-rapport | *"Wanneer was de laatste Gage R&R op de meter die dit getal heeft geproduceerd?"* |
| **2. Stabiliteit** | NIST/SEMATECH: capability alleen geldig op statistisch stabiel proces (SPC-kaart geen signalen). | Geen regelkaart over meetperiode | *"Was er over dezelfde periode een SPC-kaart draaiend? Wat toonde die?"* |
| **3. Subgroepering** | AIAG / ko-spc-109: rationele subgroepen — één bron (machine/caviteit/shift/recept), dicht in tijd. | Vermengde subgroepen (meerdere caviteiten per subgroep) | *"Één bron per subgroep — zelfde machine, caviteit, shift, recept? Waar is dat gedocumenteerd?"* |

**Fictieve case-anker (enige toegestane illustratie):** lijnmanager claimt Cpk = 1,5. Teamleider stelt drie vragen: *was het stabiel?* (geen regelkaart), *hoe waren de subgroepen?* (vier caviteiten vermengd), *is MSA gedaan?* (standaard schuifmaat, geen Gage R&R). Conclusie: het getal kan correct zijn, maar zonder antwoord op deze drie vragen weet niemand het. Eerst valideren, dan beslissen. **Markeer altijd expliciet dat dit een fictieve case is** — niet uit één specifiek bedrijf.

---

## Checklist na de sessie

- [ ] Alle wb-01-werkbladen gefotografeerd (met toestemming, voor learning analytics + eigen evaluatie)
- [ ] Welke voorwaarde bleek bij de groep het vaakst 'onbekend'? (Input voor volgende sessie — als "3. Subgroepering" structureel onbekend is, is er een gap in module 1-2)
- [ ] Welke maandag-acties zijn opgeschreven? (Lijstje voor opvolg-coaching of volgende sessie)
- [ ] Parkeerflip-vragen overgedragen aan trainer van volgend blok (ko-spc-403, Six Sigma belt-rollen)
- [ ] xAPI-statements verstuurd: `experienced` (wb-03 gemarkeerd), `attempted` (wb-01 eigen-analyse ingevuld), `completed` (wb-02 STARRT ingevuld + maandag-actie uitgesproken)
- [ ] Korte handover naar trainer van volgende blok: welke deelnemers hadden geen eigen getal (mogelijk voorkennis-gap), welke vroegen naar formules (mogelijk content-verdiepings-behoefte), welke hadden automotive-achtergrond (resource voor audit-vragen)

---

*AIMM Curriculum | SPC Module 3 (Op Maat) | Capability-valkuilen — drie voorwaarden vóór het getal telt*
*Bronnen: ko-spc-303 | NIST/SEMATECH e-Handbook of Statistical Methods — Process Capability | AIAG Measurement Systems Analysis Reference Manual (4th ed.) | Ford Production Part Approval Process (PPAP 4th edition) | Minitab Process Capability Documentation*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
