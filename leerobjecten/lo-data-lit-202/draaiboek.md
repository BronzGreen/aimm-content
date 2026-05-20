# Datakwaliteit beoordelen — drie checks die je zelf kunt doen — Draaiboek
*Data Literacy Module 2 (Train) | Workshop-blok 30 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer voert drie datakwaliteitschecks (volledigheid, consistentie, actualiteit) zelfstandig uit op een productiedataset en geeft een onderbouwd stoplicht-oordeel. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen, B1 |
| **Voorkennis** | Module 1 (Gebruik) afgerond — kent data-typen en weet waarom datakwaliteit telt |
| **Stadium (H&B)** | Bewust bekwaam — kent het concept, oefent nu de procedure |
| **Begeleidingsstijl** | Coachen — weinig sturing, veel ondersteuning |
| **Ruimte** | Clusters van 2-4, beamer, flap-over met drie kolommen voorgemarkeerd |
| **Plek in module** | Workshop-blok 2 — bouwt op lo-data-lit-201, leidt naar lo-data-lit-203 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:10 | Drie checks zelf uitvoeren op voorbeelddataset | ervaren | 10 min |
| 00:10 - 00:18 | Duo-reflectie: wat zag je, wat was lastig? | reflecteren | 8 min |
| 00:18 - 00:25 | Drie checks expliciet maken — vuistregels en stoplicht | theoretiseren | 7 min |
| 00:25 - 00:30 | Actieplan eigen werkvloer | experimenteren | 5 min |

**Totaal:** 30 minuten — geen aparte pauze (workshop-blok).
**Buffer:** 1 min flexibel per blok; gebruik voor doorvragen in fase 2 of opvang in fase 4.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 (n + 2 reserve per stuk).
- [ ] Print de voorbeelddataset spuitgieten (25 rijen, A4, n + 5 reserve).
- [ ] Bereid flap-over voor: drie kolommen **VOLLEDIGHEID** | **CONSISTENTIE** | **ACTUALITEIT**.
- [ ] Open `presentatie.slidev.md` op je laptop en test met de beamer.
- [ ] Lees `ko-data-lit-202.yaml` door — zorg dat de drie vuistregels paraat zijn.

### Het uur ervoor
- [ ] Hang de flap-over zichtbaar voor de groep.
- [ ] Leg per stoel: pen, voorbeelddataset, werkblad wb-01.
- [ ] Houd wb-02, wb-03, wb-04 apart — uitdelen pas bij start van het blok.
- [ ] Markeerstiften groen/oranje/rood per duo klaarleggen.
- [ ] Open slide 1.

---

## Blok-details

### Blok 1: Drie checks zelf uitvoeren — voorbeelddataset
**00:00 - 00:10** | 10 min | Kolb-fase: ervaren

**Doel:** Deelnemer voert de drie checks individueel uit op een voorbeelddataset uit een spuitgieterij. Geen theorie vooraf — het gaat om eigen ontdekking.

**Werkvorm:** Individuele werkblad-oefening met dataset.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Geef de feed-up: *"In Module 1 leerde je dat data overal zit. Vandaag leer je in 30 minuten of die data te vertrouwen is. We doen drie checks — volledigheid, consistentie, actualiteit. Geen theorie eerst. Je voert ze direct uit op een dataset uit een spuitgieterij. Daarna kijken we wat er onder zit."*

2. **Toon slide 2** (30 sec) — de drie checks groot in beeld:
    - **Volledigheid** — is de dataset compleet?
    - **Consistentie** — kloppen de waarden?
    - **Actualiteit** — hoe oud is de data?

3. **Deel de voorbeelddataset uit** (30 sec). Zeg: *"Voor je ligt productiedata van een spuitgietmachine. 25 batches. Vijf kolommen: batchnummer, datum, cyclustijd, afkeur, operator. Pak ook werkblad 1 erbij."*

