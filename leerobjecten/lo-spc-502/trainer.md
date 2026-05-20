---
id: lo-spc-502-trainer
knowledge_object_id: ko-spc-502
version: trainer
title: Attribuut-regelkaarten (c, p, np, u) — trainer-pakket
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
correlation_id: ronde26-lo-spc-502
---

# Attribuut-regelkaarten (c, p, np, u) — voor de trainer

**Leerobject:** lo-spc-502
**Kennisobject:** ko-spc-502
**Doelgroep:** MBO-3 operator (primair), MBO-4 (secundair); B1-B2
**Duur:** 45 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | c-kaart oefening op fictieve PCB-assemblagecasus (individueel), STARRT-reflectie op late escalatie + plenaire transfer-ronde, handout c vs p vs np + Nelson-regel-1 + escalatieketen |
| Kolb-startfase | Ervaren — eerst zelf 8/6/9 beoordelen, dán theorie en escalatie |
| Begeleidingsstijl | Trainen — bewust onbekwaam, normaliserend ("achteraf simpel, ter plekke om 7 uur is het echt een keuze") |
| Materialen | wb-01 t/m wb-03, A3-print diagram-lo-spc-502.svg, flip-over met kaarttype-beslisschema (vast/variabel n × defect/defective), rekenmachines (1 per duo) voor √c̄-berekening |

## Wat de deelnemer leert

De deelnemer kan bij telgegevens van een assemblage-inspectie (defecten per vaste eenheid) herkennen dat een c-kaart het passende kaarttype is (en niet p of np), de UCL berekenen met c̄ + 3√c̄, een punt boven UCL herkennen als Nelson-regel-1 signaal, en een passende escalatiestap kiezen (apart zetten, quarantaine, leverancier informeren). Aan het einde benoemt hij/zij minimaal 3 van de 4 oefenvragen correct: kaartkeuze + onderbouwing, UCL ≈ 7,1 (LCL afgekapt op 0), Nelson-regel-1 markering, 2 escalatiestappen in juiste volgorde.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:15 | c-kaart oefening: PCB-casus 8/6/9 | Individueel wb-01: kaartkeuze + UCL + signaal + escalatie |
| Reflecteren | 0:15-0:30 | STARRT op een late-escalatie-ervaring + plenaire Transfer-ronde | Individueel wb-02 + 1-2 deelnemers delen Transfer |
| Theoretiseren | 0:30-0:45 | Handout: c vs p vs np + Nelson-regel-1 + escalatieketen | Trainer-geleide doorloop, koppeling aan oefening |

## Tips voor de trainer

- **Open normaliserend.** "Achteraf lijkt dit simpel. Ter plekke, om 7 uur 's ochtends, met een ploeg die door moet — dan is dit echt een keuze. We gaan die keuze nu kalm maken."
- **Bij rondloop blok 1: vragen stellen, geen antwoorden.** "Wat tel je eigenlijk: defecte boards of defecten?" "Is je eenheid elke keer even groot?"
- **Bij c/np-verwarring scherp.** "Eén PCB met 3 soldeerfouten = 1 defective (np), maar 3 defecten (c). c-kaart telt totaalaantal fouten; np telt aantal afgekeurde eenheden." Verwijs naar handout-beslisschema.
- **Bij wisselende n: p of u, niet np of c.** Bron AIAG SPC + NIST/SEMATECH §6.3.3.
- **Bij Nelson-regels op c/p-kaart: kritisch.** "Alleen regel 1 en sommige run-patronen zijn direct toepasbaar. Regels gebaseerd op normaalverdeling (2-uit-3 buiten 2σ) moeten getoetst worden bij Poisson/Binomiaal." Bron: Nelson 1984 + AIAG §III.
- **Bij STARRT plenair: alleen Transfer vrijwillig delen.** Rest van STARRT blijft persoonlijk. Geef ruimte voor stilte.
- **Verbind oefening met escalatie-keten.** "Eerste punt boven UCL = Nelson-regel-1 — precies wat jullie zagen." Kaartkeuze (c vs p vs np) is het echte vakmanschap, berekening is eenvoudig.

## Valkuilen

- **Defecten (c) verward met defective eenheden (np).** Direct corrigeren met PCB-voorbeeld. Anders verkeerd kaart-type → ruis in signaalherkenning.
- **Wisselende sample-size zonder p/u te kiezen.** "Bij wisselende n → p (defectives) of u (defecten). Niet np of c."
- **Nelson-regels klakkeloos op attribuutkaart.** Stop kort, leg verschil uit (Poisson/Binomiaal vs normaal). Anders worden run-rules verkeerd toegepast.

## Voorbereiding

- [ ] wb-01, wb-02, wb-03 printen (1 per deelnemer + reserve)
- [ ] diagram-lo-spc-502.svg op A3 printen, zichtbaar in zaal
- [ ] Flip-over: kaarttype-beslisschema (vast/variabel n × defect/defective)
- [ ] Beamer + HDMI testen, presenter-modus
- [ ] Pennen, markeerstiften, rekenmachines (1 per duo, voor √2,4)
- [ ] Vraag deelnemers vooraf om één eigen telgrootheid in gedachten te hebben

## Transferopdracht

Geef de deelnemer mee dat hij/zij deze week op de eigen lijn één kwaliteitsgrootheid kiest die per vaste eenheid wordt geteld (defecte soldeerpunten per 50 boards, krassen per 100 stuks, foute labels per pallet) en in werkschrift noteert: eenheid, wat je telt, gemiddelde per eenheid (vraag teamleider/rapport). Bereken zelf UCL met c̄ + 3√c̄. Plus: vraag teamleider of leverancierscode/batch-ID aan de telgegevens gekoppeld is — zonder traceerbaarheid is terugroepen lastig.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
