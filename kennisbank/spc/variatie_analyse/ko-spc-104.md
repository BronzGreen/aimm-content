---
id: ko-spc-104
title: Common cause vs special cause variatie — de didactische spil van SPC
type: concept_uitleg
domain: spc
subdomain: variatie_analyse
summary: 'Common cause = systeemvariatie, het normale gedrag van een proces.

  Special cause = uitzonderlijke invloeden die het gewone gedrag

  tijdelijk verstoren. Operators moeten dit verschil kunnen herkennen

  voordat ze ingrijpen.'
source_centrality: 0.7
source_ref: Deming 'Out of the Crisis' (1986); Wheeler 'Understanding Variation' (1993)
status: validated
updated_at: '2026-05-19'
correlation_id: ronde4-lo-spc-104
---

# Common cause vs special cause variatie — de didactische spil van SPC

## Het Deming-onderscheid

Deming maakte in *Out of the Crisis* (1986) het onderscheid centraal:
- **Common causes** zitten **in het systeem zelf** — kleine
  temperatuurschommelingen, materiaalvariatie, normale slijtage,
  meetruis
- **Special causes** zijn **uitzonderlijke invloeden** die het
  gewone gedrag tijdelijk verstoren — defecte sensor, verkeerde
  materiaalbatch, fout gereedschap, verstopte nozzle

Wheeler heeft dit later toegankelijk uitgewerkt voor dagelijkse
kwaliteitspraktijk.

## Voor operators: praktische vertaling

| Common cause = | Special cause = |
|----------------|-----------------|
| Lijn schommelt binnen normale patroon | Er is iets ánders gebeurd dan normaal |
| Kleine temperatuurschommeling | Verkeerde materiaalbatch geladen |
| Minieme materiaalvariatie | Vastlopend thermokoppel |
| Normale slijtage | Verstopte nozzle |
| Normale meetruis | Verkeerd gereedschap gemonteerd |

## Hoe je ze herkent in de data

| Common cause | Special cause |
|--------------|----------------|
| Willekeurige spreiding rond centrumlijn | Sprong, trend, cluster, oscillatie |
| Geen onwaarschijnlijke patronen | Lange reeks aan één kant, punt buiten grenzen |

## Waarom geen losse meetwaarde beoordelen
Eén onderdeel op 100,02 g zegt weinig. Tien opeenvolgende punten die
omhoog kruipen op een spuitgietlijn zegt veel meer. **SPC beoordeelt
tijdreeksen, geen losse waardes.**


## Praktijkvoorbeeld

Bij een spuitgietlijn beweegt onderdeelgewicht door de dag heen tussen
99,8 en 100,2 gram door buitentemperatuur en koelwater. Dat is common
cause — laat dat met rust.

Maar als gewicht plotseling drie meetcycli achtereen op 100,5 gram
uitkomt na een matrijswissel, is dat special cause. Onderzoek de
matrijsinstelling.
