# Handout: De Nelson-rules — patronen op de regelkaart
*Patroonherkenning op Shewhart-kaarten — Lloyd S. Nelson (1984)*

**Module 2 — SPC Train | Naslagwerk**

---

> **Kernidee**  
> Wachten op één punt buiten ±3σ is vaak te laat. Echte verstoringen verraden zich meestal eerst via een patroon — een trend, een shift, een rare oscillatie. Lloyd Nelson heeft in 1984 acht regels geformaliseerd. In deze sessie oefenen we met de **6 hoofdregels (1 t/m 6)**. Regel 7 en 8 komen later — als je subgroepering goed begrijpt.

---

## De 6 hoofdregels — referentietabel

| Regel | Patroon op de kaart | Wat zegt het over je proces? | Wat doe je als operator? |
|:-----:|---------------------|------------------------------|--------------------------|
| **1** | 1 punt buiten ±3σ (boven UCL of onder LCL) | Sterke aanwijzing dat er iets ánders is gebeurd | Meetfout uitsluiten · laatste proceswijziging checken · verdacht product apart leggen · teamleider informeren |
| **2** | 9 punten op rij aan één kant van de centrumlijn | Procesgemiddelde lijkt verschoven (shift) | Check set-up · gereedschap · offset · grondstofbatch · matrijstemperatuur |
| **3** | 6 punten op rij stijgend of dalend | Trend — vaak slijtage of opwarming | Check drift: gereedschapsslijtage · matrijskoeling · slijpsteen · drukverlies |
| **4** | 14 punten afwisselend op–neer | Systematische oscillatie | Zoek twee afwisselende oorzaken: twee operators · twee caviteiten · pulserende regeling |
| **5** | 2 van 3 punten voorbij ±2σ aan dezelfde kant | Kleine maar serieuze shift — vroege waarschuwing | Reageer sneller dan bij regel 2 · check dezelfde oorzaken (set-up, batch, temp) |
| **6** | 4 van 5 punten voorbij ±1σ aan dezelfde kant | Subtielere shift — proces drijft weg | Check of proces wegloopt vóór er overschrijdingen komen |

---

## 🔵 Patroonherkennings­schema's

*Mini-tijdreeksen — gebruik dit naast de quiz om kaart en regel naast elkaar te zien.*

### Regel 1 — Punt buiten de grens

```
     +3σ ─────────────────────────●─  ← ALARM: punt buiten UCL
     +2σ ··············●···········
      CL ──●──●──●──●─────────────
     −1σ ········●····●···········
     −3σ ─────────────────────────
```
*Eén meting boven UCL of onder LCL. Klassiek alarm.*

---

### Regel 2 — 9 punten één kant

```
     +2σ ······●···●···●···●·······●···●···●···●··
     +1σ ──●──────────────────────────────────────
      CL ─────────────────────────────────────────
     −1σ ─────────────────────────────────────────
```
*Negen metingen op rij allemaal boven (of allemaal onder) de centrumlijn. Geen punt hoeft buiten de grens te vallen — het patroon is genoeg.*

---

### Regel 3 — Trend (6 punten omhoog of omlaag)

```
     +2σ ·····························●
     +1σ ························●····
      CL ──●──────────────●──●──────
     −1σ ······●─────●───────────────
```
*Zes metingen op rij die elke keer hoger (of elke keer lager) liggen. Vaak: matrijs warmt op · gereedschap slijt · slijpsteen verstompt.*

---

### Regel 4 — Oscillatie

```
     +2σ ──●──────●──────●──────●──────●─
      CL ─────────────────────────────────
     −2σ ─────●──────●──────●──────●──────
```
*Veertien metingen die strak afwisselen hoog–laag. Wijst op twee bronnen die elkaar afwisselen: twee caviteiten · twee operators die om en om meten · een pulserende regeling.*

---

### Regel 5 — Kleine shift (2 van 3 voorbij ±2σ)

```
     +3σ ─────────────────────────────────────
     +2σ ─────────────────●·──●·······────────
     +1σ ●··●···●·······●·····────────────────
      CL ─────────────────────────────────────
```
*Twee van de laatste drie metingen vallen voorbij +2σ (of −2σ) aan dezelfde kant. Eerder signaal dan regel 2 — dus reageer sneller.*

