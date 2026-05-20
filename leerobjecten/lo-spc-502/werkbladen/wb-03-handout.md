# Handout: c-kaart, Nelson-regel-1 en de escalatieketen
*Attribuutkaart kiezen, UCL berekenen, op tijd aan de bel trekken*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**
> **"Tel je defecten per gelijke eenheid, dan is het een c-kaart. Eén punt boven UCL = Nelson-regel-1: nu escaleren, niet afwachten."**

---

## 🔵 Welke kaart — c, p, np of u?

*Attribuutkaarten horen bij ja/nee-meten (defect ja/nee) of tellen (hoeveel defecten). De keuze hangt af van twee vragen.*

**Vraag 1:** Tel je **defecten** (een item kan er meerdere hebben) of **defecte stuks** (elk stuk telt 1×)?
**Vraag 2:** Is je **eenheid** (of steekproef) elke keer even groot, of varieert hij?

| Je telt... | Eenheid is... | Kaart | Voorbeeld |
|------------|---------------|:-----:|-----------|
| **Defecten** | **constant** (bijv. altijd 50 boards) | **c** | Soldeerfouten per 50 PCB's |
| **Defecten** | variabel (soms 30, soms 80) | u | Fouten per meter stof (wisselende rollen) |
| **Defecte stuks** | constant | np | Defecte lampen per 100 getest |
| **Fractie defect** (%) | variabel | p | % defecte pallets per levering |

**In onze casus:** je telt fouten (een board kan er meerdere hebben) per vaste eenheid (50 boards). → **c-kaart.**

---

## 🟣 De c-kaart: formules

> De c-kaart gaat uit van een **Poisson-verdeling** (tellingen met een klein verwachte waarde per eenheid). De 3-sigma-regel gebruikt √c̄ als ruwe standaardafwijking.

| Grootheid | Formule | Opmerking |
|-----------|---------|-----------|
| **Centerlijn** | c̄ (historisch gemiddeld aantal fouten per eenheid) | Bijv. 2,4 fouten per 50 boards |
| **UCL** | c̄ + 3 × √c̄ | Bovengrens |
| **LCL** | c̄ − 3 × √c̄ | Als < 0, **afkappen op 0** |

**Uitgewerkt voor c̄ = 2,4:**

- √2,4 ≈ 1,549
- 3 × 1,549 ≈ 4,65
- **UCL** = 2,4 + 4,65 ≈ **7,1**
- **LCL** = 2,4 − 4,65 = −2,25 → **LCL = 0**

Een punt ≥ 8 fouten ligt dus buiten UCL.

---

## 🟢 De casus uit de oefening — stap voor stap

*Assemblagelijn PCB. 50 boards per uur geïnspecteerd op soldeerfouten. c̄ = 2,4. Na materiaalwissel:*

| Uur | Fouten | Boven UCL (7,1)? | Betekenis |
|-----|:------:|:----------------:|-----------|
| t=0 | 8 | **Ja** | **Nelson-regel-1 — eerste signaal. Escaleren nu.** |
| t=1 | 6 | Nee | Hoog, maar binnen UCL — op zichzelf geen signaal |
| t=2 | 9 | **Ja** | **Bevestiging — patroon is echt** |

> **De operatorles:** niet wachten op bevestiging. Bij t=0 is de materiaalbatch verdacht; bij t=2 is het zeker.

---

## 🟠 Nelson-regel-1 — het krachtigste signaal

**Nelson-regel-1:** één punt buiten de ±3σ-grenzen (bij c-kaart: boven UCL of onder LCL).

> Bij een stabiel Poisson-proces is de kans op Nelson-regel-1 door toeval ongeveer **0,3%**. Als je het toch ziet, is de kans dat er écht iets bijzonders gebeurt véél groter dan de kans op pech.

Dit is de reden dat één punt al genoeg is om in actie te komen — je hoeft niet te wachten op een tweede bevestiging.

---

## 🔴 De escalatieketen — in volgorde

*Wat gebeurt er tussen 'signaal gezien' en 'leverancier gebeld'?*

| # | Stap | Door wie? | Wanneer? |
|---|------|-----------|----------|
| 1 | Operator informeert **teamleider** | Operator | Direct na eerste signaal (t=0) |
| 2 | Boards van verdachte uren **apart zetten** | Operator + ploeg | Binnen 15 min na melding |
| 3 | Escalatie naar **kwaliteit en engineering** | Teamleider | Binnen 30 min na melding |
| 4 | Materiaalbatch in **quarantaine** | Engineering / magazijn | Binnen 1 uur |
| 5 | **Leverancier** informeren — terugroepen batch | Inkoop / kwaliteit | Binnen 2 uur |
| 6 | Productie hervatten met monsters **vorige batch** | Operator + teamleider | Zodra batch bevestigd OK |

**Tijdswinst:** escalatie binnen 2 uur beperkt de impact tot **~150 boards** (3 uur × 50). Zonder escalatie raakt het probleem al snel een hele shift — duizenden stuks.

---

## 🟡 Voorwaarde: materiaal-traceerbaarheid

De hele keten werkt alleen als duidelijk is **welke batch wanneer op welke lijn is gebruikt**. Zonder die registratie:

- **Nelson-regel-1 zie je nog steeds** — maar je weet niet welke batch je moet terugroepen
- Boards apart zetten werkt — maar je mist de batches die al weg zijn
- De leverancier kan niet gericht onderzoeken

**Praktische check voor jouw lijn:**
- Wordt de leverancierscode of batch-ID gekoppeld aan de uur-inspectie?
- Kan je achteraf zien welke boards welk materiaal hebben gehad?
- Staat dit in het MES-systeem, op papier, of nergens?

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **c-kaart** | Regelkaart voor aantal defecten per gelijke eenheid |
| **c̄** | Historisch gemiddeld aantal defecten per eenheid (centerlijn) |
| **UCL** | Upper Control Limit — bovengrens van de regelkaart |
| **LCL** | Lower Control Limit — ondergrens (kan 0 zijn bij c-kaart) |
| **Nelson-regel-1** | Eén punt buiten ±3σ = signaal van special cause |
| **Special cause** | Variatie uit een aanwijsbare oorzaak (bijv. andere batch) |
| **Common cause** | Normale dagelijkse variatie van een stabiel proces |
| **Quarantaine** | Materiaal apart zetten tot onderzocht is of het mag |
| **Traceerbaarheid** | Koppeling tussen materiaal-batch en eindproduct |

---

## 🟢 Onthoud dit

1. **Defecten per vaste eenheid** = c-kaart (niet p, niet np).
2. **UCL = c̄ + 3√c̄**, LCL afkappen op 0 als negatief.
3. **Eén punt boven UCL = Nelson-regel-1** = nu handelen, niet afwachten.
4. **Eerste stap is altijd: teamleider informeren en boards apart zetten.**
5. **Leverancier-terugroep** werkt alleen met goede materiaal-traceerbaarheid.
6. **Binnen 2 uur escaleren** beperkt schade van 1 shift naar enkele honderden stuks.

---
*Bron: ko-spc-502 (c-kaart casus); AIAG SPC Reference Manual; NIST/SEMATECH Engineering Statistics Handbook; Nelson (1984) "The Shewhart Control Chart — Tests for Special Causes" | AIMM Module 2 — SPC Train | v1.0*