4. **Doe alle drie de checks** (8 min) — zet timer op 8 min. *"Doe alle drie de checks individueel. Schrijf op wat je vindt. Het mag op gevoel — er is geen perfect antwoord. Ik loop rond."*

5. **Loop rond, COACH met vragen, geef GEEN antwoorden:**
    - *"Wat zie je in deze kolom?"*
    - *"Hoeveel cellen zijn leeg — tel even?"*
    - *"Welke eenheid staat hier? En hier?"*
    - *"Hoe oud is de laatste rij?"*

**Materiaal:**
- [ ] Voorbeelddataset spuitgieten (1 per deelnemer)
- [ ] wb-01-ervaren.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slides 1-2
- [ ] Timer

> **Tips voor de trainer:**
> - Loop rond, MAAR ga niet bij iemand zitten. Korte coach-momenten van 30 sec per deelnemer.
> - Geef GEEN antwoord op 'klopt dit?' — vraag terug: *"Wat denk JIJ?"*
> - Als iemand vastloopt na 3 min: geef ÉÉN check tegelijk. *"Doe nu eerst alleen volledigheid."*

> **Differentiatie:**
> - **MBO-3 basis:** print de drie vuistregels op een sticker die op tafel ligt: *Tellen wat leeg is / Kijken of het klopt / Kijken hoe oud het is*. Stuk-voor-stuk verlaagt de drempel.
> - **MBO-4 sneller:** vraag *"Welke check zou bij JOUW dataset op het werk de grootste blinde vlek zijn?"*

> **Valkuil — verlamde deelnemer:**
> Iemand zit 5 min met pen in hand zonder iets op te schrijven. Geef richting via een concrete tel-opdracht: *"Tel even kolom 3 — hoeveel cellen zijn leeg?"* Concrete actie haalt de drempel weg.

> **Plan B:**
> - **Te weinig tijd (10 min niet gehaald):** stop bij 8 min, vat samen wat je rondlopend hebt gehoord. Verschuif de tijd uit fase 4.
> - **Online sessie:** stuur de dataset als gedeeld scherm of PDF. Werkblad in chat als foto. Duo's in breakout rooms.

---

### Blok 2: Duo-reflectie — wat zag je, wat was lastig?
**00:10 - 00:18** | 8 min | Kolb-fase: reflecteren

**Doel:** Deelnemer vergelijkt eigen bevindingen met die van een collega. Patronen herkennen — niet 'goed of fout', maar wat valt op?

**Werkvorm:** Duo-reflectie met werkblad.

**Instructie:**

1. **Deel werkblad 2 uit** (30 sec). Zeg: *"Pak een buurman. Vergelijk wat je hebt gevonden. Drie vragen op het werkblad: wat zag je, wat was lastig, wat verraste je?"*

2. **Toon slide 4** (30 sec) — de drie reflectievragen.

3. **Duo-gesprek** (5 min) — zet timer op 5 min. Loop rond. Luister mee. Verzamel 2-3 sterke observaties voor de plenaire ronde. Stel doorvragen waar het stokt:
    - *"Wat denk je dat er gebeurd is in die batches met afkeur 200%?"*
    - *"Heb je dit type fout ook op je eigen werkvloer gezien?"*

4. **Plenaire deel-ronde** (2 min) — toon slide 5. Vraag:
    - *"Wat viel er op bij volledigheid?"* — vang 1-2 voorbeelden.
    - *"Wat bij consistentie?"* — vang 1-2.
    - *"Wat bij actualiteit?"* — vang 1-2.
    - Schrijf 1-2 sleutelwoorden per kolom op de flap-over (lege cellen, typfouten, oude data).

**Materiaal:**
- [ ] wb-02-reflecteren.md (1 per deelnemer)
- [ ] Slides 4-5
- [ ] Flap-over (drie kolommen)
- [ ] Stiften zwart + drie kleuren

