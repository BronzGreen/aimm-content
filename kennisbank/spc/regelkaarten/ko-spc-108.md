---
id: ko-spc-108
title: Zeven regelkaart-types — keuzehulp voor maakindustrie
type: framework
domain: spc
subdomain: regelkaarten
summary: 'Zeven standaard regelkaart-types: X̄-R, X̄-S, I-MR (continue data),

  en p, np, c, u (attribuutdata). Keuze hangt af van datatype,

  subgroepomvang en variabiliteit. Tabel met operator-leesregels en

  maakindustrie-voorbeelden per type.'
source_centrality: 0.7
source_ref: NIST/SEMATECH Engineering Statistics Handbook; ISO 7870-1, 7870-2; ASQ;
  Minitab documentation
status: validated
updated_at: '2026-05-19'
correlation_id: ronde9-lo-spc-108
---

# Zeven regelkaart-types — keuzehulp voor maakindustrie

## De zeven kaart-types

| Regelkaart | Wanneer gebruiken | Hoe gemaakt | Operator leest hem zo | Maakindustrie-voorbeeld |
|-----------|-------------------|-------------|------------------------|---|
| **X̄-R** | Continue metingen, kleine subgroepen 2-8 (typisch 4-5) | Gemiddelde + range per subgroep | Boven: verschuift gemiddelde; onder: stabiele spreiding? | 5 onderdelen per 2 uur wegen op spuitgietlijn |
| **X̄-S** | Continue metingen, grotere subgroepen of meer precisie | Gemiddelde + standaarddeviatie per subgroep | Geschikt als n groter is en range te grof wordt | Diameter/diktemetingen in automatische meetcel |
| **I-MR** | Eén meting per moment of batch | Individuele waarden + moving range | Handig bij batch-, tank-, lotmetingen | Viscositeit per batch in voeding/chemie |
| **p-kaart** | Attribuutdata, **wisselende** steekproefomvang | Percentage defecte stuks | Defectpercentage en patronen in tijd | % lekkende verpakkingen per gecontroleerde steekproef |
| **np-kaart** | Attribuutdata, **vaste** steekproefomvang | Aantal defecte stuks per vaste steekproef | Zelfde logica als p, maar in aantallen | Aantal fout-geassembleerde sets in monsters van 50 |
| **c-kaart** | Tellingen per **gelijke** eenheid | Aantal defecten per vaste eenheid | Meer fouten per object dan normaal? | Aantal krassen per vast plaatoppervlak |
| **u-kaart** | Tellingen per **wisselende** eenheid (oppervlakte/tijd) | Defecten per eenheid of inspectievolume | Defectdichtheid, niet ruwe telling | Aantal fouten per meter folie |

## Twee extra vuistregels

1. **R vs S**: gebruik R-kaarten bij **kleine** subgroepen, S-kaarten
   bij **grotere**. NIST: zodra subgroep groter wordt, wordt S-kaart
   efficiënter dan R-kaart.

2. **I-MR alleen als laatste keuze**: gebruik I-MR pas als
   subgroeperen écht niet kan. Als logische mini-steekproeven mogelijk
   zijn (zelfs n=2), is X̄-R of X̄-S meestal informatiever.

## Beslis-stroom

```
Continue metingen?
  Ja → Subgroep mogelijk?
        Ja → n klein (<=8)? → X̄-R
            n groter? → X̄-S
        Nee → I-MR
  Nee (telling van defecten)?
        Defectpercentage?
          Vaste n → np
          Wisselende n → p
        Defectaantal per eenheid?
          Vaste eenheid → c
          Wisselende eenheid → u
```


## Praktijkvoorbeeld

Vier voorbeelden uit de maakindustrie:

1. Operator weegt elke 2 uur 5 onderdelen op spuitgietlijn → **X̄-R**
2. Productlijn meet elke seconde de diktemeting via lasersensor (n=30
   per minuut) → **X̄-S**
3. Voedselbedrijf meet viscositeit van elke batch (één meting per
   batch) → **I-MR**
4. Verpakkingslijn telt aantal lekkende pakken per uurlijkse steekproef
   van 100 → **np-kaart**
