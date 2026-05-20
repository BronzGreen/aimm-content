---
id: ko-smart-mfg-202
title: 'Drempelwaarden instellen: wanneer moet het systeem alarm slaan?'
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een procedure in vier stappen om drempelwaarden voor sensoren te bepalen,
  in te stellen en bij te stellen op basis van praktijkervaring.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1
status: validated
updated_at: '2026-05-20'
correlation_id: ronde15-lo-smart-mfg-202
---

# Drempelwaarden instellen: wanneer moet het systeem alarm slaan?

Een sensor meet continu, maar wanneer is een waarde **echt afwijkend**? Dat bepaal je met een **drempelwaarde** — de grens waarbij het systeem een waarschuwing geeft. Te laag ingesteld krijg je te veel valse alarmen. Te hoog ingesteld mis je echte problemen.

Met deze vier stappen stel je een goede drempelwaarde in.

### Stap 1: Normaalwaarden verzamelen (100 cycli meten)

Voordat je een drempel kunt instellen, moet je weten wat normaal is. Meet de sensor tijdens **minimaal 100 productiecycli** onder normale omstandigheden.

- Gebruik dezelfde productinstellingen (materiaal, snelheid, gereedschap).
- Meet op verschillende momenten van de dag (begin shift, midden, eind).
- Schrijf alle waarden op of exporteer ze uit het systeem.

### Stap 2: Bandbreedte bepalen

Bereken uit je meetwaarden:
- Het **gemiddelde** (alle waarden optellen, delen door het aantal).
- De **spreiding** (hoe ver wijken waarden af van het gemiddelde?).
- Een vuistregel: de drempel zet je op het **gemiddelde plus twee keer de spreiding**. Dit vangt 95% van de normale variatie op *(2-sigma-regel uit de statistiek — geldt voor normaalverdeelde data; bij scheve verdelingen kies je andere drempels)*.

Voorbeeld: gemiddelde trilling = 0.3 mm/s, spreiding = 0.1 mm/s.
Drempel = 0.3 + (2 x 0.1) = **0.5 mm/s**.

### Stap 3: Drempel instellen in het systeem

Voer de berekende drempelwaarde in het monitoringsysteem in. De meeste systemen hebben twee niveaus:
- **Waarschuwing** (geel): de waarde komt in de buurt van de drempel. Je gaat extra letten op deze sensor.
- **Alarm** (rood): de waarde overschrijdt de drempel. Actie is nodig.

Stel de waarschuwing in op 80% van de drempel en het alarm op 100%.

### Stap 4: Testen en bijstellen

Geen drempelwaarde is meteen perfect. Na het instellen:
- Draai minimaal **1 week** met de nieuwe drempels.
- Houd bij hoeveel **valse alarmen** je krijgt (alarm terwijl de machine prima draait).
- Houd bij of je **gemiste problemen** hebt (storing zonder voorafgaand alarm).
- Stel bij: te veel valse alarmen? Drempel iets omhoog. Gemist probleem? Drempel omlaag.


## Praktijkvoorbeeld

Een operator stelt drempelwaarden in voor een trillingssensor op een draaibank. Na 100 cycli meten is het gemiddelde 0.3 mm/s met een spreiding van 0.1 mm/s. Hij stelt de drempel in op 0.5 mm/s. In de eerste week krijgt hij 12 valse alarmen — te veel. Na overleg met de technische dienst blijkt dat bij het wisselen van gereedschap de trillingen kort oplopen. Hij past de drempel aan naar 0.8 mm/s en voegt een vertraging van 10 seconden toe (het alarm gaat pas af als de waarde langer dan 10 seconden boven de drempel blijft). Daarna krijgt hij nog maar 1 vals alarm per week, en het systeem detecteert succesvol een slijtend lager twee dagen voor de geplande vervanging.
