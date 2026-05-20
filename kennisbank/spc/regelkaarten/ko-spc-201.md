---
id: ko-spc-201
title: De acht Nelson-rules — patronen die signaleren dat het proces is veranderd
type: framework
domain: spc
subdomain: regelkaarten
summary: 'Lloyd Nelson breidde in 1984 de Western Electric-rules uit naar acht

  regels voor patroonherkenning op een Shewhart-kaart. Elk patroon wijst

  op een specifiek type special cause: shift, trend, oscillatie, mixture

  of stratificatie. Voor MBO-onderwijs gefaseerd toepassen.'
source_centrality: 0.7
source_ref: Nelson L.S. (1984) 'The Shewhart Control Chart—Tests for Special Causes'
  Journal of Quality Technology; NIST/SEMATECH Handbook
status: validated
updated_at: '2026-05-20'
correlation_id: ronde14-lo-spc-201
---

# De acht Nelson-rules — patronen die signaleren dat het proces is veranderd

## Waarom meer dan "punt buiten de grenzen"?
Een Shewhart-kaart met alleen de regel "één punt buiten ±3σ" is vaak
te grof. Echte verstoringen verraden zich vaak eerder via patronen
dan via één extreem punt. Lloyd Nelson formaliseerde dit in 1984 in
acht regels — een uitbreiding op de klassieke Western Electric-rules.

## De acht Nelson-rules

| Regel | Patroon | Inhoudelijke betekenis | Wat doet de operator? |
|-------|---------|------------------------|------------------------|
| **1** | 1 punt buiten ±3σ | Sterke aanwijzing voor special cause | Meetfout uitsluiten, laatste proceswijziging checken, verdachte output veiligstellen, teamleider informeren |
| **2** | 9 punten aan één kant van centrumlijn | Procesgemiddelde lijkt verschoven | Kijk naar set-up, gereedschap, offset, grondstofbatch, matrijstemperatuur |
| **3** | 6 punten stijgend of dalend | Trend, vaak slijtage of opwarming | Controleer drift: gereedschapsslijtage, temperatuur, slijpsteen, drukverlies |
| **4** | 14 punten afwisselend op/neer | Systematische oscillatie | Zoek naar twee afwisselende oorzaken: twee operators, twee caviteiten, pulserende regeling |
| **5** | 2 van 3 voorbij ±2σ zelfde kant | Kleine maar serieuze shift | Reageer sneller dan bij regel 2; vroege waarschuwing |
| **6** | 4 van 5 voorbij ±1σ zelfde kant | Nog subtielere shift | Controleer of proces aan het wegdrijven is vóór echte overschrijdingen |
| **7** | 15 punten binnen ±1σ | Verdacht weinig variatie, vaak stratificatie of te brede limieten | Check subgroepering, meetmethode of datastromen; "te mooi" kan fout zijn |
| **8** | 8 punten buiten ±1σ aan beide kanten | Mixture, bronwissel of twee populaties | Zoek naar gemengde bron: twee machines, twee leveranciers, twee recepten |

## Tegenintuïtieve regels 7 en 8
"Weinig spreiding" lijkt gunstig, maar Nelson noemt dit juist
diagnostisch verdacht. Het kan wijzen op **stratificatie** — data die
kunstmatig glad zijn doordat binnen één subgroep van meerdere bronnen
is gemeten. Sterk voorbeeld waarom steekproefstrategie onderdeel is
van proceskennis, geen detail.

## Didactisch gefaseerd toepassen
Niet alle 8 regels tegelijk in operatortraining:

| Fase | Regels | Reden |
|------|--------|-------|
| **Beginner** | 1, 2 | Basisstabiliteit |
| **Gevorderd** | + 3, 4, 5, 6 | Patroonherkenning |
| **Expert** | + 7, 8 | Diagnostische verdieping bij goed begrip subgroepering |

## Onderscheid met Western Electric
WECO is compacter (4 hoofdregels). Nelson is uitgebreider en
didactisch rijker. In automotive wordt vaak pragmatisch gewerkt met
een beperkte set + strikte reaction plans.


## Praktijkvoorbeeld

Op een spuitgietlijn meet de operator gewicht elke 10 minuten. Na
twee uur ziet hij **6 punten stijgend** (regel 3): 99,8 → 99,85 →
99,9 → 99,95 → 100,0 → 100,05 g. Geen enkel punt is buiten de
grenzen. Maar het patroon is duidelijk: een trend.

De operator controleert de matrijskoeling — die blijkt deels verstopt.
De pers liep langzaam warmer en duwde meer materiaal in de matrijs.
Zonder regel 3 had de operator pas bij overschrijding van UCL
(regel 1) ingegrepen — uren later, met afkeur tot gevolg.
