---
id: lo-ai-fund-205-trainee
knowledge_object_id: ko-ai-fund-210
version: trainee
title: Hoe label je trainingsdata voor een AI-model op de werkvloer?
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
correlation_id: ronde18-lo-ai-fund-205
---

# Hoe label je trainingsdata zo dat een AI-model er echt beter van wordt?

Een AI-model is zo goed als de labels die jij erop zet. Wie de foto's beoordeelt — jij dus — bepaalt mee of het model straks werkt op de lijn. Lijken jouw labels niet op die van je collega? Dan leert het model twee verhalen tegelijk. En het kiest geen van beide goed.

## Wat leer je?

Je kunt na deze sessie zelf trainingsdata labelen. Je past de vier principes van goed labelen toe. Je meet hoe vaak jij en een collega hetzelfde antwoord geven. En je herkent de vier valkuilen bij labelwerk.

## Wat is data labelen eigenlijk?

Een AI-model leert van voorbeelden. Bij elk voorbeeld hoort het juiste antwoord. Dat antwoord noem je een **label** (etiket).

Een voorbeeld uit een spuitgieterij. De inspectiecamera ziet honderden producten per uur. Bij elke foto zet een operator een etiket: **GOED**, **TWIJFEL** of **AFGEKEURD**. Het model leert van die antwoorden.

Zonder labels weet het model niet wat goed of fout is. Dit type leren heet **supervised learning** (leren met gelabelde voorbeelden). Labelen is dus geen typeklus — het is de plek waar jouw vakkennis in het model komt.

## Vier principes van goed labelen

Niet elk label is bruikbaar voor een AI-model. Vier dingen bepalen of jouw werk telt.

### 1. Consistentie

Hetzelfde voorbeeld krijgt altijd hetzelfde label. Dat geldt voor jou over de hele dag. Het geldt ook tussen jou en een collega. Lukt dat niet, dan leert het model twee verhalen.

Je meet dit door je labels te vergelijken met die van een collega. Daarover later meer.

### 2. Helderheid

De labels staan vooraf vast. Met **grenswaarden**. Niet vaag.

Een goed schema:

- **GOED** — geen zichtbaar defect op het zichtvlak.
- **TWIJFEL** — defect kleiner dan 1 mm of buiten het zichtvlak.
- **AFGEKEURD** — zichtbaar defect groter dan 1 mm op het zichtvlak.

Een nieuwe collega leest dit en kan het gebruiken. Dat is de test.

### 3. Dekking

Alle situaties zitten in de trainingsdata. Niet alleen de makkelijke. Ook de zeldzame.

- Krassen die je bijna nooit ziet — moeten erin.
- Defecten in de nachtploeg — moeten erin.
- Producten van een nieuwe leverancier — moeten erin.

Wat de AI nooit heeft gezien, kan hij niet goed beoordelen.

### 4. Domeinkennis

Jij weet wat een label betekent in de praktijk. Een operator met tien jaar ervaring ziet een grenzending direct. Een buitenstaander niet.

Die kennis maakt jouw label waardevol. Zonder vakkennis valt labelwerk uit elkaar — je krijgt foto's met antwoorden waar niemand achter staat.

## Hoe meet je of jij en je collega het eens zijn?

De vakterm is **inter-rater agreement** (inter-beoordelaar-overeenkomst). Het is een getal. Het zegt hoe vaak twee mensen hetzelfde label geven aan hetzelfde voorbeeld.

Hoe meet je het?

1. Twee operators labelen dezelfde 20 voorbeelden. Zonder elkaar te zien.
2. Vergelijk per voorbeeld: **zelfde** of **verschil**.
3. Tel de "zelfdes" en deel door 20.

Stel: 17 keer hetzelfde label, 3 keer verschil. Dan is je overeenkomst 17 / 20 = 85 procent.

Vuistregel uit de praktijk: **80 procent of meer is werkbaar**. Lager dan 80 procent? Dan ligt het zelden aan de operators. Het ligt vaak aan een schema dat nog niet helder genoeg is.

Twee operators die het niet eens zijn, is dus geen storing. Het is een signaal — voor wie het schema beheert.

## Vier valkuilen bij labelwerk

Iedereen die labelt, loopt deze tegen het lijf. Herken ze, dan kun je ze voor zijn.

### Vermoeidheids-drift

