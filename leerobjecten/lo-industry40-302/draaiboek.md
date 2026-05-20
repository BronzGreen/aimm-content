# Data-pipeline ontwerpen voor een digital twin — Draaiboek
*AIMM Industry 4.0 | Module 2 (Train) | 45 min | 8-16 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK
> 🎯 BLOOM TOEPASSEN — fysiek A3-tekenen is het hart van de sessie
> 🔁 KIRKPATRICK GEDRAG — transfer naar werkvloer borgen via IT-vraag

**Datum:** ________  **Trainer:** ________
**Locatie:** ________  **Deelnemers:** ___ personen

---

## ⚠️ Belangrijk: coachen, niet doceren

Deelnemers zijn bewust_bekwaam — ze kennen sensor en dashboard apart, maar overzien het pad zelden in zijn geheel. Pak de coach-rol op. Stel vragen, laat zelf raden, geef pas in fase 3 de termen.

**Drie sturende principes voor de hele sessie:**

1. **GEEN termen in fase 1.** Geen 'latentie', 'failover' of 'volume' uitspreken. Laat de groep met eigen woorden komen ('vertraging', 'data kwijt', 'te duur').
2. **A3-tekening is het hart.** Deelnemers tekenen hun toegewezen knooppunt fysiek op A3. Kort de uitleg in, niet de tekening.
3. **Vraagteken = goede uitkomst.** Niet zelf beantwoorden in de zaal. "Goede vraag — die gaat mee aan IT." Dat is Kirkpatrick gedrag.

**VERMIJD:** te snel naar theorie, drie keuzes op één deelnemer laden, spuitgieterij-voorbeeld kort behandelen, vraagtekens van deelnemers in de zaal oplossen.

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoelen** | 1. Deelnemers benoemen de vier knooppunten in juiste volgorde |
| | 2. Deelnemers onderbouwen drie ontwerp-keuzes met één zin per keuze |
| | 3. Deelnemers tekenen een pipeline voor eigen werkvloer-casus met vraagtekens als geldige uitkomst |
| **Bloom-niveau** | Toepassen — niet alleen benoemen, maar zelf tekenen voor eigen casus |
| **Kirkpatrick-doel** | Gedrag — concrete vraag voorbereid voor IT/teamleider |
| **Doelgroep** | MBO-4 operator, 8-16 deelnemers |
| **Voorkennis** | lo-industry40-021 (digital twin), ko-industry40-301 (sensor-keuze) |
| **Begeleidingsstijl** (manier van begeleiden) | **Coachen** — stel vragen, geen voorzeggen, vraagteken = waardevol |
| **Ruimte** | U-opstelling, ruimte aan muur voor 4 A3's, tafels voor duo-werk |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Ervaren — Drie storings-fragmenten | 🟢 werkvorm | 12 min |
| 00:12 - 00:22 | Reflecteren — Buurman-check + plenair | 🟣 reflectie | 10 min |
| 00:22 - 00:35 | Theoretiseren — Vier knooppunten + A3-tekening | 📘 theorie | 13 min |
| 00:35 - 00:45 | Experimenteren — Eigen pipeline (of bewust met vraagtekens) | 🟠 afsluiting | 10 min |

*Totaal: 45 min.*

---

## Blok-details

### 🟢 Blok 1: Ervaren — Drie storings-fragmenten
**00:00 - 00:12** | 12 min

**Doel:** Deelnemers herkennen drie werkvloer-situaties waarin het misgaat tussen sensor en scherm. Met EIGEN woorden, geen vaktermen.

**Werkvorm:** Trainer toont drie fragmenten op het scherm + individueel invullen (Kolb-fase 1)

**Materiaal:**
- [ ] Werkblad wb-01-drie-storingen.md (1 per deelnemer)
- [ ] Beamer + drie fragmenten (foto/video van dashboard-haperingen)
- [ ] Pen per deelnemer

**Instructie:**
1. Open warm: "Welkom. Vandaag gaan we tekenen — letterlijk. Aan het einde heeft iedereen zijn eigen pipeline op papier."
2. Schets de context: "Een sensor alleen levert geen inzicht. Het gaat om het pad ertussen. We beginnen bij drie momenten waar het misgaat."
3. Deel wb-01-drie-storingen.md uit.
4. Toon **fragment 1** (30 sec): operator wijst naar dashboard waarop temperatuur van 30 seconden geleden staat in plaats van nu. Vraag: "Wat denken jullie dat hier mis is gegaan tussen de sensor en het scherm?"
5. Toon **fragment 2** (30 sec): dashboard met lege grafiek tussen 14:00 en 15:00 — geen data binnengekomen die uren. Zelfde vraag.
6. Toon **fragment 3** (30 sec): teamleider laat cloud-rekening zien — €2.500 in plaats van begrote €120. Zelfde vraag.
7. Zet timer op 6 minuten. Deelnemers schrijven per fragment één zin op het werkblad — eerste vermoeden, geen vakterm nodig.
8. Loop na 3 minuten rond. Bevestig elke poging. Lees mee.
9. Schrijf 3-4 antwoorden per fragment op het bord — zonder oordeel.

