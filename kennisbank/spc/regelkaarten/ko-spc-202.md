---
id: ko-spc-202
title: Gevoeligheid versus vals alarm — de afweging bij meer signaalregels
type: concept_uitleg
domain: spc
subdomain: regelkaarten
summary: 'Meer signaalregels = meer gevoeligheid voor echte verstoringen, maar

  ook meer vals alarm. Bij kale Shewhart: 1 vals alarm per ~371 punten.

  Met WECO-uitbreiding: ~1 per 91,75 punten (Champ & Woodall 1987).

  Operator mag niet verdrinken in statistische schijnprecisie.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Handbook; Champ & Woodall (1987) Technometrics; Minitab
  documentation
status: validated
updated_at: '2026-05-20'
correlation_id: ronde15-lo-spc-202
---

# Gevoeligheid versus vals alarm — de afweging bij meer signaalregels

## De fundamentele afweging
Elke extra signaalregel verhoogt de **gevoeligheid** (sneller echte
verstoringen detecteren) maar verhoogt ook het **vals alarm-risico**
(alarm krijgen waar geen echt probleem is).

## Cijfers (ARL — Average Run Length)
Bij een proces dat in werkelijkheid stabiel is:

| Configuratie | Gemiddeld vals alarm |
|--------------|----------------------|
| Kale Shewhart-regel (alleen punt buiten ±3σ) | Eens per ~371 punten |
| + Klassieke WECO-uitbreiding (4 regels) | Eens per ~91,75 punten |
| + Volledige Nelson-set (8 regels) | Aanzienlijk frequenter |

De ARL=91,75 voor WECO is berekend door Champ & Woodall (1987), niet
origineel uit NIST. Dit gegeven verschijnt vaak zonder bron — let op
bij citeren.

## Gevolg voor operator-training
Operators moeten leren signalen herkennen, maar ze mogen niet
**verdrinken in statistische schijnprecisie**. Te veel regels =
alarm-fatigue → operators negeren ook echte signalen.

## Didactisch antwoord: gefaseerde aanpak
- **Module 1 (Gebruik)**: alleen regel 1 + 2 — basisstabiliteit
- **Module 2 (Train)**: regels 3-6 — trend en mixsignalen
- **Module 3 (Op Maat)**: regels 7-8 — diagnostische verdieping
  (alleen bij goed begrip van subgroepering)

Minitab pleit in dezelfde geest voor **beperkte inzet van tests**:
detectiekracht verhogen zonder operator te overladen.

## Operator-implicatie
Een vals alarm = een **echte stopzetting van de productie**. Vals
alarm is dus geen "kostenloze ruis" — het is verloren productietijd
en mogelijk verloren vertrouwen in de kaart.


## Praktijkvoorbeeld

Een lijn die 8 uur per dag draait, meet elke 5 minuten. Dat zijn 96
punten per dag. Met kale Shewhart: ~1 vals alarm per 4 dagen. Met
WECO: ~1 per dag. Met volledige Nelson: meerdere per dag.

Voor operators die alarm-vermoeidheid hebben (en daardoor signalen
gaan negeren), is een beperktere regelset effectiever dan een
gevoelige regelset die ze niet meer serieus nemen.
