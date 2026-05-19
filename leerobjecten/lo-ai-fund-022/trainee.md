---
id: lo-ai-fund-022-trainee
knowledge_object_id: ko-ai-fund-022
version: trainee
title: Wat is een neuraal netwerk? — patroonherkenning in lagen
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
correlation_id: ronde10-lo-ai-fund-022
---

# Hoe weet de camera boven de lopende band dat een product een defect heeft?

Op steeds meer werkplekken kijkt een camera mee. Hij wijst aan: deze beugel heeft een kras, deze niet. Voor veel operators voelt dat als magie of als een black box. Het is geen van beide. Het is wiskunde — en in dit blok zie je hoe het op hoofdlijnen werkt.

## Wat leer je?

Je kunt na deze sessie in eigen woorden uitleggen wat een neuraal netwerk (neural network) is. Je herkent op een schema waar de input zit, waar de lagen zitten, en waar de output uitkomt. En je kunt voor je eigen werkplek aanwijzen waar zo'n model meekijkt.

## Een neuraal netwerk in drie blokken

Een neuraal netwerk is een rekenmodel dat patronen leert uit duizenden voorbeelden. Het werkt in drie stappen:

1. **Input** — wat gaat erin. Bijvoorbeeld een foto van een metalen beugel op de lopende band.
2. **Lagen** — hier zit het rekenwerk. Veel kleine eenheden, neuronen (neuron) genoemd, kijken elk naar een stukje van het beeld. De eerste laag herkent simpele dingen: lijnen, randen. De volgende laag herkent vormen. De laatste lagen herkennen complete patronen: een kras, een deuk, een ontbrekende schroef.
3. **Output** — wat eruit komt. Bijvoorbeeld een antwoord: 'goed' of 'kras op positie 3'.

Het netwerk leert door duizenden voorbeelden te zien. Het ziet 1.300 foto's van goede producten en 295 foto's van foute. Daarna herkent het zelf het verschil.

### Waarom heet het 'neuraal'?

De naam komt van hersencellen. In je hoofd zitten miljoenen zenuwcellen, neuronen, die met elkaar verbonden zijn. Een neuraal netwerk is daarop geïnspireerd. Maar let op: het is geen brein. Het is een rekenmodel. De vergelijking met hersenen helpt om het beeld te krijgen, meer niet.

## Twee misverstanden om uit de weg te ruimen

- **Het is geen magie.** Iemand heeft het gebouwd, getraind en getest. Elk antwoord komt uit rekenwerk.
- **Het werkt niet precies zoals een brein.** De naam wekt die suggestie, maar de overeenkomst is oppervlakkig.

Wat het wél is: laagsgewijze patroonherkenning op basis van voorbeelden.

## Wat dit betekent op de werkvloer

Een bedrijf dat kunststof brandstoftanks maakt, gebruikte zo'n model voor camera-inspectie. Het model leerde van 1.300 synthetische foto's en 295 echte foto's. Daarna herkende het 70% van de defecten correct, in real-time, terwijl de operator aan het werk was *(bron: Soldatos 2024, Artificial Intelligence in Manufacturing, Ch. 17-18)*.

70% klinkt niet zo hoog. Maar het betekent: de camera vangt 70 van de 100 defecten meteen. De rest blijft het werk van mensen. Het model neemt het werk dus niet over — het helpt.

### Waarom jouw kennis nodig blijft

Een neuraal netwerk is zo goed als de voorbeelden waarmee het getraind is. Slechte voorbeelden in, slecht model uit. Daarom geldt:

- Jij weet wat een 'goed' product is op je lijn
- Jij ziet als eerste wanneer er iets nieuws misgaat dat het model nog niet kent
- Jij bepaalt mee welke foto's gebruikt worden als 'goed' en 'fout'

Zonder die kennis kan het model niet leren. En dat verandert niet — ook niet als het model beter wordt.

## Zelf zien gebeuren?

Twee extra hulpmiddelen die bij dit leerobject horen — beide maken het laag-voor-laag-rekenwerk visueel:

- **Video (~90 seconden):** zie hoe een foto van een tandwiel door 3 lagen stroomt, en hoe elke laag iets abstracter herkent (randen → vormen → object). Bestand: `video/composition.tsx` (Remotion-project).
- **Interactief "Lagen verkennen":** klik door 3 inputs (tandwiel, gespoten plaat, kras-defect) × 4 lagen en zie per combinatie wat het netwerk op dat moment "ziet". Bestand: `model-lagen-verkennen.jsx`.

Vraag je trainer welke variant in jouw sessie gebruikt wordt.

## Na deze sessie

Loop deze week één keer langs de inspectiecamera of het sensorsysteem op jouw lijn. Schrijf drie dingen op: waar hangt de camera precies (boven welke band, bij welke machine), wat is de output (een goed/fout antwoord, een klasse, of een getal), en waar komen de trainingsfoto's vandaan (wie maakt of beoordeelt die). Heb je geen camera op je eigen lijn? Vraag een collega van een andere lijn waar bij hen wordt meegekeken. Praat er ook even over met een kwaliteitscollega: *"Wie bepaalt eigenlijk wat de camera ziet als goed of fout?"* Je ontdekt vaak dat die keuze ergens ooit gemaakt is — en niet altijd door iemand die nu nog op de lijn werkt. Neem je notities mee naar de volgende sessie.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-buurman-reflectie.md`](./werkbladen/wb-01-buurman-reflectie.md) — Buurman reflectie
2. [`wb-01-camera-briefje.md`](./werkbladen/wb-01-camera-briefje.md) — Camera briefje
3. [`wb-02-buurman-reflectie.md`](./werkbladen/wb-02-buurman-reflectie.md) — Buurman reflectie
4. [`wb-02-handout-lagen.md`](./werkbladen/wb-02-handout-lagen.md) — Handout lagen
5. [`wb-03-eigen-lijn.md`](./werkbladen/wb-03-eigen-lijn.md) — Eigen lijn
6. [`wb-03-handout-lagen.md`](./werkbladen/wb-03-handout-lagen.md) — Handout lagen
7. [`wb-04-eigen-lijn.md`](./werkbladen/wb-04-eigen-lijn.md) — Eigen lijn

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-022`](../../kennisbank/ai_fundamentals/neural_networks_conceptueel/ko-ai-fund-022.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
