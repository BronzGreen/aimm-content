# Handout — data-pipeline (data-leiding)
*Werkblad Kolb-fase 3 — Theoretiseren*

**Naam:** ____________________  **Datum:** __________

---

> **De definitie**
> Een data-pipeline (data-leiding) is het pad dat sensor-data aflegt van meten tot gebruiken. Elke meting doorloopt vier knooppunten. Bij elk knooppunt zijn er keuzes te maken. Drie keuzes bepalen of de pipeline werkt: latentie (vertraging), volume (hoeveelheid data) en failover (terugval bij fout).

---

## De vier knooppunten — het pad in beeld

```
+----------+      +--------------+      +----------+      +-------------+
|          | ---> |              | ---> |          | ---> |             |
|  SENSOR  |      |  EDGE-BUFFER |      |  OPSLAG  |      |  CONSUMENT  |
|          |      |  (tussen-    |      |          |      |  (dashboard |
|  meet    |      |   station)   |      |  bewaart |      |   of model) |
|          |      |  filtert     |      |          |      |             |
+----------+      +--------------+      +----------+      +-------------+
     1.                  2.                  3.                 4.
```

| # | Knooppunt | Wat gebeurt er |
|---|-----------|----------------|
| **1** | **Sensor** | De bron. Een trillings-, temperatuur-, beeld- of druk-sensor meet en verstuurt. |
| **2** | **Edge-buffer (tussenstation)** | Klein opslag- en filter-punt bij de machine. Vaak een industriële computer ernaast. Bewaart data tijdelijk als de verbinding wegvalt. Vat samen: alleen relevante data gaat door. |
| **3** | **Opslag** | Centrale plek waar data wordt bewaard. Soms een server ter plaatse, soms in de cloud. Hier zit weken tot maanden aan historie. |
| **4** | **Consument** | De plek waar de data wordt gebruikt. Dashboard voor de operator. AI-model dat patronen voorspelt. Rapportage voor de productieleider. |

> **Vuistregel:** een goed ontworpen pipeline is voor de operator onzichtbaar. Alles werkt gewoon. Pas als er iets niet klopt, merk je dat er onderhuids veel keuzes zijn gemaakt.

---

## De drie ontwerp-keuzes

Bij elk pipeline-ontwerp wegen drie keuzes. Bron: Anaya et al. (2024); Bakopoulos et al. (2024).

### Keuze 1 — Latentie (vertraging): hoe snel moet de data er zijn?

| Optie | Tijd | Voorbeeld |
|-------|------|-----------|
| **Real-time** | onder 1 seconde | Veiligheids-alarm als iemand te dicht bij een robot komt |
| **Near-realtime** | onder 60 seconden | Temperatuur die boven een drempel uitkomt |
| **Batch** | uren of dagen | Maandrapport over productie |

*Hoe sneller, hoe duurder. Niet alles hoeft real-time. Vraag eerst: wat heeft de gebruiker echt nodig?*

### Keuze 2 — Volume (hoeveelheid data): wat doe je ermee?

Een trillingsensor kan duizend metingen per seconde doen. Bij tien sensoren en vierentwintig uur productie loopt dat richting honderden miljoenen metingen per dag. Te veel om allemaal naar de cloud te sturen.

De slimme oplossing zit bij de edge-buffer: daar vat je samen. Stuur bijvoorbeeld elke tien seconden het gemiddelde, plus elke afwijking. Je bespaart soms 99% aan data zonder informatie te verliezen.

### Keuze 3 — Failover (terugval bij fout): wat als er iets stopt?

Drie vragen tellen mee:

- Wat gebeurt er als de verbinding tussen edge-buffer en opslag wegvalt?
- Wat als de opslag vol raakt?
- Wat als de sensor zelf stuk gaat?

Een goede pipeline heeft twee dingen ingebouwd: **buffering** (de edge-buffer bewaart data totdat de verbinding terug is) en **alarmen** (de operator krijgt melding bij sensor-uitval).

---

## Wat de operator merkt — drie storings-signalen

| Wat je op het dashboard merkt | Wat er ondertussen misgaat | Welke keuze klopt niet |
|-------------------------------|----------------------------|-------------------------|
| **Het dashboard loopt achter** | Data doet er te lang over om bij het scherm te komen | Latentie te hoog |
| **Er ontbreekt data in een grafiek** | Verbinding viel weg en niemand bewaarde de data | Geen failover |
| **De cloud-rekening loopt op** | Alle ruwe metingen gaan naar de cloud zonder filter | Geen volume-controle |

*De drie fragmenten uit fase 1 komen hier terug. Markeer met je markeerstift welke keuze bij elk fragment hoorde.*

---

## Voorbeeld om vast te houden — spuitgieterij met 50 mallen

| | Eerste ontwerp | Tweede ontwerp |
|--|-----------------|-----------------|
| **Wat doet de sensor?** | Stuurt elke seconde direct naar de cloud | Stuurt elke seconde naar de edge-buffer |
| **Wat doet de edge-buffer?** | Niets — geen edge-buffer ingebouwd | Vat samen: gemiddelde per 30 seconden, plus elke afwijking groter dan 3 graden |
| **Wat gaat naar de opslag?** | Alles | Alleen wat ertoe doet |
| **Cloud-rekening per maand** | 2.500 euro | 120 euro |
| **Dashboard-snelheid** | Real-time, maar duur | Resolutie van 30 seconden — ruim voldoende voor temperatuur |

*Verschil: factor twintig in kosten. Dezelfde sensoren, dezelfde vraag, een ander pipeline-ontwerp.*

---

## Teken de pipeline na

*Trek pijlen tussen de vier knooppunten en zet bij elk knooppunt een woord uit de spuitgieterij-casus. Geen verkeerd antwoord — het gaat om het zien van het pad.*

```
   ________          ________          ________          ________
  |        |        |        |        |        |        |        |
  |        | -----> |        | -----> |        | -----> |        |
  |        |        |        |        |        |        |        |
  |________|        |________|        |________|        |________|

     1.                2.                 3.                4.
```

Mijn invulling bij de spuitgieterij:

- 1. Sensor: ______________________________________
- 2. Edge-buffer: ______________________________________
- 3. Opslag: ______________________________________
- 4. Consument: ______________________________________

---

## Vuistregel om te onthouden

> **Een goede data-pipeline is als een goede waterleiding.** De bron levert. Een tussenstation regelt druk en filter. Een reservoir bewaart. De kraan thuis werkt altijd. Pas als de kraan hapert, zoek je terug langs het pad. De drie keuzes — latentie, volume, failover — zijn de kranen waar de pipeline-ontwerper aan kan draaien.

---
*Bron: Anaya et al. (2024), Manufacturing Digital Twin Framework, pp. 181-183; Bakopoulos et al. (2024), Digital-Twin-Enabled Framework, Ch. 5 | AIMM Industry 4.0 — Module 2 (Train) | v1.0*
