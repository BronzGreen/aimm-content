# Draaiboek: Anomaliedetectie in de productie

**Leerobject:** lo-smart-mfg-092
**Kennisobject:** ko-smart-mfg-092
**Doelgroep:** MBO-3 operator, B1 taalniveau
**Duur:** 45 minuten
**Groepsgrootte:** 6-12 deelnemers
**Opstelling:** U-vorm of groepstafels (4 per tafel)

---

## Kernprincipe: Ik doe - Wij doen - Jij doet

Deze sessie is opgebouwd volgens het scaffolding-principe:

| Fase | Wie doet? | Ondersteuning | Activiteit |
|------|----------|---------------|------------|
| 1. Ervaren | **Trainer** doet voor | Maximaal | Worked example met sensordata |
| 2. Reflecteren | **Groep** doet samen | Veel | Begeleide oefening (3 waarden) |
| 3. Theoretiseren | **Trainer** legt uit | Medium | Kort theoretisch kader |
| 4. Experimenteren | **Duo's** doen zelf | Minimaal | 5 sensorwaarden + antwoordmodel |

---

## Voorbereiding (15 minuten voor aanvang)

### Materialen printen
- [ ] Werkblad 1: Meekijk-werkblad (1x per deelnemer)
- [ ] Werkblad 2: Reflectie-werkblad (1x per deelnemer)
- [ ] Werkblad 3: Theorie-handout (1x per deelnemer)
- [ ] Werkblad 4: Oefening met antwoordmodel (1x per deelnemer)

### Scherm/beamer klaarzetten
- [ ] Sensordata-overzicht voor worked example (temperatuur 82 graden, druk 4,2 bar)
- [ ] Drie oefenwaarden voor groepsoefening (trillingen, energie, temperatuurreeks)
- [ ] SVG-diagram drie soorten anomalieen

### Ruimte
- [ ] Flip-over + stiften
- [ ] Stoelen in U-vorm of groepstafels
- [ ] Optioneel: echte sensor om te laten zien

---

## FEED-UP (0:00 - 0:01)

Spreek hardop uit bij aanvang:

> "Na deze sessie kun je zelf afwijkingen herkennen in sensordata van een machine. Je leert drie soorten afwijkingen kennen. Aan het eind oefen je zelfstandig met vijf sensorwaarden."

Dit is de feed-up: de deelnemer weet WAAR hij naartoe werkt.

---

## ACTIVITEIT 1: Worked Example (0:01 - 0:10)

### Doel
De trainer doet VOOR hoe je een anomalie herkent. De deelnemers kijken en noteren.

### Scaffolding-niveau: IK DOE

### Stap voor stap

**0:01** Deel werkblad 1 uit. Zeg: "Ik ga jullie laten zien hoe ik afwijkingen herken in sensordata. Kijk mee en schrijf op wat je opvalt."

**0:02** Toon het sensordata-overzicht. Wijs aan:

> "Kijk, hier zie ik de temperatuur van een motor. Normaal is 65 tot 70 graden. Maar hier zie ik 82 graden. Dat is 12 graden boven het maximum. Dit is duidelijk een afwijking."

Pauze. Laat noteren.

> "We noemen dit een **puntanomalie** — een enkel meetpunt dat flink afwijkt."

**0:05** Tweede voorbeeld:

> "En hier: de druk is 4,2 bar. Tijdens productie is normaal 3,0 tot 3,5 bar. Maar kijk naar het tijdstip: 07:15. De machine is net opgestart. Bij opstart mag de druk hoger zijn, tot 4,5 bar. Dus 4,2 bar is hier GEEN afwijking."

Pauze. Laat noteren.

> "Maar om 14:00 uur zou 4,2 bar WEL een afwijking zijn. Dit noemen we een **contextuele anomalie** — de situatie bepaalt of het normaal is."

**0:08** Stel de groep een vraag:

> "Zien jullie het verschil? Bij de eerste keek ik alleen naar het getal. Bij de tweede moest ik ook weten WAT de machine deed."

### Valkuilen
- Te snel gaan. Deelnemers moeten kunnen meeschrijven.
- Al de groep laten meedoen. Dit is de IK DOE fase.
- Meer dan twee voorbeelden doen. Twee is genoeg.

