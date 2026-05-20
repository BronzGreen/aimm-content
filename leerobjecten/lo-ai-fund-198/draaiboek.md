# Kritisch denken over AI — Draaiboek
*AI Fundamentals Module 1 (Gebruik) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan drie checks toepassen op een AI-output, herkent bias in werkvloer-context, en kan vier kritische vragen formuleren voor IT of leverancier — in 2-3 minuten per advies. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1A + lo-ai-fund-181 + lo-ai-fund-186 doorlopen |
| **Stadium (Hersey & Blanchard)** | Bewust onbekwaam — vermoedt dat kritisch denken nodig is, mist procedure |
| **Begeleidingsstijl (manier van begeleiden)** | Trainen — procedurele kennis, scaffolding-drieluik |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over of bord |
| **Plek in module** | Verdieping op 'attitude' uit lo-ai-fund-181. Operationaliseert sterk/zwak uit lo-ai-fund-186. Bereidt voor op lo-ai-fund-204 (bias). |
| **Bloom-niveau** | Toepassen (procedureel) — niet alleen kennen maar uitvoeren |
| **Kirkpatrick-niveau** | Gedrag — transfer naar werkvloer met meetbare check-routine |

---

## Sessie-overzicht

| Tijd | Activiteit | Type (Kolb-fase / leerfase) | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Spuitgietmachine — drie vragen zelf doorlopen | ervaren | 12 min |
| 00:12 - 00:22 | Buurman-check + drie namen op het bord | reflecteren | 10 min |
| 00:22 - 00:35 | Handout 3 checks + bias + 4 kritische vragen | theoretiseren | 13 min |
| 00:35 - 00:45 | Eigen AI-advies + drie checks + één vraag | experimenteren | 10 min |

**Totaal:** 45 minuten.
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Test de Slidev-presentatie.
- [ ] Flip-over of bord — drie kolommen voorbereiden met de drie VRAGEN (zonder check-namen): "1 — Klopt met ervaring?", "2 — Compleet/precies?", "3 — Wat als tegenvalt?". In fase 2 hernoemen.
- [ ] Tweede flip-over: wantrouwen-vs-kritisch-tabel uit handout, klaar voor fase 3.
- [ ] Optioneel: open `model-kritisch-denken-ai.jsx` in een React-sandbox (CodeSandbox/Vite-preview) als digitaal alternatief — beschikbaar voor wie sneller wil oefenen of voor zelfstandig nawerk.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Spuitgietmachine — drie vragen zelf doorlopen
**00:00 - 00:12** | 12 min | Kolb-fase (leerfase): ervaren

**Doel:** Deelnemer doorloopt drie vragen op een werkvloer-casus — zonder dat hij weet dat dit later "de drie checks" heten.

**Werkvorm:** Plenaire opening (2 min), casus + IK DOE vraag 1 (3 min), individueel vragen 2 en 3 (6 min), brug (1 min).

**Instructie:**

1. **Open de sessie** (2 min) — toon slide 1. Zeg: *"De komende 45 minuten leer je hoe je een AI-advies in 2-3 minuten kunt checken — zonder ALLES te wantrouwen. Drie checks, vier vragen. Aan het eind heb je een routine die in elke productieshift past."* Pauze.

2. **Casus + IK DOE vraag 1** (3 min) — deel wb-01 uit. Lees casus hardop voor: *"Operator bij een spuitgietmachine krijgt deze week een advies van het AI-systeem: 'verhoog cyclustijd met 1,2 seconde om afkeur te verminderen'. Het advies klinkt duidelijk. Hij twijfelt — vorige maand werd een advies opgevolgd en bleek het niet te kloppen. Het is nu juli — buiten is het al een tijd warm."* Doe vraag 1 hardop voor (IK DOE): *"Vraag 1 — klopt dit met wat hij zelf weet? Voor mij: vorige maand klopte het niet, dat is een hint. En sinds toen werd het warmer. Warmere mallen hebben juist kortere cyclustijden nodig. Niet langere. Hier voelt iets niet kloppen. Nu jullie — beantwoord vraag 2 en 3."*

3. **Individueel vragen 2 en 3** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. Bij vastlopers: *"Vraag 2 — wat staat er bij het advies, en wat ontbreekt? Vraag 3 — wat verlies je als je het volgt en het zou tegenvallen?"*

4. **Afsluiten + brug** (1 min) — vraag: *"Wie heeft minimaal vraag 2 en 3 ingevuld?"* Tel handen. *"Niemand hoeft te delen. Eerst je buurman."*

**Materiaal:**
- [ ] Slides 1-3
- [ ] wb-01-casus-spuitgietmachine.md (1 per deelnemer)
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Geef GEEN check-namen (betrouwbaarheid, kwaliteit, bedoelde effecten) in dit blok.
> - Bij IK DOE: hardop denken — niet conclusies dicteren.
> - Tel innerlijk tot 7 na elke open vraag.

