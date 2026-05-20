---
id: ko-spc-301
title: Cp en Cpk — wat ze zeggen over potentieel versus werkelijke prestatie
type: concept_uitleg
domain: spc
subdomain: procesbekwaamheid
summary: 'Cp = (USL−LSL)/6σ vertelt of de spreiding **smal genoeg** is.

  Cpk = min[(USL−μ)/3σ, (μ−LSL)/3σ] vertelt of die smalle spreiding

  ook **goed in het tolerantievak ligt**. Een proces kan goede Cp

  hebben en lage Cpk: gecentreerd zit het scheef.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Engineering Statistics Handbook; ASQ; Ford PPAP 4th ed.;
  Minitab documentation
status: validated
updated_at: '2026-05-20'
correlation_id: ronde18-lo-spc-301
---

# Cp en Cpk — wat ze zeggen over potentieel versus werkelijke prestatie

## De twee indices

| Index | Formule | Wat zegt het? |
|-------|---------|---------------|
| **Cp** | (USL − LSL) / 6σ | Is de spreiding smal genoeg ten opzichte van de tolerantie? (Potentieel) |
| **Cpk** | min[(USL−μ)/3σ, (μ−LSL)/3σ] | Past die spreiding ook werkelijk in het tolerantievak? (Werkelijke prestatie) |

Waarbij:
- USL = upper specification limit (bovengrens klant)
- LSL = lower specification limit (ondergrens klant)
- σ = procesvariatie (binnen-subgroep)
- μ = procesgemiddelde

## De operator-zin
"Cp vertelt of de spreiding smal genoeg is. Cpk vertelt of die smalle
spreiding ook **goed in het tolerantievak ligt**."

Een proces kan dus een aardige Cp hebben (smal genoeg) en toch een
lage Cpk (te dicht tegen één van de tolerantiegrenzen).

## Interpretatietabel (industriële vuistregels)

| Cp/Cpk | Interpretatie |
|--------|---------------|
| **< 1,0** | Niet capabel — afkeur structureel waarschijnlijk |
| **= 1,0** | Theoretisch passend, maar kwetsbaar voor drift en meetonzekerheid |
| **≥ 1,33** | Veelgebruikte industriële ondergrens |
| **≥ 1,67** | Zwaardere automotive of kritische eis (Ford PPAP) |
| **≈ 2,0** | Gecentreerd kortetermijnproces op zes sigma (Cp = 2,0 = 12σ tolerantievak) |

## Voorwaarden voor zinvolle berekening
Capability is alleen zinvol als:
1. Het proces is **stabiel** (eerst SPC-regelkaart valideren)
2. Het meetsysteem is **geschikt** (Gage R&R / MSA voltooid)
3. De **verdelingsaanname** is redelijk (vaak normaal)
4. De data zijn **representatief**

Ford eist expliciet: MSA vóór capability study. NIST en Minitab
benadrukken: eerst stabiliteit, dan normaliteit, dan capability.

## Drie veelgemaakte fouten
1. **Capability op instabiel proces** → één mooi getal over data
   uit meerdere toestanden
2. **Slechte subgroepering** → kortetermijn- en langetermijnvariatie
   door elkaar
3. **Slecht meetsysteem** → Cpk zegt evenveel over de meter als
   over de machine


## Praktijkvoorbeeld

Spuitgietlijn: onderdeelgewicht moet tussen 99,5 g en 100,5 g liggen
(USL=100,5, LSL=99,5). Stabiele lijn: gemiddeld 99,9 g, σ=0,12 g.

**Cp** = (100,5 − 99,5) / (6 × 0,12) = 1,00 / 0,72 ≈ **1,39**
→ de spreiding lijkt in potentie goed.

**Cpk** = min[(100,5 − 99,9)/0,36 ; (99,9 − 99,5)/0,36]
       = min[1,67 ; 1,11] = **1,11**
→ de pers staat te dicht tegen de **ondertolerantie** aan.

**De operatorles:** de pers schiet niet "te wijd", maar staat scheef.
De juiste actie is **centreren** (procesgemiddelde naar 100,0
brengen), niet harder proberen de spreiding te verkleinen.
