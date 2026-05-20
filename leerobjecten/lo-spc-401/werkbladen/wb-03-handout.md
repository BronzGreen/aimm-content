# Handout: Six Sigma en SPC — de positionering
*Six Sigma — definitie, historie, en hoe SPC erin past*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"Een regelkaart is niet het hele verbeterproces, maar wel het instrument waarmee je ziet of een verbetering werkelijk blijft staan."**

Pak je markeerstift. Markeer wat je nog niet wist, en wat je herkent uit je eigen lijn. Twee minuten.

---

## 1. Wat is Six Sigma?

**Six Sigma** is een **data-gedreven verbeterbenadering** die procesvariatie reduceert en het numerieke kwaliteitsdoel **3,4 defects per million opportunities (DPMO)** koppelt aan een **6σ-prestatieniveau** (ASQ-definitie).

Kortom: minder variatie, minder defecten, aantoonbaar.

---

## 2. Historische oorsprong

| Jaar | Wie | Wat |
|------|-----|-----|
| **1986** | Motorola, Bill Smith | Six Sigma als gestructureerde verbeterbenadering geformuleerd |
| **Jaren '90** | General Electric, Jack Welch | Brede opschaling — Six Sigma wordt managementmainstream |

Six Sigma is dus geen recent begrip — het is ruim 35 jaar oud en diep geworteld in de management-praktijk.

---

## 3. Let op — didactische valkuil: het 1,5σ-shift-detail

De bekende **3,4 DPMO** is gekoppeld aan een **1,5σ-shift-aanname** in de Six Sigma-traditie. "Zes sigma" in Six Sigma-taal is dus **niet identiek** aan de zuiver kortetermijnkans van een perfect gecentreerde normale verdeling zonder drift.

In operator-onderwijs hoeft dit niet diep wiskundig, maar moet het wel correct benoemd worden:

> **Sigma-niveau is in Six Sigma een managementmaat voor defectkans, niet simpelweg een synoniem voor Cpk.**

Als je kwaliteitscoördinator zegt: "We zitten op sigma-niveau 4" — dat is niet hetzelfde als "Cpk = 4/3". Het is een management-kengetal voor defectkans, berekend inclusief de 1,5σ-shift.

---

## 4. Hoe verhouden SPC en Six Sigma zich?

SPC is **geen concurrent** van Six Sigma — SPC is een **deelverzameling**.

| Aspect | SPC | Six Sigma |
|--------|-----|-----------|
| **Scope** | Procesbewaking | Volledig verbeterproject |
| **Tools** | Regelkaarten, Cpk, p-kaarten | DMAIC + SPC + FMEA + DOE + process mapping + MSA |
| **Plaats in DMAIC** | Vooral **Control**-fase (ook meetbron in Measure) | Het hele Define-Measure-Analyze-Improve-Control |

---

## 5. DMAIC — de vijf fasen van Six Sigma

```
   ┌────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐
   │ DEFINE │ →  │ MEASURE │ →  │ ANALYZE │ →  │ IMPROVE │ →  │ CONTROL │
   │ probleem│    │ baseline│    │ oorzaken│    │  testen │    │ borgen  │
   └────────┘    └─────────┘    └─────────┘    └─────────┘    └────┬────┘
        ▲                                                           │
        └──────────  nieuwe afwijking ──────────────────────────────┘
```

| Fase | Centrale vraag | Typische tools | Waar zit SPC? |
|------|---------------|----------------|----------------|
| **Define** | Wat is het probleem? | SIPOC, projectcharter, CTQ | Nee |
| **Measure** | Wat is de huidige prestatie? | SPC-baseline, Gage R&R | **Ja — baseline** |
| **Analyze** | Waardoor ontstaat het? | Visgraat, 5-Why, Pareto, hypothesetoets | Als data-bron |
| **Improve** | Welke verandering helpt? | Pilot, DOE, standaardwerk | Als monitoring-tool tijdens pilot |
| **Control** | Hoe borgen we de winst? | Control plan, permanente SPC-kaart, audits | **Ja — kernrol** |

