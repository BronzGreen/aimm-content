# Mijn Eigen Analyse: Is dit Cpk-Getal Betrouwbaar?
*Capability-valkuilen — toetsen aan de drie voorwaarden*

**Naam:** ____________________  **Datum:** __________
**Lijn / proces:** ____________________  **Getal uit:** (☐ kwaliteitsrapport ☐ MES-export ☐ klantaudit ☐ teamdashboard ☐ anders: ______)

---

> **Over dit werkblad** *(blok 2 — experimenteren, A3 of A4 dubbelzijdig)*
> Neem één concreet, gerapporteerd capability-getal uit jouw werkpraktijk. Geen hypothetisch geval — een echt getal dat nu ergens rondgaat en mogelijk een beslissing stuurt. Je legt het langs de drie voorwaarden uit het kennisobject. Waar je iets niet weet: "onbekend" mag — dat is de hele les. Onbekend = eerst uitzoeken vóór het getal een beslissing stuurt.

---

## 0. Het getal

**Welk getal ga je toetsen?**

| Indicator | Gerapporteerde waarde | Wie rapporteerde het? | Wanneer? |
|-----------|----------------------|----------------------|----------|
| Cp / Cpk / Pp / Ppk (omcirkel) | | | |

**Welke beslissing hangt af van dit getal?** *(investering, klantvrijgave, PPAP-indiening, escalatie, dashboard-groen/rood?)*

_______________________________________________

_______________________________________________

---

## 🔵 Voorwaarde 1 — Is het meetsysteem geschikt?

*Ford PPAP eist Gage R&R / MSA (AIAG-methode) vóór capability. Een ruisige meter blaast procesvariatie op — dan zegt Cpk evenveel over de meter als over de machine.*

**Is er een geldig Gage R&R / MSA-rapport voor dit meetsysteem?**

- ☐ Ja — rapport aanwezig, %GRR-waarde bekend: _______ %
- ☐ Ja — rapport aanwezig, maar %GRR niet opgezocht
- ☐ Nee — geen rapport bekend
- ☐ Onbekend — moet opgevraagd worden bij: _______________

**Bron / bewijs** *(waar staat het rapport, wie heeft het gedaan, wanneer?)*

_______________________________________________

**AIAG-vuistregel (MSA 4e):** %GRR < 10% = goed · 10–30% = marginaal · > 30% = niet geschikt voor capability.

**Jouw oordeel voor voorwaarde 1:**

- ☐ Meetsysteem bewezen geschikt — kan door
- ☐ Meetsysteem twijfelachtig — Gage R&R inplannen vóór getal-acceptatie
- ☐ Onbekend — eerst bron ophalen

---

## 🟠 Voorwaarde 2 — Was het proces stabiel?

*NIST/SEMATECH: capability-formules zijn alleen geldig op een statistisch stabiel proces. Op een instabiel proces is σ een mix van gewone variatie + verstoringen — het getal verandert dag tot dag.*

**Is er een SPC-regelkaart over dezelfde periode als de capability-studie?**

- ☐ Ja — regelkaart gezien, geen out-of-control signalen
- ☐ Ja — regelkaart gezien, wél signalen (dan is capability niet valide)
- ☐ Ja — regelkaart bestaat, maar niet geraadpleegd vóór de capability-berekening
- ☐ Nee — geen regelkaart over deze periode
- ☐ Onbekend

**Bron / bewijs** *(welke kaart, welk archief, welke periode?)*

_______________________________________________

**Over welke periode is het getal berekend?** *(uren, dagen, weken, shifts?)*

_______________________________________________

**Jouw oordeel voor voorwaarde 2:**

- ☐ Stabiliteit aangetoond — kan door
- ☐ Stabiliteit onbekend — regelkaart opvragen
- ☐ Proces was aantoonbaar instabiel — getal niet bruikbaar

---

## 🟣 Voorwaarde 3 — Waren de subgroepen rationeel?

*Binnen-subgroep σ moet alléén ruis bevatten. Subgroepen die shifts, recepten of caviteiten mengen, vermengen korte- en langetermijnvariatie — Cpk wordt te conservatief of te optimistisch (zie ko-spc-109).*

**Hoe waren de subgroepen samengesteld?**

| Kenmerk | Beschrijving |
|---------|-------------|
| Subgroep-grootte (n) | |
| Frequentie (elk uur / elke shift / …) | |
| Één machine / lijn / caviteit? | |
| Binnen één shift, recept, operator? | |

**Waren de subgroepen rationeel (zelfde omstandigheden, dicht in tijd, één bron)?**

- ☐ Ja — rationele subgroepen, expliciet gedefinieerd
- ☐ Twijfelachtig — meerdere caviteiten / shifts / recepten in één subgroep
- ☐ Nee — duidelijk vermengd (bv. 5 metingen per uur over 4 caviteiten)
- ☐ Onbekend — subgroep-definitie niet gedocumenteerd

**Bron / bewijs** *(documentatie subgroep-strategie, SPC-plan, procedure?)*

_______________________________________________

**Jouw oordeel voor voorwaarde 3:**

- ☐ Subgroepering rationeel — kan door
- ☐ Subgroepering twijfelachtig — definitie opvragen
- ☐ Vermenging bevestigd — getal is vertekend (onder- of overschat)

---

## 🔴 Samenvatting: kan dit getal een beslissing dragen?

| Voorwaarde | Ja / Nee / Onbekend | Bron |
|-----------|--------------------|------|
| 1. Meetsysteem geschikt (Gage R&R / MSA) | | |
| 2. Proces stabiel (SPC-regelkaart) | | |
| 3. Subgroepering rationeel | | |

**Drie keer "ja met bron"** = getal is bruikbaar voor de beslissing.
**Eén of meer keer "onbekend"** = eerst uitzoeken vóór de beslissing.
**Eén of meer keer "nee"** = getal is niet bruikbaar — herrekenen na correctie.

---

## 🟢 Mijn drie vragen aan de rapporteur

*Formuleer concrete vragen — per voorwaarde één. Noem de naam van wie je het gaat vragen.*

**Vraag over meetsysteem** — aan: ____________________

> _______________________________________________

**Vraag over stabiliteit** — aan: ____________________

> _______________________________________________

**Vraag over subgroepering** — aan: ____________________

> _______________________________________________

---

## 🟣 Mijn maandag-actie

*Eén concrete, vandaag al uitvoerbare eerste stap. Niet de mooiste — de kleinste die echt beweging brengt.*

> _______________________________________________
>
> _______________________________________________

**Wie ga je benaderen?** ____________________ · **Wanneer?** ____________________

---

> 💡 **Onthoud:** Capability is niet één formule maar drie voorwaarden. Een operator die alleen "Cpk = 1,2" leest, weet niet of dat getal betrouwbaar is. Een operator die de drie voorwaarden toetst, kan de juiste vragen stellen — en voorkomt dat investeringen naar de verkeerde plek gaan.

---
*Bron: ko-spc-303; NIST/SEMATECH e-Handbook; AIAG MSA Reference Manual (4e); Ford PPAP 4th edition | AIMM Module 3 — SPC Op Maat | v1.0*
