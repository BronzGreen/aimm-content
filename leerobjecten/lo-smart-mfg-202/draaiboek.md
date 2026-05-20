# Drempelwaarden instellen: wanneer slaat het systeem alarm? — Draaiboek
*Predictive Maintenance Module 2 (Train) | Workshop-blok 40 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan drempelwaarden voor sensoren bepalen, instellen en bijstellen — volgens de vier stappen (meten, berekenen, instellen, evalueren) en met maximaal 1 vals alarm per week. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | LO-201 afgerond — eigen basislijn-getallen idealiter meegebracht uit de transferopdracht |
| **Stadium (H&B)** | Bewust bekwaam — wil zelf kunnen ingrijpen, minder afhankelijk van technische dienst |
| **Begeleidingsstijl** | Coachen — niet voorzeggen, vragen stellen, berekening laten controleren |
| **Ruimte** | U-opstelling of clusters van 4. Beamer + scherm. Rekenmachine of telefoon-app per duo. Flap-over. |
| **Plek in module** | Workshop-blok 2 — bouwt voort op LO-201, opstap voor LO-205 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Storingsquiz: 6 sensorgrafieken — normaal/waarschuwing/alarm | ervaren | 8 min |
| 00:08 - 00:15 | Duo-reflectie: hoe bepaalde je de grens? | reflecteren | 7 min |
| 00:15 - 00:25 | Theorie: 4 stappen + voorbeeld Ahmed | theoretiseren | 10 min |
| 00:25 - 00:40 | Echte data — bereken, stel in, plan evaluatie | experimenteren | 15 min |

**Totaal:** 40 minuten — geen aparte pauze.
**Buffer:** 1 min per blok flexibel.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve.
- [ ] Print of druk de oefendata van wb-04 (100 metingen, getallen klaar voor berekening) per deelnemer.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Check: hebben de deelnemers basislijn-getallen meegenomen uit LO-201? Vraag het van tevoren via groepsapp.

### Het uur ervoor
- [ ] Leg per stoel: pen, markeerstift.
- [ ] Verzamel rekenmachines / vraag deelnemers vooraf telefoon mee te nemen.
- [ ] Schrijf op flap-over: **drempel = gemiddelde + (2 x spreiding)**.
- [ ] Hang tweede flap-over op met **"Parkeerlijst"** voor afdwalende vragen.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Storingsquiz — 6 sensorgrafieken
**00:00 - 00:08** | 8 min | Kolb-fase: ervaren

**Doel:** Deelnemer beoordeelt 6 sensorgrafieken op het oog. Maakt zichtbaar dat 'gevoel' alleen niet genoeg is — er is een rekenmethode nodig.

**Werkvorm:** Individuele oefening met werkblad wb-01-ervaren.

**Instructie:**

1. **Open de sessie** (45 sec) — toon slide 1. Zeg: *"Vorige sessie hebben jullie je eigen basislijn gemeten. Vandaag: vanaf welke waarde slaat het systeem alarm? Dat ga je zelf bepalen."*

2. **Trigger** (45 sec) — vraag: *"Wie heeft basislijn-getallen meegenomen?"* Vang 1-2 reacties. Geen oordeel als niemand. *"Geen probleem — vandaag krijg je oefendata."*

3. **Werkblad uitdelen + opdracht** (1 min) — deel wb-01 uit. Toon slide 2. Zeg: *"Zes sensorgrafieken. Per grafiek: normaal, waarschuwing of alarm? Schrijf op waarom je dat denkt. Geen rekenmachine nodig — gebruik je gevoel."*

4. **Werken** (5 min) — zet timer op 5 min. Loop rustig rond. Stel geen sturende vragen. Bij vastlopen: *"Waar kijk je naar?"*

5. **Verzamelmoment** (30 sec) — *"Pen neer. Tel je antwoorden. We bespreken zo."*