> **💡 Tips voor de trainer:**
> - **GEEN termen geven nog.** Geen 'latentie', 'failover' of 'volume'. Laat de groep komen met 'vertraging', 'data kwijt', 'te duur'.
> - Bij geen antwoord: "Wat is je eerste vermoeden? Geen verkeerd antwoord."
> - Twijfel bevestigen: "Dat is een goede start."

> **🔴 Valkuil:** Te snel een term invullen ('ah, dat is latentie!'). Houd je tong vast — bewaar voor fase 3.

> **🔄 Alternatief (geen beamer):** Print de drie fragmenten als foto's op A4 + één korte beschrijving per fragment.

> **Overgang naar blok 2:** "Mooi. Laten we deze vermoedens samen leggen — wie ziet wat de buurman ook zag?"

---

### 🟣 Blok 2: Reflecteren — Buurman-check + plenair
**00:12 - 00:22** | 10 min

**Doel:** Duo's vergelijken hun antwoorden, formuleren één gemeenschappelijke oorzaak per fragment. Plenair: drie categorieën op het bord (snelheid / hoeveelheid / wat-als-stop).

**Werkvorm:** Duo (5 min) + plenair (5 min) (Kolb-fase 2)

**Materiaal:**
- [ ] Werkblad wb-02-buurman-check.md (1 per deelnemer)
- [ ] Bord of flipover + stiften

**Instructie:**
1. Overgang: "Tijd om samen te kijken. Vorm een duo met je buurman."
2. Deel wb-02-buurman-check.md uit.
3. Duo-instructie (5 min): "Leg jullie antwoorden naast elkaar. Per fragment één gemeenschappelijke zin: 'Hier ging het mis bij ___.'"
4. Loop rond. Stuur op kort en concreet.
5. Plenaire ronde (5 min): "Wie heeft een gemeenschappelijke zin voor fragment 1?" Schrijf op het bord — zonder oordeel.
6. Doe dit voor fragment 2 en 3.
7. **STEL DE KERNVRAAG:** "Op welke drie plekken in het pad van sensor naar scherm kan het misgaan?" Wacht 5-7 seconden.
8. Stuur — als groep niet komt — met hint: "Eén heeft met snelheid te maken. Eén met hoeveelheid. Eén met wat-als-er-iets-stopt."
9. Schrijf drie categorieën op het bord: **SNELHEID** | **HOEVEELHEID** | **WAT-ALS-STOP**. Koppel fragmenten: fragment 1 = snelheid, fragment 2 = wat-als-stop, fragment 3 = hoeveelheid.

> **💡 Tips voor de trainer:**
> - Duo's die snel klaar zijn: "Welke vraag zou je aan IT stellen voor fragment 2?"
> - Bevestig de werkvloer-woorden ('vertraging', 'data kwijt'). Geef nog GEEN vaktermen.
> - De drie categorieën op het bord blijven staan — komt straks terug.

> **🔴 Valkuil:** Duo komt niet tot één zin. Vraag: "Wat hebben jullie hetzelfde gezien?"

> **🔄 Alternatief (oneven groep):** Eén trio in plaats van duo — verloopt iets langzamer.

> **Overgang naar blok 3:** "Drie categorieën op het bord. Nu krijgen die ook hun officiële namen — en we tekenen het pad."

---

### 📘 Blok 3: Theoretiseren — Vier knooppunten + drie keuzes + A3-tekening
**00:22 - 00:35** | 13 min

**Doel:** Vier knooppunten benoemen (sensor → edge-buffer → opslag → consument). Drie keuzes koppelen aan de drie categorieën van het bord. Deelnemers tekenen hun toegewezen knooppunt op A3.

**Werkvorm:** Korte uitleg (5 min) + A3-tekenen subgroepen (4 min) + langslopen plenair (4 min) (Kolb-fase 3)

**Materiaal:**
- [ ] Werkblad wb-03-handout-pipeline.md (1 per deelnemer)
- [ ] A3-vellen — 4-8 stuks (één per knooppunt-subgroep)
- [ ] Dikke stiften (zwart/blauw/rood) — 4 sets
- [ ] Tape of magneten — voor A3's aan de muur
- [ ] Markeerstift per deelnemer

**Instructie:**

