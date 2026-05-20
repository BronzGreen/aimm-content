---
id: ko-smart-mfg-521
title: 'Jouw kwaliteitsprobleem kiezen: waar kost afkeur het meest?'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Voordat je AI-inspectie implementeert, moet je het juiste probleem kiezen.
  Analyseer je afkeurdata, bereken de kosten per defecttype, en prioriteer het probleem
  waar AI het meeste oplevert.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-420
status: validated
updated_at: '2026-05-20'
correlation_id: ronde24-lo-smart-mfg-521
---

# Jouw kwaliteitsprobleem kiezen: waar kost afkeur het meest?

AI-inspectie werkt het best als je het op het **juiste probleem** richt. Niet elk defect is even geschikt voor een camera-systeem, en niet elk defect kost evenveel. Begin daarom met een analyse: waar zit het meeste geld?

## Stap 1: Verzamel je afkeurdata

Pak de afkeurregistratie van de afgelopen 3 maanden. Kijk naar:

- **Welke defecttypes** komen voor? (krassen, deuken, kleurafwijkingen, maatafwijkingen, ontbrekende onderdelen)
- **Hoe vaak** komt elk type voor? (afkeurpercentage per product)
- **Hoeveel kost** elk afgekeurd product? (materiaal + arbeid + verloren productietijd)

## Stap 2: Bereken de totale kosten per defecttype

Gebruik deze formule:

**Totale kosten = afkeurpercentage x aantal producten per maand x kosten per afgekeurd stuk**

*Tabel hieronder: fictief rekenvoorbeeld ter illustratie — vul zelf in met je eigen afkeurcijfers.*

| Defecttype | Afkeur% | Productie/maand | Kosten/stuk | Totale kosten/maand |
|---|---|---|---|---|
| Krassen | 4% | 5.000 | EUR 12 | EUR 2.400 |
| Deuken | 2% | 5.000 | EUR 45 | EUR 4.500 |
| Maatafwijking | 1% | 5.000 | EUR 80 | EUR 4.000 |

In dit voorbeeld zijn **deuken** het duurst, ook al komen ze minder vaak voor dan krassen.

## Stap 3: Beoordeel de geschiktheid voor AI-inspectie

Niet elk defect is even makkelijk te detecteren met een camera. Beoordeel per defecttype:

| Vraag | Goed geschikt | Minder geschikt |
|---|---|---|
| Is het defect **zichtbaar** op een foto? | Krassen, deuken, kleurafwijkingen | Interne scheuren, gewichtsverschillen |
| Is het defect **consistent herkenbaar**? | Duidelijke krassen | Subtiele kleurvariaties |
| Kun je het defect **goed fotograferen**? | Oppervlaktedefecten | Defecten in holle ruimtes |

## Stap 4: Prioriteer

Combineer de twee analyses:

1. **Hoge kosten + goed geschikt** = start hier met je AI-pilot
2. **Hoge kosten + minder geschikt** = onderzoek of betere camera-opstelling helpt
3. **Lage kosten + goed geschikt** = eventueel later toevoegen
4. **Lage kosten + minder geschikt** = niet doen

## Praktijkvoorbeeld

*Fictieve illustratie — plausibele cijfers voor een MKB-metaalbedrijf, niet een specifieke casus.*

Bij een fabrikant van metalen onderdelen analyseert een operator de afkeurregistratie. Deuken kosten het meest (EUR 4.500/maand) en zijn visueel goed herkenbaar. Hij kiest deuken als eerste AI-pilot. Krassen volgen later als het systeem eenmaal draait.
