# CHANGELOG

> Auto-gegenereerd door `aimm publish`. Elke publish-run voegt een sectie
> bovenaan toe met een kontext-regel + per-artefact bullets.
> Conform ADR-040 #7 is een kontext-regel verplicht bij runs met meer dan
> één wijziging — automatische runs worden later (indien ingevoerd) gemarkeerd
> als "Automatische publish".

---

## 2026-05-12 — publish-2026-05-12-first-adapter-run

**Kontext:** Eerste publicatie via `aimm publish` (ShowcaseRepoAdapter,
Sprint 2 stappen 3 + 3.5 in de hoofdrepo). Vervangt hand-crafted Sprint 1
tracer-content met auto-gegenereerde output. Bevestigt dat het end-to-end
flow werkt: gevalideerde KO+LO in AIMM → adapter met platte frontmatter +
enrichments → showcase-repo.

Gewijzigd:

- `lo-data-lit-101/trainee.md` — inline SVG na H1, Werkbladen-footer met
  links per Kolb-fase, Verder-sectie met links naar KO + trainer + interactief
  model. Frontmatter platgeslagen (showcase-subset van Pydantic-schema).
- `lo-data-lit-101/trainer.md` — path-rewrites (`./draaiboek.md`,
  `./slidev/presentatie.slidev.md`, `./trainee.md`); kleine YAML-formatting-
  verschillen.
- `lo-data-lit-101/README.md` — geregenereerd met auto-LO-overview vanuit
  pipeline-yamls.
- `ko-data-lit-101.md` — frontmatter platgeslagen (id/title/type/domain/
  subdomain/summary/source_centrality/source_ref/status/updated_at).

Warning gerapporteerd door adapter: `trainer.yaml` heeft
`target_audience: trainer` — niet schema-conform; gecorrigeerd naar
`operator` in showcase-frontmatter (zie [issue #53](https://github.com/BronzGreen/aimm/issues/53)).

---

## 2026-05-12 — sprint-1-tracer-lo-data-lit-101

**Kontext:** Sprint 1 tracer-bullet voor ADR-040 — eerste volledig gepubliceerde
LO inclusief onderliggend KO. Handmatige conversie van pipeline-output naar
showcase-frontmatter; valideert de lees-ervaring voordat de ShowcaseRepoAdapter
in Sprint 2 wordt gebouwd.

Toegevoegd:

- **KO** `ko-data-lit-101` "Wat is data? Voorbeelden van je eigen werkvloer"
  (gevalideerd door Jim Bemelen, 2026-05-11) — eerste KO in `data_literacy/data_begrippen/`
- **LO** `lo-data-lit-101` (gevalideerd) met:
  - `trainee.md` (B1, MBO-3 operator, 35 min)
  - `trainer.md` (B2 één-A4)
  - `draaiboek.md` (timing per blok)
  - 4 werkbladen — volledige Kolb-cyclus
  - SVG-diagram (vier datasoorten)
  - Slidev-bron (`slidev/presentatie.slidev.md`)
  - Standalone HTML interactief model (`interactive/model.html`)

Bevindingen voor Sprint 2/3:

- Legacy KO mist `source_centrality`-veld (ADR-037-introductie was later) — backfill nodig in adapter
- `developer.yaml` heeft afwijkende structuur (`design_decisions` + `versioning` ipv `metadata.status`) — schema-divergentie, ongeschikt voor showcase tot besluit gemaakt
- Trainer-yaml gebruikt `target_audience: trainer` in plaats van `operator` met `version: trainer` — schema-niet-conform

---

## 2026-05-11 — initial-skeleton

**Kontext:** Initiële repo-setup voor Sprint 1 tracer-bullet (ADR-040). Nog
geen gepubliceerde artefacten — folder-skeleton, README-templates en
CHANGELOG-stub handmatig aangemaakt.

Toegevoegd:

- Root `README.md` met leeswijzer, status-disclaimer en feedback-uitleg
- `kennisbank/README.md` als index-stub
- `leerobjecten/README.md` als index-stub
- `modules/README.md` als index-stub
- `kennisbank/RETRACTED.md` en `leerobjecten/RETRACTED.md` als tombstone-indexen
- `.gitignore`
