# Vision-model configureren: parameters instellen — Draaiboek
*AI-Vision Module 2 (Train) | Workshop-blok 30 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan de drempelwaarde van een vision-model instellen en het effect uitleggen op recall en valse alarmen, en kan een passende keuze onderbouwen voor een specifieke situatie. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 + LO-006 (visuele inspectie) en LO-511 (data labelen) |
| **Stadium (H&B)** | Bewust bekwaam — wil zelf aan de knoppen draaien |
| **Begeleidingsstijl** | Coachen — open vragen, faciliteer eigen ontdekking |
| **Ruimte** | Clusters van 4 met laptops voor simulator (optioneel), beamer, flap-over |
| **Plek in module** | Workshop in Module 2 — leidt naar LO-513 (confusion matrix) en LO-514 (verbeteren) |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | Drempelwaarde-quiz met simulator | ervaren | 10 min |
| 00:10 - 00:18 | Duo-reflectie: dilemma eigen werkplek | reflecteren | 8 min |
| 00:18 - 00:23 | Recall, valse alarmen, testset | theoretiseren | 5 min |
| 00:23 - 00:30 | Actieplan: jouw product | experimenteren | 7 min |

**Totaal:** 30 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Test `model-lo-smart-mfg-512.html` op een laptop — werkt de simulator?
- [ ] Bedenk een productvoorbeeld uit jouw branche (spuitgietproduct, gefreesd onderdeel).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over op met as: links **streng** (veel valse alarmen), rechts **soepel** (laat door).
- [ ] Schrijf op een tweede flap-over: **"Wat is bij jullie erger: weggooien of doorlaten?"**
- [ ] Open slide 1 + simulator op de tafels (of beamer).

---

## Blok-details

### Blok 1: Drempelwaarde-quiz met simulator
**00:00 - 00:10** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer ervaart direct het effect van een drempelwaarde-keuze: meer streng = meer valse alarmen, meer soepel = defecten doorgelaten.

**Werkvorm:** Individuele oefening met werkblad wb-01-ervaren + interactieve simulator (model-lo-smart-mfg-512.html).

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 30 minuten leer je een vision-model afstellen. Aan het eind weet je hoe je de juiste streng-of-soepel keuze maakt voor jouw lijn."*

2. **Trigger** (1 min) — vraag: *"Stel je voor: een AI-camera zegt 'afkeuren' op 1 op de 5 producten. Wat denk je?"* Vang 1-2 reacties (te streng / kapot / verspilling). Reageer: *"Vandaag leer je waarom dat gebeurt en wat je eraan doet."*

3. **Werkblad uitdelen + simulator introduceren** (1 min) — deel wb-01 uit. Toon slide 2. Zeg: *"Op de simulator zie je 100 producten met bekende uitkomst. Schuif de drempelwaarde. Kijk wat er gebeurt. Schrijf op werkblad: bij welke waarde komt het beste resultaat voor jouw lijn?"*

4. **Individueel werken** (6 min) — zet timer op 6 min. Loop rond. Bij vragen: *"Wat is voor jullie erger: een goed product weggooien of een fout doorlaten?"* Geen voorzeggers.

