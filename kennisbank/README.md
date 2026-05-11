# Kennisbank

> De inhoudelijke laag (WAT) — atomaire concepten van 1-3 minuten. Doelgroep-
> agnostisch (ADR-037): een kennisobject beschrijft een concept zoals het in
> de bron staat, niet voor wie het bedoeld is. Doelgroep-binding gebeurt pas
> in het leerobject (zie [`../leerobjecten/`](../leerobjecten/)).

## Indeling op domein

Kennisobjecten zijn geordend op inhoudelijk domein en subdomein. Zie
[`docs/taxonomy.md`](https://github.com/BronzGreen/aimm/blob/main/docs/taxonomy.md)
in de hoofdrepo voor de volledige taxonomie.

| Domein | Beschrijving |
|---|---|
| `ai_fundamentals/` | AI-basis: ML, supervised/unsupervised, neural networks, evaluatiemetrics |
| `data_literacy/` | Datageletterdheid: statistiek-basis, data-kwaliteit, visualisatie, interpretatie |
| `industry_4_0/` | Industrie 4.0: connected manufacturing, digital twin, IoT, cyber-physical systems |
| `smart_manufacturing/` | Smart manufacturing-praktijken: predictive maintenance, AI vision, optimalisatie |
| `spc/` | Statistical Process Control: control charts, variatie, Six Sigma |
| `oee/` | Overall Equipment Effectiveness: beschikbaarheid, prestatie, kwaliteit |

(Folders worden automatisch aangemaakt door `aimm publish` bij eerste
publicatie binnen een domein.)

## Frontmatter-conventie

Elk KO-bestand begint met YAML-frontmatter conform
[`templates/showcase/frontmatter.md`](https://github.com/BronzGreen/aimm/blob/main/templates/showcase/frontmatter.md)
in de hoofdrepo. Belangrijke velden voor reviewers:

- `id` — uniek KO-id (bijv. `ko-pred-maint-001`)
- `domain` / `subdomain` — classificatie
- `summary` — kernboodschap in 1-2 zinnen
- `source_centrality` — 0.0-1.0, hoe centraal het concept in de bron staat (ADR-037, agnostisch)
- `source_ref` — bronverwijzing
- `status` — alleen `validated` verschijnt in deze repo (ADR-040 #4)
- `updated_at` — datum van laatste validatie
- `correlation_id` — pipeline-run die dit KO produceerde (traceability)

## Index

(Auto-gegenereerd door `aimm publish` — herschrijft deze tabel met
`id | title | domain | subdomain | updated_at` per KO.)

| ID | Title | Domain | Subdomain | Updated |
|---|---|---|---|---|
| [`ko-data-lit-101`](./data_literacy/data_begrippen/ko-data-lit-101.md) | Wat is data? Voorbeelden van je eigen werkvloer | `data_literacy` | `data_begrippen` | 2026-05-11 |

## Teruggetrokken kennisobjecten

Zie [`RETRACTED.md`](./RETRACTED.md) voor KO's die uit publicatie zijn
gehaald (tombstone-conventie, ADR-040 #6).