> **Tips voor de trainer:**
> - In de plenaire ronde: schrijf alleen wat de groep zegt — niet wat jij denkt dat het juiste antwoord is.
> - Als iemand zegt *"ik heb niks gevonden"*: vraag *"Welke kolom heb je het langst naar gekeken?"* Daar zit de eerste observatie.
> - Tel innerlijk tot 5 na elke vraag. Stilte trekt antwoorden los.

> **Valkuil — discussie domineert:**
> Twee deelnemers blijven hangen op één rare waarde. Bedank, parkeer: *"Goeie vondst — schrijf hem op. Doe nu eerst de andere twee checks."*

> **Valkuil — MBO-4 stuurt MBO-3:**
> Stop subtiel: *"Karim, schrijf JOUW eerste indruk eerst even op. Daarna vergelijken jullie."*

> **Differentiatie:**
> - **Gemengde groep:** vorm tweetallen MBO-3 + MBO-4. Bewaak dat MBO-4 sparringpartner is, niet voorzegger.

---

### Blok 3: Drie checks expliciet — vuistregels en stoplicht
**00:18 - 00:25** | 7 min | Kolb-fase: theoretiseren

**Doel:** De eigen ontdekking krijgt een naam en een framework. Deelnemer koppelt eigen aanpak aan de drie vuistregels en het stoplichtsysteem.

**Werkvorm:** Trainer-geleide handout-bespreking met directe koppeling naar de eigen bevindingen.

**Instructie:**

1. **Deel wb-03-theoretiseren.md uit** (30 sec). Zeg: *"Pak je markeerstift. Tijdens het doorlopen markeer je wat voor jou nieuw is."*

2. **Toon slide 6** (1 min) — de drie vuistregels:
    - **Volledigheid:** tel lege cellen per kolom. >10% leeg = oranje. >25% leeg = rood.
    - **Consistentie:** klopt de waarde met de eenheid? Buitenproporties? Mengsel?
    - **Actualiteit:** hoe oud is het laatste record? Past dat bij je beslissing?

3. **Werk de spuitgiet-dataset hardop door** (3 min) — slide 7:
    - *"Volledigheid: 3 lege cellen in cyclustijd op 25 = 12%. Dat is oranje."*
    - *"Consistentie: twee batches met afkeur 200%. Dat kan niet — typfout, hoort 20%. Oranje."*
    - *"Actualiteit: laatste rij van vorige week. Voor wekelijks rapport groen. Voor beslissing van vandaag oranje."*

4. **Toon het stoplichtsysteem** (1 min 30) — slide 8:

    | Stoplicht | Betekenis |
    |---|---|
    | **Groen** | Bron is bruikbaar zonder voorbehoud |
    | **Oranje** | Bruikbaar mits met aandacht — meld in conclusie 'data is incompleet op punt X' |
    | **Rood** | Niet gebruiken voor beslissing — eerst aanvullen of verifiëren |

