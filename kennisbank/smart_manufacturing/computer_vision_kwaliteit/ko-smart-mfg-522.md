---
id: ko-smart-mfg-522
title: 'Eigen trainingsdata maken: foto''s van jouw producten'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Om AI-inspectie op jouw producten te laten werken, heb je trainingsdata nodig
  van jouw eigen productielijn. Je maakt een camera-opstelling, zorgt voor consistente
  belichting, maakt genoeg foto's per defecttype, en labelt ze met je team.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-412
status: validated
updated_at: '2026-05-20'
correlation_id: ronde24-lo-smart-mfg-522
---

# Eigen trainingsdata maken: foto's van jouw producten

In Module 2 heb je geleerd hoe je foto's labelt en een model configureert — met voorbeeldfoto's. Nu ga je het doen met **jouw eigen producten**. Dat betekent: een camera-opstelling bouwen, foto's maken, en samen labelen.

## Stap 1: Camera-opstelling bouwen

Je hebt geen dure apparatuur nodig. Een eenvoudige opstelling werkt al:

| Onderdeel | Optie | Waarom |
|---|---|---|
| **Camera** | Smartphone op statief | Vaste hoogte en hoek = consistente foto's |
| **Achtergrond** | Wit vel papier of doek | Geen afleidende rommel op de achtergrond |
| **Verlichting** | 2 lampen aan weerszijden | Geen schaduwen, gelijkmatig licht |
| **Positie** | Markering op tafel | Elk product op dezelfde plek |

**Vuistregel:** als alle foto's eruitzien alsof ze door dezelfde machine zijn gemaakt, is de opstelling goed.

### Veelgemaakte fouten

- **Wisselend licht**: een raam in de buurt zorgt voor schaduwverschillen per tijdstip. Gebruik kunstlicht.
- **Wisselende afstand**: zonder statief maak je de ene foto van dichtbij, de andere van ver. Gebruik een vast punt.
- **Rommelige achtergrond**: gereedschap, andere producten of handen in beeld verwarren het model.

## Stap 2: Hoeveel foto's heb je nodig?

Meer is beter, maar kwaliteit gaat voor kwantiteit:

| Doel | Minimum foto's | Ideaal |
|---|---|---|
| Simpel (goed vs. defect) | 100 totaal | 200-300 |
| Per defecttype | 50 per type | 100 per type |
| Subtiele defecten | 100 per type | 200+ per type |

**Belangrijk:** zorg voor een **goede balans**. Niet 190 goede en 10 defecte foto's — dan leert het model dat alles goed is. Streef naar minimaal 30% defecte foto's *(vuistregel class balance; exacte ratio afhankelijk van defectzeldzaamheid)*.

## Stap 3: Samen labelen met je team

Labelen doe je niet alleen. Werk met je team:

1. **Spreek labelcriteria af**: wanneer is iets een defect? Hoe groot moet een kras zijn? Schrijf het op.
2. **Label samen**: iedereen labelt dezelfde foto's. Vergelijk de labels.
3. **Check steekproefsgewijs**: pak 20 gelabelde foto's en laat een collega opnieuw labelen. Komen jullie op hetzelfde uit?

### Waarom samen labelen?

In Module 2 ontdekte je dat je buurman soms anders labelt. Datzelfde probleem speelt bij je eigen producten. Door samen criteria af te spreken en steekproefsgewijs te controleren, wordt je dataset betrouwbaar.

## Stap 4: Verdeel in trainingsset en testset

Net als in Module 2:

- **80% trainingsset**: het model leert hiervan
- **20% testset**: hiermee controleer je het model

*80/20 is gangbare ML-conventie (Géron 2019, Hands-On ML). Grote datasets: soms 90/10, kleine sets: 70/30.*

**Let op:** zorg dat beide sets een goede mix hebben van goede en defecte producten.

## Praktijkvoorbeeld

Een team van 3 operators bij een kunststofverwerker bouwt een eenvoudige foto-opstelling: witte achtergrond, twee lampen, telefoon op statief. Ze spreken af: een kras langer dan 2mm is een defect. In 3 dagen maken ze 300 foto's (150 goed, 150 defect). Ze labelen samen en controleren steekproefsgewijs. Resultaat: een bruikbare dataset voor hun eerste AI-model.
