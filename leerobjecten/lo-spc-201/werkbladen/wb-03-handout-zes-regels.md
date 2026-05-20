# Handout: de zes Nelson-regels op één blad
*Handout — Kolb-fase 3 (theoretiseren) · naslagwerk*

**Module 2 — SPC Train | Patroonherkenning op de regelkaart**

---

> **Kernidee**
> Wachten op één punt buiten de grenzen is vaak te laat. Echte verstoringen verraden zich eerder via patronen. Een trend, een verschuiving, een rare oscillatie. Lloyd Nelson schreef in 1984 acht regels op. Vandaag oefenen we met regels 1 tot en met 6. Regels 7 en 8 komen later.

---

## Over dit werkblad

Dit is geen oefen-werkblad. Dit is je naslag. Hou het naast je quiz en straks naast je eigen kaart op de lijn. De zes regels staan hier kort uitgelegd, met een voorbeeld uit de werkvloer.

---

## De zes regels — referentietabel

| Regel | Patroon op de kaart | Wat zegt het over je proces? | Eerste actie als operator |
|:-----:|---------------------|------------------------------|---------------------------|
| **1** | 1 punt buiten ±3σ (boven UCL of onder LCL) | Sterke aanwijzing dat er iets anders is gebeurd | Meetfout uitsluiten · laatste wijziging checken · verdacht product apart · teamleider informeren |
| **2** | 9 punten op rij aan één kant van de centrumlijn | Het procesgemiddelde lijkt verschoven (shift) | Check set-up · gereedschap · offset · grondstofbatch · matrijstemperatuur |
| **3** | 6 punten op rij stijgend of dalend | Trend — vaak slijtage of opwarming | Check drift: gereedschapsslijtage · matrijskoeling · slijpsteen · drukverlies |
| **4** | 14 punten afwisselend op-neer | Systematische oscillatie | Zoek twee afwisselende oorzaken: twee operators · twee caviteiten · pulserende regeling |
| **5** | 2 van 3 punten voorbij ±2σ aan dezelfde kant | Kleine maar serieuze shift — vroege waarschuwing | Reageer sneller dan bij regel 2 · check dezelfde oorzaken |
| **6** | 4 van 5 punten voorbij ±1σ aan dezelfde kant | Subtielere shift — proces drijft weg | Check of het proces wegloopt vóór er overschrijdingen komen |

---

## De zes regels — één voor één

### Regel 1 — Punt buiten de grens

```
     +3σ ─────────────────────────●─  ← ALARM: punt buiten UCL
     +2σ ··············●···········
      CL ──●──●──●──●─────────────
     −1σ ········●····●···········
     −3σ ─────────────────────────
```

Eén meting boven UCL of onder LCL. Klassiek alarm. Dit kennen de meeste operators al. Het is de basis.

**Voorbeeld werkvloer:** spuitgieten, onderdeelgewicht. Punt 11 valt op 100,7 g terwijl UCL = 100,2 g. Net na een matrijswissel. Eerst meting checken. Daarna product apart leggen.

---

### Regel 2 — 9 punten aan één kant

```
     +2σ ······●···●···●···●·······●···●···●···●··
     +1σ ──●──────────────────────────────────────
      CL ─────────────────────────────────────────
     −1σ ─────────────────────────────────────────
```

Negen metingen op rij allemaal boven (of allemaal onder) de centrumlijn. Geen enkel punt hoeft buiten de grens te vallen. Het patroon is het signaal. Vaak een teken dat het gemiddelde is verschoven (shift).

**Voorbeeld werkvloer:** CNC-frees, diameter. Na een offset-verstelling zit het proces consistent te hoog. Geen enkele meting buiten ±3σ, maar wel 9 op rij boven de centrumlijn.

---

### Regel 3 — Trend (6 punten omhoog of omlaag)

```
     +2σ ·····························●
     +1σ ························●····
      CL ──●──────────────●──●──────
     −1σ ······●─────●───────────────
```

Zes metingen op rij die elke keer hoger (of elke keer lager) liggen. De trend zegt: er kruipt iets in één richting. Vaak slijtage of opwarming.

**Voorbeeld werkvloer:** spuitgieten, gewicht. De waarden lopen op: 99,80 → 99,85 → 99,90 → 99,95 → 100,00 → 100,05 g. Geen punt buiten de grenzen. Toch is er iets aan de hand. De matrijskoeling blijkt deels verstopt.

---

### Regel 4 — Oscillatie (14 punten afwisselend)

```
     +2σ ──●──────●──────●──────●──────●─
      CL ─────────────────────────────────
     −2σ ─────●──────●──────●──────●──────
```

Veertien metingen die strak afwisselen hoog-laag-hoog-laag. Dit is geen ruis. Dit is ritme. Twee bronnen wisselen elkaar af.

