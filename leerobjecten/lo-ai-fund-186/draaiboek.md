# Wat AI goed kan — en waar het mis gaat — Draaiboek
*AI Fundamentals Module 1 (Gebruik) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan vier sterke en vier zwakke kanten van AI benoemen, herkent welke zwakte bij de lasersnijder-casus speelde, en formuleert een concrete check voor een eigen AI-systeem. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1A + lo-ai-fund-181 (AI-geletterdheid) doorlopen |
| **Stadium (Hersey & Blanchard)** | Bewust onbekwaam — vermoedt dat AI niet onfeilbaar is, mist het mentale kader |
| **Begeleidingsstijl (manier van begeleiden)** | Trainen — IK DOE / WIJ DOEN / JIJ DOET drieluik |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over of bord |
| **Plek in module** | Verdieping op 'kennis' uit lo-ai-fund-181. Bereidt voor op lo-ai-fund-198 en lo-ai-fund-204. |

---

## Sessie-overzicht

| Tijd | Activiteit | Type (Kolb-fase / leerfase) | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Lasersnijder — wat dacht AI, wat zag operator? | ervaren | 12 min |
| 00:12 - 00:22 | Buurman-check + twee lijstjes op bord | reflecteren | 10 min |
| 00:22 - 00:35 | Handout 4 sterktes + 4 zwaktes + halve-flessen-regel | theoretiseren | 13 min |
| 00:35 - 00:45 | Eigen werkvloer-systeem + concrete check | experimenteren | 10 min |

**Totaal:** 45 minuten.
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Test de Slidev-presentatie.
- [ ] Flip-over of bord — twee kolommen voorbereiden: links **"AI is STERK in..."**, rechts **"AI is ZWAK in..."**. Leeg laten; vullen in fase 2.
- [ ] Tweede flip-over: halve-flessen-regel-tabel (vier rijen) voor fase 3.
- [ ] Optioneel: open `model-ai-sterk-zwak-herkenner.jsx` in een React-sandbox (CodeSandbox/Vite-preview) als digitaal alternatief — beschikbaar voor wie sneller wil oefenen of voor zelfstandig nawerk.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel.
- [ ] Open slide 1 in presenter-modus.

---

## Blok-details

### Blok 1: Lasersnijder — wat dacht AI, wat zag operator?
**00:00 - 00:12** | 12 min | Kolb-fase (leerfase): ervaren

**Doel:** Deelnemer ondervindt aan de lasersnijder-casus dat AI iets kan missen wat een operator wel ziet — zonder dat zwaktes al benoemd zijn. Trainer doet sterkte-analyse hardop voor (IK DOE); deelnemers analyseren zelf wat de AI niet zag.

**Werkvorm:** Plenaire opening (2 min), casus presenteren + IK DOE sterkte-analyse (3 min), individueel vraag 2-4 (6 min), brug (1 min).

**Instructie:**

1. **Open de sessie** (2 min) — toon slide 1. Zeg: *"De komende 45 minuten kijken we naar twee kanten van AI. Wat doet AI heel goed — en waar gaat het meestal mis op de werkvloer? Aan het eind kun jij voor JOUW systeem benoemen op welke sterkte het leunt en welke zwakte het grootste risico is."* Pauze.

2. **Casus + IK DOE sterkte-analyse** (3 min) — deel wb-01 uit. Lees casus hardop voor. Daarna doe hardop voor: *"Vraag 1 — wat doet het systeem hier goed? Voor mij: het rekent snel. Het vergelijkt duizenden snijpaden. Het wordt niet moe. Het zou nooit een rekenfout maken. Dat zijn echte sterktes. Nu jullie — wat ziet het systeem NIET? En zou je het advies volgen?"*

3. **Individueel vraag 2-4** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. Bij vastlopers: *"Wat zou een ervaren operator opmerken bij een dunne plaat? Wat staat er niet in het AI-advies?"*

4. **Afsluiten + brug** (1 min) — vraag: *"Wie heeft minimaal vraag 2 en 3 ingevuld?"* Tel handen. *"Niemand hoeft te delen. Eerst je buurman."*

**Materiaal:**
- [ ] Slides 1-3
- [ ] wb-01-casus-lasersnijder.md (1 per deelnemer)
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Geef GEEN zwakte-naam (bias, context). Bevestig observaties zonder labelen.
> - Visualiseer de wachtende plaat hardop. *"Stel je voor — een verwarmde plaat ligt te wachten. Dun materiaal. Wat gebeurt er?"*
> - Tel innerlijk tot 7 na elke open vraag.

> **Valkuil — zwakte-naam verklappen:**
> Iemand zegt *"het systeem was getraind op dikker materiaal"*. Bevestig: *"Mooi, onthoud dat. Daar geven we straks een naam aan."*

