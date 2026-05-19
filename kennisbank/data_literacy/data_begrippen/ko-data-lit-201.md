---
id: ko-data-lit-201
title: 'Datatypes herkennen: getallen, categorieen, tijd, tekst'
type: framework
domain: data_literacy
subdomain: data_begrippen
summary: 'Er zijn vier soorten data op de werkvloer: getallen (meten/tellen), categorieen
  (groepen/labels), tijddata (wanneer iets gebeurde) en tekst (opmerkingen/logs).
  Als je weet welk type data je hebt, weet je ook wat je ermee kunt doen.'
source_centrality: 0.7
source_ref: AIMM Competentieframework Data Literacy, competentie data_begrip.train
status: validated
updated_at: '2026-05-19'
correlation_id: ronde9-lo-data-lit-201
---

# Datatypes herkennen: getallen, categorieën, tijd, tekst

Er zijn vier soorten data op de werkvloer: getallen (meten/tellen), categorieën (groepen/labels), tijddata (wanneer iets gebeurde) en tekst (opmerkingen/logs). Als je weet welk type data je hebt, weet je ook wat je ermee kunt doen.

In Module 1 heb je geleerd wat data is. Nu gaan we een stap verder: welke **soorten** data zijn er? Want niet alle data is hetzelfde. En het type data bepaalt wat je ermee kunt doen.

### De vier datatypes op de werkvloer

**1. Getallen (numerieke data)**
Alles wat je kunt meten of tellen:
- Temperatuur: 182,5 graden
- Gewicht: 3,42 kg
- Productieaantal: 847 stuks
- OEE: 72%

Met getallen kun je **rekenen**: gemiddelde, maximum, minimum, trend.

**2. Categorieën (categorische data)**
Labels of groepen. Je kunt er niet mee rekenen, maar je kunt er wel mee **sorteren en tellen**:
- Machinetype: CNC-frees, draaibank, lasersnijder
- Foutcode: E-01, E-02, E-03
- Ploeg: ochtend, middag, nacht
- Beoordeling: goed, matig, afgekeurd

**3. Tijddata**
Wanneer iets gebeurde. Essentieel voor **trends en patronen**:
- Starttijd: 06:30
- Storingsduur: 14 minuten
- Datum: 2026-04-08
- Week: week 15

Met tijddata kun je zien: wordt het beter of slechter over tijd?

**4. Tekst (vrije tekst)**
Opmerkingen, logboeknotities, beschrijvingen:
- "Trillingen bij hoog toerental"
- "Gereedschap gewisseld na 200 stuks"
- "Klant klaagt over oppervlakte-afwerking"

Tekst is lastig om automatisch te verwerken, maar bevat vaak de **belangrijkste informatie** over het waarom.

### Hoe bepaal je het datatype?

Stel jezelf drie vragen:
1. **Kun je ermee rekenen?** Ja --> getal. Nee --> ga naar vraag 2.
2. **Is het een keuze uit een vaste lijst?** Ja --> categorie. Nee --> ga naar vraag 3.
3. **Gaat het over wanneer?** Ja --> tijd. Nee --> het is tekst.

### Waarom is dit belangrijk?

Als je weet welk type data je hebt, weet je ook:
- Wat je ermee kunt doen (rekenen, sorteren, trend bekijken)
- Hoe je het moet invoeren (getal in een getal-veld, niet als tekst)
- Welke fouten je kunt verwachten (een temperatuur van "warm" is geen getal)


## Praktijkvoorbeeld

Op een verpakkingslijn registreert het systeem per doos:
- **Gewicht**: 2,48 kg (getal)
- **Productlijn**: A3-Premium (categorie)
- **Tijdstip**: 14:32:07 (tijd)
- **Opmerking operator**: "Doos scheef op de band" (tekst)

De teamleider wil weten hoeveel dozen te licht waren. Dat kan hij alleen uitrekenen met het gewicht (getal), niet met de opmerking (tekst). Maar de opmerking vertelt hem WAAROM de doos te licht was.
