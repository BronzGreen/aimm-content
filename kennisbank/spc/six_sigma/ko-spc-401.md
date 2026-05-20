---
id: ko-spc-401
title: Six Sigma — wat het is en hoe het zich verhoudt tot SPC
type: concept_uitleg
domain: spc
subdomain: six_sigma
summary: 'Six Sigma is een data-gedreven verbeterbenadering met als numeriek

  doel 3,4 defects per million opportunities (DPMO). Ontstaan bij

  Motorola (1986, Bill Smith), opgeschaald bij GE onder Welch. SPC

  is een deelverzameling van Six Sigma — vooral in de Control-fase.'
source_centrality: 0.7
source_ref: ASQ Six Sigma definitie en historie; Motorola/Bill Smith oorsprong; GE/Jack
  Welch opschaling
status: validated
updated_at: '2026-05-20'
correlation_id: ronde19-lo-spc-401
---

# Six Sigma — wat het is en hoe het zich verhoudt tot SPC

## Definitie
Six Sigma is een data-gedreven verbeterbenadering die procesvariatie
reduceert en het numerieke kwaliteitsdoel **3,4 defects per million
opportunities** (DPMO) koppelt aan een 6σ-prestatieniveau (ASQ).

## Historische oorsprong
| Jaar | Wie | Wat |
|------|-----|-----|
| **1986** | Motorola, Bill Smith | Six Sigma als gestructureerde verbeterbenadering geformuleerd |
| **Jaren '90** | General Electric, Jack Welch | Brede opschaling — Six Sigma wordt managementmainstream |

## Het 1,5σ-shift detail (didactische valkuil)
De bekende 3,4 DPMO is gekoppeld aan een **1,5σ-shift-aanname** in
de Six Sigma-traditie. "Zes sigma" in Six Sigma-taal is dus **niet
identiek** aan de zuiver kortetermijnkans van een perfect gecentreerde
normale verdeling zonder drift.

In operatoronderwijs hoeft dit niet diep wiskundig te worden uitgelegd,
maar moet wel correct benoemd worden:
> Sigma-niveau is in Six Sigma een managementmaat voor defectkans,
> niet simpelweg een synoniem voor Cpk.

## Hoe verhouden SPC en Six Sigma zich?
SPC is **geen concurrent** van Six Sigma maar een **deelverzameling**:

| Aspect | SPC | Six Sigma |
|--------|-----|-----------|
| Scope | Procesbewaking | Volledig verbeterproject |
| Tools | Regelkaarten, Cpk | DMAIC + SPC + FMEA + DOE + process mapping + MSA |
| Plaats in DMAIC | Vooral **Control**-fase | Het hele Define-Measure-Analyze-Improve-Control |

## Didactische boodschap voor operators
"Een regelkaart is niet het hele verbeterproces, maar wel het
instrument waarmee je ziet of een verbetering werkelijk blijft staan."

## Andere Six Sigma-tools (waar SPC niet over gaat)
- **FMEA** (Failure Mode and Effects Analysis)
- **Process mapping** (SIPOC, value stream mapping)
- **Measurement Systems Analysis** (Gage R&R)
- **Design of Experiments** (DOE)
- **Hypothesetoetsing**
- **5-Why** en visgraat-diagrammen


## Praktijkvoorbeeld

*Fictieve illustratie van een Six Sigma project — plausibele Cpk/uitval-cijfers, niet een specifieke casus.*

Een verpakkingslijn loopt al jaren met SPC-kaarten (regel 1 + 2),
Cpk = 1,15 — capabel maar niet uitmuntend. Het kwaliteitsteam
besluit een Six Sigma-project op te starten:

- **Define**: probleem = uitval van 0,8% door scheve etiketten
- **Measure**: baseline-Cpk vaststellen, defecten classificeren
- **Analyze**: visgraat → oorzaak ligt bij temperatuursschommeling
  in lijmreservoir
- **Improve**: temperatuur-PID-regeling toevoegen, pilotrun
- **Control**: SPC-kaart op temperatuur + regelkaart op uitval om
  verbetering te borgen

SPC was hier de **bewakingstool in de Control-fase**, terwijl Six
Sigma de bredere verbeterstructuur leverde.
