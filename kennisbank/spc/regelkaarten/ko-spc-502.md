---
id: ko-spc-502
title: Assemblage casus — c-kaart en defecte materiaalbatch terugroepen
type: voorbeeld
domain: spc
subdomain: regelkaarten
summary: 'Assemblage-operator inspecteert 50 boards/uur op soldeerfouten.

  c-kaart: centerlijn 2,4 fouten/50 boards, UCL ≈ 7,1. Na materiaalwissel

  sprong naar 8/6/9 fouten — eerste punt buiten UCL (Nelson-regel 1).

  Materiaalbatch teruggeroepen vóór impact op meerdere shifts.'
source_centrality: 0.7
source_ref: Maakindustrie-praktijk; AIAG SPC Reference Manual; geïllustreerd uit operator-cases
status: validated
updated_at: '2026-05-20'
correlation_id: ronde26-lo-spc-502
---

# Assemblage casus — c-kaart en defecte materiaalbatch terugroepen

## Productiecontext
- **Productie**: assemblagelijn voor printplaten (PCB)
- **Inspectie**: per uur 50 geassembleerde boards visueel op
  soldeerfouten
- **Datatype**: tellingen per gelijke eenheid (50 boards) → **c-kaart**

## Berekening control limits
- **Centerlijn (c̄)**: historisch 2,4 fouten per 50 boards
- **UCL = c̄ + 3√c̄** = 2,4 + 3√2,4 = 2,4 + 4,65 ≈ **7,1**
- **LCL** = c̄ − 3√c̄ = 2,4 − 4,65 < 0 → LCL = 0

## Het signaal
Na een **materiaalwissel** (nieuwe leverancier-batch):

| Uur | Aantal fouten | Beoordeling |
|-----|---------------|-------------|
| t=0 | 8 | **Boven UCL — Nelson regel 1!** |
| t=1 | 6 | Hoog, maar binnen UCL |
| t=2 | 9 | **Weer boven UCL — bevestiging** |

Patroon wijst op special cause verbonden aan **nieuwe materiaalbatch**.

## Escalatie en respons
1. Operator informeert teamleider direct na het eerste signaal
2. Boards uit verdachte productie-uren apart zetten
3. Escalatie naar **kwaliteit en engineering**
4. Materiaalbatch in **quarantaine**
5. Leverancier informeren — **terugroepen** voor onderzoek
6. Productie hervatten met monsters van vorige batch

## Resultaat
Terugroep voorkomt dat **meer dan één shift** wordt beïnvloed.
Escalatie binnen 2 uur na eerste signaal beperkt impact tot
~150 boards (3 uur × 50), waarvan onderzoek nodig is.

## Lessen
- **c-kaart geschikt** voor defecten per gelijke eenheid
- UCL-formule: **c̄ + 3√c̄** (Poisson-aanname)
- LCL kan negatief uitkomen → afkappen op 0
- **Nelson-regel 1 zelf bij c-kaart** = krachtig signaal
- **Materiaal-traceerbaarheid** is voorwaarde voor effectieve
  escalatie

## Inzetbaarheid in modules
| Module | Inzet |
|--------|-------|
| **1 Gebruik** | Herkennen: wat zegt deze c-kaart? Wat doe je? |
| **2 Train** | Inrichten: wanneer kies je c boven p of u? |
| **3 Op Maat** | Ontwerpen: hoe richt je traceerbaarheid en escalatie in? |


## Praktijkvoorbeeld

[De casus zelf is het voorbeeld]

De keuze voor c-kaart (niet p of np):
- Niet **p**: dan zou je % defecten meten (defecten/50). c is
  intuïtiever bij **fouten per object**.
- Niet **np**: np telt defecte stuks, niet defecten zelf. Eén board
  kan meerdere soldeerfouten hebben.
- **c**: telt defecten per **vaste eenheid** (50 boards) — exact
  wat hier gebeurt.
