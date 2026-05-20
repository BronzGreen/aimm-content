---
id: ko-smart-mfg-514
title: 'Het model verbeteren: meer data, betere labels, bijstellen'
type: tip
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Een vision-model wordt beter door iteratief te verbeteren. Analyseer de fouten,
  voeg gerichte data toe, verbeter labels en hertest. Het model is nooit af — het
  wordt steeds een beetje beter.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-412
status: validated
updated_at: '2026-05-20'
correlation_id: ronde24-lo-smart-mfg-514
---

# Het model verbeteren: meer data, betere labels, bijstellen

Een vision-model is nooit "af". Net als een machine op de productielijn heeft het **onderhoud en bijsturing** nodig. Het goede nieuws: verbeteren is een helder, herhaalbaar proces.

## De verbetercyclus

Het verbeteren van een model volgt altijd dezelfde vier stappen:

1. **Test** — draai het model op nieuwe producten en bekijk de confusion matrix
2. **Analyseer** — welke fouten maakt het model? Welk type defect mist het?
3. **Verbeter** — voeg gerichte data toe, verbeter labels, of stel de drempel bij
4. **Hertest** — draai het model opnieuw en vergelijk de resultaten

Herhaal dit totdat het model goed genoeg is voor jouw situatie.

## Drie manieren om te verbeteren

### 1. Meer data toevoegen

Als het model een bepaald type defect mist, voeg dan **meer foto's van dat type** toe.

- Het model mist kleine krassen? Maak 50 extra foto's van kleine krassen.
- Het model verwart schaduwen met defecten? Maak foto's met verschillende belichting en label ze als "goed".
- Er verschijnt een nieuw type defect? Label foto's van het nieuwe defect en hertrainen.

**Vuistregel:** voeg niet zomaar meer foto's toe. Voeg **gerichte** foto's toe van wat het model fout doet.

### 2. Labels verbeteren

Soms zit het probleem niet in de hoeveelheid data, maar in de **kwaliteit van de labels**.

Controleer:
- Zijn alle labels correct? Een verkeerd label leert het model de verkeerde dingen.
- Zijn de labels consistent? Spreek duidelijke criteria af met je team.
- Zijn de categorieën logisch? Misschien moet je "defect" opdelen in specifiekere types.

### 3. Drempelwaarde bijstellen

Soms hoef je het model niet te hertrainen — je kunt de **drempelwaarde** aanpassen.

- Te veel gemiste defecten? Verlaag de drempel (strenger).
- Te veel valse alarmen? Verhoog de drempel (soepeler).
- Of: maak de twijfelzone breder (meer producten naar handmatige controle).

## Wanneer is het "goed genoeg"?

Er is geen perfect model. De vraag is: **is het beter dan de huidige situatie?**

| Vergelijk met | Vraag |
|---|---|
| **Handmatige controle** | Vindt het model meer defecten dan een operator na 6 uur werken? |
| **Kosten** | Wegen de gemiste defecten op tegen de kosten van valse alarmen? |
| **Veiligheid** | Is de recall hoog genoeg voor jouw product? |

**Vuistregel voor de maakindustrie** *(richtgetallen uit industriepraktijk — ijken per product en risicoprofiel)*:
- Veiligheidsonderdelen: recall > 95%
- Standaard kwaliteitscontrole: recall > 85%, precision > 80%
- Cosmetische controle: precision > 90%

## Het model blijft leren

Een vision-model is een levend systeem:

- **Nieuwe producten** = nieuwe foto's nodig
- **Nieuwe defecten** = hertraining nodig
- **Veranderingen in productieproces** (ander materiaal, andere machine) = hervalidatie nodig

Plan periodieke hervalidatie in — net als je dat doet voor meetinstrumenten op de lijn.

## Praktijkvoorbeeld

*Fictieve illustratie van het hertrainings-patroon — plausibele cijfers, geen specifieke casus.*

Na de eerste test van een vision-model voor lakdefecten blijkt dat het model krassen goed vindt (recall 95%) maar kleurafwijkingen vaak mist (recall 60%). De operator maakt 80 extra foto's van kleurafwijkingen en voegt die toe aan de trainingsset. Na hertraining stijgt de recall voor kleurafwijkingen naar 85%. Een maand later verschijnt een nieuw type defect (luchtbellen in de lak) dat het model niet kent. De operator labelt 50 foto's van luchtbellen, hertraint het model, en het systeem herkent ook dit defect.
