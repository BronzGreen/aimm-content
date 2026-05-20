# Handout: De DMAIC-Cyclus en Tools per Fase
*DMAIC — Define, Measure, Analyze, Improve, Control (Six Sigma)*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"DMAIC dwingt de volgorde: meten → analyseren → veranderen → borgen. Elke fase heeft een eigen vraag, eigen tools en eigen rollen."**

Pak je markeerstift. Markeer wat je herkent uit projecten die wél werkten — en wat je herkent uit projecten die niet werkten. Twee minuten.

---

## De cyclus in één plaatje

```
   ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
   │ DEFINE   │ →  │ MEASURE  │ →  │ ANALYZE  │ →  │ IMPROVE  │ →  │ CONTROL  │
   │ (probleem)│    │(baseline)│    │(oorzaken)│    │(testen)  │    │ (borgen) │
   └──────────┘    └──────────┘    └──────────┘    └──────────┘    └─────┬────┘
        ▲                                                                  │
        └──────────  nieuwe afwijking ─────────────────────────────────────┘
```

Vijf fases. Geen fase overslaan, geen fase verkort. Pijl van Control terug naar Define is geen versiersel — als je in Control nieuwe afwijkingen ziet, begin je een volgend Define.

---

## Centrale vraag + valkuil + één tool per fase

| Fase | Centrale vraag | Belangrijkste valkuil | Eerste tool die past |
|------|---------------|----------------------|----------------------|
| 🔵 **Define** | Wat is het probleem en waarom is het belangrijk? | Te brede scope ("hele lijn verbeteren") | Projectcharter — SMART probleem + scope + business case |
| 🟠 **Measure** | Wat is de huidige prestatie? | Geen baseline — "we gaan meten" | SPC-baseline (controlekaart) — laat variatie + stabiliteit zien |
| 🟣 **Analyze** | Waardoor ontstaat het probleem? | Mono-causaal denken ("het ligt aan X") | Visgraat (Ishikawa, 6M) — brede brainstorm |
| 🟢 **Improve** | Welke verandering lost het op? | Te grote stap — direct lijn-breed uitrollen | Pilot — kleinschalig + success-criterium |
| 🔴 **Control** | Hoe borgen we de winst? | Vergeten of "doen we later wel" | Control plan — wat, hoe vaak, door wie, reactie |

---

## Volledige tools-tabel per fase

### 🔵 DEFINE — Wat is het probleem?

| Tool | Wanneer inzetten? | Wanneer overslaan? |
|------|-------------------|--------------------|
| **SIPOC** (Supplier-Input-Process-Output-Customer) | Meerdere stakeholders, scope onduidelijk | Eén lijn met heldere klant en grenzen |
| **Projectcharter** | Altijd — formele goedkeuring + budget | Nooit overslaan |
| **Klachtdefinitie / Voice of Customer** | Externe klant betrokken | Intern proces zonder externe klant |
| **CTQ-tree** (Critical to Quality) | Vertaling klantbehoefte → meetbare eis | Eis is al meetbaar geformuleerd |

### 🟠 MEASURE — Wat is de huidige prestatie?

| Tool | Wanneer inzetten? | Wanneer overslaan? |
|------|-------------------|--------------------|
| **SPC-baseline (controlekaart)** | Altijd — laat de huidige variatie zien én of het proces stabiel is | Nooit overslaan voor Improve-fase |
| **Cp / Cpk-berekening** | Continue meetwaarden met klanttoleranties | Bij kwalitatieve defecten (gebruik p-kaart) |
| **Gage R&R / MSA** | Twijfel over meetsysteem (nieuwe meter, handmeting, scheidsrechter) | Meetsysteem net gevalideerd of digitaal/automatisch |
| **Defectdefinities** | Discrete defecten met onduidelijke grenzen | Defect is zwart-wit (binnen/buiten tolerantie) |
| **Pareto van baseline** | Meerdere defectsoorten — prioriteren | Eén dominant defect |

### 🟣 ANALYZE — Waardoor ontstaat het probleem?

| Tool | Wanneer inzetten? | Wanneer overslaan? |
|------|-------------------|--------------------|
| **Visgraat (Ishikawa, 6M)** | Brede brainstorm: Mens, Machine, Materiaal, Methode, Meting, Milieu | Eén dominante hypothese al bekend |
| **Pareto-analyse** | Prioriteren binnen meerdere oorzaken (80/20) | Eén oorzaak domineert al duidelijk |
| **5x Waarom** | Eén symptoom traceren naar root cause | Meerdere parallelle oorzaken |
| **Hypothesetoets / SPC-stratificatie** | Vermoeden van shift tussen ploegen, batches, machines | Geen sub-groepen of geen data |
| **DOE (Design of Experiments)** | Meerdere variabelen die elkaar beïnvloeden | Eén duidelijke variabele — gewone pilot volstaat |

### 🟢 IMPROVE — Welke verandering lost het op?

| Tool | Wanneer inzetten? | Wanneer overslaan? |
|------|-------------------|--------------------|
| **Pilot / kleinschalige test** | Altijd — niet meteen lijn-breed uitrollen | Aanpassing is risicovrij én reversibel |
| **DOE (Design of Experiments)** | Multi-variabele optimalisatie (parameter-instellingen) | Eén-knop-aanpassing |
| **Standaardwerk** | Variatie door verschillende werkwijzen | Volledig geautomatiseerd proces |
| **Poka-Yoke (foutpreventie)** | Menselijke fouten voorkomen door ontwerp | Procesvariatie zonder menselijke component |
| **Change management plan** | Aanpassing raakt > 1 ploeg/lijn/team | Lokale aanpassing, één team |

