---
id: lo-industry40-302-trainee
knowledge_object_id: ko-industry40-302
version: trainee
title: Data-pipeline ontwerpen voor een digital twin — vier knooppunten, drie keuzes
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: ervaren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde16-lo-industry40-302
---

# Data-pipeline ontwerpen voor een digital twin — vier knooppunten, drie keuzes

Een sensor op zich levert nog geen inzicht. De data moet ergens heen. Pas als die data via een goede pipeline (data-leiding) bij het dashboard of het AI-model komt, ontstaat er waarde. In de vorige sessies leerde je wat een digital twin (digitale tweeling) is en hoe je een sensor kiest. Nu kijken we naar het pad tussen de twee. Want een hapertend dashboard, ontbrekende data en een te hoge cloud-rekening hebben vaak één gemeenschappelijke oorzaak: de pipeline is niet goed ontworpen.

## Wat leer je?

Je kunt na deze sessie zelf een eenvoudige data-pipeline tekenen voor een machine of lijn van jullie werkvloer. Je benoemt daarbij vier knooppunten en onderbouwt drie ontwerp-keuzes met één zin per keuze.

## De vier knooppunten — het pad van meten naar gebruiken

Elke meting doorloopt vier knooppunten. Stel je een waterleiding voor. Het water komt uit de bron. Het gaat door een tussenstation. Het wordt opgeslagen in een reservoir. En het wordt uiteindelijk gebruikt door de gebruiker thuis. Sensor-data werkt precies zo.

1. **Sensor.** De bron. Een trillings-, temperatuur-, beeld- of druk-sensor meet en verstuurt.
2. **Edge-buffer (tussenstation).** Een klein opslag-punt bij de sensor zelf. Vaak een industriële computer naast de machine. Hier wordt data tijdelijk bewaard als de verbinding wegvalt. Hier wordt ook gefilterd: alleen relevante data gaat door.
3. **Opslag.** De centrale plek waar data wordt bewaard. Soms ter plaatse in een server, soms in de cloud. Hier zit weken tot maanden aan historie.
4. **Consument.** De plek waar de data wordt gebruikt. Een dashboard voor de operator. Een AI-model dat patronen voorspelt. Een rapportage voor de productieleider.

Een goed ontworpen pipeline is voor de operator onzichtbaar. Alles werkt gewoon. Pas als er iets niet klopt, merk je dat er onderhuids veel keuzes zijn gemaakt.

## Drie ontwerp-keuzes — wat bepaalt of het werkt

Bij elk pipeline-ontwerp wegen drie keuzes. Bron: Anaya et al. (2024); Bakopoulos et al. (2024).

### Latentie (vertraging) — hoe snel moet de data er zijn?

- **Real-time** (onder 1 seconde): bijvoorbeeld een veiligheids-alarm wanneer iemand te dicht bij een robot komt.
- **Near-realtime** (onder 60 seconden): bijvoorbeeld een temperatuur die boven een drempel komt.
- **Batch** (uren of dagen): bijvoorbeeld een maandrapport over productie.

Hoe sneller, hoe duurder. Niet alles hoeft real-time. Vraag jezelf eerst af wat de gebruiker echt nodig heeft.

### Volume (hoeveelheid data) — wat doe je ermee?

Een trillingsensor kan duizend metingen per seconde doen. Bij tien sensoren en vierentwintig uur productie gaat dat richting honderden miljoenen metingen per dag. Te veel om allemaal naar de cloud te sturen. De slimme oplossing zit bij de edge-buffer: daar vat je samen. Stuur bijvoorbeeld elke tien seconden het gemiddelde plus elke afwijking. Je bespaart soms 99% aan data zonder dat je informatie verliest.

### Failover (terugval bij fout) — wat als er iets stopt?

Drie vragen tellen mee. Wat gebeurt er als de verbinding tussen edge en opslag wegvalt? Wat als de opslag vol raakt? Wat als de sensor zelf stuk gaat? Een goede pipeline heeft twee dingen ingebouwd. Buffering — de edge-buffer bewaart data totdat de verbinding terug is. En alarmen — de operator krijgt melding bij sensor-uitval.

## Wat de operator merkt — drie storings-signalen

Drie ervaringen verraden dat de pipeline niet klopt:

- **Het dashboard loopt achter.** Latentie is te hoog.
- **Er ontbreekt data in een grafiek.** Geen failover bij verbindings-verlies.
- **De cloud-rekening loopt op.** Geen volume-controle bij de edge-buffer.

Wie deze signalen herkent, weet welke vraag hij aan IT moet stellen. Dat scheelt veel zoekwerk.

## Een voorbeeld om vast te houden — spuitgieterij met vijftig mallen

Een spuitgieterij wil de temperatuur van vijftig mallen monitoren. Het eerste ontwerp: elke sensor stuurt elke seconde direct naar de cloud. Resultaat: cloud-kosten lopen op tot tweeduizend vijfhonderd euro per maand. Te duur voor de waarde die het oplevert.

Het tweede ontwerp gebruikt een edge-buffer per machine. Elke dertig seconden gaat het gemiddelde door, plus elke afwijking groter dan drie graden. Cloud-kosten dalen naar honderdtwintig euro per maand. De dashboard-snelheid blijft acceptabel — een resolutie van dertig seconden is voor temperatuur ruim voldoende. Dezelfde sensoren, dezelfde vraag, een ander pipeline-ontwerp. Verschil: factor twintig in kosten.

## Na deze sessie

Kies deze week één machine of lijn op jullie werkvloer waar een dashboard of AI-model sensor-data gebruikt.

Teken op een A4 de vier knooppunten met pijlen: sensor, edge-buffer (tussenstation), opslag, consument.

Beantwoord vervolgens drie vragen schriftelijk: (1) welke latentie (vertraging) heeft jullie dashboard nu — onder 1 seconde, onder 60 seconden, of in batch? (2) wordt de data ergens samengevat, en zo ja waar? (3) wat gebeurt er als de verbinding tussen edge-buffer en opslag een uur wegvalt?

Vraag bij twijfel één antwoord aan IT of de teamleider. Neem je tekening en notities mee naar de volgende sessie.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-drie-storingen.md`](./werkbladen/wb-01-drie-storingen.md) — Drie storingen
2. [`wb-02-buurman-check.md`](./werkbladen/wb-02-buurman-check.md) — Buurman check
3. [`wb-03-pipeline-handout.md`](./werkbladen/wb-03-pipeline-handout.md) — Pipeline handout
4. [`wb-04-eigen-pipeline.md`](./werkbladen/wb-04-eigen-pipeline.md) — Eigen pipeline

## Verder

- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