> **Valkuil — check-namen verklappen:**
> Bij een goed antwoord: bevestig zonder term. "Mooi — onthoud die zin."

> **Valkuil — bias-naam te vroeg:**
> Iemand zegt "het systeem is op iets anders getraind". Bevestig zonder "bias" te noemen. *"Goed gezien — daar geven we straks een naam aan."*

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers: "Wat zou je doen als jij die operator was — direct opvolgen, of eerst doorvragen?"
> - **Teamleider sneller:** Bij snel klaar: "Welke andere AI-adviezen heb je gezien die achteraf niet klopten?" Voorbereiding op fase 4.

**Antwoordmodel werkblad 1:**
- **Vraag 1 (klopt met ervaring):** Vorige maand klopte het advies niet. Sindsdien veranderde iets — eind juni werd het warm.
- **Vraag 2 (compleet):** Geen datum. Geen zekerheidsscore. Niet zichtbaar op welke periode het systeem is getraind.
- **Vraag 3 (als tegenvalt):** 30 minuten productieverlies per shift + mogelijke kwaliteitsproblemen.
- **Oordeel:** "Eerst doorvragen" of "niet opvolgen" zijn beide goede antwoorden — met argumentatie.
- **Vraag aan IT:** "Op welke periode is dit systeem getraind?"
- **Eigen opmerking:** Eigen werkvloer-anecdote — variabel.

**Transitie naar blok 2:** *"Niemand hoeft te delen. Eerst je buurman."*

---

### Blok 2: Buurman-check + drie namen op het bord
**00:12 - 00:22** | 10 min | Kolb-fase (leerfase): reflecteren

**Doel:** Deelnemer herkent dat de drie vragen uit fase 1 drie verschillende soorten check waren — betrouwbaarheid, kwaliteit, (on)bedoelde effecten.

**Werkvorm:** 5 min duo's, 4 min plenair drie namen, 1 min brug.

**Instructie:**

1. **Duo-uitwisseling** (5 min) — toon slide 4. Deel wb-02 uit. *"Tweetal met je buurman. Vergelijk je antwoorden op de drie vragen. Vergelijk eerst — oordeel daarna."* Zet timer op 5 minuten. Loop rond.

2. **Drie namen op het bord** (4 min) — wijs op het bord (drie kolommen met vragen). *"Drie verschillende soorten check. Vraag 1 ging over: klopt het met ervaring? Daar geef ik nu een naam aan — BETROUWBAARHEID."* Schrijf onder vraag 1: BETROUWBAARHEID. *"Vraag 2 ging over: is het compleet en precies? Naam: KWALITEIT."* Schrijf. *"Vraag 3 ging over: wat als het tegenvalt? Naam: (ON)BEDOELDE EFFECTEN."* Schrijf. *"Jullie hebben deze drie checks net zelf doorlopen — zonder ze nog te kennen."*

3. **Brug naar de definitie** (1 min) — sluit af: *"Drie checks. In 2-3 minuten. Plus iets dat we nog niet hebben benoemd — waarom klopte het advies eigenlijk niet?"*

**Materiaal:**
- [ ] Slide 4
- [ ] wb-02-buurman-drie-checks.md
- [ ] Bord of flip-over met drie kolommen
- [ ] Stiften
- [ ] Timer

> **Tips voor de trainer:**
> - De drie kolommen op het bord uit fase 1 hernoemen — niet nieuw tekenen.
> - "Jullie hebben de checks zelf doorlopen" — empowerment.

> **Valkuil — bias al noemen:**
> Bias hoort in fase 3. Hier alleen de drie checks-namen.

> **Differentiatie:**
> - **Gemengde groep:** Operator + teamleider in duo. Operator brengt eigen ervaring, teamleider brengt 'hoe checken we als organisatie?'.

**Antwoordmodel werkblad 2:**
- **Stap 1 (vergelijken):** Variabel. Verwachting: bij vraag 1 dichtst bij elkaar (ervaring), bij vraag 3 grotere verschillen (risico-inschatting).
- **Stap 2 (focus):** Vraag 1 = klopt het. Vraag 2 = is het compleet. Vraag 3 = wat als tegenvalt.
- **Drie namen tabel:** Vraag 1 → Betrouwbaarheid. Vraag 2 → Kwaliteit. Vraag 3 → (On)bedoelde effecten.
- **Stap 3 (meeste twijfel):** Variabel.
- **Eén zin samen:** Bijvoorbeeld "een operator heeft nodig: ervaring, een complete melding, en zicht op gevolgen."

**Transitie naar blok 3:** *"Drie checks. Plus iets nieuws — wat is bias eigenlijk?"*

---