5. **Bruggetje naar fase 4** (1 min) — *"Drie checks. Drie vuistregels. Een stoplicht. Nu pas je het toe op je eigen werkvloer."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (1 per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 6-8
- [ ] diagram-lo-data-lit-202.svg op A3 of via beamer

> **Tips voor de trainer:**
> - Verwijs ELKE keer terug naar wat de groep in fase 2 zelf heeft genoemd. *"Karim zei net: lege cellen. Dat is volledigheid."* Dit maakt het framework hun eigen ontdekking, niet jouw lesje.
> - Het stoplichtsysteem is bewust eenvoudiger dan een ++/+/-/--scoring. Voor MBO-3 werkt minder onderscheid beter.
> - Als iemand vraagt naar uitgebreide datakwaliteit-dimensies: parkeer naar lo-data-lit-302.

> **Valkuil — trainer geeft college:**
> Houd het kort. Maximaal 7 min, anders haakt de doener af. Dit is GEEN nieuw inzicht — dit is ankering.

---

### Blok 4: Actieplan eigen werkvloer
**00:25 - 00:30** | 5 min | Kolb-fase: experimenteren

**Doel:** Deelnemer kiest een dataset op de eigen werkvloer en plant de drie checks voor de komende week.

**Werkvorm:** Individueel actieplan met optionele peer-check.

**Instructie:**

1. **Deel wb-04-experimenteren.md uit** (30 sec). Zeg: *"Vijf minuten. Kies één dataset op je eigen werkvloer. Plan wanneer en hoe je de drie checks doet."*

2. **Toon slide 9** (30 sec) — de vier vragen op het werkblad:
    - Welke dataset ga ik checken?
    - Wanneer doe ik het?
    - Wat doe ik met een rood stoplicht?
    - Met wie deel ik de uitkomst?

3. **Individueel invullen** (3 min) — zet timer op 3 min. Loop rond. Coach met vragen:
    - *"Welke data zie je elke dag?"* (helpt MBO-3 die geen dataset kan kiezen)
    - *"Wanneer is dat morgen mogelijk — voor of na de ploegwissel?"*
    - *"Wat doe je als je twee oranje en één rood vindt?"*

4. **Korte peer-check** (1 min) — *"Draai je werkblad om naar je buurman. Eén minuut: vraag of zijn plan haalbaar is voor de komende week."*

5. **Feed-forward + afsluiting** (30 sec) — *"Volgende week komen we hierop terug. Je transferopdracht: voer dit plan deze week uit. Bespreek de uitkomst met je teamleider in het volgende overleg. Als je verder wilt: lo-data-lit-302 doet dezelfde checks systematisch op een hele afdeling."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (1 per deelnemer)
- [ ] Pen per deelnemer
- [ ] Slide 9
- [ ] Timer

> **Tips voor de trainer:**
> - Geef GEEN voorbeeld-dataset. Eigen keuze is essentieel voor autonomie en transfer.
> - Bij twijfel: *"Welke dataset gebruik je het vaakst om een beslissing te nemen?"* Dat is de juiste.
> - Sluit af met een toon van vertrouwen — niet *"hopelijk lukt het"* maar *"jullie hebben de checks vandaag gedaan, je kunt het nu zelf"*.

> **Valkuil — actieplan blijft vaag:**
> *"Ik ga deze week eens kijken naar onze data."* — niet specifiek genoeg. Vraag terug: *"Welke data, welke dag, welk uur?"*

> **Valkuil — uitloop fase 3:**
> Als blok 3 uitloopt, kort fase 4 in tot 4 min: skip de peer-check. Beter een ingevuld actieplan dan een uitgelopen theorie-blok.

> **Plan B:**
> - **Online sessie:** vervang peer-check door 'paste je actieplan in de chat'. Trainer leest 1-2 hardop voor.

---

## Tijdsoverzicht

| Tijd | Activiteit | Kolb-fase | Duur |
|------|-----------|-----------|------|
| 00:00 - 00:01 | Feed-up + drie checks introduceren | opening | 1 min |
| 00:01 - 00:10 | Drie checks zelf uitvoeren op dataset | ervaren | 9 min |
| 00:10 - 00:18 | Duo-reflectie + plenair delen | reflecteren | 8 min |
| 00:18 - 00:25 | Vuistregels en stoplichtsysteem | theoretiseren | 7 min |
| 00:25 - 00:30 | Actieplan eigen werkvloer | experimenteren | 5 min |
| **Totaal** | | | **30 min** |

---

## Materiaallijst

| Item | Aantal | Opmerkingen |
|------|--------|-------------|
| Voorbeelddataset spuitgieten (25 rijen) | n + 5 | Geprint, A4 |
| wb-01-ervaren.md | n + 2 | Geprint |
| wb-02-reflecteren.md | n + 2 | Geprint |
| wb-03-theoretiseren.md | n + 2 | Geprint |
| wb-04-experimenteren.md | n + 2 | Geprint |
| Pen per deelnemer | n + 5 | |
| Markeerstift groen/oranje/rood per duo | n/2 sets | Voor stoplicht-markering |
| Flap-over met drie kolommen | 1 | VOLLEDIGHEID / CONSISTENTIE / ACTUALITEIT |
| Stiften (zwart + 3 kleuren) | 1 set | Bij flap-over |
| Beamer + HDMI-kabel | 1 | Vooraf testen |
| diagram-lo-data-lit-202.svg op A3 | 1 | Optioneel als visueel anker |
| model-lo-data-lit-202.html (laptop/tablet) | 1 | Optioneel — snel-check tijdens fase 4 |
| Timer / mobiel met geluid | 1 | |

---

## Antwoordmodel — wat je in fase 2 zou moeten horen

### Volledigheid
- Lege cellen in cyclustijd (3 op 25 = 12%, oranje)
- Geen lege cellen in batchnummer of datum (groen)

### Consistentie
- Twee batches afkeur 200% (typfout, hoort 20% — oranje)
- Eenheden cyclustijd in seconden, consistent (groen)
- Operator-namen soms voornaam, soms achternaam (oranje, niet rood)

### Actualiteit
- Laatste rij van vorige week (5 dagen oud)
- Voor wekelijks rapport groen, voor dagelijks groen-oranje

### Eindoordeel groep
Dataset = oranje. Bruikbaar mits met aandacht, met expliciete melding in conclusie dat cyclustijd-data incompleet is en twee batches typfouten bevatten.

---

## Differentiatie naar competentiestadium

| Stadium | Hoe herken je het? | Aanpassing |
|---------|--------------------|-----------|
| **Bewust onbekwaam** (lager dan verwacht) | Zegt 'wat zijn checks?' — moet eerst Module 1 herhalen | Kort terug naar lo-data-lit-101 voor de basis. Niet opdringen — ander tempo. |
| **Bewust bekwaam** (verwacht stadium) | Doet de checks, twijfelt bij scoren, zoekt bevestiging | Coach met vragen, geef geen antwoorden. Bevestig pas in fase 3. |
| **Onbewust bekwaam** | Doet de checks intuïtief, vraagt naar uitgebreid framework | Vraag *"Hoe zou je dit op meerdere bronnen tegelijk doen?"* — bruggetje naar lo-data-lit-302. |

---

## Hofstede-check (NL-context)

| Dimensie | Hoe geborgd in dit blok |
|----------|-------------------------|
| **Lage machtsafstand** | Trainer geeft GEEN scores, deelnemer scoort zelf en onderbouwt. Coach met vragen, niet met antwoorden. |
| **Lage onzekerheidsvermijding** | Drie geheugenankers in plaats van uitgebreid framework. Stoplichtsysteem (groen/oranje/rood) laagdrempeliger dan ++/+/-/--. |
| **Autonomie-taal** | Werkbladen gebruiken *je kunt* / *je mag*. Eigen dataset-keuze in fase 4. |
| **Korte machtsafstand in feedback** | Geen individuele beoordeling. Peer-check in fase 4 = collega-perspectief, niet trainer-oordeel. |

---

## Verbinding met andere leerobjecten in de module

```
MODULE 2 (Train):
lo-data-lit-201 (data verzamelen) → [DIT BLOK lo-data-lit-202] → lo-data-lit-203 (data presenteren) → lo-data-lit-204 (simpele analyse)

MODULE 3 (Op maat) — verdiepingsroute:
[DIT BLOK lo-data-lit-202] → lo-data-lit-302 (audit op eigen afdeling)
```

Verwijs in het bruggetje (Blok 4) naar lo-data-lit-302 als verdiepingsroute. Daar wordt de check systematisch toegepast op meerdere bronnen tegelijk.

---

*Data Literacy v0.6 | Module 2: Train | KO 202 — Datakwaliteit beoordelen*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0 | Trainer-versie*
