# Eigen productiedata verzamelen en beoordelen — Draaiboek
*Predictive Maintenance Module 3 (Op Maat) | Workshop-blok 55 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan een data-audit uitvoeren op de eigen machine, sensoren inventariseren, datakwaliteit beoordelen op vier criteria, en bepalen of er minimaal 3 maanden historische data beschikbaar is. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 + 2 afgerond. Begrijpt PM, kan anomaliescores lezen, geoefend met voorbeelddata. |
| **Stadium (H&B)** | Bewust bekwaam — kan zelfstandig de eigen lijn analyseren |
| **Begeleidingsstijl** | Coachen — open vragen, geen voorzeggers |
| **Ruimte** | Clusters van 4, beamer, flap-over, ruimte voor duo-werk |
| **Plek in module** | Eerste workshop-blok in Module 3 — opstap naar LO-504 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Eigen machine verkennen: sensoren tellen | ervaren | 15 min |
| 00:15 - 00:30 | Duo-uitwisseling: wat viel op? | reflecteren | 15 min |
| 00:30 - 00:40 | Vier criteria voor datakwaliteit | theoretiseren | 10 min |
| 00:40 - 00:55 | Actieplan: wat heb ik nog nodig? | experimenteren | 15 min |

**Totaal:** 55 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Bedenk één voorbeeldmachine uit jouw branche (spuitgieten, CNC, freesbank).
- [ ] Bekijk vooraf welke deelnemers een 'oude' machine hebben — bereid je voor op vk-04.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift, scoringsformulier (wb-01).
- [ ] Hang flap-over op met de 4 criteria (volledigheid, consistentie, nauwkeurigheid, tijdstempel).
- [ ] Schrijf op een tweede flap-over: links **"Vragen voor later"**, rechts **"Vraag technische dienst"**.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Eigen machine verkennen — sensoren tellen
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** Deelnemer brengt zelfstandig de sensoren op de eigen machine in kaart. Dit wordt de basis voor de hele audit.

**Werkvorm:** Individuele inventarisatie op werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"Module 3 begint nu echt voor jou. We gaan van voorbeelddata naar jouw machine. De komende 55 min check je: heb ik genoeg goede data om een pilot te starten?"*

2. **Trigger** (1 min) — vraag: *"Hoeveel sensoren denk je dat er op jouw machine zitten?"* Vang 2-3 ruwe schattingen. Schrijf ze op flap-over (3? 8? 20?). Reageer: *"Aan het eind van deze sessie weet je het preciezer."*

3. **Werkblad uitdelen + introduceren** (1 min) — deel wb-01 uit. Toon slide 2. Zeg: *"Loop in gedachten langs je machine. Welke sensoren zitten erop? Waar zitten ze? Werken ze? Wordt de data opgeslagen? Hoe lang? 12 minuten."*

4. **Individueel werken** (12 min) — zet timer op 12 min. Loop rond als coach. Stel open vragen:
    - *"Weet je zeker dat er geen sensoren in de PLC zitten die je niet ziet?"*
    - *"Heb je de technische dienst weleens gevraagd?"*
    - *"Wat staat er op je HMI?"*
    Geef geen antwoorden.

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voor- of meedenken. Het werkblad is een eigen-onderzoek.
> - Als iemand snel klaar is: vraag *"Ken je ook de meetfrequentie van die sensoren?"*

> **Differentiatie:**
> - **MBO-3 basis:** als iemand vastloopt, geef ankerpunt: *"Wat staat er op je bedieningspaneel?"*
> - **MBO-4 sneller:** vraag *"Welke sensor zou voor jou de meest interessante zijn voor een PM-pilot? Waarom?"*

> **Valkuil — 'wij hebben geen data' (vk-04):**
> Bevestig: *"Bijna altijd zit er meer dan je denkt — kijk naar je teller, je bedrijfsuren, je storingslog."* Liever 3 sensoren dan nul.

> **Valkuil — operator weet sensoren niet (vk-01):**
> *"Wat je ziet is een goed begin. De rest komt deze sessie en deze week erbij."*

---

### Blok 2: Duo-uitwisseling — wat viel op?
**00:15 - 00:30** | 15 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt patronen door zijn audit te vergelijken met die van een collega. Inzicht: wat ik niet weet, weet hij misschien wel.

**Werkvorm:** Duo-gesprek met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-02 uit. Toon slide 3.

2. **Duo's vormen** (30 sec) — *"Zoek iemand met een andere machine. Vergelijk jullie scoringsformulieren."*

3. **Duo-gesprek** (10 min) — zet timer op 10 min. Loop rond. Stel verdiepende vragen:
    - *"Wat ontdekte je dat je niet verwachtte?"*
    - *"Wat is bij jullie hetzelfde, wat anders?"*
    - *"Heeft je buurman tips voor jou? Andersom?"*

4. **Plenaire deel-ronde** (3 min) — toon slide 4. Vraag 2 duo's om hun grootste ontdekking te delen (max 1 min per duo). Vat samen op flap-over: 3-4 sleutelwoorden (PLC-data, opslagfrequentie, oude machine).

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Eigen ingevuld scoringsformulier (wb-01)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Schrijf op flap-over alleen wat de groep zegt.
> - Tel innerlijk tot 7 na elke vraag. Stilte = denken.
> - Bij sceptische opmerking: erken, parkeer voor fase 4.

> **Differentiatie:**
> - **Gemengde groep:** vorm duo's MBO-3 + MBO-4. MBO-4 luistert eerst.

---

