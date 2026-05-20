# Handout: I-MR configureren en Nelson-regel 3 herkennen
*I-MR — Individual + Moving Range — en de trend-regel*

**Module 2 — SPC Train | Naslagwerk + actieplan eigen lijn**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Een stijgende of dalende reeks binnen de control limits is al een signaal. 6 opeenvolgende punten dezelfde kant op = Nelson-regel 3 = trend."**

Wachten op een punt buiten UCL is vaak te laat: dan liggen er al uitvallers. Regel 3 pakt de drift vóór de spec-overschrijding.

---

## Wanneer kies je een I-MR-kaart?

| Situatie | Chart | Waarom |
|----------|-------|--------|
| Je meet **meerdere stuks tegelijk** uit één toestand van de machine (bijv. 5 stuks uit dezelfde caviteit) | **X̄-R** | Natuurlijke subgroep; gemiddelde + spreiding is betrouwbaarder |
| Je meet **één stuk per meetmoment** of stukken met tijd ertussen | **I-MR** | Geen natuurlijke subgroep; elke meting is uniek |
| **Destructieve meting** (je hebt maar één resultaat per toets) | **I-MR** | Geen subgroep mogelijk |
| **Dure of tijdrovende meting** | **I-MR** | Vaak één per uur of per shift |

**Voorbeeld (uit ko-spc-501):** CNC-frees, seriële boorgat-bestelling, elk uur 3 stuks meten met digitale schuifmaat. Elke meting is uniek (geen natuurlijke subgroep uit één machinetoestand) → **I-MR**.

---

## Hoe werkt een I-MR-kaart?

Een I-MR-kaart heeft **twee chart-lijnen** onder elkaar:

| Lijn | Wat plot je? | Wat bewaak je? |
|------|--------------|----------------|
| **I-chart** (Individual) | Elke individuele meting | Het proces-niveau (waar zit het gemiddelde?) |
| **MR-chart** (Moving Range) | Het absolute verschil tussen opeenvolgende metingen | De korte-termijn-variatie (hoe rustig is de lijn?) |

**Control limits worden berekend uit de eerste ~20 stabiele metingen:**

- **I-chart:** UCL = X̄ + 2,66 · MR̄ ; LCL = X̄ − 2,66 · MR̄
- **MR-chart:** UCL = 3,267 · MR̄ ; LCL = 0

> Je hoeft deze formules niet uit je hoofd. Het MES-systeem of engineering berekent ze voor je. Maar je moet weten: de grenzen zijn **niet de klanttolerantie** — het zijn statistische grenzen op basis van het proces zelf.

---

## De zeven Nelson-regels kort

| Regel | Signaal |
|-------|---------|
| **1** | 1 punt buiten UCL of LCL |
| **2** | 9 opeenvolgende punten aan dezelfde kant van de middellijn |
| **3** | **6 opeenvolgende punten allemaal stijgend of allemaal dalend** — **trend** |
| **4** | 14 opeenvolgende punten afwisselend op en neer |
| **5** | 2 van de 3 opeenvolgende punten in zone A (> 2σ van middellijn) |
| **6** | 4 van de 5 opeenvolgende punten in zone B (> 1σ van middellijn) |
| **7** | 15 opeenvolgende punten in zone C (binnen 1σ — "te rustig") |

**Voor deze sessie focussen we op regel 1 en regel 3.**

---

## 🔵 Regel 3 uitgelicht: de trend

**6 of meer opeenvolgende punten** gaan allemaal dezelfde kant op — stijgend of dalend.

**Waarom 6?**  
Statistisch is de kans dat 6 punten toevallig op rij stijgen ongeveer 1 op 64 (≈ 1,5%). Bij die kans spreek je niet meer van toeval — dan is er een systematische oorzaak.

**Waarom is dit vroeger dan regel 1?**  
Regel 1 merkt de uitslag pas op als een punt de control limit overschrijdt. Regel 3 pakt de beweging erheen: **je ziet de drift aankomen**.