---

### Regel 6 — Subtiele shift (4 van 5 voorbij ±1σ)

```
     +2σ ─────────────────────────────────────
     +1σ ──────────────●──●──●─────●──●───────
      CL ──●──●──●──●─────────────────────────
     −1σ ──────●──●──────────────────────────
```
*Vier van de laatste vijf metingen vallen voorbij +1σ aan dezelfde kant. Proces is aan het wegdrijven — nog vóór de UCL.*

---

## 🟠 Welke regel kies je voor jouw lijn?

| Type machine / situatie | Eerst deze regels checken |
|-------------------------|---------------------------|
| Spuitgieten met matrijswisselen | **Regel 1, 2, 3** (shift na wissel · trend door koeling) |
| Spuitgieten meerdere caviteiten | **Regel 1, 4** (oscillatie tussen caviteiten) |
| CNC-frees met gereedschapsslijtage | **Regel 1, 3** (trend door slijtage) |
| CNC met twee operators | **Regel 1, 4** (oscillatie tussen werkstijlen) |
| Stabiele machine, fijne kwaliteit nodig | **Regel 1, 5, 6** (vroege shifts oppikken) |

---

## 🔴 Kies klein: niet alle 6 tegelijk

> Begin deze week met **regel 1 + 1 of 2 patroonregels** die passen bij jouw lijn.  
> Beter goed met 2 regels dan slordig met 6.

Als je meer wilt: pak er volgende week één bij. Patroonherkenning is een vaardigheid die groeit door doen, niet door alle regels uit je hoofd te leren.

---

## 🟢 Wat doe je als je een patroon ziet?

1. **Schrik niet.** Een patroon is een signaal, niet meteen afkeur. Kijk eerst, handel daarna.
2. **Koppel aan een gebeurtenis.** Wat is er recent gewijzigd? Matrijswissel · batch · gereedschap · shift · operator · setting?
3. **Check de meting zelf.** Klopt het instrument? Is er meetfout?
4. **Onderneem actie passend bij de regel.** Gebruik de tabel hierboven.
5. **Noteer wat je hebt gezien én wat je hebt gedaan.** Dat helpt jou en de volgende shift.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Shewhart-kaart** | Regelkaart met centrumlijn en ±1σ, ±2σ, ±3σ-grenzen |
| **UCL / LCL** | Upper / Lower Control Limit — boven- en ondergrens (±3σ) |
| **Centrumlijn (CL)** | Het gemiddelde van je proces |
| **σ (sigma)** | Maat voor de normale spreiding van je proces |
| **Shift** | Een verschuiving van het procesgemiddelde |
| **Trend** | Een geleidelijke beweging in één richting |
| **Oscillatie** | Strak wisselen tussen hoog en laag |
| **Special cause** | Uitzonderlijke invloed van buiten het normale gedrag |

---

## 🟣 Verdieping voor later: regel 7 en 8

> **Niet voor deze sessie — alleen als achtergrond.**

Nelson heeft nog twee regels die op het eerste gezicht raar lijken:

- **Regel 7** — *15 punten allemaal binnen ±1σ.* Lijkt goed (weinig spreiding!), maar Nelson noemt dit verdacht: vaak een teken dat er iets met je meetmethode of subgroepering niet klopt. "Te mooi om waar te zijn."
- **Regel 8** — *8 punten allemaal buiten ±1σ aan beide kanten.* Wijst op een mengsel van twee bronnen — twee machines die door elkaar lopen, twee leveranciers, twee recepten.

Deze regels behandelen we in een vervolgsessie, omdat ze pas zinvol zijn als je goed begrijpt hoe je subgroepen samenstelt. Voor nu: als je deze patronen ziet, leg ze voor aan je teamleider.

---
*Bron: Nelson, L.S. (1984) ‘The Shewhart Control Chart — Tests for Special Causes’, Journal of Quality Technology · NIST/SEMATECH Handbook | AIMM Module 2 — SPC Train | v1.0*
