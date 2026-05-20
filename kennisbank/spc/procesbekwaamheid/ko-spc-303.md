---
id: ko-spc-303
title: Capability-valkuilen — drie didactische fouten die getallen waardeloos maken
type: tip
domain: spc
subdomain: procesbekwaamheid
summary: 'Capability-indices (Cp, Cpk, Pp, Ppk) hebben drie veelgemaakte fouten:

  rekenen op een instabiel proces, slechte subgroepering, en een slecht

  meetsysteem. Elk produceert mooie getallen die niets zeggen over

  werkelijke procesprestatie.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Handbook; AIAG MSA Reference Manual; Ford PPAP 4th edition;
  Minitab documentation
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-spc-303
---

# Capability-valkuilen — drie didactische fouten die getallen waardeloos maken

## Fout 1: Capability rekenen op een instabiel proces
Een proces moet **eerst stabiel** zijn voor capability-berekening
zinvol is. Doe je het op een instabiel proces:
- Je krijgt één getal over data uit **meerdere toestanden**
- De σ is een mix van gewone variatie en verstoringen
- Conclusies zijn willekeurig: morgen krijg je een ander getal

**Volgorde:** SPC-regelkaart → bevestig stabiliteit → daarna pas Cpk.

## Fout 2: Slechte subgroepering
Subgroepen die meerdere shifts, recepten of caviteiten mengen,
vermengen kortetermijn- en langetermijnvariatie:
- Binnen-subgroep σ wordt **te groot** (omdat shift-effecten erin
  zitten)
- Cp/Cpk wordt daardoor **te conservatief** geschat
- Of: subgroepen worden te dicht bij elkaar genomen → onderschatting
  van werkelijke variatie → Cp/Cpk te optimistisch

**Regel:** rationele subgroepen (zie ko-spc-109) — vrijwel zelfde
omstandigheden, dicht in tijd, één bron.

## Fout 3: Slecht meetsysteem
Als de meetfout groot is, zegt Cpk evenveel over de **meter** als
over de **machine**:
- Een ruisige meter blaast de schijnbare procesvariatie op
- Werkelijk capabele processen lijken niet capabel
- Investering gaat naar de verkeerde plek (machine ipv meetsysteem)

**Volgorde:** Gage R&R / MSA → meetsysteem geschikt? → daarna pas
capability-studie. Ford eist dit expliciet in PPAP.

## De juiste volgorde
```
1. Meetsysteem geschikt?  (Gage R&R / MSA)
        ↓ Ja
2. Proces stabiel?         (SPC-regelkaart over voldoende periode)
        ↓ Ja
3. Verdeling redelijk?     (normaliteit-check)
        ↓ Ja
4. Capability berekenen    (Cp, Cpk, Pp, Ppk)
        ↓
5. Pas dan beslissingen nemen op basis van getallen
```

## Implicatie voor operator-onderwijs
Capability mag in MBO-onderwijs **niet alleen over formules** gaan.
Het gaat over:
- Proces-stabiliteit (SPC eerst)
- Subgroepstrategie (rationale subgroep)
- Meetkunde (Gage R&R / MSA)

Een operator die alleen "Cpk = 1,2" leest weet niet of dat getal
betrouwbaar is. Een operator die de drie voorwaarden begrijpt, kan
de juiste vragen stellen.


## Praktijkvoorbeeld

Een lijnmanager rapporteert "Cpk = 1,5 voor onze nieuwe productlijn".
Een kritische teamleider stelt drie vragen:

1. **"Was het proces stabiel toen je dit berekende?"**
   → "We hebben 100 metingen genomen over 3 dagen." → Maar was er
   een regelkaart die geen out-of-control signalen gaf?

2. **"Hoe waren de subgroepen?"**
   → "Vijf metingen per uur, vier caviteiten door elkaar." → Caviteit-
   effecten zitten in σ — Cpk is mogelijk onderschat.

3. **"Is het meetsysteem gevalideerd?"**
   → "We gebruiken de standaard schuifmaat." → Gage R&R is niet
   gedaan — de getallen kunnen voor 30% meetfout bevatten.

Conclusie: het getal 1,5 is misschien correct, maar zonder antwoord
op deze drie vragen weet niemand het. Eerst valideren, dan
beslissingen nemen.
