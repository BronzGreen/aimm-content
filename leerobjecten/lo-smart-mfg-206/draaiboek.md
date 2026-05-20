# Sensordata interpreteren met SHAP — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 25 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan een SHAP-grafiek lezen, de top-3 sensoren benoemen, ze groeperen per systeem en de juiste eerste actie kiezen. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Basis predictive maintenance. Kent anomaliescore. Heeft eerder met dashboards gewerkt. |
| **Stadium (H&B)** | Bewust bekwaam — kent de machine, leert nu een nieuw hulpmiddel |
| **Begeleidingsstijl** | Coachen — open vragen, geen voorzeggers |
| **Ruimte** | U-opstelling of clusters van 4, beamer, flap-over |
| **Plek in module** | Workshop-blok in Module 2 — bouwt op LO-205, leidt naar LO-207 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Storingsquiz: 3 SHAP-grafieken | ervaren | 8 min |
| 00:08 - 00:15 | Duo-reflectie: vergelijk je antwoorden | reflecteren | 7 min |
| 00:15 - 00:20 | 5-stappenplan + vuistregeltabel | theoretiseren | 5 min |
| 00:20 - 00:25 | Actieplan: jouw eerstvolgende melding | experimenteren | 5 min |

**Totaal:** 25 minuten — geen aparte pauze (workshop-blok).
**Buffer:** half minuut per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bedenk één voorbeeldmachine uit jouw branche (CNC, freesbank, spuitgietmachine).

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Hang flap-over zichtbaar op met de 5-stappenkapstok (lezen → groeperen → richting → oorzaak → actie).
- [ ] Schrijf op een tweede flap-over: links **"Vragen voor later"**, rechts **"SHAP = vingerwijzing, niet conclusie"**.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Storingsquiz — 3 SHAP-grafieken
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer geeft een eigen oordeel op 3 SHAP-grafieken. Die ervaring wordt het ankerpunt voor het stappenplan in fase 3.

**Werkvorm:** Individuele quiz met werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 25 minuten leer je een SHAP-grafiek lezen. Tegen het eind weet je in 5 stappen waar je moet beginnen met zoeken bij een anomaliemelding."*

2. **Trigger** (30 sec) — vraag: *"Wat doe jij nu als er een anomaliemelding komt op je machine?"* Vang 1-2 reacties. Reageer alleen met *"herkenbaar"*.

3. **Werkblad uitdelen + introduceren** (30 sec) — deel wb-01 uit. Toon slide 2. Zeg: *"Drie casussen — drie SHAP-grafieken. Lees per grafiek: welke sensor draagt het meest bij? Welk systeem? Wat is je eerste actie?"*

4. **Individueel werken** (5 min) — zet timer op 5 min. Loop rustig rond. Stel geen sturende vragen. Bij vastloper: *"Welke sensor staat bovenaan? Wat zegt het percentage?"*

5. **Verzamelmoment** (1 min) — *"Pen neer. We bespreken straks — niet nu al delen."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voorzeggen. De waarde zit erin dat duo's verschillend oordelen.
> - Als iemand alle 3 binnen 2 min klaar heeft: vraag *"Schrijf bij elke casus ook één twijfel op."*

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt, geef het ankerpunt: *"Lees de top-1, dan de top-2, dan welke samen horen."*
> - **MBO-4 sneller:** vraag *"Welke informatie mis je in de grafiek om een echte beslissing te nemen?"*

> **Valkuil — deelnemer kent SHAP niet uit eigen dashboard:**
> Bevestig: *"Stel je voor dat je dit zou zien — hoe zou je het lezen?"* Niet uitleggen wat het juiste antwoord is.

---

### Blok 2: Duo-reflectie — vergelijk je antwoorden
**00:08 - 00:15** | 7 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt dat het lezen van een SHAP-grafiek niet eenduidig is — en dat groeperen per systeem (stap 2) helpt om er greep op te krijgen.

**Werkvorm:** Duo-gesprek met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 3.

2. **Duo's vormen** (30 sec) — *"Zoek iemand met wie je nog niet gesproken hebt. Vergelijk je antwoorden van de quiz."*

3. **Duo-gesprek** (4 min) — zet timer op 4 min. Loop rond. Luister. Stel verdiepende vragen:
    - *"Bij welke casus verschilden jullie het meest?"*
    - *"Hoe heb jij de top-1 gekozen?"*
    - *"Welke sensoren hoorden voor jou bij elkaar?"*

4. **Plenaire deel-ronde** (2 min) — toon slide 4. Vraag:
    - *"Bij welke casus verschilden jullie het meest? Waarom?"* Vang 2 antwoorden.
    - *"Welke sensoren horen voor jullie bij elkaar?"* Schrijf 3-4 sleutelwoorden op flap-over (spilsysteem, koelsysteem, voedingssysteem). Zeg dan: *"Dit is precies stap 2 van het stappenplan dat zo komt."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf alleen wat de groep zegt — niet jouw lijstje.
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden los.
> - Bij sceptische opmerking ('SHAP zegt het toch zelf'): erken, parkeer voor fase 3.

> **Valkuil — SHAP voelt als orakel:**
> Bevestig: *"SHAP geeft de getallen, jij geeft de richting."* Schrijf op flap-over: SHAP = vingerwijzing.

