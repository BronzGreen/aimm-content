# Handout: Cpk vs Ppk — wat ervaart je klant écht?
*Pp/Ppk — langetermijn-procesbekwaamheid (ko-spc-302)*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"Cpk laat zien wat je proces kan. Ppk laat zien wat je klant ervaart. De gap tussen beide is zelf een diagnostisch signaal."**

Pak je markeerstift. Markeer de Ford-drempel (1,67) en de vier oorzaken van tussen-subgroep-variatie. Twee minuten.

---

## 1. Het verschil in één tabel

| Index-paar | Spreiding | Wat het meet |
|------------|-----------|--------------|
| 🔵 **Cp / Cpk** | Binnen-subgroep σ (kortetermijn) | Wat het proces **kan** als het stabiel is |
| 🔴 **Pp / Ppk** | Totale σ (langetermijn) | Wat de **klant uiteindelijk ervaart** |

**Bijna altijd geldt:** Cpk ≥ Ppk.

Waarom? Omdat tussen subgroepen (shifts, batches, setups) dingen schuiven die binnen één subgroep niet zichtbaar zijn. Die "tussen-subgroep-variatie" telt mee in Ppk maar niet in Cpk.

---

## 2. De gap als diagnose

| Gap (Cpk − Ppk) | Interpretatie | Waar ligt de actie? |
|------------------|---------------|---------------------|
| **< 0,10** | Stabiel proces, weinig tussen-subgroep-variatie | Op het proces zelf (als Cpk te laag) |
| **0,10 – 0,20** | Merkbare tussen-subgroep-variatie | Kijk naar batches, shifts, setups |
| **> 0,20** | Groot gat — systeem rondom proces is onrustig | Op het **systeem rondom**: setup, shift-overdracht, batch |

> **Kernidee:** een grote gap los je niet op met de machine strakker zetten. Je lost hem op door wat erbuiten gebeurt onder controle te krijgen.

---

## 3. Vier typische oorzaken van tussen-subgroep-variatie

1. **Materiaalbatch-wissels** — nieuwe batch, iets andere eigenschappen
2. **Shift-overdracht** — ploeg A en B stellen niet identiek in
3. **Setup-aanpassingen** — wisseltijd niet gestandaardiseerd
4. **Temperatuur** — dag/nacht, seizoen, locatie op de vloer

---

## 4. Industrie-eisen — Ford PPAP en AIAG

| Norm | Eis |
|------|-----|
| **Ford PPAP (4th edition, actueel)** | Ppk ≥ **1,67** voor relevante kritische kenmerken |
| **AIAG SPC Reference Manual** | Vergelijkbare eisen per kritisch kenmerk |
| **General Motors / VW** | Vaak hetzelfde of strenger |
| **NIST/SEMATECH e-Handbook** | Statistische definities en berekeningen |

**Waarom zo streng?** Omdat de klant de langetermijn-realiteit ervaart. Een Ppk van 1,67 betekent dat er ruimte blijft tot de tolerantiegrens ook als je shifts, batches en temperatuurverschillen meetelt.

---

## 5. Formules in het kort

**Cpk** (kortetermijn, binnen-subgroep):

Cpk = min(USL − μ, μ − LSL) / (3 × σ_within)

**Ppk** (langetermijn, totale spreiding):

Ppk = min(USL − μ, μ − LSL) / (3 × σ_total)

**Pp** (zonder centrering, langetermijn):

Pp = (USL − LSL) / (6 × σ_total)

> **Let op:** Cpk en Ppk corrigeren voor centrering. Cp en Pp niet. Rapporteer altijd beide — het paar (Cp, Cpk) of (Pp, Ppk) — nooit alleen Cp of Pp.

---

## 6. Operator vs teamleider — wie doet wat?

| Taak | Operator (MBO-4) | Teamleider (MBO-4) |
|------|------------------|---------------------|
| Data leveren | Eerlijk meten + registreren | Export uit MES / kwaliteit organiseren |
| Cpk/Ppk aflezen | Uit rapport halen | Berekenen of laten berekenen |
| Oorzaak-hypothese | Patronen op de vloer herkennen | Stratificatie per shift/batch maken |
| Actie op systeem rondom | Afwijking bij shift-overdracht melden | Setup-procedure herzien, shift-afspraak maken |