### 🔴 CONTROL — Hoe borgen we de winst?

| Tool | Wanneer inzetten? | Wanneer overslaan? |
|------|-------------------|--------------------|
| **Control plan** | Altijd — vastlegging wat, hoe vaak, door wie, met welke reactie | Nooit overslaan |
| **SPC-controlekaart (permanent)** | Continue bewaking kritische maat | Bij niet-meetbare eigenschap |
| **Reactieplan bij signaal** | Altijd — operator moet weten wat te doen bij regel-trigger | Nooit overslaan |
| **Visuele standaarden** | Werkvloer-zichtbare bewaking (poster, dashboard, kleurcode) | Volledig digitale bewaking met alarm |
| **Maandelijkse audit** | Naleving niet vanzelfsprekend | Volledig geautomatiseerd proces |

---

## Operator vs teamleider — wie doet wat per fase?

| Fase | Operator | Teamleider (jij) |
|------|----------|------------------|
| **Define** | Probleem-ervaring inbrengen | SIPOC-sessie faciliteren, charter opstellen |
| **Measure** | Eerlijke baseline-metingen | Meetplan, Gage R&R organiseren, datakwaliteit bewaken |
| **Analyze** | Patronen herkennen ("vooral bij batch X") | Visgraat- en 5-Why-sessies leiden, stratificatie |
| **Improve** | Pilots uitvoeren, eerlijk rapporteren | DOE coördineren, change management |
| **Control** | SPC-kaart bijhouden, signalen rapporteren | Control plan opstellen, audits uitvoeren |

> **Onthoud:** jullie organiseren het denken — je team levert het materiaal. Geen DMAIC zonder operators die meedoen.

---

## Spuitgiet-anchor (referentievoorbeeld)

> **De casus.** Spuitgietlijn met chronisch 1,2 % afkeur op onderdeelgewicht. Doel: < 0,3 % in 3 maanden, business case €40.000.
>
> - **Define** — scope: één lijn, één maat (gewicht), één doelgetal in drie maanden.
> - **Measure** — SPC-baseline + Gage R&R (meetsysteem verklaarde 18 % van variatie — eerst meter, dan machine).
> - **Analyze** — visgraat onthulde drie oorzaken (matrijskoeling, materiaalvocht, restdruk) — niet één.
> - **Improve** — DOE met 8 runs → nieuwe parameter-set → pilot bevestigt 0,4 %.
> - **Control** — control plan met SPC-bewaking op drie kritische parameters, werkinstructies, maandelijkse audits. Resultaat na 4 maanden: 0,28 % afkeur.

Dit is de schaal — concreet, meetbaar, met einde. Geen sjabloon om te kopiëren — wel een ijkpunt voor je eigen Define.

---

## Wanneer welke tool overslaan? — Snelle checklist

| Tool | Sla over als... |
|------|-----------------|
| **SIPOC** | Scope is al duidelijk, één lijn |
| **Gage R&R** | Meetsysteem net gevalideerd of digitaal |
| **Visgraat** | Eén dominante hypothese is al onderbouwd |
| **DOE** | Eén variabele speelt — gewone pilot volstaat |
| **Pareto** | Eén defect domineert > 80% |
| **Maandelijkse audit** | Volledig automatische bewaking met alarm |

**Pas de zwaarte van je tools aan op de complexiteit van je probleem.**

---

## Onthoud dit

1. **Define = scherpte** — vaag probleem = vaag project = vaag resultaat
2. **Measure = baseline** — geen baseline, geen project
3. **Analyze = oorzaken vinden, niet oplossingen bedenken** — verleiding weerstaan
4. **Improve = pilot, dan uitrol** — nooit lijn-breed in één keer
5. **Control = borging vanaf dag 1** — niet aan het einde "even regelen"
6. **Tools dienen de fase** — overslaan mag, mits onderbouwd

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **DMAIC** | Define-Measure-Analyze-Improve-Control: Six Sigma-route voor bestaande processen |
| **DMADV** | Define-Measure-Analyze-Design-Verify: voor ontwerp van nieuwe processen |
| **PDCA** | Plan-Do-Check-Act (Deming): lichtere cyclus, geen vervanging voor DMAIC |
| **SIPOC** | Supplier-Input-Process-Output-Customer — proces-overview op één pagina |
| **CTQ** | Critical to Quality — meetbare klanteis |
| **Gage R&R** | Meetsysteem-analyse (Repeatability & Reproducibility) |
| **DOE** | Design of Experiments — gestructureerde multi-variabele experimenten |
| **Poka-Yoke** | Foutpreventie door ontwerp (Japans: "fout-vermijding") |
| **Control plan** | Vastlegging hoe een verbetering structureel geborgd wordt |
| **6M** | Visgraat-categorieën: Mens, Machine, Materiaal, Methode, Meting, Milieu |

---

> **Volgende stap.** In blok 2 ga je deze structuur toepassen op je eigen lijn — het DMAIC-canvas (wb-02). Hou deze handout open als referentie.

---
*Bron: ko-spc-402 (DMAIC); ASQ DMAIC-definitie; Pyzdek 'Six Sigma Handbook'; Ford / AIAG Control Plan-richtlijnen | AIMM Module 3 — SPC Op Maat | v1.1*
