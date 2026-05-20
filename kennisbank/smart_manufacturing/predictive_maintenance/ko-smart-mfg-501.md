---
id: ko-smart-mfg-501
title: 'Jouw machine kiezen: waar zit de grootste winst?'
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een stapsgewijs framework om de machine te identificeren waar predictive
  maintenance de grootste besparing oplevert — op basis van ongeplande stilstand,
  kosten per uur en potentiele besparing.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1 + Mobley (2002) Ch. 8-9
status: validated
updated_at: '2026-05-20'
correlation_id: ronde22-lo-smart-mfg-501
---

# Jouw machine kiezen: waar zit de grootste winst?

Je hebt in Module 1 en 2 geleerd wat predictive maintenance is en hoe je anomaliescores interpreteert. Maar nu komt de vraag: **op welke machine ga je het toepassen?** Niet elke machine levert evenveel winst op. Met dit framework kies je de machine waar de grootste besparing zit.

### Stap 1: Identificeer de machine met de meeste ongeplande stilstand

Pak de storingsregistratie van de afgelopen 6-12 maanden erbij. Kijk naar:
- Welke machine stond het vaakst ongepland stil?
- Hoe lang duurde elke stilstand gemiddeld?
- Waren het steeds dezelfde soort storingen?

Tip: als er geen storingsregistratie is, vraag het je collega's. Operators weten precies welke machine de meeste problemen geeft.

### Stap 2: Bereken de kosten van stilstand per uur

Elke ongeplande stilstand kost geld. Hoeveel? Dat verschilt per machine en per productielijn. Denk aan:

- **Directe kosten**: verloren productie (aantal producten x verkoopprijs)
- **Arbeid**: monteurs die de storing verhelpen
- **Materiaal**: vervangende onderdelen (soms spoedbestelling = duurder)
- **Gevolgkosten**: vertraging in de rest van de lijn, boetes bij te late levering

Vuistregel: tel de directe kosten en de arbeidskosten bij elkaar op. Dat geeft al een goede indicatie.

### Stap 3: Schat de potentiele besparing

Predictive maintenance voorkomt niet alle stilstand — maar wel een groot deel. Een realistische schatting:

- **50-70%** van de ongeplande stilstand is voorspelbaar met sensoren *(bron: Mobley, R.K. (2002). An Introduction to Predictive Maintenance, hoofdstukken 8-9 — klassieke referentie in het PM-vakgebied)*
- Reken met 50% als conservatieve schatting
- Besparing per jaar = aantal uren ongeplande stilstand x kosten per uur x 50%

**Voorbeeld:**
Machine X staat 40 uur per jaar ongepland stil. Kosten: EUR 500 per uur.
Potentiele besparing: 40 x EUR 500 x 50% = **EUR 10.000 per jaar**.

### De keuze maken

Kies de machine met de hoogste potentiele besparing. Maar houd ook rekening met:
- Zijn er al sensoren aanwezig? (makkelijker starten)
- Is de machine toegankelijk voor sensorplaatsing?
- Staat het onderhoudsteam open voor deze aanpak?

De beste pilot is een machine waar de winst duidelijk is EN waar het praktisch haalbaar is.


## Praktijkvoorbeeld

Bij een metaalverwerkend bedrijf in Brabant stonden drie machines regelmatig stil: een CNC-draaibank (25 uur/jaar), een lasrobot (15 uur/jaar) en een hydraulische pers (60 uur/jaar). De kosten per uur: CNC EUR 400, lasrobot EUR 600, pers EUR 350. Potentiele besparing (50%): CNC EUR 5.000, lasrobot EUR 4.500, pers EUR 10.500. De keuze viel op de hydraulische pers — de hoogste besparing. Bovendien had de pers al een temperatuursensor, waardoor de start eenvoudig was. Na zes maanden was de ongeplande stilstand met 55% gedaald en de besparing EUR 11.550.
