---
id: ko-smart-mfg-524
title: 'Van pilot naar productie: AI-inspectie implementeren'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: AI-inspectie implementeren doe je in drie fases. Eerst een pilot op 1 productielijn,
  dan uitrol naar meer lijnen, en uiteindelijk AI-inspectie als standaard werkwijze.
  Elke fase heeft eigen succesfactoren en valkuilen.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 412-420
status: validated
updated_at: '2026-05-20'
correlation_id: ronde25-lo-smart-mfg-524
---

# Van pilot naar productie: AI-inspectie implementeren

Je hebt je kwaliteitsprobleem gekozen, trainingsdata gemaakt en een business case berekend. Nu moet het ook echt gaan werken. Dat doe je in drie fases: pilot, uitrol, standaard.

## Fase 1: Pilot op 1 lijn (2-3 maanden)

Start klein. Kies de lijn waar je de meeste impact verwacht (je hebt dit in de probleemanalyse bepaald).

### Wat je doet

| Actie | Waarom |
|---|---|
| Camera **naast** de bestaande inspecteur plaatsen | Beide controleren — je vergelijkt resultaten |
| AI-resultaten dagelijks vergelijken met inspecteur | Je ziet waar de AI goed is en waar niet |
| Wekelijks de prestaties meten | Detectiepercentage en valse alarmen bijhouden |
| Feedback van operators verzamelen | Zij weten waar het systeem niet klopt |

### Succesfactoren

- **Niet meteen de inspecteur vervangen**: de AI draait eerst mee als tweede paar ogen
- **Duidelijke KPI's afspreken**: wanneer is de pilot geslaagd? (bijv. >90% detectie, <10% vals alarm)
- **Operators betrekken**: zij kennen de producten het best. Hun feedback verbetert het model.
- **Wekelijks bijsturen**: drempelwaarde aanpassen, extra trainingsdata toevoegen

### Veelgemaakte fouten

- Te snel willen uitrollen ("het werkt al na 2 weken!")
- Geen duidelijke stop/go criteria
- Operators niet betrekken bij de evaluatie
- Model niet bijtrainen na nieuwe producttypen of defecten

## Fase 2: Uitrol naar meer lijnen (1-2 maanden)

Als de pilot succesvol is (KPI's gehaald), rol je uit.

### Wat je doet

| Stap | Actie |
|---|---|
| 1 | Resultaten pilot presenteren aan management en operators |
| 2 | Camera's plaatsen op 2-3 extra lijnen |
| 3 | Per lijn trainingsdata maken (andere producten = andere foto's nodig) |
| 4 | Per lijn drempelwaarden instellen |
| 5 | Operators op nieuwe lijnen trainen in het systeem |

### Let op

- **Andere lijn = andere producten = ander model**. Je kunt niet zomaar het model van lijn 3 op lijn 1 zetten.
- **Standaardiseer het proces**: maak een checklist voor camera-opstelling, labelen en configuratie.
- **Wijs een eigenaar aan**: wie bewaakt de kwaliteit van de AI-inspectie?

## Fase 3: Standaard werkwijze (doorlopend)

AI-inspectie is nu de norm. Maar een model heeft onderhoud nodig.

### Doorlopende taken

| Taak | Frequentie |
|---|---|
| Prestaties monitoren (detectie, vals alarm) | Wekelijks |
| Model bijtrainen met nieuwe defecttypen | Per kwartaal of bij nieuwe producten |
| Hardware controleren (camera, belichting) | Maandelijks |
| Feedback van operators verwerken | Doorlopend |
| Data backup maken | Wekelijks |

### Wanneer gaat het mis?

- **Model-degradatie**: het model presteert na verloop van tijd slechter. Oorzaak: producten veranderen, nieuwe defecttypes verschijnen. Oplossing: regelmatig bijtrainen.
- **Vertrouwen verdwijnt**: operators gaan het AI-systeem negeren. Oorzaak: te veel valse alarmen. Oplossing: drempelwaarde bijstellen, operators betrekken.
- **Geen eigenaar**: niemand voelt zich verantwoordelijk voor het systeem. Oplossing: wijs iemand aan die het systeem bewaakt.

## Praktijkvoorbeeld

*Fictieve illustratie ter onderbouwing van het driefasenplan — cijfers zijn plausibel maar niet terug te voeren op één specifieke casus.*

Een fabrikant van aluminium profielen volgt het driefasenplan. Pilot op lijn 3: na 6 weken vindt de AI 92% van de defecten (inspecteur: 85%). Ze kiezen voor AI als eerste screening, inspecteur controleert twijfelgevallen. Uitrol naar lijn 1 en 5. Na 6 maanden is AI-inspectie standaard op 3 lijnen. De kwaliteitsmanager monitort wekelijks en het model wordt elk kwartaal bijgetraind.