**Illustratie uit ko-spc-501:** bij 0,0004 mm slijtage per uur stijgt een diameter over 40 uur met 0,016 mm. Start 9,990 mm → eind 10,006 mm. Nog binnen spec (≤ 10,02 mm) — maar de trend stond al uren op de kaart.

---

## 🟣 Typische trend-veroorzakers

| Veroorzaker | Waar zie je het? |
|-------------|------------------|
| **Gereedschapsslijtage** | CNC-frees, draaibank, boor, stansgereedschap |
| **Temperatuur-drift** | Spuitgieten (opwarming cavitieit), meetbank ('s ochtends koud) |
| **Materiaaluitputting** | Bad-concentratie galvaniseerlijn, koelvloeistof, smeermiddel |
| **Zettings-drift** | Mechanische afstelling die langzaam verschuift door trillingen |

---

## 🟠 Wat doe je bij een trend? — de 5 operator-stappen

*Uit ko-spc-501, CNC-frees casus:*

| # | Stap | Toelichting |
|---|------|-------------|
| 1 | **Stop de machine** | Of signaleer en laat een bevoegde collega stoppen |
| 2 | **Meet het gereedschap** | In de casus: 0,015 mm slijtage bevestigd |
| 3 | **Vervang de tooling** | Of laat vervangen — pas ná meten |
| 4 | **Documenteer** | Signaal + oorzaak + actie + effect |
| 5 | **Hervat productie** | Met monitoring of de kaart weer rustig wordt |

> **Niet:** direct vervangen zonder meten. Dan weet je morgen niet of de trend door slijtage kwam of door iets anders.

---

## 🔴 Drie valkuilen — pas op!

| # | Valkuil | Wat is er aan de hand? |
|---|---------|------------------------|
| 1 | **Alleen op regel 1 letten** | Je pakt de signalen pas als de uitval er al is. → **Ook regel 3 actief bewaken.** |
| 2 | **I-MR gebruiken terwijl X̄-R kan** | Als je echte subgroepen hebt, is X̄-R gevoeliger. → **Eerst kijken: is er een natuurlijke subgroep?** |
| 3 | **Control limits verwarren met klantspec** | UCL/LCL zijn statistisch, USL/LSL komen van de klant. → **Twee aparte dingen.** |

---

## 🟢 Onthoud dit

1. **I-MR bij unieke metingen** (geen natuurlijke subgroep).
2. **Een trend binnen UCL is al een signaal** — regel 3 is vroeger dan regel 1.
3. **6 opeenvolgende punten dezelfde kant op** = trend.
4. **Eerste actie bij trend: meten/checken**, niet direct vervangen.
5. **Documentatie** is het enige dat organisatie-leren oplevert.
6. **Control limits ≠ klantspec.**

---

## 📋 Actieplan: mijn eigen lijn

*Vul dit onderaan in tijdens de workshop (fase 4 — experimenteren).*

**Machine / lijn:** _______________________________________________

**Kritische maat:** _______________________________________________

**Tolerantie:** USL = __________   LSL = __________

**Huidige meetfrequentie:** _______________________________________________

**Meet ik 1 stuk per keer, of meerdere tegelijk uit dezelfde machinetoestand?**

_______________________________________________

**Op basis daarvan kies ik:**  ⚪ I-MR   ⚪ X̄-R   **omdat:**

_______________________________________________

_______________________________________________

**Mogelijke trend-veroorzaker op deze lijn** (slijtage / temperatuur / materiaaluitputting / anders):

_______________________________________________

**Transferopdracht deze week:**  
Kijk in het MES-systeem of het kwaliteitsrapport naar de laatste ~20 metingen van deze maat. Zie je een trend (regel 3)? Noteer je bevinding en neem mee naar de volgende sessie.

---
*Bron: ko-spc-501 (CNC-frees casus — I-MR en gereedschapsslijtage); AIAG SPC Reference Manual; Nelson (1984) — Western Electric runs rules uitgebreid; operator-cases maakindustrie | AIMM Module 2 — SPC Train | v1.0*