---

## 6. Six Sigma-tools buiten SPC

Tools waar SPC niet over gaat, maar die in een breder Six Sigma-project wél relevant zijn:

| Tool | Wat doet het? | Wanneer relevant? |
|------|---------------|-------------------|
| **FMEA** (Failure Mode and Effects Analysis) | Risico's vooraf inventariseren | Nieuwe processen, wijzigingen met risico |
| **SIPOC / process mapping** | Proces in kaart brengen | Scope onduidelijk, meerdere stakeholders |
| **Gage R&R / MSA** | Meetsysteem valideren | Twijfel over meting (handmeting, nieuwe meter) |
| **DOE (Design of Experiments)** | Meerdere parameters tegelijk testen | Multi-variabele optimalisatie |
| **Hypothesetoetsing** | Statistisch toetsen of verschil echt is | Shift tussen ploegen, batches |
| **5-Why / visgraat** | Oorzaakanalyse | Analyze-fase |

Herken je een probleem op je lijn waarvan je weet dat het met alleen regelkaart-bewaking niet opgelost wordt? Grote kans dat een van deze tools het volgende stapje is.

---

## 7. De didactische boodschap voor operators

> **"Een regelkaart is niet het hele verbeterproces, maar wel het instrument waarmee je ziet of een verbetering werkelijk blijft staan."**

Dit is precies de waarde die SPC binnen Six Sigma levert:
- **Vóór het project** — SPC geeft je baseline in Measure.
- **Tijdens het project** — SPC monitort je pilot in Improve.
- **Na het project** — SPC borgt de verbetering in Control.

Maar SPC zelf vindt geen oorzaken en ontwerpt geen oplossingen. Daar zijn de andere tools voor.

---

## 8. Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Six Sigma** | Data-gedreven verbeterbenadering met doel 3,4 DPMO |
| **DPMO** | Defects Per Million Opportunities — kwaliteitsmaat |
| **σ (sigma)** | Statistische standaarddeviatie — maat voor variatie |
| **Sigma-niveau** | Managementmaat voor defectkans (inclusief 1,5σ-shift) |
| **Cpk** | Capability-index uit SPC-data — niet hetzelfde als sigma-niveau |
| **DMAIC** | Define-Measure-Analyze-Improve-Control — Six Sigma-route voor bestaande processen |
| **DMADV** | Voor het ontwerpen van **nieuwe** processen |
| **1,5σ-shift** | Aanname dat procesgemiddelde op lange termijn 1,5σ verschuift |
| **FMEA** | Risico-analyse: wat kan er misgaan en hoe erg? |
| **Gage R&R** | Meetsysteem-analyse (Repeatability & Reproducibility) |
| **DOE** | Design of Experiments — multi-variabele experimenten |
| **SIPOC** | Supplier-Input-Process-Output-Customer — proces-overview |

---

## 9. Onthoud dit

1. **Six Sigma = verbeterraamwerk, SPC = bewakingstool binnen dat raamwerk.**
2. **DMAIC geeft de volgorde: meten → analyseren → veranderen → borgen.**
3. **SPC zit vooral in Control (borging) en Measure (baseline).**
4. **Sigma-niveau ≠ Cpk** — verschillende maten, verschillende context.
5. **Wanneer SPC stokt, kijk naar visgraat / 5-Why / Gage R&R / DOE.**
6. **Motorola 1986, GE jaren '90** — Six Sigma is geen hype, het is doorbewezen.

---

> **Volgende stap.** In blok 2 doe je een STARRT-reflectie op een moment waar SPC alleen niet volstond (wb-02). In blok 3 positioneer je één eigen vraagstuk in DMAIC (wb-01).

---
*Bron: ko-spc-401 (Six Sigma en SPC); ASQ Six Sigma definitie en historie; Motorola/Bill Smith 1986; GE/Jack Welch opschaling jaren '90; Pyzdek — Six Sigma Handbook | AIMM Module 3 — SPC Op Maat | v1.0*
