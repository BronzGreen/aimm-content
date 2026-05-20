---
id: ko-data-lit-204
title: 'Een simpele data-analyse uitvoeren: van vraag naar antwoord'
type: framework
domain: data_literacy
subdomain: data_driven_besluitvorming
summary: 'Een data-analyse volgt vier stappen: vraag formuleren, data verzamelen,
  analyseren en concluderen. Met dit stappenplan kun je zelf een eenvoudige analyse
  uitvoeren op je eigen werkvloer.'
source_centrality: 0.7
source_ref: AIMM Competentieframework Data Literacy, competentie data_driven_besluitvorming.train
status: validated
updated_at: '2026-05-19'
correlation_id: ronde11-lo-data-lit-204
---

# Een simpele data-analyse uitvoeren: van vraag naar antwoord

Een data-analyse volgt vier stappen: vraag formuleren, data verzamelen, analyseren en concluderen. Met dit stappenplan kun je zelf een eenvoudige analyse uitvoeren op je eigen werkvloer.

In Module 1 heb je geleerd hoe je data-gedreven beslissingen neemt. Nu ga je het zelf doen: een simpele data-analyse van begin tot eind.

### Het vier-stappenplan

**Stap 1: Formuleer je vraag**

Een goede analyse begint met een goede vraag. Niet "hoe gaat het met de productie?" maar:
- "Waarom is het afkeurpercentage op dinsdag hoger dan op andere dagen?"
- "Hoeveel ongeplande stilstand hadden we deze maand per machine?"
- "Is de doorlooptijd de afgelopen vier weken gestegen of gedaald?"

Een goede vraag is:
- **Specifiek** -- niet "hoe gaat het?" maar "hoeveel?"
- **Beantwoordbaar met data** -- je kunt er een getal bij vinden
- **Relevant** -- het antwoord helpt je iets te verbeteren

**Stap 2: Verzamel je data**

Waar vind je de data die je nodig hebt?
- Dashboard of MES-systeem
- Logboek of formulieren
- Excel-bestanden
- Collega's die het weten

Check de datakwaliteit (volledigheid, consistentie, actualiteit) voordat je verder gaat.

**Stap 3: Analyseer**

Voor een simpele analyse heb je drie technieken:
1. **Vergelijken** -- is het meer of minder dan vorige week/maand/jaar?
2. **Groeperen** -- verschilt het per machine, per ploeg, per dag?
3. **Tellen** -- hoe vaak komt dit voor?

**Stap 4: Concludeer en adviseer**

Trek een conclusie en koppel die aan een actie:
- **Conclusie:** wat zegt de data?
- **Mogelijke oorzaak:** wat zou de reden kunnen zijn?
- **Advies:** wat stel je voor?

Let op: data vertelt je WAT er aan de hand is, niet altijd WAAROM.

### De valkuilen

- **Cherry-picking:** alleen de data laten zien die je punt bewijst
- **Correlatie is geen oorzaak:** omdat twee dingen samen veranderen, betekent niet dat het een het ander veroorzaakt
- **Te kleine steekproef:** een conclusie op een dag data is onbetrouwbaar


## Praktijkvoorbeeld

Een operator merkt dat zijn machine vaker stilvalt op maandagochtend. Hij besluit het uit te zoeken:

1. **Vraag:** "Hoeveel ongeplande stops had mijn machine per dag de afgelopen vier weken?"
2. **Data:** Hij haalt de storingsregistratie uit het MES-systeem. 20 werkdagen, 47 ongeplande stops totaal.
3. **Analyse:** Hij groepeert per dag: maandag 14 stops (30%), dinsdag t/m vrijdag elk 8-9 stops (17-19%).
4. **Conclusie:** "Maandag heeft bijna dubbel zoveel stops. De machine staat het weekend stil en koelt af. Advies: een opwarmprotocol invoeren op maandagochtend."
