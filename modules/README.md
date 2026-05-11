# Modules

> Complete modules van ~4 uur volgens het 3-staps progressiemodel:
> **gebruik → train → op_maat**. Elke module combineert pre-workshop
> leerobjecten, een hands-on workshop (Shared Learning Team-format), en
> post-workshop verwerking inclusief assessment en badge-criteria.

## Het 3-staps progressiemodel

Elke AI use-case in de maakindustrie volgt hetzelfde patroon:

| Stap | Context | Data | Activiteit | Uitkomst |
|---|---|---|---|---|
| `gebruik` | voorbeeld | voorbeeld | demonstratie, leren gebruiken | "Snappen wat er mogelijk is" |
| `train` | voorbeeld | voorbeeld | zelf configureren, model trainen, interpreteren | "Ervaren wat het potentieel is" |
| `op_maat` | eigen | eigen | eigen productiedata, eigen model, business case | "AI-winst voor jouw organisatie verzilveren" |

## Structuur per module

```
module-<slug>-<step>-<NNN>/
├── README.md            # module-overzicht (recipe, leerbijeenkomsten, competenties)
└── leerbijeenkomst-*.md # uitwerking per leerbijeenkomst (hands-on sessie)
```

Module-README's bevatten frontmatter conform
[`templates/showcase/frontmatter.md`](https://github.com/BronzGreen/aimm/blob/main/templates/showcase/frontmatter.md):

- `id` — `module-<slug>-<step>-<NNN>`
- `use_case` — verwijzing naar de use-case
- `progression_step` — `gebruik` / `train` / `op_maat`
- `duration_hours` — typisch 4
- `target_audience`, `content_level` — voor wie deze module is
- `learning_objects` — lijst van LO-id's in de module
- `status` — alleen `validated` verschijnt (ADR-040 #4)

## Index

(Auto-gegenereerd door `aimm publish`.)

| ID | Title | Step | Audience | Duur | Updated |
|---|---|---|---|---|---|
| _(nog geen artefacten — Sprint 1 tracer)_ | | | | | |
