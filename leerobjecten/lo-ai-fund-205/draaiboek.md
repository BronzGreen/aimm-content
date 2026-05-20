# Data labelen op de werkvloer — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan zelf trainingsdata labelen volgens vier principes, meet inter-rater agreement (inter-beoordelaar-overeenkomst) met een collega, herkent twee van vier valkuilen, en maakt een mini-labelschema voor de eigen werkvloer. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 afgerond + lo-ai-fund-132 (trainingsdata-kwaliteit) + lo-ai-fund-117 (supervised vs unsupervised) |
| **Stadium (Hersey & Blanchard)** | Bewust bekwaam — theorie van trainingsdata bekend (Module 1), handeling nog niet zelf gedaan |
| **Begeleidingsstijl (manier van begeleiden)** | Coachen — hoge relatiegerichtheid, lagere taakgerichtheid; vragen-stellen i.p.v. antwoord-geven |
| **Ruimte** | U-opstelling of clusters van 4 (buurman moet naast deelnemer kunnen zitten), beamer + scherm, flip-over of bord |
| **Plek in module** | Eerste hands-on LO van Module 2 (Train). Brengt Module-1-theorie (kwaliteit > hoeveelheid) tot operationeel meetbaar gedrag. |
| **Bloom-niveau** | Toepassen — labelen + meten + mini-schema maken |
| **Kirkpatrick-niveau** | Gedrag — concrete actie deze week op de eigen lijn |

---

## Sessie-overzicht

| Tijd | Activiteit | Type (Kolb-fase / leerfase) | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Eerste labelsessie — 20 voorbeelden | 🟢 ervaren | 12 min |
| 00:12 - 00:22 | Buurman-vergelijking + inter-rater agreement | 🟣 reflecteren | 10 min |
| 00:22 - 00:35 | Handout vier principes + vier valkuilen | 📘 theoretiseren | 13 min |
| 00:35 - 00:45 | Eigen mini-labelschema + valkuil + actie | 🟠 experimenteren | 10 min |

**Totaal:** 45 minuten.
**Buffer:** 1 min per blok flexibel (kan opgenomen worden in fase 3 of fase 4).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve per werkblad. **Of** kies digitaal voor wb-04 aanvulling: laad `model-label-valkuilen.jsx` op een React-sandbox en test op één tablet.
- [ ] Test de Slidev-presentatie (`lo-ai-fund-205-presentatie.slidev.md`) op de beamer.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `DataLabelenVideo`, ~91s, 5 scenes) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4. Plan inzet in fase 3 (theoretiseren) bij de handout-uitleg.
- [ ] Flip-over of bord — boven aan een kolom-rij voorbereiden voor fase 2 met drie kopjes: **Verschil 1 / Verschil 2 / Verschil 3**.
- [ ] Tweede bord-veld zichtbaar: kernzin *"Verschillen = schema-signaal, geen storing"*. Niet vooraf opschrijven — pas in fase 2 onthullen.
- [ ] Lees voorbeeld 1 van wb-01 een keer hardop voor jezelf. Dat is je IK DOE in fase 1.

### Het uur ervoor
- [ ] Leg per stoel klaar: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel — deze deel je in elke fase opnieuw uit.
- [ ] Open slide 1 in presenter-modus.
- [ ] Zet stoelen zo dat elke deelnemer een buurman naast zich heeft (geen blokken van één).

---

## Blok-details

### 🟢 Blok 1: Eerste labelsessie — 20 voorbeelden
**00:00 - 00:12** | 12 min | Kolb-fase (leerfase): ervaren

**Doel:** Deelnemer labelt voor het eerst zelf 20 voorbeelden volgens een vooraf-gedefinieerd schema. Ervaart aan den lijve dat een schema met drie labels (GOED / TWIJFEL / AFGEKEURD) niet vanzelf eenduidig is — vooral bij grensgevallen.