> **Differentiatie:**
> - **Gemengde groep:** vorm duo's MBO-3 + MBO-4. Bewaak: MBO-4 luistert eerst, deelt daarna.

---

### Blok 3: 5-stappenplan + vuistregeltabel
**00:15 - 00:20** | 5 min | Kolb-fase: theoretiseren

**Doel:** De ervaring uit fase 1 wordt gekoppeld aan het 5-stappenplan en de vuistregeltabel.

**Werkvorm:** Trainer-geleide handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **5-stappenplan** (3 min) — toon slide 5 (diagram-lo-smart-mfg-206.svg). Loop ze één voor één langs:
    - *"Stap 1: lees — welke sensor staat bovenaan?"*
    - *"Stap 2: groepeer — welke sensoren horen samen in een systeem?"*
    - *"Stap 3: richting — te hoog, te laag, of normaal?"*
    - *"Stap 4: oorzaak — vuistregeltabel geeft de meest waarschijnlijke."*
    - *"Stap 5: actie — check, meld, of grijp in."*
    - Wijs naar de flap-over-kapstok.

3. **Vuistregeltabel + koppeling aan quiz** (1 min 30) — toon slide 6. Vertel:
    - *"Kijk naar casus 1 op je werkblad. Spiltemperatuur hoog samen met trillingen — dat hoort bij het spilsysteem. Vuistregel: koeling check + lager toerental."*
    - Bevestig: *"Het stappenplan vervangt het 'ik kijk maar wat'. Het werkt voor élke SHAP-grafiek."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-6
- [ ] diagram-lo-smart-mfg-206.svg (op slide 5)
- [ ] Flap-over (5-stappenkapstok)

> **Tips voor de trainer:**
> - Houd het tempo strak — 5 min is krap, geen ruimte voor uitweidingen.
> - Bij vraag over Shapley values of cooperative game theory: parkeer.
> - Verwijs steeds terug naar wat de groep al gezegd heeft in fase 2.

> **Valkuil — te technisch:**
> Houd het bij visuele uitleg. Voor MBO-3: 'het percentage zegt hoeveel deze sensor bijdraagt.'

> **Differentiatie:**
> - **MBO-3 basis:** gebruik altijd hetzelfde voorbeeld (casus 1, freesmachine). Niet wisselen.
> - **MBO-4 sneller:** noem term 'feature attribution', parkeer voor LO-207.

---

### Blok 4: Actieplan — jouw eerstvolgende melding
**00:20 - 00:25** | 5 min | Kolb-fase: experimenteren

**Doel:** Deelnemer vertaalt het stappenplan naar één concrete actie bij de eerstvolgende anomaliemelding op de eigen machine.

**Werkvorm:** Individueel actieplan + korte deelronde.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-04 uit. Toon slide 7. Zeg: *"Drie vragen: welke machine? Welke sensor geeft bij jou vaak problemen? Wat is je eerste actie als die in de top-3 staat?"*

2. **Individueel werken** (3 min) — zet timer op 3 min. Loop rond. Help concretiseren:
    - *"Welke machine zit op jouw lijn?"*
    - *"Welke sensor zit er meestal achter een storing? Spil, koeling, voeding?"*

3. **Korte deel-ronde** (1 min) — vraag 2 deelnemers om hun actie kort te delen (max 30 sec).

4. **Afsluiting + transferopdracht** (30 sec) — toon slide 8. *"Deze week: bij de eerstvolgende anomaliemelding gebruik je het 5-stappenplan. Noteer je bevinding in de werkorder. Volgende sessie: zelf grenswaarden bepalen — LO-207."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 7-8
- [ ] Timer

> **Tips voor de trainer:**
> - Concreet maken is de competentie. Vage actieplannen ('ik ga SHAP gebruiken') terugsturen met *"welke sensor specifiek?"*
> - Bewaar 30 sec voor de transferopdracht — niet overslaan.

> **Differentiatie:**
> - **MBO-3 basis:** één actie is genoeg.
> - **MBO-4 sneller:** vraag *"Welke sensor zou volgens jou vaak in de top-3 staan maar nooit op het dashboard verschijnt?"* — opent de deur naar LO-207.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort fase 4 in tot 4 min door werktijd op 2 min te zetten. Sla transferopdracht nooit over.

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
| ☐ | Flap-over (5-stappenkapstok) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over reserve | 1 vel | Voor parkeerlijst |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 3 SHAP-grafieken individueel beoordelen | Eigen oordeel als startpunt |
| 2 reflecteren | Duo: waar verschilden jullie? | Inzicht: groeperen helpt |
| 3 theoretiseren | 5-stappenplan + vuistregeltabel | Stappen als kapstok |
| 4 experimenteren | Eerstvolgende melding op eigen machine | Concrete transfer |

**Slagingscriterium:** Top-3 sensoren benoemen + per systeem groeperen + juiste eerste actie kiezen.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: welke sensoren noemden deelnemers? (input voor LO-207)
- [ ] Sceptici genoteerd voor 1-op-1 in volgende sessie
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `completed` (handout), `attempted` (actieplan)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | Sensordata interpreteren met SHAP*
*Bron: Lundberg & Lee (2017). SHAP. + Cruz et al. (2024). AI in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
