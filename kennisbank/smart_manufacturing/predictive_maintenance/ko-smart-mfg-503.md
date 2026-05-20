---
id: ko-smart-mfg-503
title: Een business case maken voor predictive maintenance
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een template om de kosten van de huidige situatie te vergelijken met de verwachte
  besparing door predictive maintenance, inclusief ROI-berekening en terugverdientijd.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1 + Mobley (2002) Ch. 12
status: validated
updated_at: '2026-05-20'
correlation_id: ronde22-lo-smart-mfg-503
---

# Een business case maken voor predictive maintenance

Je weet nu welke machine je wilt aanpakken en welke data je hebt. Maar voordat je begint, moet je laten zien dat het de investering waard is. Een goede business case overtuigt je leidinggevende, de technische dienst en het management.

### De huidige situatie: wat kost het nu?

Bereken de kosten van ongeplande stilstand voor je gekozen machine:

| Kostenpost | Berekening | Per jaar |
|-----------|-----------|---------|
| Verloren productie | uren stilstand x producten per uur x marge | EUR ... |
| Arbeid monteurs | uren x uurtarief | EUR ... |
| Spoedonderdelen | aantal x meerprijs | EUR ... |
| Gevolgkosten | vertragingen, boetes, klantverlies | EUR ... |
| **Totaal huidig** | | **EUR ...** |

### De investering: wat kost predictive maintenance?

| Investering | Eenmalig | Per jaar |
|-----------|---------|---------|
| Sensoren (indien nodig) | EUR 200-2.000 | - |
| Installatie + aansluiting | EUR 500-2.000 | - |
| Software/platform | - | EUR 500-3.000 |
| Opleiding (deze modules) | inbegrepen | - |
| Onderhoud sensoren | - | EUR 200-500 |
| **Totaal investering** | **EUR ...** | **EUR ...** |

### De verwachte besparing

- Reductie ongeplande stilstand: **50-70%** *(bron: Mobley, R.K. (2002). An Introduction to Predictive Maintenance, hoofdstukken 8-9 — klassieke PM-referentie)*. Reken conservatief met 50%.
- Besparing per jaar = totaal huidig x 50%
- Extra besparing: minder preventief onderhoud (alleen vervangen wat nodig is)

### ROI en terugverdientijd

**ROI** = (besparing per jaar - kosten per jaar) / eenmalige investering x 100%

**Terugverdientijd** = eenmalige investering / (besparing per jaar - kosten per jaar)

Vuistregels *(gangbaar in de maakindustrie, te valideren per organisatie)*:
- ROI boven 100% in het eerste jaar = sterke business case
- Terugverdientijd onder 12 maanden = makkelijk goedgekeurd
- Begin klein (1 machine) en bewijs de resultaten

### Tips voor een overtuigende presentatie

- Gebruik echte cijfers van je eigen machine, geen schattingen
- Laat de storingsregistratie zien — feiten overtuigen meer dan beloftes
- Benoem ook niet-financiele voordelen: veiliger werken, minder stress, hogere kwaliteit
- Stel voor om het als pilot te doen: laag risico, snel resultaat


## Praktijkvoorbeeld

*Fictief rekenvoorbeeld ter illustratie — gebaseerd op gangbare kostenstructuren, niet op een specifieke casus.*

Een teamleider bij een kunststofverwerker maakte de volgende business case voor een spuitgietmachine. Huidige kosten ongeplande stilstand: EUR 24.000 per jaar (48 uur x EUR 500/uur). Investering: EUR 1.800 eenmalig (2 sensoren + installatie) en EUR 1.200 per jaar (platform + onderhoud). Verwachte besparing: EUR 12.000 per jaar (50% reductie). ROI: (12.000 - 1.200) / 1.800 = 600%. Terugverdientijd: 1.800 / (12.000 - 1.200) = 2 maanden. De business case werd dezelfde week goedgekeurd. Na 8 maanden bleek de reductie zelfs 62%, waardoor de werkelijke besparing EUR 14.880 was.
