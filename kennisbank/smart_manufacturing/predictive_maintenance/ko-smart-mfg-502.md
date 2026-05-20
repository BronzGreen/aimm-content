---
id: ko-smart-mfg-502
title: Eigen productiedata verzamelen en beoordelen
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: 'Een stapsgewijze data-audit van je eigen productielijn: welke sensoren heb
  je, welke data wordt al opgeslagen, wat is de kwaliteit, en wat heb je nog nodig
  voor predictive maintenance?'
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1
status: validated
updated_at: '2026-05-20'
correlation_id: ronde22-lo-smart-mfg-502
---

# Eigen productiedata verzamelen en beoordelen

Voordat je een predictief model kunt bouwen, moet je weten wat je hebt. Welke data wordt er al verzameld op jouw lijn? Is die data bruikbaar? En wat ontbreekt er nog? Met deze data-audit breng je dat in kaart.

### Stap 1: Inventariseer je sensoren

Loop langs je machine en beantwoord deze vragen:
- Welke sensoren zitten er op? (temperatuur, trillingen, druk, stroom, geluid)
- Waar zitten ze precies? (motor, spindel, hydrauliek, koeling)
- Hoe oud zijn ze? Worden ze gekalibreerd?
- Zijn er sensoren die het niet meer doen?

Schrijf alles op. Veel operators weten niet precies welke sensoren er op hun machine zitten — dit is het moment om dat uit te zoeken.

### Stap 2: Check wat er wordt opgeslagen

Sensoren die meten maar niet opslaan zijn waardeloos voor predictive maintenance. Controleer:
- Wordt de sensordata opgeslagen? Waar? (PLC, SCADA, cloudplatform, logboek)
- Hoe vaak wordt er gemeten? (elke seconde, elke minuut, elk uur)
- Hoe lang wordt data bewaard? (een dag, een week, een jaar)
- Kun je de data exporteren of bekijken?

Voor predictive maintenance heb je minimaal **3 maanden historische data** nodig. Liefst 6-12 maanden.

### Stap 3: Beoordeel de datakwaliteit

Niet alle data is bruikbare data. Check deze vier punten:

1. **Volledigheid**: zitten er gaten in de data? (uitval, weekenden, vakanties)
2. **Consistentie**: meet de sensor steeds op dezelfde manier?
3. **Nauwkeurigheid**: kloppen de waarden met de werkelijkheid?
4. **Tijdstempel**: heeft elke meting een datum en tijd?

Vuistregel *(pragmatische industriestandaard, geen harde norm)*: als meer dan 10% van de data ontbreekt of onbetrouwbaar is, moet je eerst de dataverzameling verbeteren voordat je een model bouwt.

### Stap 4: Bepaal wat je nog nodig hebt

Vergelijk wat je hebt met wat je nodig hebt:
- Ontbreken er sensoren? Welke? (een trillingssensor kost EUR 200-500)
- Moet de meetfrequentie omhoog?
- Moet de opslagperiode langer?
- Heb je iemand nodig die de data kan exporteren?

Maak een lijstje: wat is er, wat werkt, wat ontbreekt. Dat is je startpunt voor de business case.


## Praktijkvoorbeeld

Een operator bij een verpakkingsbedrijf deed een data-audit op zijn vulmachine. Resultaat: er zaten drie sensoren op (temperatuur koelwater, druk hydrauliek, snelheid transportband), maar alleen de temperatuur werd opgeslagen — in een Excel-bestand dat de technische dienst bijhield. De druk- en snelheidsdata verdween na elke shift. Na overleg met de technische dienst werd de PLC zo ingesteld dat alle drie sensoren elke minuut logden naar een centraal systeem. Kosten: 4 uur werk van een PLC-programmeur. Resultaat: na 3 maanden was er genoeg data voor een eerste trendanalyse.
