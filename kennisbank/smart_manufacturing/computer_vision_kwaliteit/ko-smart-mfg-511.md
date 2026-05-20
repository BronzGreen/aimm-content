---
id: ko-smart-mfg-511
title: 'Trainingsdata labelen: goede en defecte producten markeren'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Een AI-model voor kwaliteitscontrole leert van gelabelde foto's. Je maakt
  consistente foto's, labelt ze als goed of defect, en verdeelt ze in een trainingsset
  en een testset.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-412
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-511
---

# Trainingsdata labelen: goede en defecte producten markeren

Een AI-model voor kwaliteitscontrole leert van **gelabelde foto's**. Dat betekent: foto's waarvan jij hebt aangegeven of het product goed of defect is. Hoe beter je labels, hoe beter het model leert.

## Stap 1: Maak consistente foto's

Goede trainingsdata begint bij goede foto's. Let op drie dingen:

- **Licht**: altijd dezelfde belichting. Wisselend licht zorgt voor schaduwverschillen die het model in de war brengen.
- **Achtergrond**: gebruik een effen achtergrond. Rommel op de achtergrond leidt het model af.
- **Hoek**: fotografeer elk product vanuit dezelfde hoek en afstand.

**Vuistregel:** als jij het verschil tussen twee foto's niet kunt zien behalve het defect, dan is de foto goed genoeg.

## Stap 2: Label elke foto

Geef elke foto een label:

- **Goed** — het product voldoet aan de kwaliteitseisen
- **Defect** — het product heeft een gebrek. Noteer ook het **type** defect (kras, deuk, kleurafwijking, ontbrekend onderdeel)

### Hoeveel foto's heb je nodig?

Als richtlijn:

| Situatie | Minimum aantal foto's |
|---|---|
| Eenvoudig (goed vs. defect) | 100-200 totaal |
| Meerdere defecttypes | 50-100 per type |
| Subtiele defecten | 200+ per type |

Meer foto's = beter model, maar de **kwaliteit** van je labels is belangrijker dan de **hoeveelheid**.

### Veelgemaakte fouten bij labelen

- **Inconsistente labels**: de ene keer is een kleine kras "goed", de andere keer "defect". Spreek duidelijke criteria af.
- **Te weinig defecten**: als je 190 goede en 10 defecte foto's hebt, leert het model dat alles goed is. Streef naar minimaal 30% defecte foto's *(vuistregel uit ML-praktijk voor class balance; exacte ratio hangt af van defectzeldzaamheid)*.
- **Verkeerde labels**: een foto van een goed product die per ongeluk als "defect" is gelabeld. Het model leert dan de verkeerde dingen.

## Stap 3: Verdeel in trainingsset en testset

Verdeel je gelabelde foto's in twee groepen:

- **Trainingsset** (80%): hier leert het model van
- **Testset** (20%): hiermee controleer je of het model goed werkt

*De 80/20-verdeling is een breed gehanteerde ML-conventie (zie o.a. Géron 2019, Hands-On ML, hfd. 2); grote datasets gebruiken soms 90/10, kleine sets een 70/30.*

**Belangrijk:** de testset mag het model nooit zien tijdens het trainen. Anders test je niet of het model nieuwe producten kan beoordelen — je test alleen of het zijn huiswerk heeft geleerd.

## Praktijkvoorbeeld

Bij een fabrikant van kunststof behuizingen maakt een operator 200 foto's van behuizingen: 100 goede en 100 met defecten (krassen, deuken, kleurafwijkingen). Elke foto krijgt een label: 'goed' of 'defect — kras' of 'defect — deuk'. Van de 200 foto's gaan er 160 naar de trainingsset (het model leert hiervan) en 40 naar de testset (om te controleren of het model goed werkt). De operator ontdekt dat foto's met wisselend licht slechte resultaten geven — consistente belichting blijkt cruciaal.
