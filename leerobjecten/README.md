# Leerobjecten

> Kennisobject + didactische schil. Elk leerobject bestaat in drie versies:
> `trainee.md` voor de deelnemer, `trainer.md` als compacte één-A4 voor de
> begeleider, en `developer.md` voor learning designers die het materiaal
> aanpassen.

## Structuur per leerobject

```
lo-<slug>-<NNN>/
├── README.md            # LO-overzicht: wat, voor wie, status, links
├── trainee.md           # de B1-NL deelnemerstekst
├── trainer.md           # compacte één-A4 trainer-samenvatting
├── draaiboek.md         # timing per blok, instructies, valkuilen, differentiatie
├── developer.md         # bronbestanden, metadata, aanpassingsinstructies
├── werkbladen/          # printbare werkbladen per Kolb-fase
├── svg/                 # didactische SVG-diagrammen
├── slidev/              # Slidev-presentatiebronnen (pre-build komt later)
└── interactive/         # React-modellen (pre-build komt later)
```

## Frontmatter-conventie

Elk versie-bestand (trainee/trainer/developer) begint met YAML-frontmatter
conform
[`templates/showcase/frontmatter.md`](https://github.com/BronzGreen/aimm/blob/main/templates/showcase/frontmatter.md)
in de hoofdrepo. Belangrijke velden voor reviewers:

- `id` — uniek LO-id per versie (bijv. `lo-pred-maint-001-trainee`)
- `knowledge_object_id` — verwijzing naar onderliggend KO, singular, geen versie-pinning (ADR-040 #5)
- `version` — `trainee` / `trainer` / `developer`
- `target_audience` — `operator` / `teamleider` / `learning_designer`
- `content_level` — `MBO-3` / `MBO-4` / `HBO`
- `language_level` — `B1` / `B2`
- `bloom_level` — leerdoel-niveau
- `kolb_start_phase` — startpunt in de leercyclus
- `guidance_style` — `instrueren` / `trainen` / `coachen` / `mentoren`
- `status` — alleen `validated` verschijnt in deze repo (ADR-040 #4)

## Interactieve componenten

GitHub rendert Markdown, SVG en Mermaid native. **Slidev-presentaties en
JSX-modellen worden als bronbestanden meegeleverd** — interactieve previews
komen in een latere fase via pre-build artefacten. Verwacht in een LO-README
een tabel:

```
## Interactieve componenten

| Bestand | Type | Status |
|---|---|---|
| slidev/intro.md     | Slidev-presentatie | Bron — pre-build later |
| interactive/quiz.jsx | React-widget       | Bron — pre-build later |
```

## Index

(Auto-gegenereerd door `aimm publish`.)

| ID | Title | Audience | Niveau | Updated |
|---|---|---|---|---|
| _(nog geen artefacten — Sprint 1 tracer)_ | | | | |

## Teruggetrokken leerobjecten

Zie [`RETRACTED.md`](./RETRACTED.md) voor LO's die uit publicatie zijn gehaald.
