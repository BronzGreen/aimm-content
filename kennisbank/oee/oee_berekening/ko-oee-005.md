---
id: ko-oee-005
title: 'OEE berekenen: een voorbeeld stap voor stap'
type: framework
domain: oee
subdomain: oee_berekening
summary: OEE bereken je door beschikbaarheid, prestatie en kwaliteit te vermenigvuldigen.
  Een uitgewerkt voorbeeld laat zien hoe elk onderdeel het totaal beinvloedt.
source_centrality: 0.7
source_ref: Competentieframework AIMM — SPC & OEE
status: validated
updated_at: '2026-05-19'
correlation_id: ronde6-lo-oee-005
---

# OEE berekenen: een voorbeeld stap voor stap

Laten we OEE stap voor stap berekenen met een concreet voorbeeld.

### De situatie

Een CNC-freesmachine heeft een dienst van 8 uur (480 minuten). Dit is wat er vandaag gebeurde:

- Geplande pauze: 30 minuten (telt niet mee)
- Storing: 25 minuten (hydraulieklek)
- Omstellen: 20 minuten (ander product)
- Ideale cyclustijd: 2 minuten per stuk
- Geproduceerd: 180 stuks
- Afgekeurd: 5 stuks
- Herbewerkt: 4 stuks

### Stap 1: Beschikbaarheid

Geplande productietijd = 480 - 30 = **450 minuten**
Stilstand = 25 + 20 = **45 minuten**
Draaitijd = 450 - 45 = **405 minuten**

**Beschikbaarheid = 405 / 450 = 90.0%**

### Stap 2: Prestatie

Theoretisch mogelijke output = 405 / 2 = **202.5 stuks**
Werkelijke output = **180 stuks**

**Prestatie = 180 / 202.5 = 88.9%**

Er zijn dus 22.5 stuks "verdwenen" door korte stops en snelheidsverlies.

### Stap 3: Kwaliteit

Goede producten = 180 - 5 - 4 = **171 stuks**

**Kwaliteit = 171 / 180 = 95.0%**

### Stap 4: OEE

**OEE = 90.0% x 88.9% x 95.0% = 76.0%**

### Wat betekent dit?

Van de geplande productietijd wordt slechts 76% **effectief** benut. De rest gaat verloren aan:
- Stilstand: 10% (storing + omstellen)
- Snelheidsverlies: ~11% (korte stops, langzamer draaien)
- Kwaliteitsverlies: ~5% (afkeur + herbewerking)

### Waar verbeter je het snelst?

Kijk naar het onderdeel met het laagste percentage. In dit voorbeeld is **prestatie** (88.9%) het zwakste punt. Onderzoek de korte stops en snelheidsverliezen -- daar zit het meeste verbeterpotentieel.

| Scenario | Beschikbaarheid | Prestatie | Kwaliteit | OEE |
|---|---|---|---|---|
| Huidige situatie | 90.0% | 88.9% | 95.0% | **76.0%** |
| Storing halveren | 92.2% | 88.9% | 95.0% | **77.9%** |
| Prestatie naar 95% | 90.0% | 95.0% | 95.0% | **81.2%** |
| Alles verbeteren | 92.2% | 95.0% | 98.0% | **85.8%** |

## Praktijkvoorbeeld

Een teamleider bij een metaalbedrijf berekent elke vrijdag de OEE van zijn drie machines. Machine A scoort 82%, machine B scoort 71%, machine C scoort 78%. Hij kijkt naar de details van machine B: beschikbaarheid 85%, prestatie 92%, kwaliteit 91%. Het probleem zit bij beschikbaarheid -- te veel stilstand. Hij analyseert de storingsregistratie en ontdekt dat dezelfde hydrauliekstoring drie keer per week optreedt. Na reparatie van de lekkage stijgt de OEE van machine B naar 79%.