5. **Verzamelmoment** (1 min) — *"Pen neer. We bespreken straks."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] model-lo-smart-mfg-512.html (op laptop per duo OF beamer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet zelf de simulator bedienen tenzij je beamer-only werkt.
> - Bij 'welke is de juiste?' — schud je hoofd: *"Er is geen juiste. Er is een keuze die past."*

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt, geef ankerpunt: *"Schuif eerst naar streng. Wat zie je? Schuif dan naar soepel. Wat zie je?"*
> - **MBO-4 sneller:** vraag *"Bij welke waarde verandert het effect het meest? Waarom?"*

> **Valkuil — denkt dat er een 'beste' is (vk-01):**
> Bevestig: *"Geen juiste, wel passende. Het hangt af van wat erger is bij jullie."*

> **Valkuil — 'dit is voor IT' (vk-05):**
> Erken kort, herstel: *"De drempelwaarde is een productiebeslissing. IT bouwt, jij stelt af."*

---

### Blok 2: Duo-reflectie — dilemma eigen werkplek
**00:10 - 00:18** | 8 min | Kolb-fase: reflecteren

**Doel:** Deelnemer verbindt de simulator-ervaring met de eigen werkplek: wat is bij ons erger — weggooien of doorlaten?

**Werkvorm:** Duo-reflectie met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 3.

2. **Duo's vormen** (30 sec) — *"Zoek iemand. Bespreek: wat gebeurde er toen je de drempelwaarde veranderde? En wat is bij jullie erger?"*

3. **Duo-gesprek** (5 min) — zet timer op 5 min. Loop rond. Stel verdiepende vragen:
    - *"Welke drempelwaarde koos je? Waarom?"*
    - *"Herken je dit dilemma op jullie lijn?"*
    - *"Wat is jullie ergste fout: een klant die klaagt of een goed product op de afkeurberg?"*

4. **Plenaire deel-ronde** (2 min) — toon slide 4. Vraag 2 deelnemers: *"Wat is bij jullie erger?"* Schrijf op flap-over twee voorbeelden (bv. voedingsmiddelen = weggooien beter dan doorlaten; cosmetisch = doorlaten beter dan weggooien).

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over (streng-soepel-as)
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf alleen wat de groep zegt op flap-over.
> - Tel innerlijk tot 7 na elke vraag.

> **Valkuil — recall en valse alarmen verward (vk-02):**
> Niet uitleggen — dat komt in fase 3. Wel signalen noteren voor je eigen referentie.

> **Differentiatie:**
> - **Gemengde groep:** vorm duo's MBO-3 + MBO-4. MBO-4 stelt vragen, voorziet niet.

---

### Blok 3: Recall, valse alarmen, testset
**00:18 - 00:23** | 5 min | Kolb-fase: theoretiseren

**Doel:** De ervaring uit fase 1 wordt gekoppeld aan twee getallen (recall, valse alarmen) en het testset-concept.

**Werkvorm:** Trainer-geleide handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift."*

2. **Drie begrippen** (3 min) — toon slide 5 (diagram-lo-smart-mfg-512.svg). Loop ze één voor één langs:
    - *"Recall: hoeveel échte defecten vindt het model? 9 op de 10 = 90% recall."*
    - *"Valse alarmen: hoe vaak schreeuwt het model op een goed product? 5 op 100 goede = 5%."*
    - *"Testset: 50-100 foto's met bekende uitkomst, helft goed, helft defect. Daarmee meet je deze twee getallen."*

3. **Koppeling aan eigen keuze** (1 min 30) — toon slide 6. Zeg: *"Streng = recall hoog, valse alarmen ook hoog. Soepel = recall lager, valse alarmen lager. Geen gratis lunch — kies wat erger is."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-6
- [ ] diagram-lo-smart-mfg-512.svg (op slide 5)
- [ ] Flap-over (streng-soepel-as)

> **Tips voor de trainer:**
> - Houd het tempo strak — 5 min is krap.
> - Twee getallen + één testset = klaar. Niet meer.

> **Valkuil — te diep (vk-03):**
> Geen ROC-curve, geen precision/F1. Voor MBO-4: parkeer voor LO-513.

> **Differentiatie:**
> - **MBO-3 basis:** gebruik altijd hetzelfde voorbeeld (testset 100, waarvan 10 defect).
> - **MBO-4 sneller:** noem 'precision' kort, parkeer voor LO-513.

---

### Blok 4: Actieplan — jouw product
**00:23 - 00:30** | 7 min | Kolb-fase: experimenteren

**Doel:** Deelnemer maakt een concreet plan: welke drempelwaarde voor welk product, welke testset, met welke buddy.

**Werkvorm:** Individueel actieplan + korte deelronde.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-04 uit. Toon slide 7. Zeg: *"Vier vragen: welk product? Welke voorlopige drempelwaarde? Hoeveel foto's in testset? Welke buddy?"*

2. **Individueel werken** (4 min) — zet timer op 4 min. Loop rond. Help concretiseren:
    - *"Welk product specifiek? Met welk defecttype?"*
    - *"Wat zegt je gevoel: streng of soepel? Waarom?"*
    - *"Wie kan met je meekijken bij het beoordelen?"*

3. **Korte deel-ronde** (2 min) — vraag 2 deelnemers om hun keuze te delen (max 1 min per persoon). Zoek contrast: 1 streng, 1 soepel.

4. **Afsluiting + transferopdracht** (30 sec) — toon slide 8. *"Deze week: bespreek met je leidinggevende. Maak een testset van 50 foto's. Volgende sessie: bespreek je testresultaten met de groep — LO-513."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 7-8
- [ ] Timer

> **Tips voor de trainer:**
> - Concreet maken is de competentie. Vage plannen ('praten met IT') terugsturen met *"wat ga je voorstellen?"*
> - Bewaar 30 sec voor de transferopdracht.

> **Differentiatie:**
> - **MBO-3 basis:** één product is genoeg.
> - **MBO-4 sneller:** vraag *"Hoe ga je het effect meten? Welke twee getallen ga je vergelijken?"*

> **Valkuil — actieplan vaag (vk-04):**
> Druk door tot er een product, getal en datum staat.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort fase 4 in tot 6 min door werktijd op 3 min te zetten. Sla transferopdracht nooit over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (streng-soepel-as) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over reserve | 1 vel | Voor parkeerlijst |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptops voor simulator | n/2 | Optioneel — anders alleen beamer |
| ☐ | model-lo-smart-mfg-512.html | 1 | Test vooraf |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Simulator: schuif drempelwaarde | Eigen ervaring met effect |
| 2 reflecteren | Duo: wat is erger bij ons? | Inzicht: context bepaalt keuze |
| 3 theoretiseren | Recall + valse alarmen + testset | Twee getallen als kapstok |
| 4 experimenteren | Eigen product, drempelwaarde, testset | Klaar voor LO-513 |

**Slagingscriterium:** Drempelwaarde gekozen + onderbouwd met effect op recall/valse alarmen + concreet actieplan met product, getal, datum.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: streng/soepel-balans van de groep (input voor LO-513)
- [ ] Sceptici en 'is voor IT'-deelnemers voor 1-op-1 markeren
- [ ] xAPI-statements verstuurd: `experienced` (simulator), `completed` (handout), `attempted` (actieplan)

---

*AIMM Curriculum | AI-Vision Module 2 (Train) | Vision-model configureren*
*Bron: Cruz et al. (2024). AI in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
