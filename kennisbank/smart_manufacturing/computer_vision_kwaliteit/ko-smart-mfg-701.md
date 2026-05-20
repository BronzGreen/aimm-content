---
id: ko-smart-mfg-701
title: 'Confidence: hoe zeker is het AI-systeem van zijn oordeel?'
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Een AI-camerasysteem zegt niet alleen 'goed' of 'kras' — het geeft ook aan
  hoe zeker het is. Die zekerheid (confidence) in procenten bepaalt welke beslissingen
  jij als operator moet nemen, en welke het systeem alleen mag nemen.
source_centrality: 0.7
source_ref: Op basis van standaard computer vision concepten, aangevuld met inzichten
  uit RLC-Oost w02-w03 materiaal
status: validated
updated_at: '2026-05-20'
correlation_id: ronde26-lo-smart-mfg-701
---

# Confidence: hoe zeker is het AI-systeem van zijn oordeel?

In Module 1 hebben we gezien dat een AI-model foto's kan herkennen — als er genoeg gelabelde voorbeelden zijn. Maar een model zegt nooit gewoon 'goed' of 'afkeuren'. Het geeft een **confidence-score** mee: een percentage dat aangeeft hoe zeker het van zijn oordeel is.

### Wat is confidence?

Stel het systeem krijgt een foto. Het model kijkt en zegt intern:

- 'Ik ben 95% zeker dat dit goed is.'
- 'Ik ben 70% zeker dat dit een kras is.'
- 'Ik ben 52% zeker dat dit een deuk is, 48% zeker dat het goed is.'

Die eerste zit dicht bij zekerheid. De tweede twijfelt. De derde twijfelt écht.

### Waarom dit belangrijk is

Een systeem dat alleen 'goed/fout' zegt verbergt de twijfel. Een systeem met confidence maakt de twijfel zichtbaar — en geeft jou de mogelijkheid om **te beslissen wat er met twijfelgevallen gebeurt**.

Drie keuzes zijn mogelijk:

- **Automatisch afkeuren** (bij alle twijfel) — veilig, maar je verspilt goede producten
- **Automatisch doorlaten** (bij alle twijfel) — snel, maar je mist defecten
- **Naar operator sturen** (bij twijfel) — beste kwaliteit, kost tijd

### De drempel

Die keuze ligt vast in een **drempel**. Bijvoorbeeld: 'bij < 90% confidence, stuur naar operator'. Onder de 90% doet het systeem niks zelf — dan mag jij beslissen.

Wie stelt die drempel in? Vaak de leverancier, bij installatie. Maar jij als operator hebt de beste informatie om te beoordelen of die drempel klopt. Als het systeem te vaak alarm slaat over goede producten, is de drempel te streng. Als het defecten laat glippen, is hij te soepel.

### De trade-off

Elke keuze kost iets. Strenge drempel (bijv. <98%) → meer alarmen bij de operator → meer werk → minder kans op gemiste defecten. Soepele drempel (bijv. <60%) → minder werk voor jou → meer kans dat iets doorglipt.

Er is geen 'goede drempel' voor elke situatie. De drempel hangt af van hoe duur een gemist defect is, hoeveel tijd een operator kan besteden aan twijfelgevallen, en hoeveel productie-snelheid verloren mag gaan.

### Wat dit voor jou betekent

Als je met een AI-camerasysteem werkt, is de eerste vraag die je moet kunnen beantwoorden: *wat is onze confidence-drempel, en waarom die?*. Als de beheerder dat niet weet, weet jij dat de drempel waarschijnlijk op de standaard-waarde van de leverancier staat — en die is bijna nooit optimaal voor jullie product.


## Praktijkvoorbeeld

Stel: jullie drempel staat op 80%. Het systeem keurt deze week 40 producten af, waarvan 30 echte defecten hadden en 10 goede waren. Een false-alarm-percentage van 25%.

Je overlegt met je teamleider. Ze kiezen voor een drempel van 70% — strengere drempel, minder twijfel doorgestuurd, maar ook strenger oordeel bij randgevallen.

Volgende week: 45 producten afgekeurd, waarvan 38 echte defecten en 7 goede. False-alarms van 25% naar 15% gedaald. Maar: productie meldt dat sommige producten worden afgekeurd die vorige week nog door kwamen. Een subtiel defect dat de klant niet ziet, wordt nu wel afgekeurd.

Is dat een verbetering? Dat hangt af van hoe jullie klant naar kwaliteit kijkt — niet van het systeem.