**Voorbeeld werkvloer:** verpakkingslijn met twee vulkoppen. De ene kop vult net iets vóller dan de andere. Om en om meten geeft een zigzag-kaart.

---

### Regel 5 — Kleine shift (2 van 3 voorbij ±2σ)

```
     +3σ ─────────────────────────────────────
     +2σ ─────────────────●·──●·······────────
     +1σ ●··●···●·······●·····────────────────
      CL ─────────────────────────────────────
```

Twee van de laatste drie metingen vallen voorbij +2σ (of −2σ) aan dezelfde kant. Eerder signaal dan regel 2. Reageer dus sneller.

**Voorbeeld werkvloer:** CNC-frees, diameter. Twee opeenvolgende metingen schieten net voorbij +2σ. Daarna één meting net binnen. Klein signaal — maar wel een vroege waarschuwing dat het proces wegdrijft.

---

### Regel 6 — Subtiele shift (4 van 5 voorbij ±1σ)

```
     +2σ ─────────────────────────────────────
     +1σ ──────────────●──●──●─────●──●───────
      CL ──●──●──●──●─────────────────────────
     −1σ ──────●──●──────────────────────────
```

Vier van de laatste vijf metingen vallen voorbij +1σ aan dezelfde kant. Subtieler dan regel 5. Maar wel een vroege waarschuwing dat het proces aan het wegdrijven is — nog vóór de UCL.

**Voorbeeld werkvloer:** voedselverwerking, vulgewicht. Vier van vijf metingen zitten net boven +1σ. Niet alarmerend. Wel iets om in de gaten te houden.

---

## Welke regel kies je voor jouw lijn?

| Type lijn of situatie | Eerst deze regels checken |
|-----------------------|---------------------------|
| Spuitgieten met matrijswisselen | **Regel 1, 2, 3** (shift na wissel · trend door koeling) |
| Spuitgieten met meerdere caviteiten | **Regel 1, 4** (oscillatie tussen caviteiten) |
| CNC-frees met gereedschapsslijtage | **Regel 1, 3** (trend door slijtage) |
| CNC met twee operators | **Regel 1, 4** (oscillatie tussen werkstijlen) |
| Verpakking met twee vulkoppen | **Regel 1, 4** (oscillatie tussen koppen) |
| Stabiele machine, fijne kwaliteit nodig | **Regel 1, 5, 6** (vroege shifts oppikken) |

---

## Kies klein: niet alle 6 tegelijk

> Begin deze week met **regel 1 plus 1 of 2 patroonregels** die passen bij jouw lijn.
> Beter goed met 2 regels dan slordig met 6.

Patroonherkenning is een vaardigheid die groeit door doen. Niet door alle regels uit je hoofd te leren. Volgende week kun je er één bij pakken.

---

## Wat doe je als je een patroon ziet?

1. **Schrik niet.** Een patroon is een signaal. Nog geen afkeur. Kijk eerst, handel daarna.
2. **Koppel aan een gebeurtenis.** Wat is er recent gewijzigd? Matrijswissel · batch · gereedschap · shift · operator · setting?
3. **Check de meting zelf.** Klopt het instrument? Is er meetfout?
4. **Onderneem actie passend bij de regel.** Gebruik de tabel hierboven.
5. **Noteer wat je hebt gezien én wat je hebt gedaan.** Dat helpt jou en de volgende shift.

---

## Vakwoorden kort uitgelegd

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

## Verdieping voor later: regel 7 en 8

> **Niet voor deze sessie — alleen als achtergrond.**

Nelson heeft nog twee regels die op het eerste gezicht raar lijken:

- **Regel 7** — *15 punten allemaal binnen ±1σ.* Lijkt goed (weinig spreiding!). Maar Nelson noemt dit verdacht. Vaak een teken dat er iets met je meetmethode of subgroepering niet klopt. "Te mooi om waar te zijn."
- **Regel 8** — *8 punten allemaal buiten ±1σ aan beide kanten.* Wijst op een mengsel van twee bronnen. Twee machines door elkaar. Twee leveranciers. Twee recepten.

Deze regels behandelen we in module 3 (op maat) — als je met je eigen data werkt. Zie je vandaag al zo'n patroon? Leg het voor aan je teamleider.

---

## Bron

Nelson, L.S. (1984). *The Shewhart Control Chart — Tests for Special Causes.* Journal of Quality Technology, 16(4), 237-239.
NIST/SEMATECH e-Handbook of Statistical Methods, sectie 6.3.2.
Western Electric Company (1956). *Statistical Quality Control Handbook* — voorloper van Nelson (4 regels).

*AIMM Module 2 — SPC Train | Handout v1.0*
