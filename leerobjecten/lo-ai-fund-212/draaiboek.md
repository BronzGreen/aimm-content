# Confusion matrix, precision en recall — Draaiboek
*AI Fundamentals Module 2 (Train) | Workshop-blok 45 minuten | 6-12 deelnemers*

> DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer leest een confusion matrix (verwarrings-matrix), berekent precision (precisie) en recall (terugvinden) uit een gegeven matrix, en kiest onderbouwd welke van de twee maten prioriteit heeft voor zijn eigen werkvloer-AI. |
| **Doelgroep** | Operators MBO-4 (primair), teamleiders MBO-4 (secundair), 6-12 personen |
| **Voorkennis** | Module 1 (Gebruik) afgerond + lo-ai-fund-133 (classificatie) + lo-ai-fund-135 (overfitting) + lo-ai-fund-205 (labelen) |
| **Stadium (Hersey & Blanchard)** | Bewust bekwaam — classificatie bekend, evaluatie-cijfers nog niet zelf geïnterpreteerd |
| **Begeleidingsstijl (manier van begeleiden)** | Instrueren — hoge taakgerichtheid omdat formules onbekend zijn, gematigde relatie-gerichtheid omdat groep al een vertrouwde leeromgeving heeft uit Module 1 |
| **Ruimte** | U-opstelling of clusters van 4 (duo's voor narekenen matrix B), beamer + scherm, flip-over of bord met ruimte voor twee 2x2 tabellen en twee formules naast elkaar |
| **Plek in module** | Derde hands-on LO van Module 2 (Train) en afsluiting van de Train-cyclus. Volgt op labelen (lo-ai-fund-205) en no-code modeltraining (lo-ai-fund-211); deelnemer interpreteert hier evaluatie-cijfers van het net-getrainde model. |
| **Bloom-niveau** | Analyseren — interpreteren van vier kwadranten, berekenen van twee maten, kiezen tussen precision en recall op basis van kosten van fouten |
| **Kirkpatrick-niveau** | Gedrag — één concrete vraag voor leverancier/IT/kwaliteit deze week |

---

## Sessie-overzicht

| Tijd | Activiteit | Type (Kolb-fase / leerfase) | Duur |
|------|-----------|------|------|
| 00:00 - 00:12 | Twee confusion matrices lezen (strenge + soepele drempel) | 🟢 ervaren | 12 min |
| 00:12 - 00:22 | Precision en recall — formules + narekenen | 📘 theoretiseren | 10 min |
| 00:22 - 00:35 | Welke fout is duurder? — twee scenario's + eigen keuze | 🟣 reflecteren | 13 min |
| 00:35 - 00:45 | Eigen werkvloer-AI doorlichten + duo-spiegel + vraag deze week | 🟠 experimenteren | 10 min |

**Totaal:** 45 minuten.
**Buffer:** 1 min per blok flexibel (kan opgenomen worden in fase 3 of fase 4).

---

## Voorbereiding

### De avond ervoor
- [ ] Print werkbladen wb-01 t/m wb-04 — n + 2 reserve per werkblad. **Of** kies digitaal voor wb-02/wb-03: laad `model-precision-recall-drempel.jsx` op een React-sandbox (StackBlitz/CodeSandbox of lokale Vite-app) en test op één tablet.
- [ ] Test de Slidev-presentatie (`lo-ai-fund-212-presentatie.slidev.md`) op de beamer. Check vooral dat de matrix-slides leesbaar zijn vanaf de achterste rij.
- [ ] **Optioneel — video previewen:** `video/composition.tsx` (export id `ConfusionMatrixVideo`) registreren in je Remotion-project en `npx remotion preview` doen. Of pre-render naar MP4 voor offline-inzet. Plan inzet na het narekenen van matrix B in fase 2 (~90s extra; rond fase 2 dan af in 8 min i.p.v. 10).
- [ ] Flip-over of bord — verdeel in drie velden vooraf:
  - **Veld links** (groot): leeg, voor matrix A in fase 1
  - **Veld midden** (groot): leeg, voor twee formules naast elkaar in fase 2
  - **Veld rechts** (klein): leeg, voor bedrijfslogica-regel in fase 3
- [ ] Schrijf op apart bord-vlak (afgedekt of klein) de vier werkvloer-zinnen klaar — onthul in fase 1 stap 2:
  - *"Goed product, terecht doorgelaten = terecht positief"*
  - *"Goed product, onterecht afgekeurd = vals negatief (vals-alarm)"*
  - *"Afgekeurd product, onterecht doorgelaten = vals positief (gemist)"*
  - *"Afgekeurd product, terecht afgekeurd = terecht negatief"*
- [ ] Reken matrix A en B een keer zelf uit met pen op papier. Dat is je IK DOE-zelfvertrouwen.

### Het uur ervoor
- [ ] Leg per stoel klaar: pen, werkblad wb-01.
- [ ] Houd wb-02, wb-03 en wb-04 apart op trainertafel — deze deel je in elke fase opnieuw uit.
- [ ] Open slide 1 in presenter-modus.
- [ ] Vraag wie geen rekenmachine of telefoon mee heeft; leg twee reserve-rekenmachines klaar.
- [ ] Zet stoelen zo dat elke deelnemer een buurman naast zich heeft (geen blokken van één — fase 2 duo's vergen het).

---

## Blok-details

### 🟢 Blok 1: Twee confusion matrices lezen — strenge + soepele drempel
**00:00 - 00:12** | 12 min | Kolb-fase (leerfase): ervaren

**Doel:** Deelnemer leest twee uitgewerkte 2x2 confusion matrices (verwarrings-matrices) uit een vleesverwerker-scenario en benoemt de vier kwadranten in werkvloer-taal. Ervaart dat een ander drempel-instelling andere fouten oplevert. Nog geen woord precision of recall, geen formule.

**Werkvorm:** Plenaire opening (1 min), conventie expliciet maken (1 min), IK DOE-modellering matrix A (3 min), zelfstandig matrix B (6 min), brug (1 min).

**Instructie:**

1. **Open de sessie** (1 min) — toon slide 1. Zeg: *"De komende 45 minuten leer je een AI-rapport-kaart kritisch lezen. In Module 1 leerden jullie dat AI patronen leert uit voorbeelden. Vorige sessie leerden jullie data labelen — de juiste antwoorden geven. Vandaag de stap erna: hoe weet je of het model écht goed werkt? Niet met één getal — met twee."* Pauze 5 seconden.

2. **Conventie expliciet maken** (1 min) — toon slide 2. Onthul vier werkvloer-zinnen op het bord. Zeg langzaam:
   - *"In dit blok gebruiken we één conventie. Positief betekent 'model zegt GOED'. Negatief betekent 'model zegt AFGEKEURD' — alarm. Vier mogelijke uitkomsten:"*
   - *"Goed product, terecht doorgelaten — dat is terecht positief."*
   - *"Goed product, onterecht afgekeurd — dat is vals negatief, vals-alarm."*
   - *"Afgekeurd product, onterecht doorgelaten — dat is vals positief, gemist."*
   - *"Afgekeurd product, terecht afgekeurd — dat is terecht negatief."*

3. **Werkblad uitdelen** (30 sec) — deel wb-01 uit. Zeg: *"Twee matrices van dezelfde vleesverwerker. 100 producten, waarvan 20 echt afgekeurd. Twee verschillende drempel-instellingen."*

4. **IK DOE — matrix A hardop** (3 min) — toon slide 3 met matrix A. Wijs op het bord en lees hardop:

   | | Model zegt: goed | Model zegt: afgekeurd |
   |---|---|---|
   | **Echt goed (80)** | 75 terecht positief | 5 vals negatief (vals-alarm) |
   | **Echt afgekeurd (20)** | 3 vals positief (gemist) | 17 terecht negatief |

   Zeg langzaam: *"Matrix A — strenge drempel. Vijfenzeventig goede producten gaan terecht door. Vijf goede stuks worden onterecht afgekeurd — vals-alarm, productieverlies. Drie afgekeurde stuks glippen door — gemist, gaan naar de klant. Zeventien afgekeurde stuks worden terecht uit de lijn gehaald."*

   Pauze. Stel de scherpe vraag: *"Drie afgekeurde stuks naar de klant. Vijf goede stuks weggegooid. Welke fout is duurder hier? Schrijf het nog niet op — we komen erop terug."*

5. **Zelfstandig matrix B** (6 min) — toon slide 4 met matrix B. Zet timer op 6 minuten. Zeg: *"Nu jullie. Matrix B — soepelere drempel, dezelfde 100 producten. Vier kwadranten benoemen in werkvloer-taal — zoals ik net deed. Daarna twee vragen op het werkblad: hoeveel vals positieven bij matrix A versus B, hoeveel vals negatieven bij A versus B? Welke matrix zou je kiezen voor jouw lijn? Het antwoord komt straks — eerst tellen."* Loop rond na 2 minuten.

6. **Coachen tijdens rondloop** (lopend) — bij vastlopers GEEN antwoord, alleen kwadrant-vragen:
   - *"Wat zegt het model bij dit kwadrant — goed of afgekeurd?"*
   - *"Is dat product echt goed of echt afgekeurd?"*
   - *"Hoe zou je dat in werkvloer-taal opschrijven — wie merkt het, en hoe?"*

7. **Afronden + brug** (1 min) — slide 5. Vraag: *"Wie heeft alle vier kwadranten van matrix B benoemd?"* Tel handen. *"Goed. Twee getallen op een rij: bij matrix A drie vals positieven, bij matrix B nul. Bij matrix A vijf vals negatieven, bij matrix B vijftien. Het antwoord op 'welke is beter' kunnen we straks pas geven — als we twee getallen hebben in plaats van vier."*

**Materiaal:**
- [ ] Slides 1-5
- [ ] wb-01-twee-confusion-matrices-vleesverwerker.md (1 per deelnemer)
- [ ] Pen
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Tel innerlijk tot 7 na elke open vraag. Stilte is je vriend.
> - Geef GEEN formule in fase 1. De woorden 'precision' en 'recall' vallen pas op slide 6.
> - Een deelnemer die heel snel klaar is: vraag *"Hoeveel vals negatieven bij matrix B? En wat zou dat op jouw lijn kosten?"* — activeer de kosten-blik die fase 3 voorbereidt.

> **🔴 Valkuil — deelnemers verwarren TP/FP/FN/TN-kwadranten:**
> Dit is de meest voorkomende valkuil van het hele LO. Conventie *"positief = goed, negatief = afgekeurd"* expliciet, en de vier werkvloer-zinnen zichtbaar op het bord houden. Bij vergissing corrigeer je MET de werkvloer-vertaling, niet met de term. *"Jij bedoelt het geval dat het product écht goed is maar het model afkeurt — dat is vals negatief."* De term volgt het beeld, niet andersom.

> **🔴 Valkuil — trainer introduceert precision/recall te vroeg:**
> Strikt scheiden. Fase 1 = tellen + werkvloer-taal. Als een deelnemer vraagt *"wat is de berekening?"* — antwoord met een wedervraag: *"wat zou je willen weten — hoe vaak het model gelijk heeft als het afkeurt, of of het alle afkeur vindt?"* Beide vragen worden formules. Maar nog niet.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Houd de vier werkvloer-zinnen groot op het bord — laat staan voor heel fase 1 en 2. Bij vastlopers: ga één kwadrant samen na door de twee vragen te stellen ('wat zegt het model? wat is het product echt?').
> - **Teamleider sneller:** Bij snel klaar: *"Wat zou een vals positief van matrix B kosten op een echte vleesverwerker — boete, recall-actie, omzet-uitval?"* Activeert kosten-blik voor fase 3 zonder de redenatie weg te geven.

**Antwoordmodel werkblad 1:**

| Element | Verwacht | Toets |
|---|---|---|
| Vier kwadranten matrix A in werkvloer-taal | "75 terecht goed / 5 onterecht afgekeurd / 3 doorgelaten afkeur / 17 terecht afgekeurd" (eigen formulering) | Werkvloer-vertaling aanwezig, niet alleen cijfer |
| Vier kwadranten matrix B in werkvloer-taal | "65 terecht goed / 15 onterecht afgekeurd / 0 doorgelaten afkeur / 20 terecht afgekeurd" | Idem |
| Vergelijking vals positief A versus B | 3 versus 0 | Cijfermatig vergeleken |
| Vergelijking vals negatief A versus B | 5 versus 15 | Cijfermatig vergeleken |
| Eerste keuze matrix A of B | Open antwoord, mag intuïtief | Geen 'goed/fout' — verandert mogelijk na fase 2 |

Veelvoorkomende eerste keuze: matrix A ("hogere getallen bij meeste kwadranten"). Geef hier niet de definitieve uitkomst — fase 2 maakt zichtbaar dat dit niet alle informatie is.

**Transitie naar blok 2:** *"Vier kwadranten — vier getallen per matrix. Het rapport-cijfer dat je van een leverancier krijgt is meestal één getal. We gaan ze terugbrengen naar twee, met betekenis."*

---

### 📘 Blok 2: Precision en recall — formules + narekenen
**00:12 - 00:22** | 10 min | Kolb-fase (leerfase): theoretiseren

**Doel:** Deelnemer kent precision (precisie) en recall (terugvinden) als twee aparte maten met twee verschillende vragen. Berekent ze voor matrix A en matrix B. Ziet de trade-off: strenger ↔ soepeler = recall ↔ precision.

**Werkvorm:** Twee formules apart op het bord (2 min), samen narekenen matrix A (3 min), duo's narekenen matrix B (3 min), plenair trade-off (2 min).

**Instructie:**

1. **Werkblad uitdelen + twee formules apart op het bord** (2 min) — deel wb-02 uit. Toon slide 6. Schrijf op het bord-veld midden NIET onder elkaar, maar naast elkaar:

   **Links:**
   > **precision (precisie):** terecht afgekeurd / (terecht afgekeurd + onterecht afgekeurd)
   > Werkvloer-vraag: *"Als het model afkeurt — heeft het dan echt gelijk?"*

   **Rechts:**
   > **recall (terugvinden):** terecht afgekeurd / (terecht afgekeurd + doorgelaten afkeur)
   > Werkvloer-vraag: *"Vindt het model alle afkeur — of glipt er iets door?"*

   Zeg langzaam: *"Twee maten. Twee verschillende vragen. Precision kijkt naar wat het model afkeurt — heeft het gelijk? Recall kijkt naar wat echt afgekeurd is — vindt het model het terug? Schrijf beide formules over op je werkblad. Vier woorden — onthoud die: terecht afgekeurd, onterecht afgekeurd, doorgelaten afkeur."*

2. **WIJ DOEN — matrix A samen narekenen** (3 min) — toon slide 7. Vraag: *"Matrix A. Terecht afgekeurd was?"* (groep: 17). *"Onterecht afgekeurd?"* (5). *"Doorgelaten afkeur?"* (3). Schrijf groot op het bord:

   > **precision A = 17 / (17 + 5) = 17 / 22 = 0,77 = 77%**
   > **recall A = 17 / (17 + 3) = 17 / 20 = 0,85 = 85%**

   Zeg: *"Precision 77% — als het model afkeurt, heeft het 77 keer van de 100 gelijk. Recall 85% — van alle echt-afgekeurde stuks vindt het model 85% terug. Drie procent — drie stuks — glippen door."*

3. **Duo's narekenen matrix B** (3 min) — toon slide 8. Zet timer op 3 minuten. Zeg: *"Tweetal met je buurman. Matrix B narekenen — zelfde twee formules, andere getallen. Check elkaars breuk, niet je intuïtie."* Loop rond.

4. **Plenair narekenen + trade-off op bord** (2 min) — toon slide 9. Vraag: *"Wat kwam eruit voor precision B?"* Wacht 7 seconden. Verwacht antwoord: 20 / (20 + 15) = 20/35 = 57%. *"En recall B?"* Verwacht: 20 / (20 + 0) = 100%. Schrijf groot op het bord, naast de A-getallen:

   > **precision B = 20 / (20 + 15) = 20/35 = 0,57 = 57%**
   > **recall B = 20 / (20 + 0) = 1,00 = 100%**

   Vier getallen groot op het bord. Vraag: *"Wat valt je op?"* Wacht 7 seconden.

   Trek expliciet: *"Strenger naar soepeler — recall stijgt van 85% naar 100%, vijftien procentpunten hoger. Maar precision zakt van 77% naar 57%, twintig procentpunten lager. Die ruil is de trade-off. Strenger = recall ↑, precision ↓. Soepeler = precision ↑, recall ↓. Beide tegelijk maximaal kan vrijwel nooit."* Schrijf de trade-off in één zin onder de vier getallen.

**Materiaal:**
- [ ] Slides 6-9
- [ ] wb-02-precision-recall-formules.md
- [ ] Rekenmachine of telefoon per deelnemer + 2 reserve
- [ ] Bord of flip-over (twee formules naast elkaar + vier getallen + trade-off-zin)
- [ ] Stiften
- [ ] Timer
- [ ] Optioneel: tablets met `model-precision-recall-drempel.jsx` voor deelnemers die de drempel-trade-off tactiel willen ervaren (vervangt of vult wb-02 aan)
- [ ] Optioneel: `video/composition.tsx` (Remotion `ConfusionMatrixVideo`, ~90s) — pre-rendered MP4 of live preview op beamer, in te zetten na het narekenen van matrix B

> **💡 Tips voor de trainer:**
> - Schrijf precision en recall NAAST elkaar, niet onder elkaar. Visueel onderscheid voorkomt dat deelnemers de formules verwarren.
> - Bij stilte na *"wat valt je op?"* — tel tot 7. Bij blijvende stilte: *"Eén getal stijgt. Het andere zakt. Welk patroon?"* Daarna nog 5 seconden.
> - Eerste-keer-rekenaars maken vaak de fout dat ze 17/(17+3) als 17/3 lezen. Schrijf de optelling tussen haakjes groot op.

> **🔴 Valkuil — rekenfouten onopgemerkt laten:**
> Bij verschillende duo-uitkomsten plenair stap-voor-stap nakijken op het bord. Schrijf de breuk groot, vraag de groep wie een ander getal heeft. Bij verschil: *"welk getal is teller, welk noemer?"* Normaliseer dat de eerste keer rekenen lastig is.

> **🔴 Valkuil — formules onder elkaar in één blok schrijven:**
> Voorkom dat. Twee formules NAAST elkaar — links precision, rechts recall. Anders gaan deelnemers in fase 3 de getallen door elkaar gebruiken.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Schrijf elke breuk groot op het bord, met de optelling tussen haakjes. Bij rekenonzekerheid: *"17 gedeeld door 22 — wat zegt je rekenmachine?"* Laat één deelnemer hardop voorrekenen.
> - **Teamleider sneller:** Bij snel klaar: *"Als jullie zelf konden draaien aan de drempel — welk getal zou je willen optimaliseren bij jullie afkeur-systeem?"* Bereidt fase 3 voor.
> - **Bij weinig tijd:** Reken matrix A samen voor, sla duo-narekenen matrix B over en schrijf B-uitkomsten direct op het bord. Maar dit verzwakt de Bloom-toepassing — alleen bij echte tijdnood.

**Antwoordmodel werkblad 2:**

| Element | Verwacht | Toets |
|---|---|---|
| Twee formules overgeschreven | precision + recall met vier woorden | Beide compleet, in eigen handschrift |
| Matrix A precision | 77% (afgerond) | Berekening 17/22 zichtbaar |
| Matrix A recall | 85% | Berekening 17/20 zichtbaar |
| Matrix B precision | 57% (afgerond) | Berekening 20/35 zichtbaar |
| Matrix B recall | 100% | Berekening 20/20 zichtbaar |
| Trade-off-zin | Eigen formulering: "strenger = recall ↑, precision ↓" of vergelijkbaar | Beide kanten benoemd |

Typische rekenfouten: verkeerde noemer (alle echt-afgekeurde versus alles wat het model afkeurt), verwisseling van vals positief en vals negatief, niet afronden (77,27% in plaats van 77%).

**Transitie naar blok 3:** *"Twee maten, één trade-off. Maar welke kant kies je — meer precision of meer recall? Dat is geen wiskunde — dat is bedrijfslogica. Twee scenario's."*

---

### 🟣 Blok 3: Welke fout is duurder? — twee scenario's + eigen werkvloer-keuze
**00:22 - 00:35** | 13 min | Kolb-fase (leerfase): reflecteren

**Doel:** Deelnemer benoemt voor twee contrasterende scenario's (luxe-segment horloges, voedselveiligheid vleesverwerker) welke fout duurder is. Trekt de bedrijfslogica-regel: precision waar vals positief duurder is, recall waar vals negatief duurder is. Kiest voor de eigen werkvloer-AI welke prioriteit moet krijgen.

**Werkvorm:** Scenario 1 plenair (3 min), scenario 2 plenair (3 min), bedrijfslogica-regel op bord (1 min), individueel eigen werkvloer-keuze (5 min), drie antwoorden plenair ophalen (1 min).

**Instructie:**

1. **Werkblad uitdelen + scenario 1: luxe-segment** (3 min) — deel wb-03 uit. Toon slide 10. Zeg: *"Scenario één. Een fabrikant van handgemaakte horloges — vierduizend euro per stuk. Visuele eindcontrole door een AI-camera. Twee fouten kunnen voorkomen."*

   Schrijf op bord-veld rechts (eerste helft, laat tweede helft leeg):
   > **Luxe-segment (horloges):**
   > Vals positief = defect horloge gaat naar klant
   > Vals negatief = goed horloge afgekeurd

   Vraag: *"Wat kost een vals positief bij dit horloge?"* Wacht 7 seconden. Verwacht antwoorden: retourzending, klantontevredenheid, merkschade. Vraag door: *"En een vals negatief?"* Verwacht: productiekost, paar honderd euro materiaal, jammer maar geen merkschade. Vraag: *"Welke is duurder?"* Wacht. Verwacht: vals positief. *"En welke maat wil je dan hoog hebben — precision of recall?"* Verwacht: precision.

   Schrijf op bord onder luxe-segment:
   > **→ vals positief duurder → precision hoog**

2. **Scenario 2: voedselveiligheid** (3 min) — toon slide 11. Zeg: *"Scenario twee. Terug naar de vleesverwerker uit fase 1. Twee fouten."*

   Schrijf op bord:
   > **Voedselveiligheid (vleesverwerker):**
   > Vals positief = afgekeurd vlees gaat naar consument
   > Vals negatief = goed vlees afgekeurd

   Vraag: *"Wat kost een vals positief in voedsel?"* Wacht 7 seconden. Verwacht: recall-actie, boete, gezondheidsschade, levens. *"En een vals negatief?"* Verwacht: productiekost, dubbele inspectie. *"Welke is duurder?"* Verwacht: vals positief. *"Maat?"* Verwacht: recall.

   Schrijf onder voedselveiligheid:
   > **→ vals positief duurder → recall hoog**

   Pauze. Vraag: *"Bij beide scenario's is vals positief duurder — maar de keuze valt verschillend uit. Hoe kan dat?"* Wacht 7 seconden. Verwacht: bij luxe is precision de juiste maat want we willen alleen écht-defect afkeuren; bij voedsel is recall de juiste maat want we willen alle afkeur vinden. Het verschil zit in WAT je wilt minimaliseren — onterechte afkeur (luxe) of gemiste afkeur (voedsel). Hou dit gesprek kort — drie minuten max.

3. **Bedrijfslogica-regel op bord** (1 min) — toon slide 12. Schrijf op het bord-veld rechts (tweede helft) groot en zichtbaar:

   > **Bedrijfslogica-regel:**
   > **Precision** belangrijk als vals positief duurder is dan vals negatief
   > **Recall** belangrijk als vals negatief duurder is dan vals positief
   > *(geen wiskundige regel — een kosten-keuze)*

   Zeg: *"Geen wiskundige regel. Een bedrijfslogica-regel. De vraag is altijd dezelfde: welke fout is duurder op deze lijn?"*

4. **Individueel — eigen werkvloer-AI** (5 min) — toon slide 13. Zeg: *"Vijf minuten — voor je eigen werkvloer. Welke AI-toepassing ken je — een inspectiecamera, een sorteersysteem, een afkeur-camera, een eindcontrole? Wat is een vals positief op die lijn? Wat is een vals negatief? Welke is duurder? Kies precision of recall. Schrijf één onderbouwing op."* Zet timer. Loop rond binnen 2 minuten.

5. **Drie antwoorden plenair ophalen** (1 min) — toon slide 14. Vraag drie deelnemers met contrasterende contexten: *"Jouw keuze? En waarom?"* Houd kort: 20 seconden per persoon. Spiegel: *"Jij koos recall omdat veiligheid telt; bij hem speelt precision omdat een retourzending meer kost dan productieverlies."* Laat de groep zien dat de regel niet één antwoord heeft maar één denkstap (kosten van fouten vergelijken).

**Materiaal:**
- [ ] Slides 10-14
- [ ] wb-03-werkvloer-keuze-precision-of-recall.md
- [ ] Bord-veld rechts (twee scenario's + bedrijfslogica-regel)
- [ ] Stiften
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Laat de groep beredeneren — geef niet zelf 'luxe = precision, voedsel = recall'. Stel kostenvragen, wacht 7 seconden. De redenatie moet van de groep komen, anders kan de deelnemer fase 4 niet zelf invullen.
> - Bij stilte na een kostenvraag: noem zelf één voorbeeld, dan stel je de vraag opnieuw. *"Een retourzending kost de fabrikant misschien 200 euro plus verzending. Wat is een afgekeurd horloge waard in productiekost?"*
> - Houd plenair gesprek max 6 minuten. De tijd is in fase 3 schaars omdat de individuele schrijfronde (5 min) en de plenaire afronding (1 min) niet ingekort mogen worden.

> **🔴 Valkuil — trainer geeft zelf het antwoord op de duurder-vraag:**
> Dit is de tweede sluipendste valkuil. Als de trainer 'hier is precision belangrijker' zegt, kan de deelnemer fase 4 niet zelf invullen. Stel kostenvragen, laat de groep redeneren. Geef pas een samenvatting nadat de groep de logica heeft uitgesproken.

> **🔴 Valkuil — twee scenario's te uitgebreid bespreken:**
> Per scenario max 3 minuten. Niet de hele vleesverwerker-bedrijfsvoering doornemen — alleen de kostenvraag (vals positief versus vals negatief) en de daaruit volgende maat-keuze. Anders blijft er geen tijd voor de eigen werkvloer.

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers in de individuele schrijfronde: geef twee voorbeelden van eigen werkvloer-AI ('de inspectiecamera op de zomerlijn', 'het afkeur-systeem bij de uitloop'). Help met de eerste 'vals positief = wat?'-vraag concreet.
> - **Teamleider sneller:** Bij snel klaar: *"Welke kosten zou je naar je manager brengen — geld, tijd, merk of veiligheid? Welke is op jullie lijn dominant?"* Activeert strategische blik.
> - **Gemengde groep:** Vraag in plenaire ronde eerst operators welke fout ze op de lijn zien, daarna teamleiders welke fout het meest druk legt op het budget.

**Antwoordmodel werkblad 3:**

| Element | Verwacht | Toets |
|---|---|---|
| Scenario 1 luxe-segment | "vals positief duurder, precision hoog" | Beide elementen aanwezig |
| Scenario 2 voedselveiligheid | "vals positief duurder, recall hoog" | Beide elementen aanwezig |
| Eigen werkvloer-AI benoemd | Concrete toepassing (inspectiecamera, sorteer, afkeur) | Niet abstract ('kwaliteit') |
| Vals positief en vals negatief voor eigen werkvloer | Beide gedefinieerd in eigen taal | Beide aanwezig |
| Welke duurder | Met onderbouwing in geld, tijd, merk of veiligheid | Onderbouwing aanwezig |
| Precision of recall gekozen | Aansluitend op duurder-keuze | Logisch consistent |

Veelgekozen onderbouwingen:
- Veiligheidskritisch (voedsel, medisch, auto): recall — vals positief kan levens kosten
- Hoge productiekost per stuk en/of merkgevoelig: precision — vals negatieven hopen productieverlies op
- Compliance- of audit-gedreven (farma, lucht- en ruimtevaart): recall — geen defect mag passeren
- Snel-bewegende consumentengoederen, lage marge: precision — vals afkeuren breekt de marge

**Transitie naar blok 4:** *"Je weet nu welke kant je kiest. Laatste tien minuten: hoe maak je er gedrag van? Drie vragen voor deze week."*

---

### 🟠 Blok 4: Eigen werkvloer-AI doorlichten + vraag deze week
**00:35 - 00:45** | 10 min | Kolb-fase (leerfase): experimenteren

**Doel:** Deelnemer kiest één concrete AI-toepassing op zijn eigen lijn, beantwoordt drie vragen schriftelijk (vals positief, vals negatief, welke duurder), kiest precision of recall als prioriteit, toetst die keuze halverwege in een DUO-SPIEGEL bij een collega, formuleert één concrete vraag voor leverancier/IT/kwaliteit deze week, en noteert één getal dat hij wil achterhalen.

**Werkvorm:** Werkblad-uitleg (1 min), individueel werken stap 1-3 (4 min), **DUO-SPIEGEL** (2 min — CAR-relatedness-anker), individueel afronden stap 4 (1 min), plenaire één-zin-ronde (1 min), transferopdracht afsluiten (1 min).

**Instructie:**

1. **Werkblad uitdelen + opdracht** (1 min) — deel wb-04 uit. Toon slide 15. Zeg: *"Laatste tien minuten. Vier stappen op het verkenningsblad. Stap 1 — kies één AI-toepassing op je eigen lijn. Stap 2 — drie vragen: wat is een vals positief, wat een vals negatief, welke is duurder? Stap 3 — kies precision of recall plus één onderbouwing. Stap 4 — formuleer één concrete vraag voor leverancier, IT of kwaliteit deze week, plus één getal dat je wilt achterhalen. Geen IT-kennis nodig — werkvloer-kennis is genoeg. Halverwege onderbreek ik even voor een duo-spiegel — ik kondig dat aan."*

2. **Individueel werken — stap 1-3** (4 min) — zet timer op 4 minuten. Loop rond binnen 2 minuten. Coach met grens-vragen, geen antwoorden:
   - *"Welk AI-systeem of welke visuele check is er op jouw lijn? De inspectiecamera bij de zomerlijn? Het afkeur-systeem bij de uitloop? Een sorteersysteem in verpakking?"*
   - *"Als dat systeem afkeurt, wat gebeurt er met dat product? En als hij niet afkeurt, en het was eigenlijk afgekeurd?"*
   - *"Wat kost een vals positief op jouw lijn — in geld, tijd, merk of veiligheid? Heb je daar een voorbeeld van uit het laatste jaar?"*

3. **DUO-SPIEGEL** (2 min) — onderbreek de stilte. Zeg: *"Stop even, vier minuten zijn om. Wissel je werkblad met je buurman of buurvrouw. Lees stap 2 en 3 van de ander — wat is bij hem of haar vals positief, wat is vals negatief, en welke maat koos hij of zij? Stel daarna één spiegel-vraag: 'klopt jouw maat-keuze met de fout die jij duurder vond?' Dit is geen beoordeling — jullie zijn elkaars kwaliteits-check. Twee minuten."* Loop rond. Bij stille duo's geef voorbeeld-spiegel: *"jij koos precision omdat vals-alarm duurder is — klopt dat met je onderbouwing?"* Na 2 min: *"Werkbladen terug. Laatste minuut: stap 4 individueel afronden — vraag + getal."*

4. **Individueel afronden — stap 4** (1 min) — kort, individueel. Trainer-vraag bij vastlopers: *"Wie zou je deze vraag moeten stellen — leverancier, IT, kwaliteit? Wanneer zie je die persoon deze week?"*

5. **Plenaire één-zin-ronde** (1 min) — toon slide 16. Zeg: *"Snel rondje — iedereen één zin: welke kant koos je (precision of recall), en welke vraag stel je deze week aan wie?"* Houd kort: max 10 seconden per persoon. Begin zelf met een voorbeeld als de stilte te lang duurt: *"Bij mij zou het recall zijn, ik vraag aan kwaliteit-Esra wat de recall is van onze afkeur-camera op de zomerlijn."* Noteer de vragen op het bord — komen terug in volgende sessie.

6. **Transferopdracht afsluiten** (1 min) — toon slide 17. Zeg: *"Drie stappen deze week. Eén — kies één AI-toepassing op je lijn, schrijf op wat een vals positief is en een vals negatief. Twee — stel die ene vraag aan leverancier, IT of kwaliteit. Drie — noteer het getal dat terugkomt. Datum laatste rapport, precision of recall in dat rapport, of de drempelinstelling die nu actief is. Neem alle drie de uitkomsten mee naar volgende sessie. Bonus — praat deze week één keer met een collega over een afkeur-moment: 'was dit een vals positief of een vals negatief?' Vaak ontdek je dat collega's de twee fout-soorten anders waarderen. Dat is een nuttig gesprek voor elk AI-traject."*

**Materiaal:**
- [ ] Slides 15-17
- [ ] wb-04-eigen-werkvloer-ai-doorlichten.md
- [ ] Pen
- [ ] Timer
- [ ] Bord (om vragen voor leverancier/IT te noteren)

> **💡 Tips voor de trainer:**
> - Plenair: max 15 seconden per persoon. Eindig op tijd. Een goede afsluiting is beter dan uitlopen.
> - Bij iemand die geen AI op de eigen lijn kent: geef twee concrete suggesties uit een buurafdeling of een ophanden zijnde implementatie. Help met de allereerste 'wat is een vals positief'-vraag concreet.
> - Bij iemand die een vraag te abstract formuleert ('ik ga letten op precision') — begrens: *"Wat doe je precies, wanneer, met wie?"* Voorbeeld: *"Donderdagmiddag vraag ik aan Esra van kwaliteit wat de recall van onze afkeur-camera is."*

> **🔴 Valkuil — eigen werkvloer-AI te vaag of niet aanwezig:**
> Voorkom dat de deelnemer afhaakt. Geef concrete voorbeelden: inspectiecamera, sorteersysteem, afkeur-camera, eindcontrole-AI, weegsysteem, lekkage-detectie bij verpakking. Help met de eerste vraag, niet met het antwoord.

> **🔴 Valkuil — vraag voor leverancier te abstract:**
> *"Ik ga vragen hoe het zit met precision"* is geen vraag. Begrens: *"Welke precision — van welk systeem, op welke lijn, in welke periode?"* Vraag wordt: *"Wat is de recall van onze afkeur-camera op de zomerlijn in de afgelopen drie maanden?"*

> **🔄 Differentiatie:**
> - **MBO-4 basis:** Bij vastlopers — geef twee voorbeelden van beoordelings-momenten op de werkvloer en laat deelnemer kiezen. Help met de eerste grenswaarde voor 'duurder'.
> - **Teamleider sneller:** Bij snel klaar: *"Hoe ga jij in jouw team systematisch precision en recall bijhouden? Welke rapportage zou je willen?"* Strategische blik.
> - **Bij niet-werkvloer-deelnemer (zeldzaam):** Laat hem een hypothetisch schema bouwen voor de vleesverwerker-casus of luxe-segment-casus uit de werkbladen.

**Antwoordmodel werkblad 4:**

| Stap | Verwacht | Toets |
|---|---|---|
| 1 — AI-toepassing | Concreet benoemd (inspectiecamera op zomerlijn, sorteer-AI in verpakking, afkeur-camera bij spuitgieten, eindcontrole-AI assemblage, weegsysteem, lekkage-detectie) | Niet abstract ('kwaliteit') |
| 2 — Vals positief eigen lijn | Concreet beschreven (wat gaat er fout, wie merkt het) | In eigen werkvloer-taal |
| 2 — Vals negatief eigen lijn | Idem | Idem |
| 2 — Welke duurder | Onderbouwing in geld, tijd, merk of veiligheid | Onderbouwing aanwezig |
| 3 — Precision of recall + onderbouwing | Eén van twee + minimaal één zin onderbouwing | Logisch consistent met stap 2 |
| 4 — Vraag voor leverancier/IT/kwaliteit | Wat-aan-wie-wanneer (donderdag aan Esra: wat is de recall van X-systeem op Y-lijn) | Concreet, niet *"ik ga letten op precision"* |
| 4 — Getal om te achterhalen | Datum laatste rapport, precision/recall-getal, drempelinstelling, of aantal vals positieven afgelopen periode | Eén concreet getal |

**Veelvoorkomende toepassingen:**
- Inspectiecamera op visuele kwaliteitslijn
- Sorteersysteem op formaat, kleur of gewicht
- Afkeur-camera bij spuitgieten of extruderen
- Eindcontrole-AI bij assemblage
- Weegsysteem met automatische afkeur
- Lekkage-detectie bij verpakking

**Veelvoorkomende vragen voor deze week:**
- "Wat is de recall van onze afkeur-camera op de zomerlijn?"
- "Hoe vaak wordt de precision opnieuw gemeten — per maand, per jaar?"
- "Welke drempel staat onze sorteer-AI op dit moment ingesteld?"
- "Wat is het laatste evaluatie-rapport — kan ik dat zien?"
- "Hoeveel vals positieven hebben we gehad de afgelopen maand?"

**Transitie naar afsluiting:** *"Mooi werk. Drie stappen deze week — daar zit beweging in. Volgende sessie bespreken we welk getal terugkwam, en welke vraag scherper gesteld kan worden bij wie geen antwoord kreeg."*

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-twee-confusion-matrices-vleesverwerker | n + 2 | A4 enkelzijdig (matrix A + matrix B + kwadrant-vragen) |
| ☐ | wb-02-precision-recall-formules | n + 2 | A4 enkelzijdig (twee formules + narekenen A en B + trade-off-vraag) |
| ☐ | wb-03-werkvloer-keuze-precision-of-recall | n + 2 | A4 enkelzijdig (twee scenario's + eigen werkvloer + onderbouwing) |
| ☐ | wb-04-eigen-werkvloer-ai-doorlichten | n + 2 | A4 enkelzijdig (vier stappen + getal-veld) |
| ☐ | Pennen | n + 5 | Reserve |
| ☐ | Rekenmachines | 2 reserve | Deelnemer brengt eigen telefoon mee |
| ☐ | Flip-over of bord | 1 | Drie velden vooraf voorbereiden (matrix A links, formules midden, scenario's + regel rechts) |
| ☐ | Dikke stiften | 3 kleuren | Zwart (formules), rood (matrices), blauw (regel) |
| ☐ | Timer / mobiel met geluid | 1 | |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen, matrix-leesbaarheid achterste rij |
| ☐ | presentatie.slidev.md geopend | 1 | Presenter-modus |
| ☐ | Optioneel: `video/composition.tsx` (Remotion, export id `ConfusionMatrixVideo`) | 1 | ~90s, na narekenen matrix B in fase 2; pre-rendered MP4 of live preview |
| ☐ | Optioneel: tablets met `model-precision-recall-drempel.jsx` | n | Aanvulling op wb-02/wb-03 voor tactiele drempel-trade-off |

n = aantal deelnemers

---

## Flexibiliteit

| Situatie | Alternatief |
|---|---|
| Fase 1 loopt uit (groep leest matrices traag) | Verkort fase 3 met 2 min: laat de individuele schrijfronde inkorten tot 3 min, en vraag plenair twee in plaats van drie antwoorden. Niet inkorten op fase 2 — daar zit de wiskundige helderheid die de rest draagt. |
| Duo's matrix B leveren verschillende uitkomsten | Plenair stap-voor-stap nakijken op het bord — schrijf 20/(20+15) groot, vraag wie een ander getal heeft, ga terug naar teller en noemer. Normaliseer: eerste keer rekenen kost tijd. |
| Een deelnemer verwart consequent vals positief en vals negatief | Loop naar bord, wijs de vier werkvloer-zinnen aan. *"Welk geval bedoel je? Wat zegt het model? Wat is het product echt?"* De term volgt het beeld. |
| Plenaire scenario-bespreking dreigt uit te lopen | Begrens per scenario tot 3 min. Bij doorgaande discussie: *"Mooi punt — parkeer voor de Bonus-opdracht deze week."* |
| Eigen-werkvloer-AI ontbreekt bij meerdere deelnemers | Suggereer concreet: afkeur-camera bij buurafdeling, sorteersysteem in verpakking, weegcontrole bij uitloop, lekkage-detectie. Help één keer met de eerste 'vals positief = wat?'-vraag. |
| Plenaire ronde fase 4 dreigt uit te lopen | Begrens tot 15 sec per persoon. Bij grote groep: laat 4 deelnemers delen, anderen schrijven op een sticky en plakken die voor je weggaan. |
| Groep is te klein (4 of minder) | Duo-narekenen in fase 2 wordt drietal. Plenaire ronde fase 4 versmelt met afsluiting. |

---

## Snel-overzicht

| Fase (leerfase) | Kernactie | Anker-uitkomst |
|------|-----------|----------------|
| 1 ervaren | Twee matrices lezen, vier kwadranten in werkvloer-taal, geen formule | Vier zinnen per matrix, twee getallen vergeleken (vals pos / vals neg) |
| 2 theoretiseren | Twee formules + narekenen A en B, trade-off op bord | precision A=77%, recall A=85%, precision B=57%, recall B=100%, trade-off-zin |
| 3 reflecteren | Twee scenario's plenair, bedrijfslogica-regel op bord, eigen keuze schrijven | Regel geformuleerd, eigen precision-of-recall-keuze met onderbouwing |
| 4 experimenteren | Eigen werkvloer-AI doorlichten + DUO-SPIEGEL + vraag voor deze week + getal om te achterhalen | Vier stappen ingevuld + duo-spiegel doorlopen + concrete vraag wat-aan-wie-wanneer |

**Slagingscriterium:** beide matrices correct gelezen in werkvloer-taal + precision en recall berekend voor minimaal één matrix op één procentpunt nauwkeurig + duurder-fout benoemd voor beide scenario's + precision-of-recall-keuze voor eigen werkvloer met onderbouwing + één concrete vraag voor leverancier/IT/kwaliteit deze week.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor reflectie op de groep)
- [ ] Genoteerd: typische rekenfouten in fase 2 (voor scherpere uitleg volgende keer)
- [ ] Genoteerd: welke werkvloer-AI's gekozen door deelnemers (input voor volgende sessie)
- [ ] Genoteerd: welke vragen aan leverancier/IT geformuleerd (komen terug)
- [ ] xAPI-statements verstuurd: `experienced`, `analyzed`, `attempted`, `completed`

---

*AIMM Curriculum | AI Fundamentals Module 2 (Train) | Confusion matrix, precision en recall*
*Bron: ko-ai-fund-212 + ko-ai-fund-133 + ko-ai-fund-135 + praktijklessen AI-evaluatie RLC Oost/Zuid 2025-2026.*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
