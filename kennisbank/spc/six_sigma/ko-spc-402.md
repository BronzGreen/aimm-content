---
id: ko-spc-402
title: DMAIC — vijf-stappen verbeterroute voor bestaande processen
type: framework
domain: spc
subdomain: six_sigma
summary: 'DMAIC = Define, Measure, Analyze, Improve, Control. Gestructureerde

  probleemoplossingsroute van Six Sigma voor bestaande processen die

  niet voldoen. Helpt operators van "ik zie een afwijking" naar "ik

  verbeter systematisch" te gaan.'
source_centrality: 0.7
source_ref: ASQ DMAIC definitie; Six Sigma classics; Pyzdek 'Six Sigma Handbook'
status: validated
updated_at: '2026-05-20'
correlation_id: ronde21-lo-spc-402
---

# DMAIC — vijf-stappen verbeterroute voor bestaande processen

## De vijf fases

| Fase | Centrale vraag | Typische tools | Operator/teamleider-relevantie |
|------|----------------|----------------|--------------------------------|
| **Define** | Wat is het probleem en waarom is het belangrijk? | SIPOC, projectcharter, klachtdefinitie | Begrijpen wat "goede output" betekent |
| **Measure** | Wat is de huidige prestatie? | SPC-baseline, Gage R&R, defectdefinities | Correct meten en uitgangssituatie vastleggen |
| **Analyze** | Waardoor ontstaat het probleem? | Visgraat, Pareto, 5x waarom, hypothesetoetsen | Oorzaken zichtbaar maken in plaats van gokken |
| **Improve** | Welke verandering lost het op? | DOE, pilots, parameterinstelling, standaardwerk | Verandering gecontroleerd testen |
| **Control** | Hoe borgen we de winst? | Control plan, SPC, visuele standaarden, escalatie | Verbetering vasthouden in dagelijkse routine |

## Waarom deze structuur?
Zonder DMAIC vervalt verbetering vaak in:
- **Snelle aannames** ("het zal wel de operator zijn")
- **Symptoombestrijding** zonder oorzaakanalyse
- **Verbeteringen die niet beklijven** ("we hadden het opgelost…")

DMAIC dwingt: eerst meten, dan analyseren, dan veranderen, dan borgen.

## Operator-rol per fase
| Fase | Wat doet de operator? |
|------|------------------------|
| Define | Bijdragen aan probleemdefinitie vanuit ervaring |
| Measure | Eerlijke baseline-metingen aanleveren |
| Analyze | Met team patronen herkennen, hypothesen genereren |
| Improve | Pilots uitvoeren, varianten testen |
| Control | SPC-kaart bijhouden, signalen rapporteren, standaardwerk volgen |

## Teamleider-rol per fase
| Fase | Wat doet de teamleider? |
|------|--------------------------|
| Define | SIPOC-sessie faciliteren, charter opstellen |
| Measure | Meetplan opzetten, Gage R&R organiseren |
| Analyze | Visgraat / 5-Why sessies leiden, data-analyse |
| Improve | DOE-experimenten coördineren, change management |
| Control | Control plan opstellen, SPC-systeem inrichten, audits |

## Verschil met andere methoden
- **PDCA** (Plan-Do-Check-Act) van Deming: lichtere cyclus,
  algemener toepasbaar
- **DMADV**: voor ontwerp van **nieuwe** processen (Design For Six
  Sigma) — DMAIC is voor **bestaande** processen


## Praktijkvoorbeeld

*Fictief DMAIC-rekenvoorbeeld — plausibele cijfers gebaseerd op typische spuitgiet-afkeur, niet op één specifieke casus.*

Een spuitgietlijn heeft chronisch 1,2% afkeur door dimensionale
afwijkingen. Het verbeterteam doorloopt DMAIC:

- **D**: Charter opgesteld — afkeur naar < 0,3% in 3 maanden, met
  bedrijfscase van €40.000 besparing
- **M**: Baseline gemeten via SPC-kaart, Gage R&R laat zien dat
  meetsysteem 18% van variatie verklaart (te hoog)
- **A**: Visgraat onthult drie hoofdoorzaken: matrijskoeling,
  materiaalvocht, instelling restdruk
- **I**: DOE met 8 runs leidt tot nieuwe parameter-set, pilot
  bevestigt 0,4% afkeur
- **C**: Control plan met SPC-bewaking op de drie kritische
  parameters, operator-werkinstructies, maandelijkse audits

Resultaat: 0,28% afkeur na 4 maanden, structureel geborgd via
SPC-kaarten.
