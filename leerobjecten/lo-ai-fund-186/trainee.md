---
id: lo-ai-fund-186-trainee
knowledge_object_id: ko-ai-fund-186
version: trainee
title: Wat AI goed kan — en waar het mis gaat
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
updated_at: '2026-05-20'
correlation_id: ronde15-lo-ai-fund-186
---

# Waar is AI sterk in — en waar gaat het meestal mis?

AI klinkt vaak alsof het alles weet. In de praktijk is het anders. AI is in een paar dingen heel goed. En in een paar dingen voorspelbaar zwak. Wie de twee lijstjes kent, voorkomt fouten en gemiste meldingen. In deze sessie leer je beide kanten. En je doet één concrete check op je eigen werkvloer.

## Wat leer je?

Je kunt na deze sessie vier sterke en vier zwakke kanten van AI in eigen woorden benoemen. Je kunt bij een werkvloer-casus aanwijzen welke zwakte een rol speelde. En je hebt één concrete check geformuleerd voor een AI-systeem op je eigen werkvloer.

## Casus — een lasersnijder met een advies

Een operator werkt zijn eerste week met een nieuwe lasersnijder. Het systeem heeft een AI-functie die de snijvolgorde optimaliseert. Op dag drie krijgt hij een advies: deze volgorde bespaart 12 procent energie.

De operator gaat aan de slag. Maar hij merkt iets. Tussen twee snijbewegingen ligt de plaat lang te wachten. Hij twijfelt: volgen of niet?

Stel jezelf drie vragen. Wat doet de AI hier goed? Wat ziet de AI niet? Wat zou jij doen in zijn plaats?

De AI is sterk: hij rekent snel, vergelijkt duizenden mogelijke paden, kiest de optie met de minste energie. De operator is sterk in iets anders: hij ziet de wachtende verwarmde plaat. Achteraf bleek de AI getraind op dikker materiaal. De dunne plaat van 2 millimeter roestvrijstaal was nieuw voor het systeem.

Bron: Npuls (2025), Raamwerk NL AI-Geletterdheid in het Onderwijs.

## Waar AI sterk in is

Vier dingen kan AI goed:

1. **Patronen herkennen** in grote hoeveelheden data. Duizenden foto's, jaren aan sensorgegevens — AI vindt verbanden die een mens niet ziet.
2. **Consistentie.** AI wordt niet moe. Niet afgeleid. Niet ongeduldig op vrijdagmiddag. Een mens ziet vermoedelijk meer fouten op een lange dienst.
3. **Snelheid.** Duizenden checks per minuut zijn geen probleem.
4. **Signalen koppelen** die een mens niet samen ziet. Bijvoorbeeld trillingen plus temperatuur plus geluid plus draaisnelheid — alles op hetzelfde moment.

Op deze sterktes leunen de meeste AI-toepassingen in de maakindustrie. Camera-inspectie. Onderhoudsvoorspelling. Voorraadbestelling. Kwaliteitsalarmen.

## Waar AI zwak in is

Vier dingen kan AI slecht:

1. **Onbekende situaties.** Heeft de AI iets nog nooit gezien? Dan mist hij het waarschijnlijk. De lasersnijder zag geen 2 millimeter staal — dus dat type vervorming kon hij niet voorzien.
2. **Context.** De AI weet niet dat het vandaag min 10 graden is en de machines 2 uur langer moeten warmlopen. Of dat er nu wordt schoongemaakt en het stof tijdelijk hoger is.
3. **Vertekening (bias).** Als de trainingsdata (de voorbeelden waarvan het systeem heeft geleerd) vooral van één type product, één ploeg of één periode kwam, werkt de AI slecht op andere typen. Voorbeeld: een AI getraind op data van de ochtendploeg ziet de middagploeg als afwijkend.
4. **Data-ruis.** Sensoren die slecht onderhouden zijn geven vreemde waarden. De AI ziet dat als "bijzonder patroon" en alarmeert ten onrechte.

