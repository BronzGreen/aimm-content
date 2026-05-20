---
id: lo-spc-501-trainer
knowledge_object_id: ko-spc-501
version: trainer
title: CNC-frees casus — I-MR kaart en gereedschapsslijtage detecteren — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde25-lo-spc-501
---

# CNC-frees casus — I-MR kaart en gereedschapsslijtage detecteren — voor de trainer

**Leerobject:** lo-spc-501
**Kennisobject:** ko-spc-501
**Doelgroep:** MBO-4 operator (primair), MBO-3 operator + teamleider MBO-4 (secundair); B1-B2
**Duur:** 45 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Trend-oefening op CNC-frees casus + extra reeks (individueel), STARRT-reflectie + korte plenaire duiding, handout I-MR + Nelson-regel 3 met geïntegreerd actieplan eigen lijn |
| Kolb-startfase | Ervaren — eerst zelf trend lezen op de CNC-casus, dán theorie en eigen-lijn-actieplan |
| Begeleidingsstijl | Trainen — bewust onbekwaam, IK DOE één voorbeeldreeks (6 stijgende punten binnen UCL) |
| Materialen | wb-01 t/m wb-03, A3-print diagram-lo-spc-501.svg, flip-over met lege I-chart voor IK DOE + I-MR/X̄-R-kolommen, linialen + pennen |

## Wat de deelnemer leert

De deelnemer kan een I-MR-regelkaart opzetten voor een eigen kritische maat (meetfrequentie kiezen, UCL/LCL en MR-limiet aflezen) en een trendpatroon (Nelson-regel 3) herkennen als vroeg signaal dat tooling-actie nodig is — vóórdat een punt buiten control limits valt. Aan het einde benoemt hij/zij op wb-03 een kritische maat met tolerantie, meetfrequentie en subgroep-redenering (waarom I-MR vs X̄-R), én herkent minimaal 2 van de 3 trendsignalen correct als regel 3 + bijbehorende eerste actie (meten/checken, niet direct vervangen).

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:15 | Trend-oefening: CNC-frees casus + extra reeks | IK DOE 6-stijgende-voorbeeldreeks, JIJ DOET wb-01 |
| Reflecteren | 0:15-0:27 | STARRT individueel + korte plenaire duiding | wb-02 + 2-3 deelnemers delen Reflectie/Transfer |
| Theoretiseren | 0:27-0:45 | Handout I-MR + regel 3 + actieplan eigen lijn | Trainer-geleide doorloop + 8 min individueel actieplan |

## Tips voor de trainer

- **Doe de IK DOE-reeks hardop denkend.** "Geen punt buiten grenzen, maar zes punten achter elkaar omhoog kruipen — trend, Nelson-regel 3. Vraagt om gereedschap te controleren, niet vervangen."
- **Bij Reeks B (over-diagnose): laat groep meetellen.** Hardop tellen omhoog/omlaag/omhoog van links naar rechts. Max 2 op rij. "Regel 3 eist er 6. Zonder dat aantal: geen trend." Normaliseer: "Deze fout maken is het doel."
- **Bij "gereedschap vervangen" als eerste actie: stop kort.** "Eerste actie is meten, niet vervangen. Anders weet je morgen niet of het slijtage, temperatuur of materiaal was. Meten is leren."
- **Bij UCL/USL-verwarring: scherp onderscheid.** "USL = 10,020 mm = klantgrens, op tekening. UCL = 10,010 mm = processignaal-grens, uit proceshistorie. Cp/Cpk gebruikt USL/LSL — regelkaarten gebruiken UCL/LCL." Verwijs naar lo-spc-301 + ko-spc-107.
- **Laat eerst tellen vóór regel 3 uitleggen.** "Uur 35 naar 36, 36 naar 37 — welke kant op?" De tel-ervaring verankert de regel sterker dan de definitie.
- **Bij subgroep-misinterpretatie ("3 stuks/uur = X̄-R"): vraag terug.** "Komen die drie stuks achter elkaar uit de machine met tijd tussen, of uit één slag/cyclus?" Sequentieel = I-MR. Simultaan = mogelijk X̄-R.
- **UCL-formule kort houden.** "UCL = X̄ + 2,66 · M̄R. Factor 2,66 uit statistische tabel — niet onthouden. MES rekent. Wat je wél onthoudt: UCL ≠ USL." Geen d2-tabel-uitleg.

## Valkuilen

- **Over-diagnose Reeks B (trend zien waar geen trend is).** Niet meteen corrigeren, laat tellen. Anders gaan operators thuis elke schommeling als trend diagnosticeren.
- **Gereedschap vervangen zonder meten.** Verbind met documentatie: "Zonder meten geen leerervaring voor je collega die morgen dezelfde trend ziet." Anders blijft organisatie reactief tooling wisselen zonder oorzaakanalyse.
- **UCL/USL door elkaar.** Stop kort, expliciet onderscheid. Anders denkt deelnemer "binnen spec = binnen control limits" — fundamenteel verwarrend, ondermijnt regelkaart-idee.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer + 2 reserve)
- [ ] diagram-lo-spc-501.svg op A3 printen, achter in zaal hangen
- [ ] Flip-over: lege I-chart-grid voor IK DOE + I-MR/X̄-R-kolommen + ruimte voor reeks-plotjes
- [ ] Beamer + HDMI testen, slide 7 met SVG klaar, IK DOE-voorbeeldreeks op slide
- [ ] Linialen + pennen + markeerstiften per deelnemer
- [ ] Timer klaarleggen
- [ ] Voorbereiding zelf: 6-stijgende-voorbeeldreeks hardop oefenen

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week één kritische maat op de eigen lijn kiest (diameter, vulgewicht, dikte) en in werkschrift noteert: machine, maat, tolerantie (USL/LSL), meetfrequentie. Beargumenteer: I-MR-waardig (unieke metingen) of subgroepen mogelijk (X̄-R)? Kijk in MES of kwaliteitsrapport naar laatste 20 metingen — zie je een trend (regel 3)? Plus: vraag teamleider/engineer: "Gebruiken we Nelson-regels voor vroege signalering, of alleen punt-buiten-UCL?"

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
