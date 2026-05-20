# Draaiboek: Resultaten interpreteren en het model verbeteren

**Leerobject:** lo-smart-mfg-513
**Kennisobjecten:** ko-smart-mfg-513, ko-smart-mfg-514
**Doelgroep:** MBO-3 operators (Module 1 afgerond)
**Totale duur:** 45 minuten
**Groepsgrootte:** 6-12 deelnemers
**Format:** Interactieve workshop (Kolb-cyclus, 4 fasen, coachend)

---

## Voorbereiding (15 min voor aanvang)

### Dit leerobject volgt direct op LO-511

De deelnemers hebben zojuist foto's gelabeld en een drempelwaarde gekozen. De confusion matrices moeten klaarliggen op basis van hun gekozen drempelwaarden. Als je met het simulatie-werkblad werkt, liggen de resultaten al vast.

### Materialen klaarzetten

| Materiaal | Aantal | Locatie |
|---|---|---|
| Confusion matrix per duo (matching hun gekozen drempelwaarde) | 1 per duo | Klaarleggen |
| Werkblad confusion matrix | 1 per deelnemer | Op de stoelen |
| Werkblad reflectie-resultaten | 1 per deelnemer | Op de stoelen |
| Handout precision, recall en verbetercyclus | 1 per deelnemer | Apart (uitdelen bij fase 3) |
| Werkblad actieplan-verbetering | 1 per duo | Apart (uitdelen bij fase 4) |
| Simulatie-werkblad (met resultaten bij aangepaste drempel) | 1 per duo | Apart (uitdelen bij fase 4) |
| Whiteboard + stiften | 1 | Vooraan |
| Rekenmachines (of telefoons) | 1 per deelnemer | Op tafel |

### Whiteboard voorbereiden

Teken een lege confusion matrix op het whiteboard:

```
              Model: GOED    Model: DEFECT
Werkelijk GOED    [    ]        [    ]
Werkelijk DEFECT  [    ]        [    ]
```

En daaronder ruimte voor:
```
Duo | Drempel | Precision | Recall
 A  |         |           |
 B  |         |           |
 C  |         |           |
```

---

## Sessie-opbouw

### Fase 1: EXPERIMENTEREN — Confusion matrix lezen (10 min)

**0:00-0:02 | Introductie (2 min)**

Zeg:

> "Jullie hebben net een model geconfigureerd. Nu gaan we kijken: hoe goed werkt het? Daarvoor gebruiken we een confusion matrix — een tabel die precies laat zien wat het model goed en fout deed."

Toon de lege confusion matrix op het whiteboard. Leg de vier vakken uit met EEN voorbeeld:

> "Terecht goed: het product is goed en het model zegt goed. Vals alarm: het product is goed maar het model zegt defect. Gemist defect: het product is defect maar het model laat het door. Terecht defect: het model vindt een echt defect."

**Houd dit kort.** Maximaal 2 minuten. De deelnemers leren het door te doen.

**0:02-0:10 | Zelf invullen (8 min)**

Deel de confusion matrices uit (per duo, matching hun drempelwaarde). Deel de werkbladen uit.

> "Vul de vier getallen in op je werkblad. Bereken daarna de precision en recall. De formules staan op het werkblad."

Loop rond. Help alleen bij rekenfouten, niet bij interpretatie. Stel coachende vragen:
- "Hoeveel valse alarmen heeft jullie model?"
- "Hoeveel defecten heeft het gemist?"
- "Wat vind je van dat getal?"

**VALKUIL:** Niet te snel naar de uitleg van precision/recall. Laat de deelnemers eerst zelf de getallen zien en voelen wat ze betekenen.

---

### Fase 2: REFLECTEREN — Vergelijking en trade-off (10 min)

**0:10-0:15 | Duo-vergelijking (5 min)**

Laat duo's hun confusion matrices vergelijken met een ander duo. Vraag:

> "Welk duo heeft de hoogste precision? Welk duo de hoogste recall? Is er een duo dat allebei hoog heeft?"

**0:15-0:20 | Plenaire terugkoppeling (5 min)**

Schrijf de resultaten van alle duo's op het whiteboard (de voorbereide tabel). Bespreek het patroon:

> "Duo A koos drempel 0.3 — streng. Hoge recall (95%), maar veel valse alarmen. Duo B koos 0.7 — soepel. Hoge precision (91%), maar 6 gemiste defecten. Zien jullie de trade-off?"

Stel de kernvraag:

> "Wat is erger voor jullie product: een vals alarm of een gemist defect?"

Laat 2-3 deelnemers reageren. Vat samen.

**BELANGRIJK:** Er is geen goed antwoord. Het hangt af van het product, het risico, de beschikbare capaciteit. Dit is de kernles.

---

### Fase 3: THEORETISEREN — Precision, recall en de verbetercyclus (10 min)

**0:20-0:25 | Precision en recall in operatortaal (5 min)**

Gebruik de resultaten van de groep als voorbeeld:

> "Precision is: als het model alarm slaat, hoe vaak is het dan echt raak? Bij duo A was dat 63%. Dat betekent: van elke 10 afgekeurde producten waren er maar 6 echt defect. De rest was vals alarm."

> "Recall is: van alle echte defecten, hoeveel vindt het model? Bij duo B was dat 63%. Dat betekent: van elke 10 echte defecten miste het model er 4."

**Gebruik GEEN wiskundige formules in je uitleg.** De formules staan op het werkblad. In de uitleg gebruik je woorden en de concrete getallen van de groep.

