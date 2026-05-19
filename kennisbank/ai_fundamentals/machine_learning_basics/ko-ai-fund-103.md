---
id: ko-ai-fund-103
title: Onzekerheid en kansrekening in AI
type: concept_uitleg
domain: ai_fundamentals
subdomain: machine_learning_basics
summary: AI-systemen werken bijna altijd met onzekere informatie. Kansrekening is
  de wiskundige basis waarmee AI-systemen omgaan met die onzekerheid en toch goede
  beslissingen nemen.
source_centrality: 0.7
source_ref: Russell & Norvig (2010). AI - A Modern Approach, 3rd ed., pp. 8-9
status: validated
updated_at: '2026-05-19'
correlation_id: ronde7-lo-ai-fund-103
---

# Onzekerheid en kansrekening in AI

See Markdown file

## Praktijkvoorbeeld

*Fictieve illustratie van het concept uit Russell & Norvig 2010, AI — A Modern Approach, 3rd ed., pp. 8-9. Percentages zijn pedagogisch.*

Een AI-systeem voor kwaliteitscontrole op een productielijn krijgt camerabeelden van elk product. Het systeem zegt niet "dit product is 100% fout", maar "er is 87% kans dat dit product een defect heeft." De operator ziet dit percentage en kan beslissen of het product handmatig gecontroleerd moet worden. Bij 87% kans is dat verstandig. Bij 15% kans misschien niet. De kans helpt de operator om een goede beslissing te nemen.