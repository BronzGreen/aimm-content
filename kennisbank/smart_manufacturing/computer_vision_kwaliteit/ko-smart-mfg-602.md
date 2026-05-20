---
id: ko-smart-mfg-602
title: Het universele patroon van elk AI-camerasysteem
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Elk AI-camerasysteem — van Google tot jouw productielijn — werkt volgens
  hetzelfde patroon van vier stappen. Als je het patroon herkent, begrijp je elk systeem.
  En zie je waar het stuk kan.
source_centrality: 0.7
source_ref: RLC-Oost (2026). Workshop w00 — Waarom computer vision? (AI Vision Learning
  Community), blok 3-4
status: validated
updated_at: '2026-05-20'
correlation_id: ronde25-lo-smart-mfg-602
---

# Het universele patroon van elk AI-camerasysteem

Je hoeft geen ingenieur te zijn om een AI-camerasysteem te begrijpen. Elk systeem — of het nu Google reCAPTCHA is, de zelfrijdende auto's van Waymo, of de inspectiecamera in jullie hal — werkt volgens hetzelfde patroon.

### Het patroon in vier stappen

```
CAMERA  →  BEELD  →  MODEL  →  BESLISSING
```

**Stap 1 — Camera (of sensor).** Iets maakt een foto of meting. Bij jullie inspectiecamera is dat een lens boven de lopende band. Bij een zelfrijdende auto zijn het acht camera's plus radar. Bij Google reCAPTCHA was het de camera in Street View.

**Stap 2 — Beeld.** Dat ruwe beeld gaat naar het systeem. Een digitale foto, een videostream, of een stuk sensordata.

**Stap 3 — Model.** Het AI-model kijkt naar het beeld en beslist: *'dit is een goede beugel'* of *'dit is een kras'*. Het model is eerder getraind — daar komen we zo op.

**Stap 4 — Beslissing.** Het systeem doet iets met de uitkomst. Afkeuren via een afvoerklep. Alarm bij de operator. Een automatische aanpassing in het volgende proces.

### De onzichtbare stap: trainingsdata

Wat je niet ziet als het systeem draait, maar wat alles bepaalt:

```
TRAININGSDATA (gelabelde foto's)
    →  MODEL WORDT BETER
        →  BETERE BESLISSINGEN
```

Deze stap is eenmalig gebeurd vóórdat het systeem live ging. Maar als het aantal foto's te klein was, of de labels niet consistent, dan zie je dat terug in de beslissingen — met meer fout-alarmen of gemiste defecten.

### Waar kan het stuk?

Elk component heeft een faalpunt. Herken ze en je weet welke vraag te stellen:

| Component | Wat kan er stuk? | Welke vraag stel je? |
|-----------|------------------|----------------------|
| Camera | Vuil op de lens, verkeerde belichting, trillingen | *Hoe vaak wordt de lens schoongemaakt?* |
| Beeld | Te lage resolutie, compressie, verkeerd uitsnede | *Zien wij dezelfde foto als het model?* |
| Model | Niet getraind op nieuwe productserie of nieuw defect | *Wanneer is dit model voor het laatst bijgetraind?* |
| Beslissing | Drempel te streng of te soepel | *Wat doet het systeem bij twijfel?* |
| Trainingsdata | Te weinig, te oud, inconsistent gelabeld | *Welke foto's zijn gebruikt en wie heeft ze gelabeld?* |

### Wat dit voor jou betekent

Als een leverancier komt praten over 'een AI-oplossing', hoef je niet te knikken. Je tekent het patroon op papier en stelt één vraag per vakje. Vijf vragen. Als de leverancier niet op alle vijf antwoord heeft, weet je dat je bij de verkeerde kant van het gesprek zit.

Het patroon is hetzelfde bij reCAPTCHA en bij jullie lopende band. Alleen de context verschilt. En het verschil in context — wie de camera ophangt, wie de foto's labelt, wie de beslissing accepteert — daar zit jouw rol.


## Praktijkvoorbeeld

Stel: de inspectiecamera boven lopende band 3 begint plotseling meer goede beugels af te keuren dan normaal. Je gaat het patroon langs:

(1) Camera — is er stof op de lens? Ja, blijkt poeder van een aanpassing gisteren. Schoonmaken.

Werkt het nog niet beter? Door naar het volgende vakje.

(2) Beeld — wordt de foto goed uitgesneden? Check: de beugel staat iets anders op de band dan vorige week. De camera hoek is onveranderd maar de beugel-positie is verschoven door een andere aanvoer.

(3) Model — is dit model getraind op deze positie? Nee, de originele trainingsdata had de beugels centraal. Het model herkent de verschoven beugel als 'afwijkend' en keurt af.

Oplossing: óf de aanvoer herstellen, óf 50 nieuwe foto's maken van de verschoven positie en het model laten bijtrainen. Welke keuze beter is, is een beslissing voor de teamleider — maar jij kunt nu uitleggen waaróm er een keuze nodig is.
