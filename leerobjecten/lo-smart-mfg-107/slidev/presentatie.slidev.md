---
theme: default
title: "AI-anomaliedetectie op CNC-machines"
info: "Hoe een AI-systeem storingen eerder opspoort bij CNC-machines -- en wat jij als operator doet"
author: AIMM / BronzGreen
transition: slide-left
mdc: true
---

# AI op CNC-machines

### Storingen opsporen voordat het misgaat

Module 1: Gebruik | 45 minuten | MBO-3

<!-- Welkom. Deze sessie gaat over de CNH Industrial case: hoe een AI-systeem afwijkingen herkent in CNC-sensordata. De knikkermetafoor is de kern: 990 blauwe knikkers (normaal), 10 rode (afwijkend). Start met de case, niet met theorie. -->

---
layout: center
---

# De knikkermetafoor

Stel je voor: een zak met **1000 knikkers**.

<v-click>

**990 blauwe knikkers** = normale sensorwaarden

Je machine draait goed. Temperatuur normaal, trillingen laag, energieverbruik stabiel.

</v-click>

<v-click>

**10 rode knikkers** = afwijkende sensorwaarden

Iets is anders. Temperatuur te hoog, trillingen nemen toe, verbruik stijgt.

</v-click>

<v-click>

Het AI-systeem leert hoe **blauwe knikkers** eruitzien.

Als er een **rode knikker** verschijnt, slaat het alarm.

</v-click>

<!-- De knikkermetafoor maakt het abstract concept tastbaar. Gebruik deze metafoor door de hele sessie heen. "Welke knikkers zijn rood?" bij elke case. -->

---
layout: two-cols
---

# Worked example: de CNC-case

**CNH Industrial -- koelsysteem CNC-machine**
*(bron: Sesana et al. 2024, AI in Manufacturing — CNH Modena)*

3 temperatuursensoren op het koelsysteem.

<v-click>

**Sensor 1:** 42 graden C *(normaal: 35-40)*

**Sensor 2:** 45 graden C *(normaal: 35-40)*

**Sensor 3:** 38 graden C *(normaal: 35-40)*

</v-click>

::right::

<v-click>

### Wat valt op?

Sensor 1 en 2 zijn **boven normaal**. Sensor 3 is normaal.

</v-click>

<v-click>

### De rode knikkers

Sensor 1 en 2 zijn rode knikkers. Het AI-systeem markeert deze als **anomalie**.

</v-click>

<v-click>

### Wat doe je als operator?

**Koelsysteem checken.** Gedeeltelijk verstopte koelleiding gevonden.

Vroegtijdig ontdekt = geen ongeplande stilstand.

</v-click>

<!-- IK DOE: Toon het dashboard op het scherm. Wijs de 3 sensoren aan. Denk hardop: "Ik kijk naar de normaalwaarde, dan naar de meting, dan bepaal ik: rood of blauw." Benoem de actie. -->

---
layout: center
---

# Groepsanalyse: nieuwe CNC-melding

**Case 2: trillingssensoren op de spindel**

<v-click>

Het AI-systeem geeft een melding. Drie trillingssensoren:

- **Sensor A:** 0,6 mm/s *(normaal: 0,2-0,4)*
- **Sensor B:** 0,5 mm/s *(normaal: 0,2-0,4)*
- **Sensor C:** 0,3 mm/s *(normaal: 0,2-0,4)*

</v-click>

<v-click>

**Bespreek samen:**

- Welke knikkers zijn **rood**?
- Wat zou de **oorzaak** kunnen zijn?
- Welke **actie** neem je als operator?

</v-click>

<!-- WIJ DOEN: Laat de groep bespreken. Stel vragen: "Welke sensoren wijken af? Hoeveel boven normaal?" Begeleid naar: lagerslijtage spindel. Geef succesfeedback. -->

---

# Het systeem in 3 stappen

Hoe werkt het AI-systeem? Drie stappen:

<v-click>

### 1. Leren wat normaal is

Het systeem bekijkt duizenden metingen van je machine als die **goed draait**. Het leert: dit zijn de blauwe knikkers.

</v-click>

<v-click>

### 2. Vergelijken met nieuwe data

Bij elke nieuwe meting vergelijkt het systeem: **past dit bij de blauwe knikkers?**

</v-click>

<v-click>

### 3. Afwijkingen markeren

Past het niet? Dan is het een **rode knikker**. Het systeem geeft een melding.

**Jij als operator beslist wat je ermee doet.**

</v-click>

<!-- NIET uitleggen: decision trees, splitting, path length. WEL: wat doet het systeem, wat zie jij, wat doe jij. Houd het bij de 3 stappen. Max 7 minuten. -->

---
layout: center
---

# Duo-opdracht: jouw beurt

**Case 3: energieverbruik-sensoren**

Werk samen met je buurman. Het AI-systeem geeft een melding.

<v-click>

- Bekijk de case-kaart
- Welke sensoren wijken af? *(welke knikkers zijn rood?)*
- Wat zou de oorzaak kunnen zijn?
- Welke actie neem je?

</v-click>

<v-click>

Jullie hebben **6 minuten**. Presenteer je conclusie kort aan de groep.

</v-click>

<!-- JIJ DOET: Deel de case-kaart uit. Laat duo's zelfstandig werken. Loop rond, stel alleen vragen als een duo vastloopt. Na afloop: laat 2-3 duo's presenteren. Geef feed-forward. -->

---
layout: center
---

# Transferopdracht

Kijk deze week bij **je eigen machine** naar de sensoren die je kent.

<v-click>

- Schrijf op welke **3 sensoren** jij het belangrijkst vindt om te bewaken
- Temperatuur? Trillingen? Druk? Energieverbruik?
- **Neem dit mee** naar de volgende bijeenkomst

</v-click>

<v-click>

### Doe ook:

Vraag de onderhoudsmonteur: **welke storingen** kwamen het afgelopen half jaar het vaakst voor op mijn machine?

Schrijf het antwoord op.

</v-click>

<!-- De transferopdracht bereidt voor op Module 2 (Train): daar gaan ze hun eigen sensordata gebruiken. De vraag aan de monteur maakt bewust welke patronen er al zijn. -->

---
layout: end
---

# Minder brandjes blussen

Een AI-systeem dat afwijkingen meldt, geeft jou de kans om in te grijpen **voordat** het misgaat.

**Leren -- Vergelijken -- Markeren**

Volgende keer: jullie eigen sensoren en storingen.

<!-- Eindig met de kernbelofte: minder onverwachte stilstand, minder stress. Herhaal de 3 stappen. -->