### Blok 3: Handout — 3 checks + bias + 4 kritische vragen
**00:22 - 00:35** | 13 min | Kolb-fase (leerfase): theoretiseren

**Doel:** Deelnemer kent drie checks formeel + bias-begrip (ploeg/machine/seizoen) + vier kritische vragen + de slimme-collega-houding.

**Werkvorm:** Drie blokken: drie checks (4 min), bias (4 min), vier vragen (3 min), slimme-collega-houding (2 min).

**Instructie:**

1. **Drie checks formeel + markeren** (4 min) — deel wb-03 uit. Toon slide 5. *"Pak je markeerstift. Drie checks die je in 2-3 minuten doet. Markeer ze."* Per check één regel: *"Betrouwbaarheid — klopt het met ervaring. Kwaliteit — is het compleet en precies. Bedoelde effecten — wat als ik dit volg en het zou tegenvallen."* Verwijs naar de spuitgietmachine-tabel in de handout.

2. **Bias-uitleg + spuitgietmachine als voorbeeld** (4 min) — toon slide 6. *"Bias is vertekening. AI leert uit data. Als die data scheef is, is de AI scheef. Niet omdat iemand het zo wilde — maar omdat de wereld waarin de AI is opgegroeid niet de hele wereld was."* Toon drie bronnen in maakindustrie: *"Eén — data uit één ploeg. Twee — data van één machine. Drie — data uit één seizoen."* Markeer de spuitgietmachine: *"Bij ons systeem: getraind op data uit december (koude fabriek). Nu juli (warme fabriek). Warmere mallen hebben juist kortere cyclustijden nodig. Bias door seizoen."*

3. **Vier kritische vragen markeren** (3 min) — toon slide 7. *"Vier vragen. Markeer ze. Eén: welke data heeft het systeem gezien? Twee: waarin lijkt mijn situatie op die data, waarin niet? Drie: welke fouten maakt dit type AI meestal? Vier: welke rol wil ik dat AI speelt — suggestie, bewaking of beslisser?"* Benadruk: *"Je hoeft ze niet allemaal te beantwoorden. Een vraag STELLEN aan IT is óók een antwoord. Vraag 4 is de belangrijkste."*

4. **Slimme-collega-houding** (2 min) — toon slide 8 (wantrouwen vs kritisch tabel). *"Kritisch denken is NIET wantrouwen. Wantrouwen klinkt: ik vertrouw die computer niet. Kritisch klinkt: ik check eerst of dit past in deze situatie. Wantrouwen is vast. Kritisch is open."* Verwijs naar halve-flessen-regel uit lo-ai-fund-186.

**Materiaal:**
- [ ] Slides 5-8
- [ ] wb-03-handout-checks-vragen.md
- [ ] Markeerstift per deelnemer
- [ ] Tweede flip-over (wantrouwen-vs-kritisch)

> **Tips voor de trainer:**
> - Bias concreet — drie bronnen, geen statistiek.
> - "Een vraag stellen is óók een antwoord" — herhalen.
> - Slimme-collega-houding visueel maken via de tabel.

> **Valkuil — bias academisch:**
> Geen algoritmische rechtvaardigheid of statistische parity. Drie bronnen + spuitgietmachine.

> **Valkuil — vier vragen als checklist:**
> Maak expliciet: niet allemaal beantwoorden. Vraag 4 is hoofdvraag.

> **Valkuil — wantrouwen-framing:**
> Bij iemand die zegt "AI vertrouw ik niet": verwijs naar tabel. *"Dat is wantrouwen. Kritisch denken is iets anders."*

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf drie checks + vier vragen groot op het bord.
> - **Teamleider sneller:** Bij vraag 4: vraag 'welke rol vervult AI bij jullie nu — en past dat?'

**Antwoordmodel werkblad 3:**
- **Drie checks markeren:** Betrouwbaarheid, kwaliteit, (on)bedoelde effecten.
- **Spuitgietmachine bias-bron:** Seizoen. Getraind op december-data, nu juli.
- **Vier vragen markeren:** (1) Welke data, (2) waarin lijkt mijn situatie, (3) welke fouten, (4) welke rol AI?
- **Korte oefening (bias-bron):** Seizoen, omdat trainingsdata uit een andere temperatuurperiode kwam.

**Transitie naar blok 4:** *"Nu jouw beurt. Een eigen AI-advies — drie checks toepassen."*

---

### Blok 4: Eigen AI-advies + drie checks + één vraag
**00:35 - 00:45** | 10 min | Kolb-fase (leerfase): experimenteren

**Doel:** Deelnemer past drie checks toe op een eigen AI-advies en kiest één kritische vraag voor IT/leverancier.