**Werkvorm:** Plenaire opening (2 min), IK DOE-modellering op voorbeeld 1 (2 min), individueel labelen voorbeelden 2-20 (8 min).

**Instructie:**

1. **Open de sessie** (2 min) — toon slide 1. Zeg: *"De komende 45 minuten gaan jullie zelf labels zetten. In Module 1 leerden jullie dat kwaliteit van trainingsdata zwaarder weegt dan hoeveelheid. Vandaag doe je het zelf. Aan het eind heb je een mini-labelschema voor je eigen lijn en weet je hoe je meet of jij en een collega het eens zijn."* Pauze 5 seconden.

2. **Werkblad uitdelen + schema lezen** (1 min) — deel wb-01 uit. Toon slide 2 met het labelschema. Lees hardop:
   - *"GOED — geen zichtbaar defect op het zichtvlak."*
   - *"TWIJFEL — defect kleiner dan 1 mm, of buiten het zichtvlak."*
   - *"AFGEKEURD — zichtbaar defect groter dan 1 mm op het zichtvlak."*

3. **IK DOE — voorbeeld 1 hardop** (2 min) — toon slide 3 met voorbeeld 1. Zeg langzaam: *"Voorbeeld 1 doe ik hardop voor. Lees met me mee. 'Matzwart oppervlak, één lichte streep van 2 mm aan de rand, geen oneffenheid op het zichtvlak.' Wat doe ik? Eerst de grens-vraag: zit het defect op het zichtvlak? Nee — aan de rand. Tweede grens-vraag: hoe groot? 2 mm. Voor mij is dit TWIJFEL — buiten zichtvlak telt licht, maar 2 mm is niet klein. Een collega zou GOED kunnen kiezen omdat het niet op zichtvlak zit. Beide zijn verdedigbaar. Daarom maken we straks de buurman-vergelijking."*

4. **Zelfstandig labelen 2-20** (6 min) — toon slide 4. Zet timer op 6 minuten. Zeg: *"Nu jullie. Voorbeelden 2 tot en met 20. Twijfel mag — zet een vraagteken in de kantlijn als je tussen twee labels schiet. Een vraagteken is geen fout; het is een vraag voor fase 2."* Loop rond na 2 minuten.

5. **Coachen tijdens rondloop** (lopend) — bij vastlopers GEEN antwoord; alleen grens-vragen:
   - *"Welke grens uit het schema gebruik je hier?"*
   - *"Wat zou je beslissen als je dit op je eigen lijn zag?"*
   - *"Zit het defect op het zichtvlak of erbuiten?"*

6. **Afronden + brug** (1 min) — slide 5. Zeg: *"Wie heeft minimaal 18 van de 20 ingevuld?"* Tel handen. *"Niemand hoeft zijn labels te delen. Eerst je buurman."*

**Materiaal:**
- [ ] Slides 1-5
- [ ] wb-01-eerste-labelsessie.md (1 per deelnemer)
- [ ] Pen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke open vraag. Stilte is je vriend.
> - Geef GEEN labels in fase 1. Anders verliest fase 2 zijn betekenis.
> - Een deelnemer die heel snel klaar is: vraag *"Bij welk voorbeeld twijfelde je?"* — niet *"Welke had jij gekozen?"*

> **🔴 Valkuil — trainer geeft te snel de 'juiste' labels:**
> Coachen, niet doceren. Bij elke vraag een wedervraag uit het schema. Het hele leerproces hangt op het zelf-worstelen. Als jij voorbeeld 7 als GOED bevestigt, kalibreren alle deelnemers stilletjes op jouw norm en zijn de verschillen in fase 2 kunstmatig laag.