**Materiaal:**
- [ ] wb-01-ervaren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Niet voorzeggen. De waarde van fase 1 is dat duo's verschillend oordelen — daar ligt fase 2.
> - Als iemand snel klaar is: vraag *"Bij welke grafiek twijfelde je het meest? Waarom?"*
> - Houd de 4-stappen-kapstok in je achterhoofd; gebruik hem nog niet.

> **Differentiatie:**
> - **MBO-3 basis:** als iemand alle 6 leeg laat: vraag *"Welke grafiek herken je? Daar beginnen we."*
> - **MBO-4 sneller:** vraag *"Hoeveel zekerheid heb je per grafiek — 50/50 of 90/10?"* Opent de twijfeldiscussie.

> **Valkuil — deelnemer voelt zich getoetst:**
> Bevestig direct: *"Er is geen goed of fout. Het gaat om jouw beoordeling — straks zien we waar het lastig wordt."*

---

### Blok 2: Duo-reflectie — hoe bepaalde je de grens?
**00:08 - 00:15** | 7 min | Kolb-fase: reflecteren

**Doel:** Deelnemer ontdekt dat verschillende operators verschillende grenzen hebben — en dat een rekenmethode helpt.

**Werkvorm:** Duo-reflectie met werkblad wb-02-reflecteren.

**Instructie:**

1. **Werkblad uitdelen + duo's vormen** (30 sec) — deel wb-02 uit. *"Zoek een buurman."* Toon slide 3.

2. **Duo-gesprek** (4 min) — zet timer op 4 min. Drie vragen op het werkblad:
    - *"Bij welke grafiek waren jullie het oneens? Welke koos jij, welke je buurman?"*
    - *"Hoe bepaalde JIJ de grens tussen normaal en waarschuwing?"*
    - *"Wat zou er gebeuren als de drempel te laag staat? En te hoog?"*
    Loop rond. Luister naar concrete redeneringen.

3. **Plenaire deel-ronde** (2 min 30) — toon slide 4. Vraag:
    - *"Wie had moeite om de grens te bepalen? Wat maakte het lastig?"* Vang 2-3 antwoorden.
    - *"Wat zou helpen om met meer zekerheid de grens te bepalen?"* Mik op antwoord: *"Een rekenmethode."*
    - Schrijf op flap-over: 2-3 sleutelwoorden + de zin *"Gevoel is niet genoeg."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 3-4
- [ ] Flap-over voor sleutelwoorden
- [ ] Timer

> **Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke vraag. Stilte trekt antwoorden los.
> - Bij scepsis ('we kunnen toch niet zelf rekenen?'): erken, parkeer voor fase 3.
> - Schrijf op flap-over alleen wat de groep zegt.

> **Differentiatie:**
> - **Gemengde groep:** in plenaire bespreking eerst MBO-3, dan MBO-4.

> **Valkuil — duo wordt afrekening:**
> Als duo's beginnen te ruzieën over wie 'gelijk had': zeg *"Niet wie gelijk had. Wat de redenering was. Daar leren we van."*

---

### Blok 3: Theorie — 4 stappen + voorbeeld Ahmed
**00:15 - 00:25** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert de vuistregel (gemiddelde + 2x spreiding) en het 4-stappenplan kennen door koppeling aan het concrete voorbeeld van collega-operator Ahmed.

**Werkvorm:** Trainer-geleide handout-bespreking met diagram.

**Instructie:**

1. **Handout uitdelen** (30 sec) — deel wb-03 uit. *"Pak je markeerstift. Markeer wat voor jou nieuw is."*

2. **4 stappen langs** (4 min) — toon slide 5 (diagram met de 4 stappen). Loop ze één voor één langs:
    - *"Stap 1: meten. Minimaal 100 cycli onder normale omstandigheden. Verspreid over de dag."*
    - *"Stap 2: berekenen. Gemiddelde + spreiding. Vuistregel: drempel = gemiddelde + (2 x spreiding). Vangt 95% van normale variatie."*
    - *"Stap 3: instellen. Twee niveaus. Waarschuwing — geel — op 80% van de drempel. Alarm — rood — op 100%."*
    - *"Stap 4: testen en bijstellen. Minimaal 1 week. Tel valse alarmen + gemiste problemen. Drempel omhoog of omlaag."*
    Wijs naar de flap-over met de formule.

