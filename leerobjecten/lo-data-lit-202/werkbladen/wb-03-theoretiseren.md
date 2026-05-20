# Handout: Drie checks voor datakwaliteit
*Datakwaliteit beoordelen -- AIMM Data Literacy*

**Naam:** ____________________  **Datum:** __________
**Module 2 -- Train: Data Literacy**

---

> **Kernidee:** Goede data zijn de basis voor goede besluiten. Met drie simpele checks weet je of je data betrouwbaar zijn. Je kunt dit zelf doen, zonder hulp van IT.

---

## De drie checks

| # | Check | Wat doe je? | Vuistregel |
|---|-------|-------------|------------|
| 1 | **Volledigheid** | Tel lege cellen per kolom | Meer dan 10% leeg? Wees voorzichtig |
| 2 | **Consistentie** | Bekijk eenheden en waarden | Zelfde eenheid? Logische waarden? |
| 3 | **Actualiteit** | Bekijk de datums | Wanneer verzameld? Nog geldig? |

---

## Check 1: Volledigheid

*Zijn alle velden ingevuld?*

- Tel het aantal lege cellen per kolom.
- Deel door het totaal aantal rijen.
- Meer dan 10% leeg = **voorzichtig**.
- Vraag jezelf af: waarom ontbreken deze data?

**Voorbeeld:** Een kolom "temperatuur" heeft 15 van 100 rijen leeg. Dat is 15%. Je kunt deze kolom niet zomaar gebruiken.

---

## Check 2: Consistentie

*Kloppen de waarden met elkaar?*

- Staan overal dezelfde eenheden? (mm of cm, niet door elkaar)
- Zijn de waarden logisch? (Een temperatuur van 500 graden in een kantoor klopt niet)
- Staan er dubbele rijen in?

**Voorbeeld:** In een kolom "gewicht" staan waarden in gram en in kilogram door elkaar. Dat geeft foute berekeningen.

---

## Check 3: Actualiteit

*Zijn de data nog vers genoeg?*

- Wanneer zijn de data verzameld?
- Is er sindsdien iets veranderd? (nieuwe machine, ander materiaal)
- Oude data kunnen leiden tot verkeerde besluiten.

**Voorbeeld:** Je gebruikt data van vorig jaar. Maar de machine is twee maanden geleden vervangen. Die oude data gelden niet meer.

---

## Samenvatting: het stoplichtsysteem

| Kleur | Betekenis | Wat doe je? |
|-------|-----------|-------------|
| **Groen** | Alle drie de checks zijn goed | Ga door, data zijn betrouwbaar |
| **Oranje** | Een of twee checks geven twijfel | Onderzoek het probleem eerst |
| **Rood** | Een of meer checks zijn slecht | Stop. Los het probleem op |

---

## Onthoud dit

> Slechte data + goed model = slecht resultaat.
> Goede data + simpel model = goed resultaat.
> **De data zijn belangrijker dan het model.**

---
*Bron: Datakwaliteit beoordelen -- AIMM Data Literacy | Module 2: Train | v1.0*