**0:25-0:30 | De verbetercyclus (5 min)**

> "Het model is niet af. Net als een machine op de lijn heeft het bijsturing nodig."

Presenteer de vier stappen: test > analyseer > verbeter > hertest.
Presenteer de drie strategieen: meer data, betere labels, drempel bijstellen.

Deel de handout uit.

**VALKUIL:** Maak de theorie niet te lang. De operators hebben de kern al ervaren. De handout is voor thuis.

---

### Fase 4: EXPERIMENTEREN — Verbeteractie (15 min)

**0:30-0:37 | Duo-opdracht (7 min)**

Deel het actieplan-werkblad uit. Zeg:

> "Jullie model is niet perfect. Dat hoeft ook niet. Maar jullie kunnen het beter maken. Analyseer de fouten. Kies een verbeterstrategie. Formuleer wat je zou veranderen."

Na de analyse: deel het simulatie-werkblad uit met resultaten bij een aangepaste drempelwaarde. Laat duo's hun verbetering testen.

Loop langs. Stel coachende vragen:
- "Welk type defect miste jullie model het vaakst?"
- "Welke strategie kozen jullie? Waarom?"
- "Werd het model beter?"

**0:37-0:42 | Presentaties (5 min)**

Laat 2-3 duo's hun verbeteractie en resultaat presenteren (1 minuut per duo).

Reageer met inhoudelijke feedback:

> "Jullie kozen voor meer data van kleurafwijkingen. Dat is precies de juiste strategie: gericht bijtrainen op wat het model mist."

**0:42-0:45 | Afsluiting + transfer (3 min)**

Vat samen:

> "Vandaag hebben jullie geleerd hoe je een model beoordeelt en verbetert. In Module 3 gaan jullie dit doen met jullie eigen producten en jullie eigen foto's."

Transferopdracht:

> "Bedenk voor je eigen product: wat is belangrijker — precision of recall? Bespreek het met je leidinggevende. Vraag ook aan de kwaliteitsafdeling: hoeveel producten worden per week onterecht afgekeurd of onterecht doorgelaten? Dat zijn de getallen voor jouw eigen confusion matrix."

---

## Differentiatie

### Snelle deelnemers

- Laat ze bij fase 1 ook de accuracy berekenen ((terecht goed + terecht defect) / totaal)
- Geef ze een bonusvraag: "Wat als je model twee types defecten moet onderscheiden? Hoe zou de confusion matrix er dan uitzien?"
- Zet ze als sparringpartner bij een duo dat moeite heeft met de berekeningen

### Deelnemers die moeite hebben met rekenen

- Help ze bij het invullen van de formules ("hier vul je het aantal terecht defect in")
- Laat ze de berekening met de rekenmachine doen
- Focus op de interpretatie: "Wat betekent dit getal voor jou op de werkvloer?"
- Koppel ze aan een sterkere rekenaar in het duo

### Deelnemers die het concept "goed genoeg" lastig vinden

- Verwijs naar de analogie met meetinstrumenten: "Geen meter is 100% nauwkeurig. Maar als hij nauwkeurig genoeg is voor jouw toepassing, is het goed."
- Vraag: "Hoe doet de operator die dit nu handmatig doet het na 6 uur werken? Is het model beter?"

---

## Veelgemaakte fouten

| Fout | Gevolg | Oplossing |
|---|---|---|
| Precision/recall te wiskundig uitleggen | Afhakers bij MBO-3 | Gebruik woorden en de concrete getallen van de groep |
| Te lang stilstaan bij formules | Verlies van energie | Formules staan op werkblad, focus op interpretatie |
| Vergeten terug te verwijzen naar LO-511 | Geen samenhang ervaren | Expliciet: "Dit is het resultaat van jullie model" |
| Verbeterfase overslaan wegens tijd | Geen afsluiting cyclus | Theorie kort houden (max 10 min), verbeterfase is essentieel |
| Te veel nadruk op "het perfecte model" | Frustratie | "Goed genoeg" is het criterium, niet "perfect" |

---

## Didactische verantwoording

| Principe | Hoe toegepast |
|---|---|
| **Coachend** (Hersey & Blanchard) | Bewust bekwaam = vragen stellen, niet voordoen. Eigen analyse en keuzes. |
| **Experiential learning** (Kolb) | Start met eigen resultaten, reflecteer op trade-off, dan theorie, dan verbeteren. |
| **Concrete ervaring** (Kolb) | Werkt met confusion matrix van eigen model, niet abstract voorbeeld. |
| **CAR-model** (Deci & Ryan) | Competentie: eigen resultaten analyseren. Autonomie: eigen verbeterstrategie kiezen. Relatie: duo-vergelijking. |
| **Transfer** | Concrete opdracht: precision vs recall voor eigen product bespreken met leidinggevende. |

---

## Na de sessie

- [ ] Werkbladen innemen (voor learning analytics)
- [ ] Noteer: wie had moeite met de berekeningen? Wie begreep de trade-off direct?
- [ ] Check: heeft iedereen de transferopdrachten begrepen (LO-511 + LO-513)?
- [ ] Update de presentatieresultaten voor de groepsreflectie in de closing

---

*AIMM Pipeline | lo-smart-mfg-513 | Draaiboek trainer-versie*
*Didactische bronnen: Hersey & Blanchard (1977), Kolb (1984), Deci & Ryan (2000)*