3. **Voorbeeld Ahmed** (4 min) — toon slide 6. Vertel:
    - *"Ahmed werkt op een draaibank. Trillingssensor. Hij meet 100 cycli."*
    - *"Gemiddelde 0.3 mm/s. Spreiding 0.1 mm/s. Zijn drempel: 0.3 + (2 x 0.1) = 0.5 mm/s."*
    - *"Eerste week: 12 valse alarmen. Te veel."*
    - *"Wat doet hij? Drempel naar 0.8. Plus vertraging van 10 sec — alarm pas als de waarde langer dan 10 sec boven 0.8 zit."*
    - *"Resultaat: 1 vals per week. EN het systeem detecteert succesvol een slijtend lager twee dagen voor geplande vervanging."*
    - Pauze. *"Twee dingen om te onthouden. Een: de eerste drempel is bijna NOOIT goed. Twee: bijstellen is geen falen, dat IS het werk."*

4. **Vragen** (1 min 30) — toon slide 7. *"Vragen over de 4 stappen of over Ahmed?"* Beantwoord kort, parkeer afdwaalende vragen.

**Materiaal:**
- [ ] wb-03-theoretiseren.md (per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 5-7
- [ ] diagram-lo-smart-mfg-202.svg (op slide 5)
- [ ] Flap-over (formule + parkeerlijst)

> **Tips voor de trainer:**
> - Houd het bij ÉÉN voorbeeld (Ahmed) en ÉÉN formule. Niet wisselen tussen voorbeelden.
> - Bij vraag over standaarddeviatie / sigma: gebruik woord 'spreiding'. Niet sigma.
> - Na het Ahmed-verhaal: stilte van 3 sec. Laat het landen.

> **Differentiatie:**
> - **MBO-3 basis:** alleen formule + Ahmed. Niet uitweiden naar 3x spreiding of vertraging-finesse.
> - **MBO-4 sneller:** vraag *"Waarom precies 2x spreiding? Wanneer zou 3x beter zijn?"* (= kritische processen). Noem bron AIMM Competentieframework v0.1.

> **Valkuil — te wiskundig (sigma, normaalverdeling):**
> Houd 'spreiding' als alledaags woord. *"Gemiddeld hoeveel wijken waarden af. Niet ingewikkelder."*

---

### Blok 4: Echte data — bereken, stel in, plan evaluatie
**00:25 - 00:40** | 15 min | Kolb-fase: experimenteren

**Doel:** Deelnemer voert de 4 stappen zelfstandig uit op echte data en maakt een actieplan voor evaluatie na 2 weken.

**Werkvorm:** Individuele oefening met actieplan-werkblad wb-04-experimenteren.

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit (bevat 100 metingen). Toon slide 8. Zeg:
    - *"Op werkblad: 100 metingen van een trillingssensor. Bereken het gemiddelde. Bereken de spreiding (er staat een hint hoe). Bepaal je drempel. Stel waarschuwing en alarm in. Schrijf actieplan voor evaluatie na 2 weken."*

2. **Werken** (10 min) — zet timer op 10 min. Loop rond. Coach-modus:
    - *"Waar ben je? Hoever zijn jullie?"*
    - *"Klopt je gemiddelde? Hoe heb je dat gecheckt?"*
    - *"En je spreiding — hoe heb je die bepaald?"*
    - *"Wat is je drempel? Klopt dat met de formule?"*
    Niet voorzeggen. Bij berekening fout: *"Reken het nog eens hardop."*

3. **Plenaire deel-ronde** (3 min) — toon slide 9. Vraag 2-3 deelnemers:
    - *"Wat was jouw drempel?"* Vang 2 antwoorden + check klopt met formule.
    - *"Wanneer ga je evalueren?"* Vang 1-2 antwoorden — moet concrete datum zijn.

4. **Transferopdracht** (1 min) — toon slide 10. Zeg:
    - *"Deze week: kies één sensor op JOUW machine. Gebruik je basislijn uit LO-201 of meet 100 cycli. Bereken de drempel. Stel hem in — vraag hulp aan de technische dienst voor de instelling als nodig. Plan evaluatie na 2 weken."*
    - *"En vraag een collega om hetzelfde te doen voor een andere sensor. Vergelijk jullie aanpak."*

**Materiaal:**
- [ ] wb-04-experimenteren.md met 100 oefenmetingen (per deelnemer)
- [ ] Pen + rekenmachine per deelnemer (of telefoon-app)
- [ ] Slides 8-10
- [ ] Timer

> **Tips voor de trainer:**
> - Coach. Niet voorzeggen. Berekenfouten zijn leermomenten.
> - Bewaar 1 minuut voor transferopdracht — niet overslaan.
> - Bij snel klaar: *"En als je drempel te laag blijkt — wat doe je dan?"* (= bijstellen, niet afhaken).

> **Differentiatie:**
> - **MBO-3 basis:** alleen drempel berekenen + actieplan. Niet ook waarschuwing-niveau berekenen.
> - **MBO-4 sneller:** vraag *"Hoe zou je een vertraging van 10 sec instellen?"* + *"Wat als je twee sensoren wilt combineren?"* = bruggetje naar LO-205.

> **Valkuil — operator durft de drempel niet zelf in te stellen:**
> *"Je hebt de berekening. De technische dienst doet alleen de knop. Maar de keus is van jou."* Verwijs naar Ahmed.

> **Valkuil — geen tijd voor afsluiting:**
> Als blok 3 is uitgelopen: kort werktijd in tot 8 min, plenaire deel-ronde tot 2 min. Sla transferopdracht NOOIT over.

---

## Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-ervaren.md | n + 2 | A4 enkelzijdig (6 grafieken) |
| ☐ | wb-02-reflecteren.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-theoretiseren.md | n + 2 | A4 dubbelzijdig (4 stappen + Ahmed) |
| ☐ | wb-04-experimenteren.md | n + 2 | A4 dubbelzijdig (100 metingen + actieplan) |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout |
| ☐ | Rekenmachines | per duo | OF telefoon-app |
| ☐ | Flap-over (formule) | 1 vel | drempel = gemiddelde + (2 x spreiding) |
| ☐ | Flap-over (parkeerlijst) | 1 vel | Voor afdwaalende vragen |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus |

n = aantal deelnemers

---

## Snel-overzicht

| Fase | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | 6 sensorgrafieken op gevoel beoordelen | Inzicht: gevoel is niet genoeg |
| 2 reflecteren | Duo: hoe bepaalde je de grens? | Behoefte aan rekenmethode |
| 3 theoretiseren | 4 stappen + voorbeeld Ahmed | Vuistregel: gemiddelde + 2x spreiding |
| 4 experimenteren | Echte data berekenen + actieplan | Eigen drempel + evaluatiedatum |

**Slagingscriterium:** Berekening correct + actieplan ingevuld met datum.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of gefotografeerd (learning analytics)
- [ ] Genoteerd: wie heeft welke sensor + drempel toegezegd? (volgmoment LO-205)
- [ ] Sceptici genoteerd voor 1-op-1 in volgende sessie
- [ ] xAPI-statements verstuurd: `experienced` (quiz), `attempted` (berekening), `completed` (actieplan)

---

*AIMM Curriculum | Predictive Maintenance Module 2 (Train) | Drempelwaarden instellen*
*Bron: AIMM Competentieframework v0.1 (drempelwaarden). Sesana et al. (2024). Artificial Intelligence in Manufacturing.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
