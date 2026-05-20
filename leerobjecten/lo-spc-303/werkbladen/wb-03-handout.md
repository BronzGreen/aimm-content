# Handout: Drie Capability-Valkuilen en de Juiste Volgorde
*Capability (Cp, Cpk, Pp, Ppk) — wanneer is het getal betrouwbaar?*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"Capability is niet één formule maar drie voorwaarden: geschikt meetsysteem, stabiel proces, rationele subgroepering. Eén voorwaarde geschonden = getal misleidend."**

Pak je markeerstift. Markeer wat je herkent uit jouw lijn. Twee minuten.

---

## De drie valkuilen in één plaatje

```
                 Cpk = 1,5
                     ↑
         ┌───────────┼───────────┐
         │           │           │
   MEETSYSTEEM   STABILITEIT   SUBGROEPEN
   (Gage R&R)   (regelkaart)   (rationeel)
         │           │           │
    Eén faalt → het getal liegt
```

Eén voorwaarde onbekend = je weet niet wat het getal waard is. Eén voorwaarde geschonden = het getal is misleidend, hoe mooi ook opgemaakt.

---

## Valkuil 1 — Capability op een instabiel proces

**Het probleem.** Op een instabiel proces is σ een mix van normale variatie + verstoringen (shift-wissels, recept-wisselingen, machine-drift). Het getal dat je uit de formule rolt is dus geen "capability" maar een gemiddeld ding over meerdere toestanden. Morgen krijg je een ander getal.

**Hoe herken je dit?**
- Er is geen SPC-regelkaart over de meetperiode
- De regelkaart toont wél out-of-control signalen (punten buiten ±3σ, runs, trends)
- De data komt uit "100 metingen over 3 dagen" zonder controle of die periode stabiel was

**Regel (NIST/SEMATECH):** SPC-regelkaart → bevestig stabiliteit → daarna pas Cpk.

**Wat is stabiliteit concreet?** Op een I-MR, X-bar/R of X-bar/S kaart: geen punten buiten controlegrenzen, geen runs van 7+ aan één kant, geen trends van 6+ omhoog of omlaag. Zie Western Electric / Nelson-regels (ko-spc-204).

---

## Valkuil 2 — Slechte subgroepering

**Het probleem.** Binnen-subgroep σ moet alléén gewone variatie bevatten. Als je subgroepen shifts, recepten of caviteiten mengt, vermengen korte- en langetermijnvariatie:

- **Te grote subgroep-σ** (shift-effecten erin) → Cp/Cpk te conservatief
- **Te dichte subgroep-σ** (alleen binnen één lot) → Cp/Cpk te optimistisch

**Voorbeeld.** Vijf metingen per uur van een spuitgietlijn met vier caviteiten: de caviteit-verschillen zitten in σ. De echte machine-capability is waarschijnlijk hóger dan het getal suggereert — of lager, afhankelijk van hoe de monsters zijn getrokken.

**Regel (AIAG / ko-spc-109):** rationele subgroepen — vrijwel zelfde omstandigheden, dicht in tijd, één bron (zelfde machine, zelfde caviteit, zelfde recept, zelfde shift).

**Pp/Ppk vs Cp/Cpk.** Pp/Ppk gebruikt totale variatie (langetermijn), Cp/Cpk gebruikt binnen-subgroep variatie (kortetermijn). Verschil tussen Pp en Cp zegt iets over subgroep-strategie: veel verschil = veel langetermijn-variatie buiten de subgroepen om.

---

## Valkuil 3 — Slecht meetsysteem

**Het probleem.** Als de meetfout groot is, zegt Cpk evenveel over de **meter** als over de **machine**. Een ruisige meter blaast de schijnbare procesvariatie op. Werkelijk capabele processen lijken niet capabel. Investering gaat naar de verkeerde plek.

**Hoe vaak is dit echt?** In automotive-audits komt het dagelijks voor. Vandaar dat Ford PPAP (4e editie) **expliciet Gage R&R eist** vóór capability-indiening. AIAG's MSA Reference Manual (4e) beschrijft de methode.

**Vuistregel (AIAG MSA 4e — %GRR):**