**Deel 1 — Uitleg vier knooppunten (3 min):**
1. Deel wb-03-handout-pipeline.md uit.
2. Schets pijl-diagram op het bord: **SENSOR → EDGE-BUFFER (tussenstation) → OPSLAG → CONSUMENT**.
3. Per knooppunt één zin met spuitgieterij-context:
   - **Sensor** — bron. Temperatuur-sensor op elk van vijftig mallen.
   - **Edge-buffer (tussenstation)** — klein opslag-punt naast de machine. Hier vatten we samen.
   - **Opslag** — centrale plek. Cloud of eigen server.
   - **Consument** — dashboard voor de operator, of AI-model dat patronen voorspelt.
4. Benoem expliciet: "Een goed ontworpen pipeline (data-leiding) is voor de operator onzichtbaar — alles werkt gewoon."

**Deel 2 — Drie keuzes gekoppeld aan de drie categorieën (2 min):**
5. Wijs naar het bord met de drie categorieën uit blok 2:
   - **SNELHEID = latentie (vertraging)** — real-time onder 1 seconde, near-realtime onder 60 seconden, batch in uren of dagen
   - **HOEVEELHEID = volume** — samenvatten in de edge-buffer scheelt vaak 99% van de data
   - **WAT-ALS-STOP = failover (terugval bij fout)** — buffering bij verbindings-verlies + alarm bij sensor-uitval
6. **SPUITGIETERIJ-ANKER (1 min):** "Eerste ontwerp: elke sensor stuurt elke seconde naar de cloud. Resultaat: €2.500 per maand. Te duur. Tweede ontwerp: edge-buffer per machine, elke 30 seconden gemiddelde + afwijkingen. Resultaat: €120 per maand. Factor twintig in kosten — door één keuze."

**Deel 3 — A3-tekenen in subgroepen (4 min):**
7. Verdeel groep in vier subgroepen (of paren): **SENSOR / EDGE-BUFFER / OPSLAG / CONSUMENT**.
8. Elk groepje krijgt één A3-vel + dikke stiften.
9. Opdracht: "Vier minuten. Teken jouw knooppunt voor de spuitgieterij-casus. Wat staat er fysiek? Hoe ziet het eruit op de werkvloer? Welke pijl gaat in en uit? Welke keuze speelt er bij JOUW knooppunt?"
10. Loop rond. Help met concrete suggesties als groepje vastloopt.

**Deel 4 — Langslopen plenair (4 min):**
11. Hang vier A3's naast elkaar aan de muur in juiste volgorde.
12. Loop met hele groep langs. Per A3: "Wat hebben jullie getekend? Welke keuze speelt hier?"
13. Trainer benoemt waar nodig: sensor = bron-volume, edge-buffer = ALLE DRIE keuzes komen samen, opslag = volume bestemming, consument = latentie-ervaring.

> **💡 Tips voor de trainer:**
> - Spuitgieterij-voorbeeld is je ANKER. Drie minuten waard. Laat factor twintig in kosten landen — dat is de business-impact.
> - Bij A3-tekenen: bevestig elke vorm. Stick figures zijn prima.
> - Bij langslopen: vraag "wat zou hier bij jullie het voorbeeld zijn?" — coach naar eigen voorbeelden, niet voorzeggen.

> **🔴 Valkuil:** A3-tekening overslaan vanwege tijdgebrek. NIET DOEN — dit is Bloom toepassen. Kort dan eerder de uitleg in.

> **🔄 Alternatief (kleine groep < 8):** Twee subgroepen die elk twee knooppunten tekenen. Iets minder fysiek, wel snel.

> **🔄 Alternatief (HBO):** Voeg toe — wie is eigenaar van de data per knooppunt? Data-governance.

> **Overgang naar blok 4:** "Mooi. Vier knooppunten staan aan de muur. Nu ga je hetzelfde doen — maar dan voor JOUW werkvloer."

---

### 🟠 Blok 4: Experimenteren — Eigen pipeline (of bewust met vraagtekens)
**00:35 - 00:45** | 10 min

**Doel:** Deelnemers tekenen op A4 hun eigen pipeline voor één machine of lijn. Drie keuze-vragen beantwoorden — of bewust een vraagteken zetten. Eén concrete vraag voorbereiden voor IT/teamleider (Kirkpatrick gedrag).

**Werkvorm:** Individueel actieplan + vrijwillige plenaire afronding (Kolb-fase 4)

**Materiaal:**
- [ ] Werkblad wb-04-eigen-pipeline.md (1 per deelnemer)

