---
id: lo-ai-fund-133-trainee
knowledge_object_id: ko-ai-fund-133
version: trainee
title: Classificatie — AI die producten of signalen in categorieen indeelt
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 40
status: validated
updated_at: '2026-05-20'
correlation_id: ronde12-lo-ai-fund-133
---

# Wat doet een AI-systeem als het 'goed' of 'afgekeurd' zegt — en wat doe jij bij twijfel?

Op steeds meer werkvloeren staat een camera of sensor die producten automatisch sorteert. Goed of afgekeurd. Kras of barst. Het scherm geeft een uitslag — maar wat staat daar nou eigenlijk? En vooral: wat doe jij als het systeem niet zeker is?

## Wat leer je?

Je kunt uitleggen wat classificatie (indeling in categorieën) is. Je herkent het verschil tussen binair (twee opties) en multi-class (meerdere opties). En je weet wat te doen bij een twijfelgeval.

## Wat is classificatie?

Classificatie is een AI-taak waarbij het model een **etiket** plakt op een ding. Geen getal — een categorie.

Een paar voorbeelden van de werkvloer:

- Een camera boven de lopende band kijkt naar een metalen plaatje en zegt: **"goed"** of **"afgekeurd"**.
- Een inspectiesysteem ziet een afgekeurd onderdeel en zegt: **"kras"**, **"barst"**, **"kleurfout"** of **"vormafwijking"**.
- Een sensor op een machine geeft door: **"normaal bedrijf"** of **"storing type B"**.

Dat etiket — dat is de klasse. Daar gaat het in dit leerobject om.

### Twee smaken: binair en multi-class

Er zijn twee soorten classificatie:

1. **Binair** (twee opties) — bijvoorbeeld goed/afgekeurd, OK/NOK, aan/uit. Het model kiest tussen twee klassen.
2. **Multi-class** (meerdere opties) — bijvoorbeeld kras / barst / kleurfout / vormafwijking. Het model kiest uit drie of meer klassen.

Allebei werken hetzelfde: het model krijgt een ding, en geeft een etiket terug.

## Wat betekent het percentage erbij?

Bij elk etiket hoort een **zekerheid**. Bijvoorbeeld:

> "Klasse: braam gedetecteerd — zekerheid 92%"

Hier zit een valkuil. Die 92% zegt **niet** dat 92% van het product een braam is. Het zegt: het model is voor 92% zeker dat dit een braam is. Het gaat over het vertrouwen van het model in zijn eigen antwoord.

Bij hoge zekerheid (boven 90%) kun je de uitslag bijna altijd volgen. Bij lage zekerheid wordt het interessant.

## Wat doe je bij twijfel?

Stel dat het systeem dit zegt over een metalen frame:

> "Klasse: goed — zekerheid 60%"
> "Klasse: vormafwijking — zekerheid 40%"

Het model leunt naar "goed", maar nauwelijks. Dit is een twijfelgeval. Wat doe je nu?

Drie opties:

- **Doorlaten** — als een afwijking op dit product weinig kost, en je vertrouwt het systeem grotendeels.
- **Handmatig nakijken** — bijna altijd de veilige keuze, vooral bij veiligheidscomponenten of dure onderdelen.
- **De instelling aanpassen** — bespreek met je teamleider of de drempel voor "afgekeurd" moet verschuiven.

Er is geen vast getal voor "hoog genoeg". Dat hangt af van wat een fout kost. Een doorgelaten kras op een sierdeel is iets anders dan op een remblok. Jouw kennis van de lijn maakt hier het verschil.

## Het verschil met regressie

Classificatie geeft altijd een **klasse** terug. Een etiket. Geen getal.

Er bestaat ook AI die een getal voorspelt — bijvoorbeeld "deze machine gaat over 23 dagen stuk." Dat heet regressie, en dat is een ander type taak. Komt later terug in een volgend leerobject.

Korte vuistregel: als het antwoord een **woord** of **categorie** is, is het classificatie. Als het antwoord een **getal** is, is het regressie.

## Na deze sessie

Loop deze week eenmaal langs een kwaliteits- of inspectiesysteem op je eigen lijn. Dat kan een camera boven de lopende band zijn, een dashboard met goed/afgekeurd-meldingen, of een storingsclassificatie van een machine. Noteer drie dingen: welk type classificatie het is (binair of multi-class), welke klassen het systeem kent (bijvoorbeeld goed / braam / maatafwijking), en de laagste zekerheid die je deze week tegenkomt. Neem je notities mee naar de volgende sessie. Vraag ook even aan een collega: *"Wat doe jij als het systeem twijfelt?"* Je ontdekt vaak dat iedereen op zijn eigen manier omgaat met die grijze gevallen — en dat is een mooi gesprek voor het hele team.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-binair-voorbeeld.md`](./werkbladen/wb-01-binair-voorbeeld.md) — Binair voorbeeld
2. [`wb-01-ervaren-eerste-classificatie.md`](./werkbladen/wb-01-ervaren-eerste-classificatie.md) — Ervaren eerste classificatie
3. [`wb-02-multi-class.md`](./werkbladen/wb-02-multi-class.md) — Multi class
4. [`wb-02-reflecteren-vier-foto-s.md`](./werkbladen/wb-02-reflecteren-vier-foto-s.md) — Reflecteren vier foto s
5. [`wb-03-handout-classificatie.md`](./werkbladen/wb-03-handout-classificatie.md) — Handout classificatie
6. [`wb-03-theoretiseren-twee-smaken.md`](./werkbladen/wb-03-theoretiseren-twee-smaken.md) — Theoretiseren twee smaken
7. [`wb-04-experimenteren-twijfelgeval.md`](./werkbladen/wb-04-experimenteren-twijfelgeval.md) — Experimenteren twijfelgeval
8. [`wb-04-twijfelgeval.md`](./werkbladen/wb-04-twijfelgeval.md) — Twijfelgeval

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-133`](../../kennisbank/ai_fundamentals/supervised_vs_unsupervised/ko-ai-fund-133.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
