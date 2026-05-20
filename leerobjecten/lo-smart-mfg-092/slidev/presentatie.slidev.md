---
theme: default
title: "Anomaliedetectie in Sensordata"
info: "Leer drie soorten afwijkingen herkennen in sensordata van productiemachines"
author: AIMM / BronzGreen
transition: slide-left
mdc: true
---

# Anomaliedetectie in Sensordata

### Herken afwijkingen voordat het misgaat

Module 1: Gebruik | 45 minuten | MBO-3

<!-- Welkom. Dit is de sessie over anomaliedetectie. De kern: operators leren drie soorten afwijkingen herkennen in sensordata. De sessie volgt het Ik doe - Wij doen - Jij doet principe. -->

---
layout: center
---

# Leerdoel

<v-click>

Na deze sessie kun je **zelf afwijkingen herkennen** in sensordata van een machine.

</v-click>

<v-click>

Je leert **drie soorten afwijkingen** kennen:

- **Puntanomalie** -- een enkel meetpunt dat afwijkt
- **Contextuele anomalie** -- afwijkend in deze situatie, normaal in een andere
- **Collectieve anomalie** -- een patroon dat afwijkt (bijv. stijgende trend)

</v-click>

<v-click>

Aan het einde oefen je zelfstandig met vijf sensorwaarden.

</v-click>

<!-- FEED-UP: Spreek dit leerdoel hardop uit aan het begin van de sessie. Het geeft de deelnemers richting en verlaagt onzekerheid. -->

---
layout: two-cols
---

# Worked Example: Ik doe het voor

**Temperatuur motor: 82 graden C**

Normaal: 65 - 70 graden

<v-click>

"Ik kijk naar de normaalwaarde: 65-70. De meting is 82. Dat is **12 graden boven het maximum**."

</v-click>

<v-click>

Dit is een **puntanomalie**.

</v-click>

::right::

<v-click>

**Druk: 4,2 bar om 07:15**

Normaal productie: 3,0 - 3,5 bar
Normaal opstart: tot 4,5 bar

</v-click>

<v-click>

"Het is 07:15 -- de machine is net opgestart. Bij opstart mag de druk hoger zijn."

</v-click>

<v-click>

Dit is **geen anomalie** in deze context. Maar om 14:00 uur zou het **wel** een anomalie zijn.

Dit is een **contextuele anomalie**.

</v-click>

<!-- IK DOE: Doe dit LANGZAAM voor. Benoem je denkstappen hardop. Laat na elk voorbeeld 30 seconden stilte voor noteren op werkblad 1. -->

---
layout: center
---

# Groepsoefening: Wij doen het samen

Drie sensorwaarden. Bespreek per waarde: **afwijkend of normaal?**

<v-click>

**Waarde 1:** Trillingen 0,8 mm/s (normaal: 0,2 - 0,4 mm/s)

</v-click>

<v-click>

**Waarde 2:** Energieverbruik 12 kWh (normaal: 8-10 kWh) -- maar zwaarder product

</v-click>

<v-click>

**Waarde 3:** Temperatuur: 68, 69, 70, 72, 74, 77, 80 graden

</v-click>

<v-click>

Wat valt jullie op aan het **patroon** bij waarde 3?

</v-click>

<!-- WIJ DOEN: Laat de groep antwoorden. Geef iedereen de ruimte, ook stille deelnemers. Bij waarde 2: laat de onzekerheid bewust bestaan. Bij waarde 3: begeleid naar de stijgende trend. -->

---
layout: two-cols
---

# Drie soorten anomalieen

**1. Puntanomalie**

Een enkel meetpunt dat ver afwijkt van normaal.

*Voorbeeld: trillingen 0,8 mm/s (normaal 0,2-0,4)*

**2. Contextuele anomalie**

Afwijkend in de ene situatie, normaal in een andere.

*Voorbeeld: hoog energieverbruik bij zwaarder product*

::right::

**3. Collectieve anomalie**

Geen enkel getal is extreem, maar het patroon is zorgelijk.

*Voorbeeld: temperatuur stijgt elke meting een paar graden*

<v-click>

### Drie stappen van detectie

1. **Voorbereiding** -- wat is normaal?
2. **Training** -- het systeem leert de patronen
3. **Detectie** -- afwijkingen worden gemarkeerd

</v-click>

<v-click>

*Een AI-systeem doet precies wat jullie net deden -- maar 24 uur per dag, bij 100 sensoren tegelijk.*

</v-click>

<!-- Verwijs TERUG naar de oefening: "Bij waarde 1 zagen jullie een puntanomalie, bij waarde 2 een contextuele, bij waarde 3 een collectieve." Houd dit kort: max 8 minuten. -->

---
layout: center
---

# Jij doet het zelf: duo-opdracht

Werk samen met je buurman. **Vijf sensorwaarden.** Per waarde:

<v-click>

1. Is dit **normaal** of **afwijkend**?
2. Welk **type** anomalie is het?
3. **Waarom** denk je dat?

</v-click>

<v-click>

Jullie hebben **8 minuten**.

</v-click>

<v-click>

Daarna bespreken we het antwoordmodel samen.

</v-click>

<!-- JIJ DOET: Deel werkblad 4 uit. Loop rond maar geef GEEN antwoorden. Stel alleen vragen terug: "Wat is de normale waarde? Wat is de context?" Na 8 minuten: antwoordmodel plenair doorlopen. -->

---
layout: center
---

# Transferopdracht

Kijk deze week naar de **sensordata of dashboards** op je werkvloer.

<v-click>

- Schrijf **drie waarden** op die je opvallen
- Bepaal per waarde: normaal of afwijkend?
- Welk type anomalie zou het zijn?

</v-click>

<v-click>

**Neem dit mee** naar de volgende bijeenkomst.

</v-click>

<v-click>

### Doe ook:

Vraag je leidinggevende: **welke sensoren** zitten er op jullie machines?

Je zult verrast zijn.

</v-click>

<!-- De transferopdracht is essentieel -- sla deze NIET over, ook niet als de tijd krap is. Het is de brug naar de werkpraktijk. -->

---
layout: end
---

# Goed gedaan!

Jullie kunnen nu drie soorten afwijkingen herkennen in sensordata.

**Puntanomalie -- Contextuele anomalie -- Collectieve anomalie**

Volgende keer: jullie eigen observaties van de werkvloer.

<!-- Sluit positief af. Benoem wat ze geleerd hebben. Herhaal de drie termen. -->