Wat hebben deze vier zwaktes gemeen? Het zijn allemaal situaties die *buiten* de wereld vallen waarop het systeem getraind is.

## De halve-flessen-regel

Behandel AI zoals een goede maar nieuwe collega op de werkvloer:

| Periode | Wat doe je? |
|---|---|
| Eerste week | Alles dubbelchecken |
| Maand 1 - 3 | Steekproeven |
| Na 6 maanden | Vertrouwen met een handvol checks per week |
| Altijd | Bij rare uitkomsten je eigen verstand gebruiken |

Dit is geen wantrouwen. Het is hetzelfde wat je met een nieuwe collega doet. Eerst kijken hoe iemand werkt. Dan stukje bij beetje meer ruimte geven. Bij twijfel: doorvragen.

## Waarom dit ertoe doet

De meeste AI-ongelukken op de werkvloer komen niet doordat AI stom is. Ze komen doordat de mensen eromheen de zwaktes niet kenden. Een lasersnijder-operator die opmerkt dat de AI iets niet zag, voorkomt 80 afgekeurde platen. Een onderhoudsmonteur die merkt dat de AI op één seizoen is getraind, voorkomt overbodige onderdelen-bestellingen.

Wie de vier sterktes en vier zwaktes kent:

- **Vertrouwt op de juiste plekken** (snelheid, consistentie, patronen).
- **Blijft alert op de juiste plekken** (onbekende situaties, context, vertekening).
- **Stelt gerichte vragen** aan IT of leverancier ("Op welke periode is dit systeem getraind?").
- **Voorkomt overschatting** — de belangrijkste oorzaak van AI-fouten in de praktijk.

## Tip — houd een klein AI-logboek

Patronen in AI-fouten zijn even leerzaam als patronen in productiefouten. Schrijf één keer per week op: ging het goed of niet — en waarom? Geen formeel document — een notitie op je telefoon werkt prima. Na een maand heb je informatie die je met IT of leverancier kunt delen.

## Zelf zien gebeuren?

Open op tablet of laptop het interactieve `model-ai-sterk-zwak-herkenner.jsx`. Je krijgt zes werkvloer-cases — van een lasersnijder die struikelt over dun materiaal tot een planningsassistent die het goed doet. Per case kies je welke zwakte hier speelt (onbekende situatie, mist context, bias, data-ruis) — of dat de AI het juist goed deed. Directe feedback met onderbouwing. Aan het eind krijg je de vuistregel: AI is sterk *binnen* zijn trainingsgebied, zwak *erbuiten*.

## Na deze sessie

Kies deze week één AI-systeem op je werkvloer dat je regelmatig tegenkomt. Bijvoorbeeld de inspectiecamera, de planning-assistent of een onderhoudsadvies-dashboard. Schrijf drie dingen op:

- Op welke sterke kant leunt dit systeem het meest — patronen, consistentie, snelheid, signalen koppelen?
- Welke zwakte zou bij jullie systeem het grootste risico zijn — onbekende situaties, context, vertekening of data-ruis?
- Welke concrete check kun je deze week één keer doen om die zwakte op te merken?

Houd dat klein. Bijvoorbeeld: "bij de eerstvolgende rare melding kijk ik welke trainingsperiode het systeem gebruikt". Neem je notities mee naar de volgende sessie. Begin deze week ook met een klein AI-logboek — een notitie op je telefoon is genoeg.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-casus-lasersnijder.md`](./werkbladen/wb-01-casus-lasersnijder.md) — Casus lasersnijder
2. [`wb-02-buurman-sterk-zwak.md`](./werkbladen/wb-02-buurman-sterk-zwak.md) — Buurman sterk zwak
3. [`wb-03-handout-sterk-zwak.md`](./werkbladen/wb-03-handout-sterk-zwak.md) — Handout sterk zwak
4. [`wb-04-eigen-risico.md`](./werkbladen/wb-04-eigen-risico.md) — Eigen risico

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-186`](../../kennisbank/ai_fundamentals/ai_ethics_en_bias/ko-ai-fund-186.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