> **Onthoud:** de operator ziet de patronen het eerst. De teamleider organiseert de diagnose en de actie.

---

## 7. Spuitgiet-anchor (fictieve referentiecase)

> Een spuitgietlijn meet over een week: **Cpk = 1,42** (binnen elke shift goed), **Ppk = 1,05** (over de hele week onvoldoende). **Gap = 0,37** (groot).
>
> Onderzoek: ploeg B stelt systematisch 0,15 mm hoger in dan ploeg A. Binnen elke shift stabiel, maar shift-wissel zorgt voor drift over de week.
>
> **Actie:** niet de machine — wel het systeem rondom. Setup-procedure standaardiseren, ploeg B trainen, SPC-kaart met stratificatie per ploeg.
>
> Na 2 maanden: Ppk naar 1,48. Ford-eis 1,67 nog niet gehaald — vervolgstap ingepland.

Dit is de schaal en het type redenering — geen sjabloon om te kopiëren, wel een ijkpunt voor je eigen diagnose.

*(Fictieve case gebaseerd op veldervaring — gebruikt ter illustratie van het diagnostische principe.)*

---

## 8. Wanneer naar DMAIC?

Als je **gap > 0,20 is én je haalt de klant-eis (Ford: Ppk ≥ 1,67) niet**, is dit een DMAIC-kandidaat.

- Define: wat is precies het probleem, wat is de business case?
- Measure: baseline-Cpk én Ppk vastleggen
- Analyze: welke tussen-subgroep-bron is dominant?
- Improve: setup/shift-procedure aanpassen, pilot draaien
- Control: SPC-kaart met stratificatie per ploeg, reactieplan

Zie lo-spc-402 voor de DMAIC-route.

---

## 9. 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Cp / Cpk** | Procesbekwaamheid-indices op binnen-subgroep (kortetermijn) variatie |
| **Pp / Ppk** | Procesprestatie-indices op totale (langetermijn) variatie |
| **σ (sigma)** | Standaardafwijking — maat voor spreiding |
| **USL / LSL** | Upper / Lower Specification Limit — klanttolerantiegrenzen |
| **Subgroep** | Kleine reeks metingen dicht bij elkaar in tijd (bijv. 5 stuks achter elkaar) |
| **Binnen-subgroep** | Variatie binnen zo'n kleine reeks |
| **Tussen-subgroep** | Variatie tussen subgroepen (verschillende shifts, batches, setups) |
| **Ford PPAP** | Production Part Approval Process — klantgoedkeuring automotive (4th edition actueel) |
| **AIAG** | Automotive Industry Action Group — beheert SPC Reference Manual |
| **NIST/SEMATECH** | Amerikaans normeringsinstituut, bron voor statistische definities |
| **Stratificatie** | Data uitsplitsen naar subgroep (ploeg, batch, machine) om verschillen zichtbaar te maken |

---

## 10. Onthoud dit

1. **Cpk vertelt wat je machine kan** — binnen één shift
2. **Ppk vertelt wat je klant ervaart** — over de hele periode
3. **De gap is zelf een signaal** — groot gat = systeem rondom onrustig
4. **Ford PPAP eist Ppk ≥ 1,67** — niet alleen een mooie Cpk
5. **Grote gap = actie op systeem rondom** — setup, shift, batch, niet de machine
6. **Altijd beide rapporteren** — nooit alleen Cp of Pp zonder Cpk/Ppk

---

> **Volgende stap.** In blok 2 ga je Cpk en Ppk voor je eigen lijn naast elkaar zetten op wb-01. Hou deze handout open als referentie.

---
*Bron: ko-spc-302 (Pp/Ppk); Ford PPAP 4th edition; AIAG SPC Reference Manual; NIST/SEMATECH e-Handbook of Statistical Methods | AIMM Module 3 — SPC Op Maat | v1.0*