| %GRR (van tolerantie of procesvariatie) | Oordeel |
|-----------------------------------------|---------|
| **< 10%** | Meetsysteem geschikt |
| **10 – 30%** | Marginaal — conditioneel acceptabel, verbetering overwegen |
| **> 30%** | Niet geschikt voor capability-studie |

**Regel (Ford PPAP):** Gage R&R / MSA → meetsysteem geschikt? → daarna pas capability-studie.

---

## De juiste volgorde — één stroomschema

```
START
   │
   ▼
 ┌───────────────────────────────────┐
 │ 1. Meetsysteem geschikt?          │ ← AIAG MSA / Ford PPAP
 │    (Gage R&R, %GRR < 30%)         │
 └───────────────────────────────────┘
   │ Ja                          │ Nee / Onbekend
   ▼                             ▼
 ┌───────────────────────────────────┐    [Eerst meetsysteem verbeteren
 │ 2. Proces stabiel?                 │     of Gage R&R uitvoeren]
 │    (SPC-regelkaart, geen signalen) │ ← NIST/SEMATECH
 └───────────────────────────────────┘
   │ Ja                          │ Nee / Onbekend
   ▼                             ▼
 ┌───────────────────────────────────┐    [Eerst stabiliseren
 │ 3. Verdeling redelijk?            │     of instabiliteit verklaren]
 │    (normaliteit-check, histogram)  │
 └───────────────────────────────────┘
   │ Ja                          │ Nee
   ▼                             ▼
 ┌───────────────────────────────────┐    [Transformatie of
 │ 4. Capability berekenen            │     non-parametrische aanpak]
 │    Cp, Cpk, Pp, Ppk               │
 └───────────────────────────────────┘
   │
   ▼
 ┌───────────────────────────────────┐
 │ 5. Beslissing nemen op basis van   │
 │    getallen — nu onderbouwd        │
 └───────────────────────────────────┘
```

---

## Per voorwaarde: wat check je, waar staat het?

### 🔵 Meetsysteem

| Check | Bron / document |
|-------|----------------|
| Gage R&R-rapport aanwezig | Kwaliteitsafdeling / MSA-register |
| %GRR < 30% (liefst < 10%) | Rapport zelf |
| Laatste studie < 5 jaar oud of nieuwste meterwissel | MSA-register |
| Methode volgens AIAG MSA 4e | Procedurebeschrijving |

### 🟠 Stabiliteit

| Check | Bron / document |
|-------|----------------|
| SPC-regelkaart over dezelfde periode | SPC-systeem / MES |
| Geen out-of-control signalen (Western Electric / Nelson) | Regelkaart zelf |
| Regelgrenzen op basis van voldoende historiek | SPC-plan |

### 🟣 Subgroepering

| Check | Bron / document |
|-------|----------------|
| Subgroep-definitie gedocumenteerd | SPC-plan / control plan |
| Eén bron per subgroep (machine, caviteit, shift, recept) | SPC-plan |
| Subgroep-grootte consistent (meestal n=3 tot n=5) | SPC-plan |
| Frequentie passend bij proces-snelheid | SPC-plan |

---

## De drie vragen die jij voortaan stelt

Bij elk Cpk-getal dat op je bureau komt:

1. **Meetsysteem** — *"Is er een geldig Gage R&R-rapport voor deze meting, en wat is %GRR?"*
2. **Stabiliteit** — *"Is er een regelkaart over dezelfde periode, en waren er out-of-control signalen?"*
3. **Subgroepering** — *"Hoe waren de subgroepen samengesteld — één machine/caviteit/shift/recept?"*

Drie keer "ja met bron" = getal bruikbaar.
Eén keer "onbekend" = eerst uitzoeken.
Eén keer "nee" = getal niet bruikbaar voor beslissing.

---

## De fictieve case — herken je dit?