> **Valkuil — antwoord 'volgen of niet' opdringen:**
> Bevestig elk antwoord. *"Eerst doorvragen"* is meestal het beste antwoord, maar alle keuzes hebben hun argumenten.

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers: "Wat zou jij doen als jij die operator was?"
> - **Teamleider sneller:** Bij snel klaar: "Welke vraag zou jij aan de leverancier stellen voordat je dit advies opvolgt?"

**Antwoordmodel werkblad 1:**
- **Stap 1 (wat doet systeem goed):** Rekent snel, vergelijkt duizenden paden, consistent, geen vermoeidheid.
- **Stap 2 (wat ziet systeem niet):** Wachtende verwarmde plaat tussen snijbewegingen + dunne 2mm materiaal die vervormt.
- **Stap 3 (advies volgen):** "Eerst doorvragen" is meest passend; ook "niet volgen" met ervaring-argument verdedigbaar.
- **Stap 4 (vraag voor leverancier/IT):** Bijvoorbeeld "op welke materiaaldiktes is dit systeem getraind?" of "houdt de optimalisatie rekening met thermische vervorming?"

**Transitie naar blok 2:** *"Niemand hoeft te delen. Eerst je buurman."*

---

### Blok 2: Buurman-check + twee lijstjes op het bord
**00:12 - 00:22** | 10 min | Kolb-fase (leerfase): reflecteren

**Doel:** Deelnemer herkent dat de zwaktes iets gemeen hebben — allemaal situaties buiten het trainingsgebied van de AI.

**Werkvorm:** 5 min duo's, 4 min plenair twee lijstjes, 1 min brug.

**Instructie:**

1. **Duo-uitwisseling** (5 min) — toon slide 4. Deel wb-02 uit. *"Tweetal met je buurman. Vergelijk wat het systeem goed deed en wat het niet zag. Eerst luisteren, dan reageren."* Zet timer op 5 minuten. Loop rond.

2. **Twee lijstjes op het bord** (4 min) — wijs op het bord. *"We vullen twee lijstjes. Links: AI is STERK in. Rechts: AI is ZWAK in. Wie geeft mij iets voor links?"* Verzamel 3-4 sterke kanten. *"En voor rechts?"* Verzamel 3-4 zwakke kanten. Stel de kernvraag: *"Wat hebben de zwaktes met elkaar gemeen?"* Pauze 5-7 seconden. Hint indien nodig: *"In alle gevallen — was het iets wat het systeem ÉÉRDER had gezien, of iets nieuws?"*

3. **Brug naar de definitie** (1 min) — sluit af met de kernzin: *"AI is sterk in wat hij heeft gezien. Zwak in wat hij nog niet zag. Laten we hier vier namen aan geven."*

**Materiaal:**
- [ ] Slide 4
- [ ] wb-02-buurman-sterk-zwak.md
- [ ] Bord of flip-over met twee kolommen
- [ ] Stiften
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf letterlijk op wat deelnemers zeggen.
> - De kernzin "sterk in wat hij heeft gezien" op het bord — laten staan voor fase 3 en 4.

> **Valkuil — formele namen voor de zwaktes al noemen:**
> "Bias" of "context" houden voor blok 3.

> **Differentiatie:**
> - **Gemengde groep:** Operator brengt werkvloer-zwakte, teamleider brengt organisatie-impact. Beide voeden de lijstjes.

**Antwoordmodel werkblad 2:**
- **Stap 1 (vergelijken):** Eigen vergelijking — variabel.
- **Stap 2 (twee lijstjes):** Sterk: snel, niet moe, patronen, signalen koppelen. Zwak: onbekende, context, eenzijdige data, ruis.
- **Stap 3 (gemeenschappelijke):** Vinkje 1 — allemaal nieuwe situaties die het systeem nog niet zag.
- **Stap 4 (lasersnijder zwakte):** Onbekende situatie (2mm staal) + context (wachttijd plaat) zijn beide aan te wijzen.
- **Eén zin samen:** Bijvoorbeeld "het systeem is goed in rekenen, maar zwak in zien wat ervaring leert."

**Transitie naar blok 3:** *"Vier namen, vier sterktes, vier zwaktes — plus een regel om mee te werken."*

---

### Blok 3: Handout — 4 sterktes + 4 zwaktes + halve-flessen-regel
**00:22 - 00:35** | 13 min | Kolb-fase (leerfase): theoretiseren

**Doel:** Deelnemer kent de vier sterktes en vier zwaktes formeel, plus de halve-flessen-regel als ontwikkelpad.

**Werkvorm:** Vier sterktes (4 min), vier zwaktes (4 min) — per zwakte 30 sec + voorbeeld-vraag aan groep, halve-flessen-regel (3 min), terugmapping lasersnijder (2 min).

**Instructie:**

