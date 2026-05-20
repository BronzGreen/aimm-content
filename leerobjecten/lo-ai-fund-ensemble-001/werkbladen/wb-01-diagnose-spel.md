# Diagnose-spel: één expert versus drie experts
*Kolb fase 1: ervaren — vijf mystery cases met drie modellen die mogen stemmen*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Ensemble Learning**

---

## Over dit werkblad

Je krijgt vijf "mystery cases" uit de maakindustrie. Per case heeft elk van drie experts (model A, B, C) een diagnose gegeven. Jij vergelijkt: wat zou je doen als je alleen expert A had? En als je alle drie meeneemt en een meerderheid laat stemmen? Tel mee bij hoeveel cases je antwoord verandert.

Geen technische voorkennis nodig. Het is precies hetzelfde principe dat een random forest gebruikt — maar dan in mensen-taal.

**Tijd:** 13 minuten.
**Werkvorm:** trainer doet case 1 voor (IK DOE), daarna werk je cases 2-5 zelfstandig.

---

## Hoe het werkt

> **Eén expert** = je volgt alleen de diagnose van model A.
> **Drie experts (ensemble)** = je laat A, B en C stemmen. De meerderheid wint. Bij twee tegen één wint de twee.

Vink af terwijl je doorgaat.

---

## Case 1 — Lager op een verpakkingslijn

> *Symptoom:* lichte trillingstoename, RPM normaal, temperatuur 2°C boven gemiddeld.

| Expert | Diagnose |
|--------|----------|
| Model A | Lagerschade beginstadium |
| Model B | Lagerschade beginstadium |
| Model C | Normale slijtage, geen actie |

**Mijn oordeel met alleen A:** ○ Actie   ○ Geen actie

**Meerderheidsoordeel A+B+C:** _______________________________________________

**Veranderde mijn antwoord?** ○ Ja   ○ Nee

---

## Case 2 — Spuitgietmachine, korte cyclustijd

> *Symptoom:* de cyclustijd schommelt 3-5%, hydrauliekdruk schommelt mee, productkwaliteit lijkt oké.

| Expert | Diagnose |
|--------|----------|
| Model A | Hydrauliek-pomp beginnende slijtage |
| Model B | Normale variatie, geen probleem |
| Model C | Sensor-ruis, kalibreren aanbevolen |

**Mijn oordeel met alleen A:** ○ Actie   ○ Geen actie

**Meerderheidsoordeel A+B+C:** _______________________________________________

**Veranderde mijn antwoord?** ○ Ja   ○ Nee

---

## Case 3 — CNC-spindel, productie van precisie-onderdelen

> *Symptoom:* afwijkende oppervlakteruwheid op de laatste 12 onderdelen, vibration-piek op 1.8 kHz.

| Expert | Diagnose |
|--------|----------|
| Model A | Spindel-onbalans |
| Model B | Spindel-onbalans |
| Model C | Spindel-onbalans |

**Mijn oordeel met alleen A:** ○ Actie   ○ Geen actie

**Meerderheidsoordeel A+B+C:** _______________________________________________

**Veranderde mijn antwoord?** ○ Ja   ○ Nee

---

## Case 4 — Pomp op een hydraulieksysteem

> *Symptoom:* drukfluctuatie 10-12% boven baseline, motorstroom +8%, geluidsniveau verhoogd.

| Expert | Diagnose |
|--------|----------|
| Model A | Pomp OK, drukinstelling controleren |
| Model B | Cavitatie aan zuigzijde |
| Model C | Cavitatie aan zuigzijde |

**Mijn oordeel met alleen A:** ○ Actie   ○ Geen actie

**Meerderheidsoordeel A+B+C:** _______________________________________________

**Veranderde mijn antwoord?** ○ Ja   ○ Nee

---

## Case 5 — Lasrobot, automotive toeleverancier

> *Symptoom:* incidentele klein lasdefect (1 op 200), stroomwaarden binnen tolerantie, geen patroon zichtbaar.

| Expert | Diagnose |
|--------|----------|
| Model A | Geen voorspellend probleem |
| Model B | Sporadische naadafwijking, monitoren |
| Model C | Geen voorspellend probleem |

**Mijn oordeel met alleen A:** ○ Actie   ○ Geen actie

**Meerderheidsoordeel A+B+C:** _______________________________________________

**Veranderde mijn antwoord?** ○ Ja   ○ Nee

---

## Bonusvoorbeeld — drie modellen op één **storingsclassificatie**

> Een ERP-systeem laat drie modellen automatisch elke nieuwe storing classificeren. Voor één concrete storing (motor warm, geluid afwijkend, productie stilgevallen) zeggen ze:

| Expert | Diagnose-categorie |
|--------|--------------------|
| Model A | Lagerprobleem |
| Model B | Motorprobleem |
| Model C | Lagerprobleem |

*Wat zou jij in dit geval registreren — en welke twijfel houd je?*

_______________________________________________

_______________________________________________

> **Hint:** twee op drie kiezen "lager". Maar één model wijkt af — en bij stem-strategie verlies je informatie. Bagging-ensembles kunnen daarom ook **kansverdelingen** rapporteren ("65% lager, 30% motor, 5% iets anders") in plaats van alleen de winnaar.

---

## Mijn samenvatting

*Vul in.*

| | Aantal cases waarin: |
|---|----------------------|
| Mijn antwoord veranderde door het ensemble | ___ van 5 |
| Het ensemble unaniem was (alle drie hetzelfde) | ___ van 5 |
| Het ensemble verdeeld was (twee tegen één) | ___ van 5 |

---

## Het verrassendste resultaat

*Welke case gaf het grootste verschil tussen "alleen A" en "alle drie"?*

○ Case 1   ○ Case 2   ○ Case 3   ○ Case 4   ○ Case 5   ○ Bonus

*Wat maakte dit verrassend?*

_______________________________________________

_______________________________________________

> **Tip:** in case 4 verandert de meerderheid waarschijnlijk je antwoord — A zat ernaast, B+C zien wel het probleem. Dat is precies waar ensembles glansrol spelen: bij twijfelgevallen waar één model misleid kan worden.

---

## Wat doen we hierna?

Je legt zo je telling naast die van je buurman. Daarna vullen we plenair een wins-tracker in: bij hoeveel cases won het ensemble bij de groep? Dat geeft je een gevoel voor wanneer ensembles wel en niet helpen. Dat gevoel hebben we straks nodig om de theorie van bagging en boosting te begrijpen.

---
*Bron: Ensemble Learning — AIMM Curriculum | Module 2: Train | v1.1*
