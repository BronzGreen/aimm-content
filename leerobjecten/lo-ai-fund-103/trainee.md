---
id: lo-ai-fund-103-trainee
knowledge_object_id: ko-ai-fund-103
version: trainee
title: Waarom een AI 'misschien' zegt — onzekerheid en kansen op de werkvloer
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 45
status: validated
updated_at: '2026-05-19'
correlation_id: ronde7-lo-ai-fund-103
---

# Hoe lees je een AI-kanspercentage — en wat doe je ermee op de werkvloer?

Soms zegt de inspectiecamera niet "goed" of "fout". Hij zegt: "78 procent kans op defect." Dat is verwarrend. Wat doe je met zo'n percentage? Vrij doorlaten? Handmatig controleren? Of de hele lijn stopzetten? In deze sessie leer je een eenvoudig kader om die keuze te maken.

## Wat leer je?

Je leert waarom een AI-systeem met percentages werkt in plaats van een vast "ja" of "nee". Je kunt bij een gegeven percentage een passende actie kiezen. En je weet welke afweging je maakt om de drempel goed te zetten.

## Drie producten op de lijn

Stel je voor. Een inspectiecamera boven de lopende band beoordeelt vandaag drie producten.

- **Product A** krijgt de melding: defect-kans 87 procent.
- **Product B** krijgt: defect-kans 15 procent.
- **Product C** krijgt: defect-kans 50 procent.

Wat doe je met elk product?

Bij A is de kans hoog. De meeste operators kiezen voor een handmatige check of direct afkeur.

Bij B is de kans laag. De meeste operators laten dit door.

Bij C — de 50 procent — wordt het lastig. De helft van een groep kiest voor "handmatig controleren". De andere helft twijfelt. Beide keuzes zijn te verdedigen. Hier zit de leerstof.

## Waarom werkt AI met kansen?

De wereld is onzeker. Een camera ziet ruis. De belichting verschilt. Een product hangt soms net even scheef op de lopende band. Geen enkel beeld is honderd procent helder.

Daarom rapporteert AI geen vast "ja" of "nee". Het systeem geeft een *waarschijnlijkheid* — een percentage dat aangeeft hoe zeker het is.

Wat betekent "87 procent kans op defect" eigenlijk? Het systeem heeft duizenden eerdere beelden gezien. Bij beelden die op deze leken bleek 87 op de 100 keer echt een defect. Bij 13 op de 100 niet. Het systeem rapporteert eerlijk: ik ben hier vrij zeker van, maar niet absoluut.

Bron: Russell & Norvig (2010), AI — A Modern Approach.

## Drie drempelgebieden

De meeste operators werken met drie gebieden:

| Defect-kans | Drempelgebied | Typische actie |
|---|---|---|
| 0 - 30 procent | Laag | Doorlaten, eventueel steekproef |
| 30 - 70 procent | Midden | Handmatig controleren |
| 70 - 100 procent | Hoog | Direct afkeuren of stop |

Dit zijn *vuistregels* (te valideren per bedrijf). De exacte grenzen verschillen per product en per bedrijf. Ze hangen af van twee dingen:

1. **Wat kost een gemiste fout?** Een autoremblok dat tot bij de klant komt? Een ingrediënt dat een productie-batch verpest? Een veiligheidsrisico? Hoe duurder de fout, hoe lager je drempel.
2. **Wat kost een onnodige check?** Tijd van een operator. Onderbreking van de lijn. Bij een goedkoop product met snelle visuele check is dit beperkt. Bij een ingewikkelde uit-elkaar-haal-actie is dit veel.

Hoe duurder de gemiste fout, hoe lager de drempel. Hoe duurder de check, hoe hoger de drempel.

## Terug naar de drie producten

Met dit kader wordt de keuze duidelijker.

- **Product A — 87 procent**: hoog drempelgebied. Vrijwel zeker een check of direct afkeur.
- **Product B — 15 procent**: laag drempelgebied. Doorlaten, eventueel een steekproef.
- **Product C — 50 procent**: midden. Hier hoort altijd een handmatige check.

Je merkt: het percentage is geen "raar getal". Het is informatie waar je iets mee kunt doen. De AI geeft niet een vaag oordeel. Hij geeft een eerlijke schatting van zijn eigen zekerheid.

## Waarom dit ertoe doet

Een productlijn met een te lage drempel laat veel defecten door. Klanten klagen. Een productlijn met een te hoge drempel stopt te vaak voor niets. Productieverlies. Tussen die twee ligt een werkbare drempel — en die hangt af van wat een gemiste fout bij jullie kost.

Wie kanspercentages leest:

- **Stelt betere vragen** aan IT of kwaliteit over de drempelinstelling.
- **Voorkomt frustratie** ("die AI is onbetrouwbaar") door percentages goed te interpreteren.
- **Helpt het team** een gefundeerde keuze maken over wanneer de drempels bijgesteld moeten worden.
- **Voorkomt blind doorlaten** bij lage percentages, en blind afkeuren bij hoge — beide kosten geld.

## Na deze sessie

Kies deze week één AI-systeem op je lijn dat met kanspercentages of betrouwbaarheidsscores werkt. Bijvoorbeeld de inspectiecamera, een onderhoudsadvies-dashboard, of een kwaliteitsalarm. Schrijf drie dingen op:

- Welke percentages zie je voorbijkomen — laag, midden, hoog?
- Welke actie volgt nu standaard bij elk niveau?
- Zou jij — op basis van wat een gemiste fout bij jullie product kost — een andere drempel willen voorstellen?

Neem je notities mee naar de volgende sessie. Praat er deze week ook één keer over met een kwaliteits- of IT-collega. Vraag: "Hoe zijn de drempels van onze inspectie-AI ingesteld? En wie heeft die ingesteld?" Je ontdekt vaak dat de drempels al lange tijd niet zijn aangepast, terwijl het product of het proces is veranderd. Dat is een waardevol gesprek voor jou én voor het team.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-drie-producten.md`](./werkbladen/wb-01-drie-producten.md) — Drie producten
2. [`wb-02-buurman-grenzen.md`](./werkbladen/wb-02-buurman-grenzen.md) — Buurman grenzen
3. [`wb-03-handout-drempelgebieden.md`](./werkbladen/wb-03-handout-drempelgebieden.md) — Handout drempelgebieden
4. [`wb-04-eigen-drempel.md`](./werkbladen/wb-04-eigen-drempel.md) — Eigen drempel

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-103`](../../kennisbank/ai_fundamentals/machine_learning_basics/ko-ai-fund-103.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
