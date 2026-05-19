---
id: ko-spc-105
title: Tampering — waarom ingrijpen op common cause variatie het proces slechter maakt
type: tip
domain: spc
subdomain: variatie_analyse
summary: 'Tampering is overreageren op common cause variatie alsof het een

  special cause is. Demings funnel experiment toont dat dit de

  spreiding juist vergroot. ''Niet elke afwijking corrigeren'' is geen

  luiheid — het is statistische discipline.'
source_centrality: 0.7
source_ref: Deming Institute Funnel Experiment; Joiner; Wheeler
status: validated
updated_at: '2026-05-19'
correlation_id: ronde6-lo-spc-105
---

# Tampering — waarom ingrijpen op common cause variatie het proces slechter maakt

## Wat tampering is
Tampering = ingrijpen op normale variatie alsof het een echt signaal
is. Een operator die na elke meting 'corrigeert' duwt het proces
heen-en-weer en vergroot de spreiding.

## Het funnel experiment van Deming
Deming demonstreerde dit met een trechter en een doel op tafel.
Vier strategieën:
1. **Niets doen** — beste resultaat (laagste spreiding)
2. **Compenseren naar doel** — verdubbelt de spreiding
3. **Compenseren naar laatste punt** — exponentieel afdrijven
4. **Compenseren naar laatste meting** — random walk

Strategie 1 (niets doen) wint altijd zolang het proces stabiel is
(alleen common cause). Het Deming Institute beschrijft het experiment
expliciet als illustratie van schadelijke effecten van aanpassingen
zonder eerst de werkelijke oorzaak te begrijpen.

Joiner vat het kernachtig samen: **overreageren verhoogt variatie
én kosten**.

## De operator-regel
'Niet elke afwijking corrigeren' is geen luiheid. Het is statistische
discipline. Wacht op een **signaal** voor je ingrijpt:
- Punt buiten de grenzen
- Een Nelson-patroon (zie ko-spc-201)
- Een trend over meerdere metingen

Reageer NIET op:
- Eén losse meting die toevallig hoog is
- Variatie binnen de normale bandbreedte
- Onderbuikgevoel zonder data

## Wat dan wel doen bij common cause?
Als de variatie te groot is voor wat het proces aankan: dat is een
**systeemverbetering**, geen operator-aanpassing. Escaleren naar
teamleider of engineering.


## Praktijkvoorbeeld

Een operator op een verpakkingslijn ziet vulgewicht 502g (specs:
500 ± 5g). Hij draait de pomp 0,2g terug. Volgende meting: 498g.
Hij draait 0,4g op. Volgende: 503g. Na een uur is de spreiding
verdubbeld door zijn 'correcties'.

Wat hij had moeten doen: niets. De waardes zaten ruim binnen specs
en binnen normale variatie.
