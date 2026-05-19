# Casuskaarten: 8 AI-meldingen

*Knip deze kaarten uit of gebruik ze als losse pagina's. Elke melding is een aparte casus.*

*Scaffolding: Melding 1-2 doet de trainer voor. Melding 3-4 bespreekt de groep. Melding 5-8 doe jij zelf.*

---

## Melding 1 - WORKED EXAMPLE (trainer doet voor)

**Machine:** Spuitgietmachine SG-04
**Melding:** Temperatuurpiek van 85 graden C na het opstarten
**Tijdstip:** 06:12 (productiestart was 06:05)
**Normaalwaarde:** 45-60 graden C tijdens productie
**Drempel:** 75 graden C

**Beoordeling trainer (think-aloud):**

> "Ik kijk eerst naar de **context**: wanneer kwam deze melding? Direct na het opstarten - 7 minuten geleden."
>
> "Ik weet uit ervaring: na het opstarten is een temperatuurpiek **normaal**. De machine warmt op."
>
> "Mijn conclusie: dit is **VALS ALARM**."
>
> "Ik klik 'vals alarm' en typ erbij: *normaal opstartgedrag*."

**Antwoordmodel:** VALS ALARM. Het AI-systeem kent het verschil nog niet tussen opstart en productie. Een temperatuurpiek bij opstart is normaal. De machine warmt op. Door jouw feedback leert het systeem dit. Volgende keer slaat het hier geen alarm meer voor.

---

## Melding 2 - WORKED EXAMPLE (trainer doet voor)

**Machine:** CNC-freesmachine FR-12
**Melding:** Trillingsniveau is 3x de normaalwaarde en neemt continu toe
**Huidige waarde:** 4,2 mm/s
**Normaalwaarde:** 1,4 mm/s
**Drempel:** 3,5 mm/s
**Verloop:** 3 uur geleden: 2,8 mm/s, 2 uur geleden: 3,1 mm/s, 1 uur geleden: 3,6 mm/s, nu: 4,2 mm/s

**Beoordeling trainer (think-aloud):**

> "Ik kijk naar het **verloop**: de trillingen zijn 3x de normaalwaarde en nemen continu toe. Dat is geen piek maar een trend."
>
> "Ik check de **waarde**: 4,2 is boven de drempel van 3,5. En het stijgt nog."
>
> "Ik weet: geleidelijk toenemende trillingen wijzen op **slijtage** van een lager of aandrijving."
>
> "Mijn conclusie: dit is **TERECHT ALARM**. Ik plan een controle in."

**Antwoordmodel:** TERECHT ALARM. Trillingen 3x normaal en continu toenemend: dat wijst op lagerslijtage (slijtage van het lager in de aandrijving). De trend over 3 uur laat zien dat het erger wordt. Goed dat het systeem dit oppikt.

---

## Melding 3 - GROEPSOEFENING (groep bespreekt samen)

**Machine:** Verpakkingslijn VP-02
**Melding:** Energieverbruik 15% hoger dan normaal
**Tijdstip:** 14:30 (halverwege de middagshift)
**Context:** Vandaag draait de lijn een ander producttype (grotere verpakkingen)
**Normaalwaarde:** 12 kWh per uur (bij standaard product)
**Huidige waarde:** 13,8 kWh per uur

Beoordeel samen: terecht of vals alarm?

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel (pas na bespreking lezen):**
> **VALS ALARM.** Bij grotere verpakkingen is een hoger energieverbruik normaal. De machine verwerkt meer materiaal. De waarde is afwijkend, maar verklaarbaar door de productwissel. Feedback aan het systeem: "vals alarm, hoger verbruik past bij groter producttype."

---

## Melding 4 - GROEPSOEFENING (groep bespreekt samen)

**Machine:** Persmachine PM-07
**Melding:** Druk daalt onverwacht van 180 bar naar 165 bar
**Tijdstip:** 10:45 (midden in productie)
**Context:** Geen productwissel, geen onderhoud, geen verandering in grondstof
**Normaalwaarde:** 175-185 bar
**Drempel:** 170 bar

Beoordeel samen: terecht of vals alarm?

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel (pas na bespreking lezen):**
> **TERECHT ALARM.** Onverwachte drukdaling zonder verklaarbare oorzaak is verdacht. De waarde zit onder de drempel. Mogelijke oorzaken: lekkage, versleten afdichting of defecte pomp. Direct controleren.

---

## Melding 5 - ZELFSTANDIG (gebruik het beoordelingsprotocol)

**Machine:** Lasersnijder LS-03
**Melding:** Focuspositie wijkt 0,3 mm af van de ingestelde waarde
**Tijdstip:** 08:20 (1 uur na productiestart)
**Context:** Nieuwe lenshouder geplaatst bij onderhoud gisteren
**Normaalwaarde:** afwijking maximaal 0,1 mm
**Drempel:** 0,2 mm

