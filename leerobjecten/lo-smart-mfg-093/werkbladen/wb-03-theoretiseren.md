# Handout: Autoencoder — AI leert wat normaal is
*Anomaliedetectie met een neuraal netwerk*

**Naam:** ____________________  **Datum:** __________
**Module 1 — Predictive Maintenance: Gebruik**

---

> **Kernidee:** Een autoencoder is een AI-model. Het leert hoe normale productiedata eruitziet. Als er iets afwijkt, kan het model de data niet goed herstellen. Dan slaat het alarm.

---

## Het model in drie stappen

| Stap | Wat gebeurt er | Vergelijking |
|------|----------------|--------------|
| **1. Invoer** | De sensordata gaat het model in (temperatuur, druk, energie) | Je bekijkt een foto |
| **2. Samenvatten** | Het model perst de data samen tot een kort overzicht | Je beschrijft de foto in drie woorden |
| **3. Herstellen** | Het model probeert de originele data terug te maken | Je tekent de foto opnieuw vanuit die drie woorden |

---

## Hoe herkent het afwijkingen?

*Vul de ontbrekende woorden in:*

1. Het model is getraind op _________________ productiedata.

2. Normale data kan het goed samenvatten en _________________.

3. Afwijkende data past niet in het geleerde _________________.

4. Het verschil tussen origineel en herstel heet de _________________.

5. Als die fout groot genoeg is, gaat er een _________________ af.

---

## Belangrijke begrippen

| Begrip | Wat het betekent |
|--------|-----------------|
| **Autoencoder** | Een AI-model dat data samenvat en weer herstelt |
| **Encoder** | Het deel dat data samenvat (comprimeert) |
| **Decoder** | Het deel dat data weer opbouwt (herstelt) |
| **Reconstructiefout** | Het verschil tussen origineel en herstel |
| **Drempelwaarde** | De grens waarbij het systeem alarm slaat |
| **Anomalie** | Een afwijking van het normale patroon |

---

## Voorbeeld uit de praktijk

> Bij het maken van brandstoftanks meet een autoencoder elke cyclus.
> Het model kent het normale patroon van temperatuur, druk en energie.
> Als een luchttoevoer verstopt raakt, verandert het patroon.
> Het model kan die data niet goed herstellen.
> De reconstructiefout is groot. Het alarm gaat af.
> De operator controleert de machine. De storing is op tijd gevonden.

---

## Controleer jezelf

*Kun je deze drie vragen beantwoorden? Kruis aan.*

- [ ] Wat doet een autoencoder met de data? (samenvatten en herstellen)
- [ ] Wanneer slaat het alarm? (als de reconstructiefout groter is dan de drempel)
- [ ] Waarom werkt het? (het model kent alleen normale patronen)

---
*Bron: Autoencoder — Anomaliedetectie in de maakindustrie | AIMM Predictive Maintenance Module 1 | v1.0*
