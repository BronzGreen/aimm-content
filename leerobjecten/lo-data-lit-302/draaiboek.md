# Een datakwaliteit-audit op je eigen afdeling — Draaiboek
*Data Literacy Module 3 (Op maat) | Workshop-blok 60 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer voert een datakwaliteit-audit uit op de eigen afdeling: scoort minimaal 4 databronnen op volledigheid / consistentie / actualiteit, benoemt de 2 grootste risico's en stelt een verbeterplan op met eigen eerste actie deze week. |
| **Doelgroep** | Operators MBO-3 (primair), MBO-4 (secundair), 6-12 personen, B1 |
| **Voorkennis** | Module 1 + 2 afgerond — kent drie checks (lo-data-lit-202), kan dashboard lezen |
| **Stadium (H&B)** | Bewust bekwaam — kent de checks, oefent nu de schaal-toepassing op eigen afdeling |
| **Begeleidingsstijl** | Coachen — weinig sturing, veel ondersteuning |
| **Ruimte** | Clusters van 2 (duo's), beamer, flap-over, laptops/tablets met toegang tot eigen MES/Excel |
| **Plek in module** | Workshop-blok 2 — bouwt op lo-data-lit-301, leidt naar lo-data-lit-303 en lo-data-lit-304 |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Snelle inventarisatie: mijn databronnen | ervaren | 15 min |
| 00:15 - 00:25 | Duo-gesprek: waar zit het risico? | reflecteren | 10 min |
| 00:25 - 00:35 | Audit-framework + scoringsschema | theoretiseren | 10 min |
| 00:35 - 01:00 | Eigen audit + verbeterplan | experimenteren | 25 min |

**Totaal:** 60 minuten — ingebouwde mini-pauze van 30 sec tussen blok 3 en 4.
**Buffer:** 1 min flexibel per blok; gebruik voor coaching in fase 4.

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 (n + 2 reserve per stuk).
- [ ] Bereid flap-over voor: leeg blad voor inventarisatie databronnen plenair.
- [ ] Tweede flap-over: TOP-2 RISICO'S met ruimte per deelnemer.
- [ ] Open `presentatie.slidev.md` en test met de beamer.
- [ ] Check: hebben deelnemers laptops/tablets met toegang tot eigen MES, Excel-bestanden, kwaliteitssysteem? Zo niet: vraag IT om gastsessie of regel handmatige uitprints van eigen data.
- [ ] Lees voorbeeld-audit spuitgieten in trainer-yaml — heb een referentie-audit paraat.

### Het uur ervoor
- [ ] Hang de flap-over zichtbaar voor de groep.
- [ ] Leg per stoel: pen, markeerstift, werkblad wb-01, set kleurstickers (rood/oranje/groen, 5 per kleur).
- [ ] Houd wb-02, wb-03, wb-04 apart — uitdelen pas op het moment.
- [ ] Open slide 1.
- [ ] Schrijf op een tweede flap-over alvast: links **"Audit = proces, geen persoon"**, rechts **"Wat kun JIJ doen?"**.

---

## Blok-details

### Blok 1: Snelle inventarisatie — mijn databronnen
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** Deelnemer brengt alle databronnen op de eigen afdeling in kaart en geeft elke bron een eerste stoplicht-score op gevoel.

**Werkvorm:** Individueel onderzoek met werkblad + plenaire inventarisatie.

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Geef de feed-up: *"In Module 2 leerden jullie de drie checks op één dataset. Vandaag passen jullie ze systematisch toe op je EIGEN afdeling. Aan het eind van dit uur heb je een audit van minimaal vier bronnen, de twee grootste risico's benoemd en een verbeterplan met jouw eerste actie deze week. Dit is geen oefening meer — dit is je eigen werkvloer."*

2. **Toon slide 2** (30 sec) — wat is een databron?
    - **MES** — Manufacturing Execution System
    - **Logboek** — handmatig op papier of in Excel
    - **Whiteboard** — bordjes met getallen
    - **Excel** — losse bestanden met productiedata
    - **Kwaliteitssysteem** — NCR / CAPA
    - **Apps + formulieren** — onderhoud, scan-apps, e-formulieren

3. **Deel werkblad 1 uit** (30 sec). Zeg: *"Vijftien minuten. Schrijf alle databronnen op die je op je afdeling kent. Daarna scoor je elke bron op gevoel: groen / oranje / rood. Ben je verbaasd over hoeveel je vindt? Schrijf het toch op."*

4. **Individueel werk** (10 min) — zet timer op 10 min. Loop rond. Coach met vragen:
    - *"Welke schermen zie je op een gemiddelde dag?"*
    - *"Waar schrijft de teamleider iets op?"*
    - *"Wat staat er op het whiteboard bij de koffieautomaat?"*
    - *"Welke app open je op je telefoon voor werk?"*

5. **Plenaire inventarisatie** (3 min 30) — toon slide 3. Vraag: *"Wat heb je gevonden? Roep maar."* Schrijf op de flap-over alle bronnen. Verwacht 5-8 verschillende soorten plenair.

6. **Korte synthese** (30 sec) — *"Op een afdeling staan 4 tot 8 databronnen. De meeste mensen kennen er 2 of 3 echt goed. De rest is grijs gebied. Vandaag maken we het zwart-wit."*

**Materiaal:**
- [ ] wb-01-ervaren.md (1 per deelnemer)
- [ ] Set stickers (rood/oranje/groen) per deelnemer
- [ ] Pen + markeerstift per deelnemer
- [ ] Slides 1-3
- [ ] Lege flap-over voor plenaire inventarisatie
- [ ] Timer

> **Tips voor de trainer:**
> - Loop rond, MAAR ga niet bij iemand zitten. Korte coach-momenten van 30 sec per deelnemer.
> - Bij iemand die zegt *"er is alleen het MES"*: noem categorieën (logboek, whiteboard, app). Vrijwel iedereen werkt met 4-6 bronnen.
> - Op de flap-over: verzamel alleen bronnen, geen scores. Scoren is individueel — niemand gaat plenair afgerekend worden.

> **Differentiatie:**
> - **MBO-3 basis:** geef de zes categorieën als ankerpunt (MES, logboek, Excel, kwaliteitssysteem, whiteboard, app). Vraag: *"Welke ken je?"* Categorieën verlagen drempel.
> - **MBO-4 sneller:** vraag *"Welke bron heeft het grootste BUSINESS-risico?"* Triggert kosten-denken.
> - **Gemengde groep:** plenair eerst MBO-3 vragen om bronnen, daarna MBO-4 als aanvulling.

> **Valkuil — deelnemer kent eigen bronnen niet:**
> Help met categorieën uit de werkvloer-praktijk. *"Wat staat er op het whiteboard? Welke app open je op je telefoon?"*

> **Valkuil — audit wordt afrekentool over collega:**
> *"Het logboek van Sven is altijd onleesbaar."* Onderbreek niet, valideer eerst: *"Frustrerend als je iets niet kan terugvinden."* Maak dan expliciet: *"We auditen het PROCES, niet de persoon."* Schrijf op flap-over: AUDIT = PROCES, GEEN PERSOON.

> **Plan B:**
> - **Geen toegang tot eigen data tijdens sessie:** geef vooraf de opdracht: *"Maak deze week een lijst van alle databronnen op je afdeling — neem hem mee."* Sessie start dan met die lijst.
> - **Online sessie:** scherm-delen niet verplicht. Werkblad in chat. Plenaire inventarisatie via collaborative whiteboard (Miro / Mural).

---

### Blok 2: Duo-gesprek — waar zit het risico?
**00:15 - 00:25** | 10 min | Kolb-fase: reflecteren

**Doel:** Deelnemer reflecteert in duo op welke bron het minst betrouwbaar is en waarom. Risico-denken activeren.

**Werkvorm:** Gestructureerd duo-gesprek met werkblad + plenaire deel-ronde.

**Instructie:**

1. **Deel wb-02-reflecteren.md uit** (30 sec). Zeg: *"Pak een buurman. Bespreek samen: welke databron vertrouw je het minst? Wat kan er misgaan? Wat zou er gebeuren als die bron faalt?"*

2. **Toon slide 4** (30 sec) — drie reflectievragen:
    - **Welke bron vertrouw ik het minst?**
    - **Wat kan er misgaan?**
    - **Wat is de schade als het misgaat?**

3. **Duo-gesprek** (5 min) — zet timer op 5 min. Loop rond. Stel doorvragen:
    - *"Hoeveel procent van het logboek is leeg?"*
    - *"Wat zou er gebeuren als je morgen een claim moest onderbouwen?"*
    - *"Wie merkt het als die bron klopt of niet?"*

4. **Plenaire deel-ronde** (4 min) — toon slide 5. Vraag 3-4 deelnemers:
    - *"Welke bron vertrouw jij het minst?"* — vang antwoord, vraag door: *"Waarom?"*
    - Schrijf sleutelwoorden op de flap-over.

5. **Korte synthese** (30 sec) — *"Sommige bronnen vertrouwen we minder dan we denken. Dat is een eerlijk inzicht. In de volgende stappen kijken we systematisch naar WAAROM."*

**Materiaal:**
- [ ] wb-02-reflecteren.md (1 per deelnemer)
- [ ] Slides 4-5
- [ ] Flap-over (sleutelwoorden risico)
- [ ] Timer

> **Tips voor de trainer:**
> - In de plenair: vraag 3-4 personen, niet iedereen. Tijdsbeheer is belangrijk in dit blok.
> - Bevestig elke deelnemer met *"helder voorbeeld"* — geen oordeel, wel erkenning.
> - Tel innerlijk tot 5 na elke vraag. Stilte trekt antwoorden los.

> **Valkuil — duo gaat audit beginnen:**
> Sommigen willen al de matrix invullen. Stop: *"Even nog niet — eerst kijken WAAR het risico zit. Scoren komt straks."*

> **Valkuil — kritiek op persoon:**
> *"Sven schrijft slecht."* Herformuleer: *"Welk PROCES rond het logboek werkt niet — geen tijd, geen sjabloon, geen training?"*

> **Differentiatie:**
> - **MBO-4 sneller:** *"Wat is de business-impact als die bron faalt? Hoeveel kost het in tijd, geld of risico?"*

---

### Blok 3: Audit-framework + scoringsschema
**00:25 - 00:35** | 10 min | Kolb-fase: theoretiseren

**Doel:** Deelnemer leert het systematische scoringsschema (++/+/-/--) en de drie criteria (volledigheid/consistentie/actualiteit) toepassen op meerdere bronnen.

**Werkvorm:** Korte presentatie met handout + voorbeeld-audit.

**Instructie:**

1. **Deel wb-03-theoretiseren.md uit** (30 sec). Zeg: *"Pak je markeerstift. Tijdens het doorlopen markeer je wat voor jou nieuw is."*

2. **Toon slide 6** (1 min) — drie criteria:
    - **Volledigheid** — tel lege cellen / ontbrekende records
    - **Consistentie** — eenheden, buitenproporties, afspraken
    - **Actualiteit** — past update-frequentie bij beslissings-frequentie?
    - *"Deze ken je uit lo-data-lit-202. Nu pas je ze systematisch toe op meerdere bronnen tegelijk."*

3. **Toon slide 7** (2 min 30) — scoringsschema vier-punts:

    | Score | Betekenis |
    |---|---|
    | **++** | Uitstekend — bruikbaar voor automatische rapportage |
    | **+** | Goed — bruikbaar voor handmatige analyse, kleine correcties |
    | **-** | Onvoldoende — alleen mits expliciet voorbehoud |
    | **--** | Slecht — eerst structureel verbeteren |

    *"In Module 2 gebruikten we groen / oranje / rood. Hier voegen we toe — ++ is beter dan +, -- is slechter dan -. Vier niveaus geeft meer onderscheid bij meerdere bronnen tegelijk."*

4. **Voorbeeld-audit hardop** (4 min) — toon slide 8. Werk het spuitgiet-voorbeeld door:
    - *"Bron 1 — MES. Volledigheid ++. Consistentie +. Actualiteit ++. Eindscore = ++."*
    - *"Bron 2 — Logboek operator. Volledigheid - (15% leeg). Consistentie - (handgeschreven). Actualiteit +. Eindscore = -."*
    - *"Bron 3 — Excel afkeur. Volledigheid +. Consistentie +. Actualiteit -- (3 weken oud). Eindscore = -."*
    - *"De LAAGSTE score per criterium bepaalt het eindoordeel. Eén -- maakt de hele bron --."*

5. **Bruggetje naar fase 4** (1 min) — *"Drie criteria. Vier scores. Eindoordeel = laagste score. Nu pas je het toe op je eigen afdeling. Daarna kies je je twee grootste risico's en maak je een verbeterplan met JOUW eerste stap."*

**Materiaal:**
- [ ] wb-03-theoretiseren.md (1 per deelnemer)
- [ ] Markeerstift per deelnemer
- [ ] Slides 6-8
- [ ] diagram-lo-data-lit-302.svg op A3 of via beamer

> **Tips voor de trainer:**
> - Verwijs ELKE keer terug naar lo-data-lit-202 — *"De drie checks ken je. Nu schalen we op."* Maakt het herkenning.
> - De regel "laagste score bepaalt eindoordeel" is belangrijk — leg het expliciet uit, anders middelen mensen onbewust.
> - Geef GEEN extra voorbeelden. Eén goed uitgewerkt voorbeeld is genoeg.

> **Valkuil — trainer geeft college:**
> Theoretiseren is geen instructie — het is ankering. Maximaal 10 min, anders haakt de doener af.

> **Valkuil — verwarring tussen stoplicht en ++/+/-/--:**
> Sommigen vragen *"waarom nu vier scores?"* Antwoord: *"Bij meerdere bronnen heb je meer onderscheid nodig. Op één dataset werkt drie kleuren. Op acht bronnen heb je vier niveaus nodig om verschil te maken."*

---

### Blok 4: Eigen audit + verbeterplan
**00:35 - 01:00** | 25 min | Kolb-fase: experimenteren

**Doel:** Deelnemer voert systematisch een audit uit op de eigen databronnen (minimaal 4), benoemt de 2 grootste risico's en maakt een verbeterplan met eigen eerste actie deze week.

**Werkvorm:** Individueel werk met coaching + groepsdeling van risico's.

**Instructie:**

1. **Deel wb-04-experimenteren.md uit** (30 sec). Zeg: *"De grootste stap. 25 minuten. Vul de audit-matrix in voor minimaal 4 bronnen. Daarna kies je je twee grootste risico's. Daarna maak je een verbeterplan met JOUW eerste actie deze week."*

2. **Toon slide 9** (30 sec) — de matrix-template:

    | Bron | Volledigheid | Consistentie | Actualiteit | Eindscore |
    |---|---|---|---|---|

3. **Audit invullen** (12 min) — zet timer op 12 min. *"Begin met je 4 belangrijkste bronnen. Geef per criterium een score (++/+/-/--). Eindscore = laagste van de drie. Ik loop rond en help."*

4. **Coach individueel** met vragen, NIET met scores:
    - *"Hoeveel procent van het logboek is leeg gemiddeld?"*
    - *"Wanneer is de Excel voor het laatst bijgewerkt?"*
    - *"Welke afspraak is er over hoe je dit invult?"*
    - Bij milde scoring (alles ++): *"Het logboek is +. Hoeveel procent leeg? Hoe oud de laatste invul? Wie checkt of hij klopt?"*

5. **Top-2 risico's** (4 min) — toon slide 10. *"Vier minuten. Kies je twee grootste risico's uit de matrix. Niet de twee laagste scores — de twee waar de SCHADE het grootst is als ze falen. Schrijf op de tweede flap-over."* Loop rond, help bij prioritering.

6. **Verbeterplan** (6 min) — toon slide 11. Format:
    - **Risico** — welk risico pak je aan?
    - **Actie** — wat ga JIJ deze week doen?
    - **Eigenaar** — wie verder is verantwoordelijk?
    - **Deadline** — wanneer evalueer je?
    - *"Niet 'de teamleider moet een nieuw MES kopen'. Wel: 'Ik maak deze week een sjabloon voor het logboek en deel het met Sven.' Eigen eerste stap."*

7. **Korte plenaire deel-ronde** (1 min 30) — *"Wie deelt zijn eerste actie deze week?"* Vang 2-3 antwoorden. Geen oordeel, alleen waarderend bevestigen.

8. **Feed-forward + afsluiting** (30 sec) — *"Transferopdracht: voer dit verbeterplan deze week uit. Bespreek je audit én verbeterplan met je teamleider in het eerstvolgende overleg. Vraag een collega om dezelfde audit te doen — vergelijk de scores. In het volgende blok (lo-data-lit-303) leer je hoe je dit visueel deelt."*

**Materiaal:**
- [ ] wb-04-experimenteren.md (1 per deelnemer)
- [ ] Pen + markeerstift per deelnemer
- [ ] Slides 9-11
- [ ] Tweede flap-over (TOP-2 risico's per deelnemer)
- [ ] model-lo-data-lit-302.html op laptop/tablet (optioneel — interactieve audit-matrix)
- [ ] Timer

> **Tips voor de trainer:**
> - Coach met vragen, geef GEEN scores. Eigen oordeel is essentieel voor transfer.
> - Bij milde scoring: vraag specifiek door op één criterium per bron.
> - Bij plenaire deel-ronde: ZWIJG na het antwoord. Laat de groep reageren — niet jij.

> **Valkuil — scoring blijft te mild:**
> Alles ++ of +. Vraag specifiek door: *"Hoeveel procent leeg? Hoe oud? Wie checkt?"* Concrete vragen halen echte score boven.

> **Valkuil — verbeterplan = wensenlijst:**
> *"De teamleider moet een nieuw MES kopen."* Vraag terug: *"Wat kun JIJ doen? Wat is jouw eerste stap deze week?"*

> **Valkuil — tijd loopt uit:**
> Bij 18 min waarschuwen: *"Zeven minuten voor matrix + verbeterplan. Doe alleen je TOP 4 — de rest komt later."*

> **Differentiatie:**
> - **MBO-3 basis:** max 4 bronnen i.p.v. minimaal 4. Gebruik stickers (groen/oranje/rood) i.p.v. ++/+/-/--. Visueel werkt beter.
> - **MBO-4 sneller:** 6-8 bronnen + één bron diepgaander. Plus: business-impact-vraag bij elke bron.

> **Plan B:**
> - **Geen toegang tot eigen data:** werk met de lijst van fase 1 + geheugen-scoring. Beter een ruwe audit dan geen audit.
> - **Online sessie:** matrix in gedeeld document (Excel / Google Sheets). Plenaire deel-ronde via chat.

---

## Tijdsoverzicht

| Tijd | Activiteit | Kolb-fase | Duur |
|------|-----------|-----------|------|
| 00:00 - 00:01 | Feed-up + module-context | opening | 1 min |
| 00:01 - 00:02 | Wat is een databron? | ervaren | 1 min |
| 00:02 - 00:12 | Individueel inventariseren + scoren | ervaren | 10 min |
| 00:12 - 00:15 | Plenaire inventarisatie | ervaren | 3 min |
| 00:15 - 00:20 | Duo-gesprek risico | reflecteren | 5 min |
| 00:20 - 00:25 | Plenaire deel-ronde | reflecteren | 5 min |
| 00:25 - 00:35 | Audit-framework + voorbeeld | theoretiseren | 10 min |
| 00:35 - 00:47 | Audit-matrix invullen | experimenteren | 12 min |
| 00:47 - 00:51 | Top-2 risico's | experimenteren | 4 min |
| 00:51 - 00:57 | Verbeterplan opstellen | experimenteren | 6 min |
| 00:57 - 00:59 | Plenaire deel-ronde eerste actie | experimenteren | 2 min |
| 00:59 - 01:00 | Feed-forward + afsluiting | experimenteren | 1 min |
| **Totaal** | | | **60 min** |

---

## Materiaallijst

| Item | Aantal | Opmerkingen |
|------|--------|-------------|
| wb-01-ervaren.md | n + 2 | Geprint |
| wb-02-reflecteren.md | n + 2 | Geprint |
| wb-03-theoretiseren.md | n + 2 | Geprint |
| wb-04-experimenteren.md | n + 2 | Geprint, A4-formaat |
| Stickers groen/oranje/rood | n × 5/kleur | Voor scoring fase 1 |
| Pen per deelnemer | n + 5 | |
| Markeerstift per deelnemer | n + 5 | |
| Lege flap-over (inventarisatie) | 1 | Voor plenaire bronnen-lijst |
| Tweede flap-over (risico's + slogans) | 1 | "Audit = proces, geen persoon" / "Wat kun JIJ doen?" |
| Stiften (zwart + 3 kleuren) | 1 set | Bij flap-over |
| Beamer + HDMI-kabel | 1 | Vooraf testen |
| Laptops/tablets per deelnemer | n | Met toegang tot eigen MES, Excel, kwaliteitssysteem |
| diagram-lo-data-lit-302.svg op A3 | 1 | Optioneel |
| model-lo-data-lit-302.html | 1 | Optioneel — interactieve audit-matrix |
| Timer / mobiel met geluid | 1 | |

---

## Antwoordmodel — voorbeeld-audit spuitgieten

| Bron | Volledigheid | Consistentie | Actualiteit | Eindscore |
|------|---|---|---|---|
| MES | ++ | + | ++ | **++** |
| Logboek operator | - (15% leeg) | - (handgeschreven) | + | **-** |
| Excel afkeur | + | + | -- (3 wkn oud) | **-** |
| Whiteboard OEE | + | -- (verschillende handschriften) | + | **-** |

### Twee grootste risico's
- **Logboek operator** — bij incident geen reconstructie mogelijk; garantieclaim mislukt.
- **Excel afkeur** — trend-analyse op verkeerde data, verkeerde verbeterprioriteit.

### Verbeterplan voorbeeld
- **Risico:** logboek 15% leeg.
- **Actie:** ik maak deze week een 1-pagina sjabloon voor het logboek met de 5 verplichte velden + voorbeeld. Deel met Sven en Karim.
- **Eigenaar:** ik (eerste week), daarna teamleider.
- **Deadline:** evaluatie 2 weken — hoeveel cellen nu leeg?

---

## Differentiatie naar competentiestadium

| Stadium | Hoe herken je het? | Aanpassing |
|---------|--------------------|-----------|
| **Bewust onbekwaam** (lager dan verwacht) | Kent drie checks niet of vaag | Kort herhaal lo-data-lit-202. Geef sticker-scoring i.p.v. ++/+/-/--. |
| **Bewust bekwaam** (verwacht stadium) | Doet de scoring, twijfelt bij grensgevallen | Coach met vragen, geef geen scores. Help bij prioritering risico's. |
| **Onbewust bekwaam** | Doet audit intuïtief, vraagt naar systematische verbeter-frameworks | Parkeer naar lo-data-lit-303 (data presenteren) en lo-data-lit-304 (dataplan). |

---

## Hofstede-check (NL-context)

| Dimensie | Hoe geborgd in dit blok |
|----------|-------------------------|
| **Lage machtsafstand** | Trainer geeft GEEN scores, deelnemer scoort zelf. Plenaire ronde = uitwisseling, geen beoordeling. |
| **Lage onzekerheidsvermijding** | Vereenvoudigd stoplichtsysteem in fase 1. Pas in fase 4 het volledige ++/+/-/--. Geleidelijke complexiteit. |
| **Autonomie-taal** | Werkbladen gebruiken *je kunt* / *je mag*. Eigen-afdeling-keuze, eigen-actie-format. |
| **Korte machtsafstand in feedback** | Bij plenaire deel-ronde: trainer reageert ALLEEN met *"helder"* of doorvraag. Groep reageert eerst. |

---

## Verbinding met andere leerobjecten in de module

```
MODULE 2 (Train):
lo-data-lit-202 (drie checks op één dataset) → BASIS voor dit LO

MODULE 3 (Op maat):
lo-data-lit-301 (data op je werkvloer) → [DIT BLOK lo-data-lit-302] → lo-data-lit-303 (data presenteren) → lo-data-lit-304 (dataplan)
```

In het feed-forward-moment verwijs je naar:
- **lo-data-lit-303** als volgende stap: hoe presenteer je deze audit-resultaten visueel aan teamleider en collega's?
- **lo-data-lit-304** als afronder van Module 3: een dataplan voor je afdeling waarin de bevindingen van deze audit worden meegenomen.

---

*Data Literacy v0.6 | Module 3: Op maat | KO 302 — Een datakwaliteit-audit op je eigen afdeling*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0 | Trainer-versie*