Na 100 foto's word je minder consistent. Je kijkt sneller. Je twijfelt minder. Je kiest vaker hetzelfde label uit gewoonte.

**Wat je kunt doen:** pauzeer elk uur. Vijf minuten weg van het scherm. Daarna ben je weer scherp.

### Confirmation bias

Dit heet ook wel **bevestigings-valkuil**. Je verwacht een label. Daardoor zie je het ook.

Stel: je hebt net tien GOEDs gezien. Bij de elfde foto kijk je sneller. Je verwacht GOED. Je ziet GOED. Ook al was er een kleine kras.

**Wat je kunt doen:** wissel periodiek met een collega. Of laat hem af en toe meekijken.

### Gemak boven precisie

Een twijfelproduct krijgt soms GOED. Omdat dat sneller is dan TWIJFEL invullen. Of omdat het anders extra werk wordt voor de afkeur-bak.

**Wat je kunt doen:** twijfel hoort het label TWIJFEL te krijgen. Niet GOED. Het schema is daar precies voor.

### Operator-verschillen

Twee operators kiezen niet altijd hetzelfde label. Sommige mensen denken dat één van de twee dan "fout zit". Dat is meestal niet zo.

Verschillen zijn signaal voor het schema. Niet voor de operator. Een collega die anders kiest, helpt jou en het AI-team om het schema scherper te maken.

## Waarom dit ertoe doet

Een goed labelschema is een **levend document**. Het start simpel. Het groeit met jullie werkervaring.

Wie zorgvuldig labelt:

- **Voorkomt valse afkeur.** Het model leert geen rommel.
- **Spaart bijtrain-rondes uit.** Eén bijtrain-ronde kost al snel duizenden labels.
- **Maakt zijn vakkennis zichtbaar** voor IT en kwaliteit.
- **Helpt collega's** doordat het schema duidelijker wordt voor iedereen.

Labelwerk is geen bijzaak. Het is de plek waar jouw werkvloer-kennis in de AI komt.

## Zelf zien gebeuren?

Twee extra hulpmiddelen die bij dit leerobject horen — beide maken labelwerk + valkuilen tastbaar:

- **Video (~90 seconden):** een korte explainer die in 5 scenes laat zien hoe data labelen werkt — van ruwe foto's naar gelabelde dataset, de 4 principes, de 4 valkuilen, en de operator-rol in de dataset. Bestand: `video/composition.tsx` (Remotion-project).
- **Interactief "Herken de valkuilen":** zes dataset-scenarios. Per dataset selecteer je welke van de 4 valkuilen aanwezig zijn (kunnen er meerdere zijn, of geen). Directe feedback met onderbouwing per scenario. Goede toepassings-oefening na de handout. Bestand: `model-label-valkuilen.jsx`.

Vraag je trainer welke variant in jouw sessie gebruikt wordt.

## Na deze sessie

Doe deze week drie kleine stappen op je eigen lijn. Geen IT-kennis nodig.

1. **Vraag rond** wie het labelschema van jullie AI-tool beheert. Vraag ook wanneer het voor het laatst is bijgewerkt.
2. **Label zelf tien voorbeelden** van je eigen lijn. Houd één pauze halverwege.
3. **Laat een collega dezelfde tien doen** zonder jouw antwoorden te zien. Tel daarna jullie overeenkomst.

Neem de uitkomsten mee naar de volgende sessie. We bespreken samen welk schema-woord de meeste twijfel gaf.

Praat deze week ook één keer met iemand van kwaliteit of IT. Vraag: "Hoeveel verschil zit er tussen onze operators op dezelfde producten?" Vaak ontdek je dat niemand het bijhoudt. Dat is een nuttige eerste vraag.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-eerste-labelsessie.md`](./werkbladen/wb-01-eerste-labelsessie.md) — Eerste labelsessie
2. [`wb-02-buurman-vergelijking.md`](./werkbladen/wb-02-buurman-vergelijking.md) — Buurman vergelijking
3. [`wb-03-handout-vier-principes-vier-valkuilen.md`](./werkbladen/wb-03-handout-vier-principes-vier-valkuilen.md) — Handout vier principes vier valkuilen
4. [`wb-04-eigen-labelschema.md`](./werkbladen/wb-04-eigen-labelschema.md) — Eigen labelschema

## Verder

- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