1. **Vier sterktes markeren** (4 min) — deel wb-03 uit. Toon slide 5. *"Pak je markeerstift. Vier sterktes — markeer ze. Eén: patronen herkennen in grote hoeveelheden data. Twee: consistentie — niet moe, niet afgeleid. Drie: snelheid. Vier: signalen koppelen — meerdere metingen tegelijk."* Per sterkte één voorbeeld uit de maakindustrie noemen. *"Op deze sterktes leunen de meeste AI-toepassingen — camera-inspectie, onderhoudsvoorspelling, voorraadbestelling."*

2. **Vier zwaktes met activatie** (4 min) — toon slide 6. *"Vier zwaktes — markeer ze. Eén: onbekende situaties. Iets wat het systeem nog nooit zag, mist het. Bij de lasersnijder: 2 millimeter staal was nieuw."* Vraag de groep: *"Voorbeeld bij jullie?"* Verzamel kort. *"Twee: context. De AI weet niet dat het vandaag min 10 graden is."* Vraag: *"Voorbeeld bij jullie?"* Idem voor *drie: bias* (eenzijdige trainingsdata, bijv. uit één ploeg) en *vier: data-ruis* (slechte sensoren).

3. **Halve-flessen-regel** (3 min) — toon slide 7 met de vier-periodes-tabel. *"Behandel AI als een nieuwe goede collega. Week 1: alles dubbelchecken. Maand 1-3: steekproeven. Na 6 maanden: vertrouwen met een handvol checks per week. Altijd: bij rare uitkomsten je eigen verstand gebruiken."* Markeer: *"Geen wantrouwen — wat je met een nieuwe collega ook zou doen."*

4. **Lasersnijder terugmapping** (2 min) — *"Bij de lasersnijder: twee zwaktes speelden. Onbekende situatie (2mm) en context (wachttijd verwarmde plaat). Een ervaren operator ziet de context — het systeem niet. Dat is geen falen — dat is het gebied buiten de training."*

**Materiaal:**
- [ ] Slides 5-7
- [ ] wb-03-handout-sterk-zwak.md
- [ ] Markeerstift per deelnemer
- [ ] Tweede flip-over (halve-flessen-regel)

> **Tips voor de trainer:**
> - Per zwakte 30 sec uitleg + groepsvraag — voorkomt monoloog.
> - Halve-flessen-regel concreet maken — gebruik "nieuwe collega" als metafoor.
> - Kernzin op het bord verwijzen: "sterk in wat hij heeft gezien, zwak in wat hij nog niet zag".

> **Valkuil — vier zwaktes als statische lijst:**
> Maak het gemeenschappelijke expliciet. *"Wat hebben ze gemeen? Allemaal buiten het trainingsgebied."*

> **Valkuil — AI cynisch framen:**
> Verwijs altijd naar halve-flessen-regel. *"Geen wantrouwen — slim omgaan."*

> **Valkuil — alleen monoloog:**
> Bij elke zwakte de groep activeren met *"voorbeeld bij jullie?"* Pauze 5-7 sec.

> **Differentiatie:**
> - **MBO-4 basis:** Schrijf de vier zwaktes groot op het bord — zichtbaar tijdens fase 4.
> - **Teamleider sneller:** Vraag tussendoor: *"Welke zwakte zie je het meest bij ons systeem?"*

**Antwoordmodel werkblad 3:**
- **Markeren:** Vier sterktes + vier zwaktes.
- **Lasersnijder zwaktes:** (1) Onbekende situatie — 2mm was niet in training. (2) Context — wachttijd verwarmde plaat zat niet in optimalisatie.
- **Kernzin:** "AI is sterk in wat hij heeft gezien. Zwak in wat hij nog niet zag."

**Transitie naar blok 4:** *"Nu jouw beurt. Welk systeem ken JIJ — en welke check ga je deze week doen?"*

---

### Blok 4: Eigen werkvloer-systeem + concrete check
**00:35 - 00:45** | 10 min | Kolb-fase (leerfase): experimenteren

**Doel:** Deelnemer kiest één AI-systeem, identificeert sterkte + zwakte + formuleert één concrete check voor deze week.