> **🔴 Valkuil — twijfel framen als zwak:**
> Sommige operators willen 'zeker' zijn. Normaliseer plenair: *"Twijfel mag — vraagteken in de kantlijn. Dat is een vraag voor fase 2, geen fout."*

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Extra tijd voor het lezen van de werkbladtekst. Bij vastlopers: ga één voorbeeld samen na — niet door het antwoord te geven, maar door de grens-vragen één voor één te stellen.
> - **Teamleider sneller:** Bij snel klaar: *"Bij welk voorbeeld zou een minder ervaren collega anders kiezen — en waarom?"* Activeert domeinkennis-bewustzijn (principe 4) zonder te spoilen.

**Antwoordmodel werkblad 1:**

Bewust geen sluitende sleutel. De kernles is dat operators verschillen vinden — sleutel zou die les ondergraven. Wel: succescriterium is ≥18 van 20 voorbeelden gelabeld, met vraagtekens toegestaan in de kantlijn. Verwacht: voorbeelden met defecten net rond 1 mm of net op de rand van het zichtvlak leveren systematisch verschillende keuzes op (en dat is precies wat we in fase 2 willen oogsten).

**Transitie naar blok 2:** *"Eerst je buurman. We gaan tellen — niet oordelen."*

---

### 🟣 Blok 2: Buurman-vergelijking + inter-rater agreement
**00:12 - 00:22** | 10 min | Kolb-fase (leerfase): reflecteren

**Doel:** Deelnemer meet eigen inter-rater agreement (inter-beoordelaar-overeenkomst) met buurman. Ontdekt dat verschillen wijzen op een onhelder schema, niet op een 'foute' operator. Drie verschillen worden plenair benoemd.