**Instructie:**
1. Overgang: "Tijd voor jezelf. Kies één machine of lijn waar sensor-data naar een dashboard gaat."
2. Deel wb-04-eigen-pipeline.md uit.
3. Instructie: "Vier knooppunten met pijlen tekenen. Dan drie vragen: (1) welke latentie hebben jullie nodig? (2) wordt data ergens samengevat? (3) wat als de verbinding wegvalt?"
4. **BENADRUK expliciet:** "Vraagteken bij een keuze is een geldig antwoord — die gaat mee als vraag aan IT of de teamleider. Dat is de bedoeling van vandaag."
5. Zet timer op 7 minuten. Loop rond.
6. **STEL VRAGEN bij rondlopen:**
   - "Welke latentie heeft jouw dashboard nu — echt real-time of is een minuut goed?"
   - "Wat merken jullie als de verbinding wegvalt?"
   - "Wordt jullie data ergens samengevat — bij de sensor of pas in de cloud?"
7. Bij grote casus ('onze hele fabriek'): help verkleinen tot één machine.
8. Bij geen casus: bied terug naar lo-industry40-021 of ko-industry40-301.
9. Plenaire afronding (3 min, vrijwillig): "Wie wil zijn pipeline kort delen?" 2-3 deelnemers, max 1 min elk. Op vrijwillige basis.
10. Bevestig transfer: "Deze week — neem je tekening mee. Vraag bij twijfel één antwoord aan IT of de teamleider. Vraag ook waar de edge-buffer fysiek staat — vaak een industriële computer naast de machine. Volgende sessie bespreken we ieders pipeline."

> **💡 Tips voor de trainer:**
> - Bevestig vraagtekens EVEN sterk als zelfverzekerde antwoorden. Vraagteken = Kirkpatrick gedrag.
> - **NIET zelf beantwoorden in de zaal.** "Goede vraag — die gaat mee aan IT."
> - Plenair vrijwillig. Niemand verplichten te delen.

> **🔴 Valkuil:** Drie vraagtekens bij één deelnemer. Bevestig, maar help er één concreet maken voor IT.

> **🔄 Alternatief (MBO-3):** Voorbeelden voorzeggen — "jouw lijn met sensor X — welke latentie denk je?"

> **🔄 Alternatief (HBO):** Teken twee pipelines naast elkaar — huidige en gewenste.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-drie-storingen.md | 1 per deelnemer + 2 extra | A4, geprint |
| ☐ | wb-02-buurman-check.md | 1 per deelnemer + 2 extra | A4, geprint |
| ☐ | wb-03-handout-pipeline.md | 1 per deelnemer + 2 extra | A4, geprint |
| ☐ | wb-04-eigen-pipeline.md | 1 per deelnemer + 2 extra | A4, geprint |
| ☐ | A3-vellen | 4-8 stuks | Voor knooppunt-tekeningen |
| ☐ | Dikke stiften (zwart/blauw/rood) | 4 sets | Voor A3-tekenen |
| ☐ | Tape of magneten | 1 set | Voor A3's aan de muur |
| ☐ | Flipover of bord + stiften | 1 set | 2-3 kleuren |
| ☐ | Markeerstift | 1 per deelnemer | |
| ☐ | Pennen extra | 5 stuks | |
| ☐ | Timer | 1 | |
| ☐ | Beamer + laptop | 1 set | Voor drie storings-fragmenten |
| ☐ | Drie storings-fragmenten | 1 set | Foto/video, vooraf testen |
| ☐ | Slidev-presentatie (optioneel) | 1 deck | `lo-industry40-302-presentatie.slidev.md` |

---

## Antwoordmodel — kort overzicht

- **wb-01:** Eén zin per fragment met eigen vermoeden. Typisch: f1 = 'internet traag', f2 = 'data kwijt', f3 = 'te duur'. GEEN vaktermen vereist.
- **wb-02:** Gemeenschappelijke duo-zin per fragment. Drie categorieën op het bord: SNELHEID, HOEVEELHEID, WAT-ALS-STOP.
- **wb-03:** Vier knooppunten gemarkeerd in juiste volgorde. Drie keuzes herkend en gekoppeld aan de drie fragmenten. Eigen A3-tekening van toegewezen knooppunt voor spuitgieterij-casus.
- **wb-04:** Eigen pipeline getekend voor één machine. Drie keuzes onderbouwd of gemarkeerd met vraagteken. Eén concrete vraag voor IT/teamleider.

## Differentiatie

- **MBO-3:** spuitgieterij visueler uitwerken (foto's), in fase 4 voorbeelden voorzeggen, A3 met voorgedrukte vakken.
- **HBO:** data-governance (wie is eigenaar?), RTO en RPO (recovery time/point objective) bij failover, in fase 4 huidige + gewenste pipeline naast elkaar.

---

*AIMM Industry 4.0 — Module 2 (Train) | Bron: Anaya et al. (2024); Bakopoulos et al. (2024), Ch. 5; EEMUA Publication 191 — Alarm Systems | Draaiboek v1.0 — Bloom toepassen + Kirkpatrick gedrag*