> *Fictieve case ter illustratie — niet uit één specifiek bedrijf.* Een lijnmanager rapporteert "Cpk = 1,5 voor onze nieuwe productlijn". Een kritische teamleider stelt drie vragen:
>
> - **"Was het proces stabiel toen je dit berekende?"** → "We hebben 100 metingen genomen over 3 dagen." → Regelkaart ontbrak.
> - **"Hoe waren de subgroepen?"** → "Vijf metingen per uur, vier caviteiten door elkaar." → Caviteit-effecten zaten in σ.
> - **"Is het meetsysteem gevalideerd?"** → "We gebruiken de standaard schuifmaat." → Geen Gage R&R — mogelijk 30% meetfout.
>
> **Conclusie:** het getal 1,5 is misschien correct, maar zonder antwoord op deze drie vragen weet niemand het. Eerst valideren, dán beslissen.

---

## Wanneer mag je een voorwaarde overslaan?

**Bijna nooit.** Maar onder deze condities is beperkte acceptatie verdedigbaar:

| Voorwaarde | Wanneer overslaan mag (met voorbehoud) |
|-----------|----------------------------------------|
| **Gage R&R** | Meetsysteem is net gevalideerd (< 1 jaar) én niet gewijzigd |
| **Stabiliteit-check** | Nooit overslaan — minimaal histogram + I-chart nodig |
| **Subgroep-analyse** | Voor een eenmalige Pp/Ppk-schatting op totale variatie (niet voor Cp/Cpk) |

**In automotive (Ford PPAP):** geen enkele voorwaarde mag worden overgeslagen. Non-conformance = herindiening.

---

## Operator-rol vs teamleider-rol

| Voorwaarde | Operator | Teamleider (jij) |
|-----------|----------|------------------|
| **Meetsysteem** | Meet consistent volgens instructie; rapporteert onzekerheid eerlijk | Vraagt Gage R&R op; plant studie bij meterwissel |
| **Stabiliteit** | Bewaakt regelkaart; rapporteert signalen | Beoordeelt stabiliteit vóór capability-claim; vraagt kaart-uitdraai |
| **Subgroepering** | Weet welke subgroep gemeten wordt | Definieert rationele subgroepen; documenteert in SPC-plan |

---

## Onthoud dit

1. **Capability is een gevolg, geen start** — eerst de drie voorwaarden, dan de formule
2. **Ford PPAP eist Gage R&R vóór capability** — automotive-audit-vereiste, geen suggestie
3. **%GRR > 30% = getal onbruikbaar** — investeer in meter vóór in machine
4. **Regelkaart vóór capability** — NIST/SEMATECH-regel, geen academisch detail
5. **Rationele subgroepen** — één bron per subgroep, zie ko-spc-109
6. **Onbekend ≠ oké** — onbekende voorwaarde = eerst uitzoeken, niet "waarschijnlijk wel goed"

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Cp** | Capability-index zonder centrering — (USL − LSL) / (6σ_binnen) |
| **Cpk** | Capability met centrering — min van afstand gemiddelde tot beide grenzen |
| **Pp / Ppk** | Performance-indices op totale (langetermijn) variatie ipv binnen-subgroep |
| **σ_binnen vs σ_totaal** | Binnen-subgroep variatie (Cp/Cpk) vs totale variatie (Pp/Ppk) |
| **Gage R&R** | Measurement System Analysis — Repeatability + Reproducibility |
| **%GRR** | Percentage meetvariatie tov proces- of tolerantie-variatie |
| **MSA** | Measurement Systems Analysis — AIAG-methode voor meetsysteem-validatie |
| **PPAP** | Production Part Approval Process — Ford/AIAG vrijgave-procedure |
| **Rationele subgroep** | Subgroep met vrijwel zelfde omstandigheden — één bron, dicht in tijd |
| **Out-of-control signaal** | Punt buiten controlegrenzen, run of trend (Western Electric / Nelson-regels) |

---

> **Volgende stap.** In blok 2 pak je één eigen gerapporteerd capability-getal en legt het langs deze drie voorwaarden (wb-01). Hou deze handout open als referentie.

---
*Bron: ko-spc-303; NIST/SEMATECH e-Handbook of Statistical Methods — hoofdstuk Process Capability; AIAG Measurement Systems Analysis Reference Manual (4e editie); Ford Production Part Approval Process (PPAP 4th edition); Minitab documentation; ko-spc-109 (rationele subgroepen); ko-spc-204 (out-of-control regels) | AIMM Module 3 — SPC Op Maat | v1.0*
