# AIMM Content — Showcase

> Private content-repo voor het AIMM-kernteam. Hier vind je de doorklikbare
> tussenresultaten van de AIMM × BronzGreen curriculum-pipeline: kennisobjecten,
> leerobjecten in drie versies, en complete modules.

## Wat hier staat

| Map | Inhoud |
|---|---|
| [`kennisbank/`](./kennisbank/) | Kennisobjecten — de inhoudelijke laag (WAT), geordend op domein en subdomein |
| [`leerobjecten/`](./leerobjecten/) | Leerobjecten in drie versies per LO: `trainee.md`, `trainer.md`, `developer.md` + werkbladen, SVG's, Slidev-bronnen, interactieve modellen |
| [`modules/`](./modules/) | Complete modules van ~4 uur — 3-staps progressiemodel (gebruik / train / op_maat) |
| [`CHANGELOG.md`](./CHANGELOG.md) | Auto-gegenereerd publicatie-logboek per `aimm publish`-run |

## Wat hier **niet** staat

Code, prompts, configuratie, tests, pipeline-tussenresultaten (bronkaarten,
classificaties). Die leven in de hoofdrepo `BronzGreen/aimm` en zijn niet
relevant voor kernteam-review op deze laag.

## Status van dit materiaal

Alles in deze repo is door de AIMM-pipeline geproduceerd en door de
Landelijke Learning Lead **inhoudelijk en didactisch gevalideerd**. Wat je
hier vindt is:

- **Geschikt voor:** inhoudelijke en didactische feedback, hergebruik van
  concepten en structuur, inspiratie voor eigen materiaal binnen RLC's.
- **Niet geschikt voor:** directe inzet bij studenten of operators zonder
  lokale validatie en aanpassing aan jullie context, doelgroep en werkvloer.

Een gevalideerd leerobject is een **werkende basis, geen klaar product**.
Lokale didactici weten beter dan wij wat past bij hun deelnemers — gebruik
dit materiaal als startpunt, niet als eindpunt.

## Feedback geven

Feedback loopt via **GitHub Discussions** op deze repo. Vier categorieën:

- **LO-feedback** — opmerkingen over een specifiek leerobject
- **KO-feedback** — opmerkingen over een specifiek kennisobject
- **Module-feedback** — opmerkingen over een module of leerbijeenkomst
- **Algemeen** — procesvragen, vragen over deze repo

Titel-conventie: `LO-001: <titel>` of vergelijkbaar — maakt zoeken later
eenvoudiger.

Voor tikfouten of kleine correcties: gebruik de ✏️ "Edit"-knop op een
bestand om direct een suggestie te openen op de hoofdrepo.

## Hoe is dit gegenereerd

Door `aimm publish` in `BronzGreen/aimm` (ShowcaseRepoAdapter, zie ADR-040).
Deze repo wordt handmatig bijgewerkt na elke validatie-ronde — geen
automatische sync. Wat hier staat is daarmee altijd "wat we staat achter",
niet een log van wat in de pipeline gebeurt.

Render-grenzen op GitHub: Markdown, SVG en Mermaid renderen native.
**Slidev-presentaties en interactieve React-componenten zijn bronbestanden
in deze repo** — interactieve previews komen in een latere fase (pre-builds
voor showcase-context).

## Cadans

| Wanneer | Wie | Wat |
|---|---|---|
| Wekelijks vr 30 min | Landelijke Learning Lead | Triage Discussions + Issues |
| Per validatie-ronde | Landelijke Learning Lead | `aimm publish` draaien in hoofdrepo |
| Maandelijks | Kernteam | Korte review: werkt de showcase-flow? |
