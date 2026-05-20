# Eigen pipeline — teken jouw pad van sensor naar scherm
*Werkblad Kolb-fase 4 — Experimenteren*

**Naam:** ____________________  **Datum:** __________
**Component of lijn die ik kies:** ____________________________________

---

> **Voor jou**
> Je kiest één machine of lijn van jullie eigen werkvloer waar sensor-data naar een dashboard stroomt. Je tekent op een groot vel (A3) de pipeline in vier knooppunten. Daarna onderbouw je drie keuzes — latentie, volume, failover — met telkens één zin. Twijfel mag. Een vraagteken is een goede uitkomst om mee terug te brengen naar IT of je teamleider.

---

## 1. Mijn keuze — wat ga ik tekenen?

*Welke machine of lijn pak je? Beschrijf in twee zinnen wat er gemeten wordt en waarvoor de data gebruikt wordt.*

Machine of lijn:

___________________________________________________

___________________________________________________

Wat wordt er gemeten?

___________________________________________________

___________________________________________________

Waarvoor wordt de data gebruikt (dashboard, AI-model, rapportage)?

___________________________________________________

___________________________________________________

---

## 2. Teken de pipeline op A3-papier

*Op het A3-vel teken je vier vakken met pijlen ertussen. Schrijf in elk vak één tot drie woorden. Maak het klein-en-duidelijk, niet groot-en-mooi.*

```
   ________          ________          ________          ________
  |        |        |        |        |        |        |        |
  |   1.   | -----> |   2.   | -----> |   3.   | -----> |   4.   |
  |        |        |        |        |        |        |        |
  |________|        |________|        |________|        |________|

   Sensor           Edge-buffer        Opslag            Consument
                    (tussenstation)
```

Vul hieronder kort in wat in elk vak op jullie werkvloer staat. Twijfel mag — zet dan een vraagteken.

- **1. Sensor** — wat meet er, en hoeveel metingen per seconde of minuut?

___________________________________________________

___________________________________________________

- **2. Edge-buffer (tussenstation)** — is er bij jullie zoiets? Waar staat het fysiek?

___________________________________________________

___________________________________________________

- **3. Opslag** — ter plaatse op een server, of in de cloud? Hoe lang wordt data bewaard?

___________________________________________________

___________________________________________________

- **4. Consument** — wie gebruikt de data? Dashboard, AI-model, rapportage?

___________________________________________________

___________________________________________________

---

## 3. Onderbouw drie keuzes — één zin per keuze

### Keuze 1 — Latentie (vertraging)

*Hoe snel moet de data er zijn?*

- [ ] **Real-time** (onder 1 seconde)
- [ ] **Near-realtime** (onder 60 seconden)
- [ ] **Batch** (uren of dagen)
- [ ] **Weet ik nog niet** — vraag voor: ____________________

Waarom dat? Eén zin:

___________________________________________________

___________________________________________________

### Keuze 2 — Volume (hoeveelheid data)

*Wordt de data ergens samengevat, of gaat alles naar de cloud?*

- [ ] Alles gaat door — geen samenvatting
- [ ] In de edge-buffer wordt samengevat, namelijk: ______________________________________
- [ ] Weet ik niet — vraag voor: ____________________

Waarom dat? Eén zin:

___________________________________________________

___________________________________________________

### Keuze 3 — Failover (terugval bij fout)

*Wat gebeurt er als de verbinding tussen edge-buffer en opslag een uur wegvalt?*

- [ ] De edge-buffer bewaart de data en stuurt later na
- [ ] Er gaat data verloren — dat zien we terug als gat in de grafiek
- [ ] De operator krijgt een alarm
- [ ] Weet ik niet — vraag voor: ____________________

Waarom dat? Eén zin:

___________________________________________________

___________________________________________________

---

## 4. Wat heb je gemarkeerd met een vraagteken?

*Verzamel hier de vraagtekens. Dit zijn de vragen die je deze week stelt aan IT of je teamleider.*

| # | Mijn vraag | Aan wie ga ik het vragen? |
|---|------------|----------------------------|
| 1 |  |  |
| 2 |  |  |
| 3 |  |  |

---

## 5. Plenaire ronde — wat zegt de groep?

*Twee of drie deelnemers delen hun tekening. Welke verschillen vallen je op? Welk idee neem je mee?*

___________________________________________________

___________________________________________________

___________________________________________________

___________________________________________________

---

## Wat neem je mee?

*Wat de groep mee terug neemt: vier knooppunten van de pipeline, drie ontwerp-keuzes (latentie, volume, failover) en een eerste tekening van de eigen pipeline.*

*Mijn belangrijkste inzicht:*

___________________________________________________

___________________________________________________

___________________________________________________

*Eén ding dat ik deze week ga doen:*

___________________________________________________

___________________________________________________

---

> **Voor de volgende sessie:** vraag deze week aan IT of je leverancier waar de edge-buffer fysiek staat — vaak een industriële computer naast de machine. Een korte rondleiding van vijf minuten geeft je een beeld bij het abstracte begrip "tussenstation". Neem je A3-tekening en je drie vraagteken-antwoorden mee.

---
*Bron: Anaya et al. (2024), Manufacturing Digital Twin Framework; Bakopoulos et al. (2024), Digital-Twin-Enabled Framework, Ch. 5 | AIMM Industry 4.0 — Module 2 (Train) | v1.0*