**Werkvorm:** Duo-vergelijking (5 min), plenair drie verschillen op het bord (4 min), brug naar theorie (1 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-02 uit. Toon slide 6. Zeg: *"Tweetal met je buurman. Twee dingen: één — tel per voorbeeld of jullie hetzelfde label hebben of een verschil. Twee — bij elk verschil onderzoek je samen: welk woord uit het schema gaf jullie twijfel?"*

2. **Duo-tellen** (5 min) — zet timer op 5 minuten. Zeg expliciet: *"Tel eerst, oordeel daarna. Tel ZELFDE versus VERSCHIL — niet GOED versus FOUT."* Loop rond. Coach bij wedstrijd-toon: *"Het is geen vergelijking van wie gelijk had. Het is een meting van het schema."*

3. **Plenair drie verschillen op het bord** (3 min) — toon slide 7. Vraag: *"Welke verschillen kwamen er uit?"* Verzamel drie verschillen op het bord (kolom 1: voorbeeldnummer; kolom 2: jouw label vs buurman; kolom 3: welk schema-woord gaf twijfel?). Per verschil één kernvraag: *"Welk woord uit het schema heeft hier voor twijfel gezorgd?"* — niet *"Wie had gelijk?"*

4. **Kernzin onthullen + brug** (1 min) — onthul nu het tweede bord-veld: **"Verschillen = schema-signaal, geen storing."** Zeg: *"Lager dan 80 procent overeenkomst betekent meestal niet dat een van de twee fout zit. Het betekent dat het labelschema nog niet helder genoeg is. Operator-verschillen zijn signaal voor wie het schema beheert — kwaliteit of IT. Hoe hoger jullie overeenkomst, hoe beter het schema is, niet hoe slimmer de operators."* Pauze 5 seconden.

**Materiaal:**
- [ ] Slides 6-7
- [ ] wb-02-buurman-vergelijking.md
- [ ] Bord of flip-over met drie kolommen
- [ ] Stiften
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Schrijf "verschil 1 / verschil 2 / verschil 3" met luchtige open vakken. Laat de groep het bord vullen — niet jij.
> - Bij stilte op de kernvraag *"Welk woord gaf twijfel?"* — tel tot 7. Daarna een hint: *"Was het 'klein'? Was het 'zichtvlak'? Was het 'grenswaarde'?"*
> - Eerste labelsessies leveren meestal 70-85 procent overeenkomst op. Onder de 80 procent is informatief, geen probleem.

> **🔴 Valkuil — verschillen framen als 'fout van de operator':**
> Iemand zegt *"ik had het toch goed"* of *"mijn buurman zit ernaast"*. Reframen direct: *"Het is geen wedstrijd, het is een meting. Het verschil dat jullie net vonden, is precies waar het schema scherper kan."* Schrijf de kernzin op het bord en wijs er straks in fase 3 nog twee keer naar.

> **🔴 Valkuil — alle verschillen plenair willen oogsten:**
> Houd het op drie. Meer verschillen verwateren de plenair-aandacht. Meld de overige verschillen: *"Houd je andere verschillen vast voor fase 4 — dat is materiaal voor je eigen schema."*

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Schrijf de meting groot op het bord: *"Aantal zelfde / 20 × 100 procent = overeenkomst"*. Bij rekenonzekerheid: *"17 keer zelfde betekent 85 procent."*
> - **Teamleider sneller:** Bij snel klaar: *"Hoe zou je dit verschil op de werkvloer aan IT melden — in één zin?"*
> - **Gemengde groep:** Combineer in duo's operator (wat zie ik feitelijk?) met teamleider (wat doen we met de meting?).

**Antwoordmodel werkblad 2:**

| Element | Verwacht | Toets |
|---|---|---|
| Aantal zelfde labels | Genoteerd (getal of breuk) | Cijfermatige antwoord, niet 'veel' of 'meeste' |
| Overeenkomst-percentage | Berekend (aantal zelfde / 20 × 100) | Min. 1 berekening getoond |
| Drie verschillen benoemd | Voorbeeldnummer + jouw label + buurman-label + schema-woord | Minimaal één verschil per duo plenair-inbrengbaar |
| Een verschil voor plenair | Genoteerd op het werkblad | Onafhankelijk van plenaire ronde — meting is leerwinst |
| Reframen-check | Verschil benoemd zonder oordeel | Geen wedstrijd-taal ('ik had gelijk') |

Typische uitkomst: 70-85 procent. Onder de 80 procent is normaal en informatief — geen reden tot zorg.

**Transitie naar blok 3:** *"Nu weten jullie hoe het in de praktijk voelt. We zetten er taal op — vier principes, vier valkuilen."*

---

### 📘 Blok 3: Handout — vier principes + vier valkuilen
**00:22 - 00:35** | 13 min | Kolb-fase (leerfase): theoretiseren

**Doel:** Deelnemer kent vier principes (consistentie, helderheid, dekking, domeinkennis) en herkent vier valkuilen (vermoeidheids-drift, confirmation bias, gemak boven precisie, operator-verschillen). Koppelt het mentale model aan de net beleefde ervaring in fase 1-2.

**Werkvorm:** Vier principes met terugkoppeling (5 min), vier valkuilen met herken-vragen (5 min), kernzin levend document (2 min), markeer-moment (1 min).

**Instructie:**

1. **Handout uitdelen + markeerstift** (1 min) — deel wb-03 uit. Zeg: *"Twee blokken. Eerst vier principes. Dan vier valkuilen. Pak je markeerstift — straks markeer je wat voor jou geldt."*

2. **Vier principes — met directe terugkoppeling** (5 min) — toon slide 8. Doorloop één voor één:
   - **(1) Consistentie** — *"Hetzelfde voorbeeld krijgt altijd hetzelfde label, ongeacht wie of wanneer. Test: meet inter-rater agreement met een collega. Jullie hebben dit net gemeten — dat is principe 1."*
   - **(2) Helderheid** — *"Labels zijn vooraf gedefinieerd met grenswaarden. Geen ambiguïteit. Test: kan een nieuwe collega het schema lezen en direct toepassen? Welke woorden uit jullie schema gaven twijfel? Dat is helderheid."* Wijs naar het bord met drie verschillen.
   - **(3) Dekking** — *"Alle relevante situaties zitten in de trainingsdata. Niet alleen makkelijke voorbeelden. Test: zijn zeldzame defecten ook opgenomen? Krassen die je twee keer per maand ziet, nachtploeg, nieuwe leverancier — moeten erin."*
   - **(4) Domeinkennis** — *"De operator weet wat een label betekent in de praktijk. Een operator met tien jaar ervaring ziet meteen of een 1 mm streep er toe doet, een buitenstaander niet. Zonder vakkennis valt labelwerk uit elkaar."*

3. **Vier valkuilen — met herken-vragen** (5 min) — toon slide 9. Doorloop één voor één:
   - **(a) Vermoeidheids-drift** — *"Na 100 foto's word je minder consistent. Wie heeft net bij voorbeeld 18 of 19 minder zorgvuldig gekeken dan bij voorbeeld 3?"* Pauze.  *"Maatregel: pauzeer elk uur."*
   - **(b) Confirmation bias (bevestigings-valkuil)** — *"Je verwacht een label, dus zie je het. Wie verwachtte vanaf voorbeeld 15 vooral GOEDs te zien?"* Pauze. *"Maatregel: wissel periodiek met een collega."*
   - **(c) Gemak boven precisie** — *"Het twijfel-product krijgt GOED omdat dat sneller is. STOP."* Schrijf groot op het bord: **"Twijfel = TWIJFEL-label, niet GOED."** *"Het schema heeft het TWIJFEL-label precies voor deze situatie. Als je twijfel als GOED labelt, leert de AI dat grenswaardes goed zijn — en dan mist hij ook echte defecten."*
   - **(d) Operator-verschillen** — *"Twee operators zijn niet altijd het eens. Dat is signaal voor het schema, geen storing. Jullie hebben dit net gemeten — dat is valkuil d. Reframen: verschillen zijn input voor wie het schema beheert."*

4. **Kernzin levend document + markeer-moment** (2 min) — toon slide 10. Zeg: *"Het labelschema is een levend document. Jullie verschillen vandaag zijn input voor de versie van volgende week. Hoe hoger de inter-rater agreement, hoe beter het schema, niet hoe slimmer de operators."* Daarna: *"Pak je markeerstift. Markeer twee principes die voor jou het belangrijkst voelen en twee valkuilen die jij vandaag het meest hebt ervaren."* 1 minuut markeer-stilte.

**Materiaal:**
- [ ] Slides 8-10
- [ ] wb-03-handout-vier-principes-vier-valkuilen.md
- [ ] Markeerstift per deelnemer
- [ ] Bord (voor regel 'twijfel = TWIJFEL, niet GOED')

> **💡 Tips voor de trainer:**
> - Bij elk principe één directe terugkoppeling naar fase 1-2. Anders blijft het lijstjes-kennis.
> - De regel *"Twijfel = TWIJFEL, niet GOED"* schrijf je groot op het bord en wijs je in fase 4 nog twee keer aan.
> - Stilte na de herken-vragen ('wie heeft net bij voorbeeld 18-19 minder zorgvuldig gekeken?') — tel tot 7. Iemand gaat lachen of knikken; dat is je opening.

> **🔴 Valkuil — vier principes als losse begrippen:**
> Bij elk principe terug naar de buurman-fase. *"Jullie hebben net consistentie gemeten."* Niet *"consistentie betekent..."*. De ervaring komt eerst, de naam erbij.

> **🔴 Valkuil — gemak-boven-precisie onbenoemd laten:**
> Dit is de sluipendste valkuil. Markeer expliciet. Geef het werkvloer-voorbeeld: *"Twee operators kiezen GOED bij een grenswaarde-product omdat anders de afkeur-bak vol raakt. De AI leert dan dat grenswaardes goed zijn. Een maand later mist hij het ook bij echte defecten."*

> **🔴 Valkuil — handout in één lap voorlezen:**
> Twee blokken — niet één. Tussen principes en valkuilen: ademhalen, vraag de groep *"Welke valkuil heb je net zelf gevoeld?"* — dat haalt aandacht terug.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Schrijf vier principes en vier valkuilen groot op het bord — laat ze staan voor fase 4.
> - **Teamleider sneller:** Vraag: *"Welk principe is op jullie werkvloer al goed geregeld — en welk is het zwakste?"* Activeert systeem-blik.
> - **Bij weinig tijd:** Houd vier principes plus regel *"twijfel = TWIJFEL"* vast; valkuilen kun je inkorten — maar laat operator-verschillen niet weg (sluit fase 2 af).

**Antwoordmodel werkblad 3:**

| Element | Verwacht | Toets |
|---|---|---|
| Twee principes gemarkeerd | Markeerstift-aanstreping | Geen 'goed/fout' — keuze is persoonlijk |
| Twee valkuilen gemarkeerd | Markeerstift-aanstreping | Idem |
| Veelgekozen principes | Consistentie + helderheid | Logisch want net beleefd in fase 2 |
| Veelgekozen valkuilen | Vermoeidheids-drift + operator-verschillen | Logisch want net ervaren bij voorbeelden 15-20 en bij buurman-vergelijking |

**Transitie naar blok 4:** *"Vier principes ken je nu. Vier valkuilen herken je. Nu jouw beurt — een mini-schema voor je eigen lijn."*

---

### 🟠 Blok 4: Eigen mini-labelschema + valkuil + actie
**00:35 - 00:45** | 10 min | Kolb-fase (leerfase): experimenteren

**Doel:** Deelnemer maakt een mini-labelschema (drie labels met grenswaarden) voor één beoordelings-moment op zijn eigen lijn, kiest één valkuil + maatregel voor de eigen werkvloer, en formuleert één concrete actie voor deze week.

**Werkvorm:** Werkblad-uitleg (1 min), individueel werken (6 min), plenaire ronde van één-zin-per-persoon (2 min), transferopdracht (1 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit. Toon slide 11. Zeg: *"Laatste 10 minuten. Vier stappen op het verkenningsblad. Stap 1 — kies één beoordelings-moment op je eigen lijn. Stap 2 — schrijf drie labels met grenswaarden. Stap 3 — kies één valkuil voor jouw werkvloer plus één maatregel. Stap 4 — kies één concrete actie voor deze week. Geen IT-kennis nodig."* Optioneel daarna: deel tablets met `model-label-valkuilen.jsx` als aanvulling — *"6 dataset-scenarios om de 4 valkuilen op datasetniveau te oefenen voordat jullie jullie eigen schema in actie zien."*

2. **Individueel werken** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. CAR (competentie / autonomie / relatedness): bij vastlopers coach door met grens-vragen:
   - *"Welk AI-systeem of welke visuele check is er op jouw lijn? De inspectiecamera? Het afkeur-systeem? Een eindcontrole?"*
   - *"Waar staat bij jou de grens tussen TWIJFEL en AFGEKEURD? Een millimeter? Een procent? Een locatie?"*
   - *"Welke collega zou jouw schema het eerst proberen — en zou hij hetzelfde label kiezen?"*
   - *"Welke van de vier valkuilen is op jullie werkvloer het grootste risico — vermoeidheids-drift, confirmation bias, gemak boven precisie, of operator-verschillen?"*

3. **Plenaire ronde** (2 min) — toon slide 12. Zeg: *"Eén ronde — iedereen één zin: welke valkuil voor jouw werkvloer, en welke actie deze week?"* Houd kort: max 15 seconden per persoon. Begin zelf met een voorbeeld als de stilte te lang duurt: *"Bij mij zou het operator-verschillen zijn — actie deze week is vragen aan kwaliteit wie ons schema beheert."*

4. **Transferopdracht + afsluiting** (1 min) — toon slide 13. Zeg: *"Deze week drie stappen op je eigen lijn. Eén — vraag wie het labelschema beheert. Twee — label tien voorbeelden zelf, met één pauze halverwege. Drie — laat een collega dezelfde tien labelen zonder jouw antwoorden, tel je inter-rater agreement. Neem alle drie de uitkomsten mee naar volgende sessie. Bonus: vraag deze week aan iemand van kwaliteit of IT — 'hoeveel verschil zit er tussen onze operators op dezelfde producten, en wie houdt dat bij?'"*

**Materiaal:**
- [ ] Slides 11-13
- [ ] wb-04-eigen-labelschema.md
- [ ] Optioneel: `video/composition.tsx` (Remotion `DataLabelenVideo`, ~91s) — pre-rendered MP4 of live preview voor fase 3
- [ ] Optioneel: tablets met `model-label-valkuilen.jsx` als aanvulling op wb-04 in fase 4
- [ ] Pen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Plenair: max 15 seconden per persoon. Eindig op tijd. Een goede afsluiting is beter dan uitlopen.
> - Bij iemand die geen beoordelings-moment kan bedenken: geef suggesties (inspectiecamera, afkeur, eindcontrole, sortering).
> - Bij iemand die een schema met zeven labels probeert: begrens. *"Drie is genoeg. Beter helder en simpel dan uitgebreid en vaag."*

> **🔴 Valkuil — mini-schema te uitgebreid:**
> Deelnemer probeert een complex schema met subcategorieën. Begrens: *"Drie labels met grenswaarden. Een nieuwe collega-test — kan hij het schema lezen en direct toepassen?"* Verwijs naar principe 2 (helderheid).

> **🔴 Valkuil — actie te abstract:**
> *"Ik ga letten op consistentie"* is geen actie. Begrens: *"Wat doe je precies, wanneer, met wie?"* Voorbeeld: *"Donderdagmiddag vraag ik aan kwaliteits-Esra wie ons labelschema beheert."*

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers — geef twee voorbeelden van beoordelings-momenten op de werkvloer en laat deelnemer kiezen. Help met de eerste grenswaarde.
> - **Teamleider sneller:** Bij snel klaar: *"Hoe ga jij in jouw team systematisch inter-rater agreement bijhouden?"* Strategische blik.
> - **Bij niet-werkvloer-deelnemer (zeldzaam):** Laat hem een hypothetisch schema bouwen voor de visuele-controle-casus uit de werkbladen.

**Antwoordmodel werkblad 4:**

| Stap | Verwacht | Toets |
|---|---|---|
| 1 — Beoordelings-moment | Concreet benoemd (inspectiecamera, afkeur, sortering, visuele eindcontrole) | Niet abstract ('kwaliteit') |
| 2 — Drie labels met grenswaarden | GOED — [criterium] / TWIJFEL — [criterium] / AFGEKEURD — [criterium]. Grenswaarden in mm, procent, locatie of meetbare term | Geen vage woorden ('mooi', 'redelijk') |
| 3 — Valkuil + maatregel | Eén van vier valkuilen + concrete maatregel (pauze elk uur, dubbelcheck, kalibratie-sessie) | Maatregel concreet, niet abstract |
| 4 — Actie deze week | Wat-wanneer-met-wie. Voorbeeld: *"Donderdag vraag ik aan Esra van kwaliteit wie ons schema beheert."* | Niet *"ik ga erop letten"* |

**Veelvoorkomende beoordelings-momenten op de werkvloer:**
- Inspectiecamera op visuele kwaliteitslijn
- Sorteersysteem op formaat of kleur
- Visuele eindcontrole bij assemblage
- Afkeur-systeem op spuitgietproducten

**Veelvoorkomende acties voor deze week:**
- Vraag bij IT/kwaliteit wie het huidige labelschema beheert
- Label zelf tien voorbeelden + laat collega hetzelfde doen
- Meet inter-rater agreement op de eigen lijn

**Transitie naar afsluiting:** *"Mooi werk. Drie stappen deze week — daar zit beweging in. Volgende sessie bespreken we welk schema-woord de meeste twijfel gaf op jullie eigen lijn."*

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-eerste-labelsessie | n + 2 | A4 enkelzijdig (20 voorbeelden + labelschema) |
| ☐ | wb-02-buurman-vergelijking | n + 2 | A4 enkelzijdig (tel-tabel + drie-verschillen-veld) |
| ☐ | wb-03-handout-vier-principes-vier-valkuilen | n + 2 | A4 dubbelzijdig (vier principes + vier valkuilen) |
| ☐ | wb-04-eigen-labelschema | n + 2 | A4 enkelzijdig (vier stappen) |
| ☐ | Pennen | n + 5 | Reserve |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Flip-over of bord | 1 | Drie verschillen + kernzin 'verschillen = schema-signaal' + regel 'twijfel = TWIJFEL, niet GOED' |
| ☐ | Dikke stiften | 2-3 | |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | Presenter-modus |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| Eerste labelsessie loopt uit (groep leest traag) | Verkort fase 3 met 2 min: laat valkuil (d) operator-verschillen kort als slot ('jullie hebben dit zelf ervaren') i.p.v. uitgebreid behandelen. |
| Buurman-vergelijking geeft hoge overeenkomst (>95%) | Reframen: *"Mooi — jullie schema is helder. Niet alle teams hebben dit. Wat maakt dat jullie zo gekalibreerd zijn?"* Trek lessen voor andere groepen. |
| Buurman-vergelijking geeft lage overeenkomst (<60%) | Reframen: *"Dat is informatief — wat dit betekent: het schema is nog niet helder. Geen probleem; precies waar fase 3 op inspeelt."* Niet sussen, niet bagatelliseren. |
| Een deelnemer wordt defensief over een verschil | Begrens: *"Het is geen wedstrijd, het is een meting."* Verwijs naar het bord met de kernzin. |
| Mini-schema in fase 4 loopt vast | Geef twee voorbeelden uit de antwoordmodel-lijst en laat de deelnemer kiezen. |
| Plenaire ronde fase 4 dreigt uit te lopen | Begrens tot 15 sec per persoon. Bij grote groep: laat 4 deelnemers delen, anderen schrijven op een sticky en plakken die voor je weggaan. |
| Groep is te klein (4 of minder) | Buurman-vergelijking wordt drietal of trio. Plenaire ronde versmelt met fase 4. |

---

## Snel-overzicht

| Fase (leerfase) | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 20 voorbeelden labelen, vraagteken mag | ≥18 ingevuld, twijfel benoemd |
| 2 reflecteren | Buurman-vergelijking + drie verschillen op bord | Overeenkomst-percentage genoteerd, drie schema-woorden geïdentificeerd |
| 3 theoretiseren | Vier principes + vier valkuilen + 'twijfel = TWIJFEL' | Twee principes + twee valkuilen gemarkeerd |
| 4 experimenteren | Eigen mini-schema + valkuil + actie deze week | Drie labels met grenswaarden + concrete actie wat-wanneer-met-wie |

**Slagingscriterium:** ≥18 voorbeelden gelabeld + inter-rater agreement gemeten + één verschil verklaard vanuit een principe + mini-schema voor eigen werkvloer + één valkuil + één actie voor deze week.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor reflectie op de groep)
- [ ] Genoteerd: typische inter-rater agreement van deze groep (voor benchmark)
- [ ] Genoteerd: welke schema-woorden de meeste twijfel gaven (input voor volgende sessie)
- [ ] Genoteerd: welke valkuilen plenair zijn gedeeld
- [ ] xAPI-statements verstuurd: `experienced`, `attempted`, `performed`, `completed`

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | Data labelen op de werkvloer*
*Bron: ko-ai-fund-002, ko-ai-fund-003, ko-ai-fund-023 + praktijklessen labelwerk RLC Oost/Zuid 2025-2026.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