**Werkvorm:** Individueel werkblad (6 min), plenaire afronding met 2-3 vragen + transferopdracht (3 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit. Toon slide 9. *"Laatste 10 minuten. Denk aan één AI-advies of melding die je deze of vorige week kreeg. Pas drie checks toe — schrijf per check één antwoord. Kies dan één van de vier kritische vragen om aan IT of leverancier te stellen."*

2. **Individueel werken** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. Bij vastlopers: *"Welk AI-systeem heb je vorige week gebruikt? Welk advies of melding kwam eruit?"* Begrens algemene vragen: *"Welke van de vier vragen, in JOUW woorden, gericht op JOUW systeem?"*

3. **Plenaire afronding + transferopdracht** (3 min) — toon slide 10. *"Wie deelt zijn kritische vraag?"* Vang 2 of 3. Toon slide 11 (transfer). *"Deze week: één AI-advies, drie checks in 2-3 minuten, één vraag aan IT. Bonus: vraag aan een collega 'hoe check jij eigenlijk?' Antwoord mee naar volgende sessie."*

**Materiaal:**
- [ ] Slides 9-11
- [ ] wb-04-eigen-advies-checks.md
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Maximaal 3 voorbeelden plenair.
> - Begrens algemene vragen — gericht op specifiek systeem en periode.
> - Eindig op tijd.

> **Valkuil — vraag te abstract:**
> "Is AI goed afgesteld?" is geen concrete vraag. Begrens: "op welke producten getraind?", "welke fouten meestal?", "welke rol moet AI hier spelen?"

> **Valkuil — geen tijd voor transfer-collega-gesprek:**
> Bij uitloop: noem alleen het collega-gesprek kort — "hoe check jij eigenlijk?"

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers: kies één van de vier vragen — schrijf in eigen woorden.
> - **Teamleider sneller:** Bij snel klaar: "Welke routine wil je in je team inbouwen?"

**Antwoordmodel werkblad 4:**
- **Stap 1 (welk advies):** Concreet — eigen werkvloer-advies.
- **Stap 2 (drie checks):** Per check één concreet argument.
- **Stap 3 (meeste twijfel):** Per deelnemer anders — alle drie kunnen overheersend zijn.
- **Stap 4 (één kritische vraag):** Bijvoorbeeld vraag 1 ("welke data?") of vraag 4 ("welke rol?"), in eigen woorden gericht op eigen systeem.
- **Stap 5 (besluit nu):** Variabel — vier opties zijn alle goed met onderbouwing.

**Transitie naar afsluiting:** *"Mooi werk. Drie checks, één vraag. 2-3 minuten per advies."*

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-casus-spuitgietmachine | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-buurman-drie-checks | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-checks-vragen | n + 2 | A4 dubbelzijdig (3 checks + bias + 4 vragen + tabel) |
| ☐ | wb-04-eigen-advies-checks | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Flip-over of bord | 1 | Drie kolommen (in fase 2 hernoemen) |
| ☐ | Tweede flip-over | 1 | Wantrouwen-vs-kritisch-tabel |
| ☐ | Dikke stiften | 2-3 | |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | Presenter-modus |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| Groep loopt uit in fase 1 | Trainer doet vraag 2 ook hardop voor. Beperk individuele tijd tot 4 min. |
| Discussie over bias-ethiek | Erken, parkeer op flip-over voor lo-ai-fund-204. |
| Plenair delen in fase 4 lukt niet | Sticky-method: kritische vraag op een sticky, plakken op bord. |
| Een deelnemer is cynisch over AI | Bevestig de zorg, verwijs naar wantrouwen-vs-kritisch-tabel. Bied de slimme-collega-houding als alternatief. |
| Groep is te klein (4 of minder) | Buurman-check wordt groeps-rondje. Plenaire ronde versmelt met fase 4. |

---

## Snel-overzicht

| Fase (leerfase) | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Drie vragen doorlopen op spuitgietmachine | Drie verschillende soorten check intuïtief gedaan |
| 2 reflecteren | Drie namen op het bord | Betrouwbaarheid / Kwaliteit / Bedoelde effecten |
| 3 theoretiseren | 3 checks + bias + 4 vragen + slimme-collega | Mentaal model: 2-3 min routine, geen wantrouwen |
| 4 experimenteren | Eigen advies + drie checks + één vraag | Concrete vraag voor IT deze week |

**Slagingscriterium:** Drie checks correct toegepast + bias-bron herkennen + één kritische vraag in eigen woorden.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt
- [ ] Genoteerd welke kritische vragen plenair zijn gedeeld
- [ ] Genoteerd: welke bias-bronnen werden herkend (input voor lo-ai-fund-204)
- [ ] xAPI-statements verstuurd: `experienced`, `completed`, `attempted`

---

*AIMM Curriculum | AI Fundamentals Module 1 (Gebruik) | Kritisch denken*
*Bron: Npuls (2025). Raamwerk NL AI-Geletterdheid in het Onderwijs, p. 9.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