### Differentiatie
- **Sterke groep:** "Wie heeft al een idee wat het derde type zou kunnen zijn?"
- **Zwakke groep:** Doe een derde voorbeeld voor (collectieve anomalie: stijgende reeks).

---

## ACTIVITEIT 2: Begeleide Groepsoefening (0:10 - 0:22)

### Doel
De groep oefent SAMEN onder begeleiding. Drie waarden, een voor een.

### Scaffolding-niveau: WIJ DOEN

### Stap voor stap

**0:10** Deel werkblad 2 uit. Zeg: "Nu gaan WE het samen doen. Ik laat drie sensorwaarden zien. Jullie bepalen of het een afwijking is."

**0:11** Waarde 1 — Trillingsniveau 0,8 mm/s (normaal 0,2-0,4):

> "Wat denken jullie — is dit een afwijking?"

Laat 2-3 deelnemers antwoorden. Bevestig:

> "Ja, dit is een puntanomalie. Het trillingsniveau is twee keer zo hoog als het maximum. Goed gezien."

**0:14** Waarde 2 — Energieverbruik 12 kWh (normaal 8-10), maar zwaarder product:

> "Is dit een afwijking?"

Laat de groep discussieren. Twee goede antwoorden zijn mogelijk.

> "Goed punt — je moet de context weten. Bij dit zwaardere product is 12 kWh misschien normaal. Dit is waarom context ertoe doet."

**0:17** Waarde 3 — Temperatuur: 68, 69, 70, 72, 74, 77, 80 graden:

> "Elke waarde apart is niet alarmerend. Maar wat valt jullie op?"

Begeleid naar de trend.

> "Dit is een **collectieve anomalie** — een stijgende trend. Geen enkel getal is extreem, maar het patroon is zorgelijk."

**0:20** Na elke waarde: "Welke stap namen jullie?" Bevestig: normaalwaarde checken, context checken, patroon checken. Laat werkblad 2 invullen.

### Valkuilen
- Zelf het antwoord geven als het stil is. Tel tot 7.
- Waarde 2 overslaan omdat het lastig is. Juist de dubbelzinnigheid is leerzaam.
- Werkblad laten invullen tijdens de bespreking. Doe het erna.

### Verdiepingsvragen (reserve)
- "Welk type was het moeilijkst?"
- "Ken je een voorbeeld van je eigen werkvloer waar een machine langzaam slechter werd?"

---

## ACTIVITEIT 3: Theorie (0:22 - 0:30)

### Doel
Kort theoretisch kader. Benoem de drie soorten, verbind met de oefening.

### Stap voor stap

**0:22** Deel werkblad 3 (theorie-handout) uit. Toon het SVG-diagram.

**0:23** Loop de drie soorten door en verwijs TERUG:

> 1. "**Puntanomalie** — bij waarde 1 zagen jullie dit: trillingen 0,8 mm/s."
> 2. "**Contextuele anomalie** — bij waarde 2: energieverbruik bij zwaarder product."
> 3. "**Collectieve anomalie** — bij waarde 3: de stijgende temperatuurreeks."

> "Jullie hebben alle drie de types al herkend. Nu weten jullie ook hoe ze heten."

**0:26** Toon de drie stappen van anomaliedetectie: Voorbereiding, Training, Detectie.

> "Een AI-systeem doet precies wat jullie net deden. Het verschil: een computer doet het 24 uur per dag, bij 100 sensoren tegelijk."

**0:28** Geef het fabrieksvoorbeeld (brandstoftanks, 100+ sensoren).

> "Als operator krijg je een melding als het systeem een afwijking vindt. Jij beslist wat je ermee doet."

### Valkuilen
- Langer dan 8 minuten praten. De groep heeft al ervaren en geoefend.
- Niet terugverwijzen naar de oefening.
- Engelse termen gebruiken. Zeg "afwijking", niet "anomaly".

---

## ACTIVITEIT 4: Zelfstandige Oefening (0:30 - 0:45)

### Doel
Duo's werken ZELFSTANDIG aan vijf sensorwaarden. Daarna antwoordmodel en succesfeedback.