**Werkvorm:** Individueel werkblad (6 min), plenaire afronding met 2-3 voorbeelden + transferopdracht (3 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit. Toon slide 8. *"Laatste 10 minuten. Kies één AI-systeem op je werkvloer. Beantwoord vijf stappen: welk systeem, welke sterkte, welke zwakte, welke check deze week, welke vraag voor IT. Houd de check KLEIN. Voorbeelden staan op het werkblad."*

2. **Individueel werken** (6 min) — zet timer op 6 minuten. Loop rond na 2 minuten. Bij vastlopers: *"Welk AI-systeem zie je dagelijks? Camera, dashboard, planning? Welke sterkte? Welke zwakte zou het grootste risico zijn?"* Bij abstracte checks: *"Wat doe je precies, wanneer, hoe lang?"*

3. **Plenaire afronding + transferopdracht** (3 min) — toon slide 9. *"Wie deelt zijn zwakte + check?"* Vang 2 of 3 voorbeelden. Toon slide 10 (transfer + logboek). *"Deze week: drie notities op één AI-systeem. Plus één concrete check. Bonus: begin een klein AI-logboek — notitie op je telefoon volstaat. Eén keer per week kort opschrijven: ging het goed of niet? Notities mee naar de volgende sessie."*

**Materiaal:**
- [ ] Slides 8-10
- [ ] wb-04-eigen-risico.md
- [ ] Pen
- [ ] Timer

> **Tips voor de trainer:**
> - Maximaal 3 voorbeelden plenair — anders loop je uit.
> - Begrens abstracte checks: "concrete check is een actie + tijdstip + duur".
> - AI-logboek als optie introduceren — geen verplichting.

> **Valkuil — check te abstract ("ik ga beter opletten"):**
> Begrens: *"Wat doe je precies, wanneer, hoe lang? Bijvoorbeeld: bij de eerstvolgende rare melding kijk ik op welke trainingsperiode het systeem werkt."*

> **Valkuil — geen tijd voor logboek-uitleg:**
> Bij uitloop: noem alleen "klein logboek op telefoon" — uitleg in trainee-versie + handout.

> **Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers: kies een van de drie voorbeeld-checks uit het werkblad.
> - **Teamleider sneller:** Bij snel klaar: *"Welke vraag stel je deze maand aan de leverancier?"* Antwoord-richting: trainingsdata, bias-rapportage.

**Antwoordmodel werkblad 4:**
- **Stap 1 (systeem):** Concreet — camera, dashboard, planning-tool.
- **Stap 2 (sterkte):** Patronen, consistentie, snelheid, of signalen koppelen — afhankelijk van systeem.
- **Stap 3 (zwakte):** Onbekende, context, bias, of data-ruis — met concrete reden.
- **Stap 4 (concrete check):** Bijvoorbeeld "bij de eerstvolgende rare melding kijk ik welke trainingsperiode" of "ik kijk twee weken of het systeem anders oordeelt in ochtend- versus middagploeg".
- **Stap 5 (vraag voor IT):** Concreet — op welke periode getraind, welk bias-onderzoek is gedaan.

**Transitie naar afsluiting:** *"Mooi werk. Eén check deze week — daar zit groei in."*

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-casus-lasersnijder | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-buurman-sterk-zwak | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout-sterk-zwak | n + 2 | A4 dubbelzijdig (4+4 + halve-flessen) |
| ☐ | wb-04-eigen-risico | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve |
| ☐ | Markeerstiften | n | Voor wb-03 |
| ☐ | Flip-over of bord | 1 | Twee kolommen sterk/zwak + kernzin |
| ☐ | Tweede flip-over | 1 | Halve-flessen-regel-tabel |
| ☐ | Dikke stiften | 2-3 | |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | Presenter-modus |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| Groep loopt uit in fase 1 (casus duurt lang) | Trainer doet vraag 2 ook hardop voor. Beperk individuele tijd tot 4 min. |
| Discussie over voorspellend onderhoud | Parkeer op flip-over. "Verdieping in module 2 (Train)." |
| Plenair delen in fase 4 lukt niet | Sticky-method: deelnemers schrijven check op een sticky en plakken op het bord. |
| Halve-flessen-regel roept weerstand op | Erken: "Het is een vuistregel — pas aan bij veiligheidskritische processen." |
| Groep is te klein (4 of minder) | Buurman-check wordt groeps-rondje. Plenaire ronde versmelt met fase 4. |

---

## Snel-overzicht

| Fase (leerfase) | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Lasersnijder-casus beoordelen | Eerste oordeel — twijfel mag |
| 2 reflecteren | Twee lijstjes + gemeenschappelijke | "Sterk in wat gezien, zwak in nieuw" |
| 3 theoretiseren | 4 sterktes + 4 zwaktes + halve-flessen | Mentaal model: trainingsgebied is grens |
| 4 experimenteren | Eigen sterkte + zwakte + concrete check | Klein begin deze week + AI-logboek |

**Slagingscriterium:** Vier sterktes + vier zwaktes benoemen + lasersnijder-zwakte correct + eigen check formuleren.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt
- [ ] Genoteerd welke checks plenair zijn gedeeld
- [ ] Genoteerd: welke vragen zijn geparkeerd
- [ ] xAPI-statements verstuurd: `experienced`, `completed`, `attempted`

---

*AIMM Curriculum | AI Fundamentals Module 1 (Gebruik) | Sterk en zwak*
*Bron: Npuls (2025). Raamwerk NL AI-Geletterdheid in het Onderwijs, p. 8.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