| Stap | Jouw beoordeling |
|------|-----------------|
| 1. Context | |
| 2. Waarde | |
| 3. Patroon | |
| 4. Actie | |

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel:**
> **TERECHT ALARM.** De afwijking is 3x de normaalwaarde en 1,5x de drempel. De nieuwe lenshouder van gisteren is de meest waarschijnlijke oorzaak. Mogelijk niet goed gekalibreerd na het onderhoud. Actie: kalibratie controleren. Tip: na onderhoud altijd extra alert zijn op afwijkingen.

---

## Melding 6 - ZELFSTANDIG (gebruik het beoordelingsprotocol)

**Machine:** Spuitgietmachine SG-04 (dezelfde als melding 1!)
**Melding:** Temperatuur 82 graden C
**Tijdstip:** 14:15 (machine draait al 8 uur)
**Context:** Geen productwissel, buitentemperatuur is 34 graden C (hittegolf)
**Normaalwaarde:** 45-60 graden C
**Drempel:** 75 graden C

| Stap | Jouw beoordeling |
|------|-----------------|
| 1. Context | |
| 2. Waarde | |
| 3. Patroon | |
| 4. Actie | |

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel:**
> **TERECHT ALARM.** Let op: dit is NIET hetzelfde als melding 1! De machine draait al 8 uur. De opstartfase is allang voorbij. 82 graden is ver boven normaal (45-60). Actie: koeling controleren, productie eventueel pauzeren. Dit is de valkuil: het lijkt op melding 1, maar de **context** is totaal anders.

---

## Melding 7 - ZELFSTANDIG (gebruik het beoordelingsprotocol)

**Machine:** Robot-lascel RL-01
**Melding:** Positieafwijking arm 3 van 0,8 mm
**Tijdstip:** 11:30
**Context:** Machine draait normaal, geen bijzonderheden
**Normaalwaarde:** afwijking maximaal 0,2 mm
**Drempel:** 0,5 mm
**Extra info:** Vorige week was er een vergelijkbare melding (0,6 mm) die vanzelf verdween

| Stap | Jouw beoordeling |
|------|-----------------|
| 1. Context | |
| 2. Waarde | |
| 3. Patroon | |
| 4. Actie | |

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel:**
> **TERECHT ALARM.** De afwijking is 4x de normaalwaarde en 1,6x de drempel. Vorige week was het 0,6 mm, nu 0,8 mm. Dit is een **trend**: het wordt erger. De vorige melding die "vanzelf verdween" was een vroeg signaal. Toenemende positieafwijking wijst op slijtage van de aandrijving. Actie: direct controleren. Onthoud: een melding die "vanzelf verdwijnt" is niet altijd goed nieuws.

---

## Melding 8 - ZELFSTANDIG (gebruik het beoordelingsprotocol)

**Machine:** Verpakkingslijn VP-02 (dezelfde als melding 3)
**Melding:** Snelheid verpakkingslijn 8% lager dan normaal
**Tijdstip:** 09:00 (net na de ochtendpauze)
**Context:** Operator heeft de lijn net herstart na de pauze
**Normaalwaarde:** 120 verpakkingen per minuut
**Huidige waarde:** 110 verpakkingen per minuut
**Drempel:** 108 verpakkingen per minuut

| Stap | Jouw beoordeling |
|------|-----------------|
| 1. Context | |
| 2. Waarde | |
| 3. Patroon | |
| 4. Actie | |

Je beoordeling: _______________________________________________

Je reden: ____________________________________________________

> **Antwoordmodel:**
> **VALS ALARM.** De lijn is net herstart na de pauze. Net als bij opstarten (melding 1) heeft de machine even nodig om op snelheid te komen. De waarde zit net boven de drempel en zal waarschijnlijk stijgen. Actie: 10 minuten wachten en opnieuw controleren. Als het dan nog laag is, is het wel een probleem.

---

## Antwoordoverzicht

| Melding | Fase | Correct antwoord | Kernreden |
|---------|------|------------------|-----------|
| 1 | IK DOE (worked example) | Vals alarm | Temperatuurpiek 85 graden C bij opstart is normaal |
| 2 | IK DOE (worked example) | Terecht alarm | Trillingen 3x normaal, continu toenemend = lagerslijtage |
| 3 | WIJ DOEN (groep) | Vals alarm | Hoger energieverbruik door ander producttype |
| 4 | WIJ DOEN (groep) | Terecht alarm | Onverwachte drukdaling zonder verklaring |
| 5 | JIJ DOET (zelfstandig) | Terecht alarm | Focusafwijking na onderhoud = kalibratieprobleem |
| 6 | JIJ DOET (zelfstandig) | Terecht alarm | Temperatuur na 8 uur is NIET hetzelfde als bij opstart |
| 7 | JIJ DOET (zelfstandig) | Terecht alarm | Toenemende positieafwijking = trend (erger dan vorige week) |
| 8 | JIJ DOET (zelfstandig) | Vals alarm | Lagere snelheid na herstart is tijdelijk |

**Verdeling:** 3x vals alarm, 5x terecht alarm
**Valkuilen:** Melding 6 lijkt op melding 1 maar is anders (context!). Melding 7 lijkt onschuldig omdat het vorige keer "vanzelf" verdween.