### Scaffolding-niveau: JIJ DOET

### Stap voor stap

**0:30** Deel werkblad 4 uit.

> "Nu gaan jullie het ZELF doen. Werk samen met je buurman. Vijf sensorwaarden. Per waarde: normaal of afwijkend? Welk type? Waarom? Jullie hebben 8 minuten."

**0:30-0:38** Loop rond. Bied MINIMALE ondersteuning. Stel alleen vragen terug:
- "Wat is de normale waarde?"
- "Wat is de context?"
- "Wat voor type zou dit zijn?"

Geef GEEN antwoorden.

**0:38** ANTWOORDMODEL — lees voor en bespreek:

> | Nr | Afwijking? | Type | Uitleg |
> |----|-----------|------|--------|
> | 1 | Ja | Puntanomalie | 91 graden vs normaal 65-70. Duidelijke afwijking. |
> | 2 | Nee | Geen | 2,8 bar is normaal bij opstart (2,5-3,2 bar). |
> | 3 | Ja | Collectief | Stijgende trend van 0,1 naar 2,3 mm/s. |
> | 4 | Ja | Contextueel | 15 kWh zonder productie. Waarom verbruikt de machine energie? |
> | 5 | Twijfel/Ja | Grenswaarde | 72 graden, net boven normaal. In de gaten houden. |

**0:42** SUCCESFEEDBACK per duo:

> "Hoeveel hadden jullie goed?"

- 5/5: "Uitstekend, jullie zijn klaar voor de volgende stap."
- 4/5: "Goed gedaan, jullie hebben de basis goed onder de knie."
- 3/5: "Goed begin, let extra op de context."
- 1-2/5: "Niet erg, dit was de eerste keer. We oefenen verder."

**0:43** AFSLUITING en transferopdracht:

> "Jullie hebben vandaag geleerd drie soorten afwijkingen te herkennen. De transferopdracht: kijk deze week naar de sensordata op je werkvloer. Schrijf drie waarden op die je opvallen. Neem dat mee naar de volgende keer."

> "En vraag je leidinggevende: welke sensoren zitten er op jullie machines?"

### Valkuilen
- Het antwoordmodel overslaan. Het antwoordmodel IS het feedbackmoment.
- Negatieve feedback geven. Elke score is een goed begin.
- De afsluiting overslaan. De transferopdracht is essentieel.

---

## Tijdsoverzicht

| Tijd | Activiteit | Scaffolding | Duur |
|------|-----------|-------------|------|
| 0:00-0:01 | Feed-up | n.v.t. | 1 min |
| 0:01-0:10 | Worked example | IK DOE | 9 min |
| 0:10-0:22 | Begeleide groepsoefening | WIJ DOEN | 12 min |
| 0:22-0:30 | Theorie | n.v.t. | 8 min |
| 0:30-0:38 | Zelfstandige oefening | JIJ DOET | 8 min |
| 0:38-0:42 | Antwoordmodel + feedback | n.v.t. | 4 min |
| 0:42-0:45 | Afsluiting + transfer | n.v.t. | 3 min |
| **Totaal** | | | **45 min** |

---

## Noodplan: tijd te kort

Als je bij activiteit 4 minder dan 10 minuten over hebt:
- Verkort de zelfstandige oefening naar 5 minuten (eerste 3 waarden)
- Bespreek het antwoordmodel alleen mondeling (niet waarde voor waarde)
- Sla de succesfeedback per duo NIET over — dat is het belangrijkste moment
- Geef de transferopdracht altijd, ook als het kort is

---

## Didactische verbeteringen t.o.v. vorige versie

Deze versie corrigeert drie tekortkomingen van de vorige versie (score 3/6):

| Probleem | Oplossing | Waar in de sessie |
|----------|-----------|-------------------|
| Geen worked examples | Trainer doet EERST voor met twee sensorwaarden | Activiteit 1 (0:01-0:10) |
| Geen scaffolding | Ik doe - Wij doen - Jij doet opbouw | Activiteiten 1-2-4 |
| Zwakke feedback | Feed-up bij start + antwoordmodel + succesfeedback | 0:00 + activiteit 4 |
