# Werkblad 2 — Een neuraal netwerk in drie lagen

*Handout — Kolb fase 3 (theoretiseren)*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 15 minuten

---

## Over dit werkblad

Dit is een handout met theorie. Je leest mee. Je markeert met je stift wat voor jou een aha-moment is. Je mag elk moment een vraag stellen. Geen vraag is raar.

In het vorige werkblad dacht je na over de camera. De groep kwam vaak uit op "in stapjes". Dat klopt. Een neuraal netwerk werkt echt in stapjes. Die stapjes heten **lagen**.

---

## De kern in vier zinnen

Een neuraal netwerk is een AI-model. Het leert patronen uit voorbeelden. Het bestaat uit drie hoofddelen. Die delen heten input, lagen en output.

Het is wiskunde. Het is geen magie. Het is ook niet exact zoals een brein. De naam komt wel van zenuwcellen, maar het werkt anders.

---

## De drie hoofddelen

| Deel | Wat is het? | Voorbeeld bij de camera |
|------|-------------|--------------------------|
| **Input (invoer)** | Wat het model binnenkrijgt. | Een foto van een product op de band. |
| **Lagen (hidden layers)** | Stapjes waarin het model patronen herkent. | Eerste laag: lijnen. Volgende laag: vormen. Laatste laag: complete patronen. |
| **Output (uitvoer)** | Het antwoord dat het model geeft. | Goed of kras. |

*Markeer met je stift wat voor jou een aha-moment is.*

---

## Kleine eenheden in elke laag

In elke laag zitten kleine rekeneenheden. Die heten **neuronen** (neurons). Elk neuron krijgt iets binnen. Elk neuron geeft iets door aan de volgende laag.

Elke verbinding tussen twee neuronen heeft een **gewicht** (weight). Een gewicht is een getal. Het zegt hoe belangrijk een verbinding is. Tijdens het trainen worden die gewichten aangepast. Zo leert het netwerk welke patronen belangrijk zijn.

Een gewicht hoog? Dan telt die verbinding zwaar mee in het antwoord.

---

## Waar komt het leren vandaan?

Het netwerk leert door duizenden voorbeelden te zien. Bij elke foto kent het systeem het juiste antwoord. Dat heet de **trainingsdata**.

Het netwerk vergelijkt zijn eigen antwoord met het juiste antwoord. Wijkt het af? Dan past het de gewichten een beetje aan. Dit gebeurt heel vaak. Na duizenden voorbeelden zit er een werkend patroon in.

---

## Voorbeeld uit de praktijk

Een producent maakt kunststof brandstoftanks. Een camera kijkt boven de band mee. Het systeem moest leren wat een goede tank is. Daar werd een CNN voor gebruikt.

**CNN** staat voor *convolutional neural network*. Dat is een netwerk speciaal voor beelden. Een CNN is heel goed in foto's beoordelen.

Het CNN zag 1.300 nagemaakte foto's en 295 echte foto's. Dat is samen bijna 1.600 voorbeelden. Daarna haalde het systeem 70% nauwkeurigheid op nieuwe foto's.

*Bron: Soldatos (2024). Artificial Intelligence in Manufacturing, hoofdstuk 17-18.*

---

## Een sorteersysteem in een ander voorbeeld

Een ander bedrijf sorteert appels in drie klassen. Klasse A is topkwaliteit. Klasse B is gewoon. Klasse C is afkeur. Boven de band hangt een camera. Het neurale netwerk geeft per appel een klasse.

De input is een foto van een appel. De lagen zoeken naar kleur, vorm en plekjes. De output is een klasse: A, B of C. Dit netwerk is getraind met meer dan 5.000 foto's.

Zie je het verband? Andere input, andere output, maar dezelfde drie hoofddelen.

---

## Wat een neuraal netwerk niet is

| Het is **geen** ... | Wat het wel is |
|---------------------|-----------------|
| Magie | Wiskunde. Stapjes met getallen. |
| Exact zoals een brein | Een rekenmodel. De naam komt van zenuwcellen. Verder is het anders. |
| Klaar zonder data | Het werkt alleen met voorbeelden. Veel voorbeelden. Goede voorbeelden. |

---

## Wat betekent dit voor jouw werk?

Het model leert van data. Operators bepalen wat goed is. Operators bepalen wat fout is. Zonder die kennis kan het model niets.

Jouw vakkennis blijft nodig. Jij weet hoe een goed product eruit hoort te zien. Jij hoort wanneer een machine raar klinkt. Een camera kan dat ook leren. Maar alleen als jij eerst de voorbeelden geeft.

---

## Vakwoorden uit deze sessie

| Vakterm | Betekenis in een zin |
|---------|---------------------|
| **Neuraal netwerk** (neural network, NN) | Een AI-model dat patronen leert uit voorbeelden. |
| **Input** (invoer) | Wat het model binnenkrijgt. Bijvoorbeeld een foto. |
| **Output** (uitvoer) | Het antwoord van het model. Bijvoorbeeld goed of kras. |
| **Laag** (layer, hidden layer) | Een stapje waarin het model rekent. |
| **Neuron** | Een kleine rekeneenheid in een laag. |
| **Gewicht** (weight) | Getal dat zegt hoe belangrijk een verbinding is. |
| **CNN** (convolutional neural network) | Een netwerk speciaal voor beelden. |
| **Trainingsdata** | De voorbeelden waarmee het netwerk leert. |

---

## Korte zelftest

*Beantwoord in eigen woorden. Een halve zin is genoeg.*

**Wat is de input bij een inspectiecamera?**

_______________________________________________

**Wat is een laag?**

_______________________________________________

**Wat is de output bij een sorteersysteem voor appels?**

_______________________________________________

**Wat is trainingsdata?**

_______________________________________________

---

## Bron

Soldatos, J. (2024). *Artificial Intelligence in Manufacturing*. Springer, hoofdstuk 17-18.

---

*AIMM x BronzGreen — AI Fundamentals · Module 1 · Neurale netwerken (lo-ai-fund-022)*