### Blok 3: Vier criteria voor datakwaliteit
**00:30 - 00:40** | 10 min | Kolb-fase: theoretiseren

**Doel:** De ervaring uit fase 1 wordt gekoppeld aan vier objectieve criteria voor datakwaliteit.

**Werkvorm:** Trainer-geleide handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **Vier criteria** (7 min) — toon slide 5 (diagram-lo-smart-mfg-502.svg). Loop ze één voor één langs met een fabrieksvoorbeeld:
    - *"Volledigheid: meet hij elke 5 min, of soms een week niets? Een gat van een week = niet volledig."*
    - *"Consistentie: temperatuur altijd in graden Celsius, niet soms in Fahrenheit. Frequentie altijd 1 per minuut, niet soms 1 per uur."*
    - *"Nauwkeurigheid: kalibratie. Een nieuwe sensor moet je vergelijken met de oude voordat je hem vertrouwt."*
    - *"Tijdstempel: PLC-tijd, sensortijd en ERP-tijd op elkaar afgestemd. Anders kun je data niet koppelen."*
    Wijs naar de flap-over.

3. **Koppeling aan eigen werkblad** (2 min 30) — toon slide 6. Vraag: *"Kijk naar je eigen scores uit fase 1. Waar scoor je goed? Waar niet?"* Vang 2-3 reacties.

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-6
- [ ] diagram-lo-smart-mfg-502.svg (op slide 5)
- [ ] Flap-over (vier criteria)

> **Tips voor de trainer:**
> - Geef bij elk criterium een voorbeeld uit hetzelfde scenario (bijv. spuitgietmachine).
> - Niet alle vier diepgaand uitleggen — visueel + voorbeeld is genoeg.

> **Valkuil — criteria voelen abstract (vk-02):**
> Liever 4 voorbeelden dan 4 definities. Als iemand niets herkent: *"Pakt jouw machine elke meting op? Of zit er een gat?"*

> **Differentiatie:**
> - **MBO-3 basis:** gebruik altijd hetzelfde voorbeeld (spuitgietmachine).
> - **MBO-4 sneller:** noem 'data drift' (data verandert in tijd). Vraag: *"Zou jouw data van 2 jaar geleden nog kloppen?"*

---

### Blok 4: Actieplan — wat heb ik nog nodig?
**00:40 - 00:55** | 15 min | Kolb-fase: experimenteren

**Doel:** Deelnemer maakt een concreet plan: welke data ontbreekt, wie kan helpen, wanneer is de actie klaar.

**Werkvorm:** Individueel actieplan + duo-feedback.

**Instructie:**

1. **Werkblad uitdelen** (30 sec) — deel wb-04 uit. Toon slide 7. Zeg: *"Vier vragen: wat ontbreekt? Wie kan helpen? Wanneer ga je het regelen? Hoe weet je dat je klaar bent?"*

2. **Individueel werken** (10 min) — zet timer op 10 min. Loop rond. Help concretiseren:
    - *"Welke specifieke sensor mis je?"*
    - *"Heb je de technische dienst al een naam? Iemand van IT?"*
    - *"Is vrijdag een realistische datum?"*

3. **Duo-feedback** (3 min 30) — *"Laat je buurman je plan lezen. Is het haalbaar? Mist er iets?"* Loop rond. Bij vage plannen: *"Welke sensor specifiek? Welke vraag stel je?"*

4. **Afsluiting + transferopdracht** (1 min) — toon slide 8. *"Deze week: ga langs je machine. Praat met de technische dienst. Vul je actieplan aan. Volgende sessie (LO-504): van pilot naar productie. Met deze data-audit als startpunt."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 7-8
- [ ] Timer

> **Tips voor de trainer:**
> - Concreet maken is de competentie. Vage plannen ('praten met IT') terugsturen.
> - Bij twijfel: *"Wat is de meest waarschijnlijke faalmodus van jouw machine? Welke sensor zit daar het dichtst bij?"*

> **Differentiatie:**
> - **MBO-3 basis:** één actie is genoeg.
> - **MBO-4 sneller:** vraag *"Hoe zou je de data labelen voor een model? Welk type faal noteer je?"*

> **Valkuil — actieplan blijft vaag (vk-03):**
> Stel doorvragen tot er een concrete naam, sensor en datum staat. Liever 1 concrete actie dan 5 vage.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort fase 4 in tot 12 min door werktijd op 8 min te zetten. Sla transferopdracht nooit over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 enkelzijdig |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Flap-over (vier criteria) | 1 vel | Vooraf voorbereid |
| ☐ | Flap-over reserve | 1 vel | Voor parkeerlijst |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Inventariseer sensoren eigen machine | Eerste data-overzicht |
| 2 reflecteren | Vergelijk met collega | Inzicht: ik weet meer / minder dan ik dacht |
| 3 theoretiseren | Vier criteria datakwaliteit | Audit-kapstok |
| 4 experimenteren | Actieplan met concrete naam + datum | Klaar voor LO-504 |

**Slagingscriterium:** Sensoren benoemd + datakwaliteit op vier criteria + concreet actieplan met naam, sensor en datum.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: welke sensoren / hiaten kwamen op? (input voor LO-504)
- [ ] Sceptici ('wij hebben geen data') voor 1-op-1 markeren
- [ ] xAPI-statements verstuurd: `experienced` (audit), `completed` (handout), `mastered` (actieplan)

---

*AIMM Curriculum | Predictive Maintenance Module 3 (Op Maat) | Eigen productiedata verzamelen en beoordelen*
*Bron: Cruz et al. (2024). Artificial Intelligence in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
