# Oefening: c-kaart, UCL en Nelson-regel-1
*Welke kaart, wat is de bovengrens, en is dit een signaal?*

**Naam:** ____________________  **Datum:** __________
**Module 2 — SPC Train | Workshop: c-kaart en escalatie**

---

> **Over dit werkblad**
> Je krijgt één fictieve PCB-assemblagecasus en werkt hem in vier korte stappen door. Je gokt niet — de formule staat op dit werkblad. Het gaat om **kiezen** (welke kaart?), **rekenen** (waar ligt de bovengrens?), **zien** (is dit een signaal?), en **beslissen** (wat is je eerste stap?).

---

## De casus (fictief — PCB-assemblage)

Je werkt op een assemblagelijn voor printplaten. Elk uur inspecteer je **50 geassembleerde boards** visueel op **soldeerfouten**. Eén board kan meerdere soldeerfouten hebben.

Over de laatste weken is het gemiddelde: **c̄ = 2,4 fouten per 50 boards.**

Vandaag, na een **materiaalwissel** (nieuwe leverancier-batch), zie je:

| Uur | Aantal soldeerfouten |
|-----|----------------------|
| t=0 | **8** |
| t=1 | **6** |
| t=2 | **9** |

---

## 🔵 Stap 1 — Welke kaart kies je?

*Je telt **fouten** (niet defecte boards — één board kan er meerdere hebben) per **vaste eenheid** (steeds 50 boards).*

**Omcirkel je keuze:**   ⚪ c-kaart   ⚪ p-kaart   ⚪ np-kaart   ⚪ u-kaart

*Waarom deze kaart? (1 zin):*

_______________________________________________

_______________________________________________

---

## 🟣 Stap 2 — Bereken de UCL

**Formule voor de c-kaart:**
UCL = c̄ + 3 × √c̄
LCL = c̄ − 3 × √c̄ *(als LCL < 0, afkappen op 0)*

**Gegeven:** c̄ = 2,4

**Werk uit:**

√2,4 ≈ _______  (gebruik rekenmachine)

3 × √2,4 ≈ _______

**UCL** = 2,4 + _______ ≈ _______

**LCL** = 2,4 − _______ = _______  → afkappen op _______

---

## 🟢 Stap 3 — Welk uur is een signaal?

*Vergelijk elk uur met je UCL. Omcirkel waar het mis gaat.*

| Uur | Fouten | Boven UCL? | Signaal? |
|-----|:------:|:----------:|:--------:|
| t=0 | 8 | ⚪ ja / ⚪ nee | ⚪ ja / ⚪ nee |
| t=1 | 6 | ⚪ ja / ⚪ nee | ⚪ ja / ⚪ nee |
| t=2 | 9 | ⚪ ja / ⚪ nee | ⚪ ja / ⚪ nee |

**Hoe heet de regel die zegt: 'één punt buiten UCL = signaal'?**

_______________________________________________

---

## 🟠 Stap 4 — Wat doe je als eerste?

*Het is t=0, je ziet 8 fouten op 50 boards. Welke stap zet jij als eerste — vóór je afwacht wat t=1 brengt?*

*Zet een cijfer (1 = nu, 2 = daarna, 3 = later, X = niet mijn stap) voor elke actie:*

___ Boards van dit uur apart zetten

___ Teamleider informeren

___ Leverancier bellen

___ Materiaalbatch in quarantaine

___ Wachten tot t=1 — misschien is het toeval

___ Engineering / kwaliteitsdienst inschakelen

*Welke stap zet jij écht zelf als eerste? (1 zin):*

_______________________________________________

_______________________________________________

---

## 🔴 Korte check

*Vul in voordat we plenair bespreken:*

| Vraag | Jouw antwoord |
|-------|---------------|
| Kaarttype | |
| UCL (afgerond op 1 decimaal) | |
| Welke uren zijn een signaal? | |
| Mijn eerste zelfgekozen stap | |

---

> **Volgende stap:** Vergelijk met je buurman (3 min). Daarna bespreken we plenair de kaartkeuze, de UCL, en jullie eerste stappen. Daarna pakken we de handout erbij.

---
*Bron: ko-spc-502 (c-kaart casus, fictieve PCB-assemblage); AIAG SPC Reference Manual | AIMM Module 2 — SPC Train | v1.0*
