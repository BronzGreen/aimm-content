# Werkblad 3 — Neuraal netwerk in drie lagen (handout)
*Wat is een neuraal netwerk? — Activiteit: Theoretiseren*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 15 minuten

---

> **De kern**
> Een neuraal netwerk (neural network, NN — een AI-model dat patronen leert uit voorbeelden) bestaat uit drie hoofddelen. De input. De lagen. De output. Het is wiskunde. Het is geen magie. Het is ook niet exact zoals een brein.

---

## De drie hoofddelen

| Deel | Wat is het? | Voorbeeld bij de camera |
|------|-------------|--------------------------|
| **Input (invoer)** | Wat het model krijgt aangeleverd. | Een foto van een product op de band. |
| **Lagen (hidden layers, tussenlagen)** | Stapjes waarin het model patronen herkent. Eerste laag: lijnen. Volgende laag: vormen. Laatste laag: complete patronen. | Lijnen rond een beugel. Vorm van een kras. |
| **Output (uitvoer)** | Het antwoord dat het model geeft. | Goed of kras. |

*Markeer met je stift wat voor jou een aha-moment is.*

---

## Kleine eenheden in elke laag

In elke laag zitten kleine rekeneenheden. Die heten **neuronen (neurons — kleine rekeneenheden)**. Elk neuron krijgt iets binnen. Elk neuron geeft iets door aan de volgende laag.

Elke verbinding tussen twee neuronen heeft een **gewicht (weight — getal dat zegt hoe belangrijk een verbinding is)**. Tijdens het trainen worden die gewichten aangepast. Zo leert het netwerk welke patronen belangrijk zijn voor een goed antwoord.

---

## Waar komt het leren vandaan?

Het netwerk leert door duizenden voorbeelden te zien. Bij elke foto kent het systeem het juiste antwoord. Het systeem vergelijkt zijn antwoord met dat juiste antwoord. Wijkt het af? Dan past het de gewichten een beetje aan. Dit gebeurt heel vaak. Na duizenden voorbeelden zit er een werkend patroon in.

**Voorbeeld uit de praktijk:** Bij een producent van kunststof brandstoftanks werd een **CNN (convolutional neural network — netwerk speciaal voor beelden)** getraind. Het systeem zag 1.300 nagemaakte foto's en 295 echte foto's. Daarna had het 70% nauwkeurigheid bij nieuwe foto's.

*Bron: Soldatos (2024). Artificial Intelligence in Manufacturing, hoofdstuk 17-18.*

---

## Wat een neuraal netwerk niet is

| Het is **geen** ... | Wat het wel is |
|---------------------|-----------------|
| Magie | Wiskunde. Stapjes met getallen. |
| Exact zoals een brein | Een rekenmodel dat is geïnspireerd op neuronen. De naam komt daar vandaan. Verder is het anders. |
| Klaar zonder data | Het werkt alleen met voorbeelden. Veel voorbeelden. Goede voorbeelden. |

---

## Wat betekent dit voor jouw werk?

Het model leert van data. Operators bepalen wat goed is. Operators bepalen wat fout is. Zonder die kennis kan het model niets. Jouw vakkennis blijft nodig.

---

## Vakwoorden uit deze sessie

| Vakterm | Betekenis in een zin |
|---------|---------------------|
| **Neuraal netwerk (neural network, NN)** | Een AI-model dat patronen leert uit voorbeelden. |
| **Input (invoer)** | Wat het model binnen krijgt. Bijvoorbeeld: een foto. |
| **Output (uitvoer)** | Het antwoord van het model. Bijvoorbeeld: goed of kras. |
| **Laag (layer, hidden layer)** | Een stapje waarin het model rekent. |
| **Neuron (neuron)** | Een kleine rekeneenheid in een laag. |
| **Gewicht (weight)** | Getal dat zegt hoe belangrijk een verbinding is. |
| **CNN (convolutional neural network)** | Netwerk speciaal voor beelden. |

---

*Bron: Soldatos, J. (2024). Artificial Intelligence in Manufacturing. Springer.*
*AIMM x BronzGreen — Module 1: Neurale netwerken (lo-ai-fund-022) — v1.0*
