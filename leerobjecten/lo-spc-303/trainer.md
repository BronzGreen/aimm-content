---
id: lo-spc-303-trainer
knowledge_object_id: ko-spc-303
version: trainer
title: Gage R&R — is je meting betrouwbaar? — trainer-pakket
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
correlation_id: ronde20-lo-spc-303
---

# Gage R&R — is je meting betrouwbaar? — voor de trainer

**Leerobject:** lo-spc-303
**Kennisobject:** ko-spc-303
**Doelgroep:** MBO-4 operator (primair), teamleider MBO-4 (secundair); B2
**Duur:** 45 min
**Bloom:** evalueren

## In één oogopslag

| | |
|---|---|
| Werkvormen | Coachende handout-doorloop drie valkuilen, individuele toetsing van een eigen Cpk-getal aan drie voorwaarden, STARRT-reflectie met afsluitende plenaire één-zin-ronde |
| Kolb-startfase | Theoretiseren — drie voorwaarden + juiste volgorde, dan toepassen |
| Begeleidingsstijl | Coachen — bewust bekwaam, doorvragen i.p.v. oplossingen geven |
| Materialen | wb-01 t/m wb-03, A3-print diagram-lo-spc-303.svg, optioneel schuifmaat + standaardblok voor Gage R&R-demo, flip-over met %GRR-drempels + drie voorwaarden-check |

## Wat de deelnemer leert

De deelnemer kan een gerapporteerd capability-getal kritisch toetsen door vóór acceptatie de drie voorwaarden te controleren — meetsysteem geschikt (Gage R&R/MSA), proces stabiel (SPC-regelkaart), subgroepering rationeel — en kan onderbouwen wanneer een getal wel of niet betrouwbaar is voor beslissingen. Aan het einde levert hij/zij een ingevulde analyse met per voorwaarde ja/nee/onbekend + bron, drie concrete vragen voor de rapporteur, en één maandag-actie. AIAG MSA, Ford PPAP en NIST/SEMATECH zijn de bronnen.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Theoretiseren | 0:00-0:12 | Drie valkuilen + juiste volgorde + bronnen | Coachende handout-doorloop, herkenningsvragen |
| Experimenteren | 0:12-0:32 | Eigen Cpk-getal toetsen aan drie voorwaarden | Individueel wb-01, trainer rondloopt met coachvragen |
| Reflecteren | 0:32-0:45 | STARRT op wb-02 + één-zin-ronde maandag-actie | Individueel + plenaire ronde |

## Tips voor de trainer

- **Anchor met de fictieve case uit het KO.** Lijnmanager claimt Cpk=1,5 zonder antwoord op drie vragen. Per valkuil: "Herken je dit? Is dit ooit gebeurd op onze lijn?"
- **Bron per standaard expliciet noemen.** Ford PPAP eist Gage R&R vóór capability. AIAG MSA beschrijft de methode. NIST/SEMATECH Handbook beschrijft stabiliteit.
- **Vermijd formule-college.** Focus op wanneer je een getal vertrouwt — niet op σ-berekeningen.
- **Bij rondloop: doorvragen, geen oplossingen.** "Weet je zeker dat het proces stabiel was — heb je de regelkaart gezien?" "Is meetsysteem gevalideerd volgens AIAG MSA?" "Hoe waren subgroepen samengesteld?"
- **"Onbekend" mag op wb-01.** "Onbekend = eerst uitzoeken vóór het getal een beslissing stuurt." Dat is precies de les.
- **Bij Gage R&R = kalibratie-misverstand: stop kort.** Kalibratie toetst nauwkeurigheid tegen referentie; Gage R&R toetst herhaalbaarheid (zelfde operator) + reproduceerbaarheid (tussen operators). Beide nodig (AIAG MSA 4th ed.).
- **%GRR-drempels: <10% acceptabel, 10-30% conditioneel, >30% niet acceptabel.** 25% zit in grijze zone — context bepaalt (AIAG MSA §II).

## Valkuilen

- **Gage R&R = kalibratie.** Direct corrigeren met onderscheid (zie tip). Anders denkt deelnemer dat gekalibreerd meetsysteem automatisch Gage R&R-compliant is.
- **%GRR-drempels verkeerd toegepast (25% = "oké").** AIAG-norm uitleggen, grijze zone benoemen, context bepaalt.
- **Geen toegang tot MSA-data.** "Die getallen zien wij niet — alleen kwaliteit." Leer de minimale operator-vraag: "Wanneer is laatste Gage R&R op deze meter gedaan, wat was de uitkomst?" Dat is de basisrol.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer)
- [ ] diagram-lo-spc-303.svg op A3 printen, zichtbaar in zaal
- [ ] Optioneel: schuifmaat + standaardblok klaarleggen voor Gage R&R-demo
- [ ] Flip-over: %GRR-drempels (<10 / 10-30 / >30) + drie voorwaarden-check
- [ ] Beamer + HDMI testen, presenter-modus
- [ ] Pennen, markeerstiften klaarleggen
- [ ] Vraag deelnemers vooraf om een eigen kwaliteitsrapport / MES-export mee te brengen

## Transferopdracht

Geef de deelnemer mee dat hij/zij komende week (1) één recent gerapporteerd capability-getal toetst langs wb-01, (2) drie vragen stelt aan de rapporteur (kwaliteit, proces-engineer of externe auditor), (3) per voorwaarde antwoord + bron noteert, (4) bepaalt of het getal bruikbaar is voor de lopende beslissing. Plus: gesprek met kwaliteitscoördinator over Gage R&R-register voor kritische meetmiddelen — AIAG MSA-richtlijn: elke 5 jaar of bij meterwissel. Geen register? Eerste agendapunt.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
