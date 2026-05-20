---
id: ko-smart-mfg-204
title: 'Je eerste predictief model configureren: een stapsgewijze handleiding'
type: framework
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een handleiding in vijf stappen waarmee een operator zelf een eenvoudig predictief
  model configureert, van machinekeuze tot werkend systeem.
source_centrality: 0.7
source_ref: AIMM Competentieframework v0.1
status: validated
updated_at: '2026-05-20'
correlation_id: ronde17-lo-smart-mfg-204
---

# Je eerste predictief model configureren: een stapsgewijze handleiding

Je hebt geleerd hoe je sensordata leest, drempelwaarden instelt en anomaliescores interpreteert. Nu ga je het **zelf doen**: een eenvoudig predictief model opzetten voor een machine op jouw werkvloer. Geen programmeerkennis nodig — je configureert het systeem stap voor stap.

### Stap 1: Kies je machine

Begin niet met de nieuwste of de duurste machine. Kies de machine met de **meeste ongeplande stilstand** in de afgelopen 3 maanden. Waarom? Daar heb je het meeste te winnen. En als het model daar werkt, is de meerwaarde direct zichtbaar.

Hoe kies je:
- Vraag de storingshistorie op bij de technische dienst.
- Kijk naar de OEE-cijfers: welke machine scoort het laagst op beschikbaarheid?
- Kies een machine waar je zelf mee werkt, zodat je de resultaten kunt beoordelen.

### Stap 2: Bepaal welke sensoren je gebruikt

De meeste machines hebben meerdere sensoren. Begin met de **drie belangrijkste**:
- **Temperatuur**: wijst op slijtage, smeringsproblemen, overbelasting.
- **Trillingen**: wijst op lagerdefecten, onbalans, losse onderdelen.
- **Druk**: wijst op lekkages, filtervervuiling, pompdefecten.

Niet elke machine heeft alle drie. Gebruik wat beschikbaar is. Twee sensoren is genoeg om te beginnen.

### Stap 3: Verzamel 2 weken normaaldata

Laat de sensoren 2 weken meten terwijl de machine normaal draait. Dit is je **trainingsdata** — het model leert hiervan wat normaal is.

Belangrijk:
- Draai zoveel mogelijk onder **standaard omstandigheden** (normaal product, normale snelheid).
- Noteer afwijkingen (productwissel, onderhoud, storing) zodat je die data later kunt uitsluiten.
- 2 weken is het minimum. Langer is beter, maar je wilt ook snel resultaat zien.

### Stap 4: Stel drempelwaarden in

Gebruik de methode uit ko-smart-mfg-202:
- Bereken het gemiddelde en de spreiding van je 2 weken data.
- Stel de waarschuwingsdrempel in op gemiddelde + 1.5x spreiding.
- Stel de alarmdrempel in op gemiddelde + 2x spreiding.
- Configureer een vertraging van minimaal 5 seconden (korte pieken negeren).

### Stap 5: Test een week en stel bij

Nu begint het echte werk. Laat het model een week draaien en houd bij:
- Hoeveel waarschuwingen krijg je per dag?
- Hoeveel daarvan zijn **vals alarm** (de machine draait prima)?
- Heb je een **echt probleem gemist** (storing zonder voorafgaand alarm)?

Vuistregels voor bijstellen:
- Meer dan 3 valse alarmen per dag? Drempels iets omhoog.
- Een storing gemist? Drempels omlaag of extra sensor toevoegen.
- Na bijstelling weer een week testen.

Na 2-3 rondes van bijstellen heb je een werkend model dat je **vertrouwt**.


## Praktijkvoorbeeld

Een operator bij een verpakkingslijn kiest de sealmachine — die stond vorige maand twee keer ongepland stil. Hij selecteert de temperatuursensor (sealbalken) en de trillingssensor (aandrijfmotor). Twee weken lang verzamelt hij normaaldata. Op maandag van week 3 stelt hij de drempels in: sealtemperatuur gemiddeld 185 graden, spreiding 3 graden, alarm op 191 graden. Trillingen gemiddeld 0.4 mm/s, alarm op 0.7 mm/s. In de testweek krijgt hij 4 valse alarmen op trillingen — steeds bij het opstarten. Hij voegt een vertraging van 30 seconden toe. Op donderdag scoort de temperatuur 189 graden en blijft stijgen. Hij plant een inspectie: het verwarmingselement vertoont slijtage. Vervanging op vrijdagochtend, gepland. Totale configuratietijd: 5 werkdagen verspreid over 3 weken.
