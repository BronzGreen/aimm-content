---
id: lo-ai-fund-204-trainee
knowledge_object_id: ko-ai-fund-204
version: trainee
title: Bias en eerlijkheid in AI — kunnen AI-systemen discrimineren?
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
correlation_id: ronde17-lo-ai-fund-204
---

# Hoe ontstaat vertekening (bias) in een AI — en wat kun je er als operator zelf aan doen?

Vertekening (bias) in AI lijkt iets voor CV-checkers (systemen die sollicitatiebrieven beoordelen) en gezichtsherkenning. Iets ver weg. Toch komt het op je werkvloer voor. Een AI die producten van een nieuwe leverancier vaker afkeurt. Een productiviteitsmeting waarin één ploeg structureel lager scoort. Het kan grote gevolgen hebben — voor geld én voor mensen. In deze sessie leer je hoe vertekening ontstaat. En je leert wat je er zelf aan kunt doen.

## Wat leer je?

Je kunt na deze sessie de drie hoofdoorzaken van vertekening in eigen woorden benoemen. Je herkent bij een werkvloer-casus welke oorzaak speelt. Je weet dat AI ook positief kan bijdragen aan inclusie. En je hebt één concrete actie gekozen voor de komende maand.

## Casus — leverancier C wordt vaker afgekeurd

Een spuitgietbedrijf gebruikt sinds twee jaar AI-kwaliteitscontrole op de visuele afdeling. Het werkt goed. Tot er een nieuwe leverancier C bijkomt voor één grondstof.

Na een maand werken blijkt: producten gemaakt met grondstof van leverancier C worden 3 keer vaker afgekeurd dan producten van leverancier A (oud en vertrouwd).

De kwaliteitsmanager gaat het na. Het AI-systeem is getraind op ruim 80.000 beelden. Daarvan kwam 92 procent van producten met grondstof A. Leverancier C heeft een iets andere kleurtint door ander pigment. Niet slechter — alleen anders.

De AI ziet "anders" en denkt "slecht". Hij keurt af.

Is dit oneerlijk tegenover leverancier C? Ja. En niet omdat iemand het zo wilde.

## Wat is vertekening (bias)?

Vertekening is **scheefheid**. AI leert uit data. Als die data scheef is, is de AI ook scheef. Niet omdat programmeurs dat willen — maar omdat de wereld waarin de AI is opgegroeid niet de hele wereld was.

Bron: Npuls (2025), Raamwerk NL AI-Geletterdheid in het Onderwijs.

## Drie oorzaken van vertekening

### 1. Scheve trainingsdata

AI leerde uit data van één bron — één ploeg, één regio, één periode, of zoals in de casus: één leverancier. Nieuwe situaties matchen niet met wat hij heeft gezien.

**In de maakindustrie:**
- Kwaliteitscontrole keurt producten van leverancier A goed en van leverancier B vaker af, terwijl beide prima zijn.
- Productiviteitsmeting ziet de middagploeg als minder productief — omdat de trainingsdata uit de ochtendploeg kwam.

### 2. Onvolledige data

Bepaalde groepen of gevallen ontbraken in de training. Wat de AI nooit heeft gezien, kan hij niet goed beoordelen.

**Een voorbeeld buiten de maakindustrie:** een CV-checker (een AI die sollicitatiebrieven beoordeelt) getraind op data uit 2015 tot 2020 herkent zij-instromers slecht. Hun loopbaan past niet in de patronen.

**In de maakindustrie:** een onderhouds-AI getraind op nieuwe machines schat oudere machines verkeerd in — hij raadt te vaak vervanging aan terwijl ze prima werken.

### 3. Stilzwijgende aannames

De data droeg aannames in zich die niet overal gelden. Een aanname is iets wat je voor waar aanneemt zonder erover na te denken.

**Voorbeeld:** "normale temperatuur is 20 graden". Geldt in een kantoor. Niet in een gieterij waar het standaard 35 graden is.

Een AI die ergens deze aanname meedraagt, geeft rare meldingen in afwijkende omgevingen.

## Wat hebben deze drie gemeen?

In alle drie gevallen oordeelt de AI **systematisch anders** over gevallen die eigenlijk gelijk zijn. Dat is het kenmerk van vertekening. Niet één losse fout — maar een patroon dat steeds dezelfde kant op wijst.

| Wat zie je? | Welke oorzaak? |
|---|---|
| Nieuwe leverancier krijgt vaker afkeur | Scheve trainingsdata |
| Bepaald type machine wordt onterecht afgewezen | Onvolledige data |
| AI werkt slecht in afwijkende omstandigheden | Stilzwijgende aannames |

## Maar: AI kan ook iets goeds

AI is niet alleen risico. Dezelfde technologie die discrimineert kan ook helpen — afhankelijk van hoe je hem inzet.

Vier kansen op de werkvloer:

1. **Meertalige werkinstructies.** Voor Poolse, Roemeense of andere anderstalige collega's. Een AI-vertaaltool maakt instructies in eigen taal.
2. **Voorleesfunctie.** Voor collega's met dyslexie of slechtziendheid. De instructie wordt voorgelezen in plaats van alleen op papier.
3. **Visuele uitleg.** Voor wie tekst lastig vindt: pictogrammen, korte filmpjes, schema's.
4. **Live ondertiteling.** Bij toolbox-meetings of trainingen, zodat iedereen kan meedoen.

Dit is geen luxe — het is inclusie. En het werkt vaak met dezelfde AI-toolkit die ook op de productielijn draait.

## Vier acties die jij kunt ondernemen

Geen IT-kennis nodig:

1. **Vraag** bij elke AI-tool: welke data is gebruikt voor training? Welke periode, welke machines, welke leveranciers?
2. **Merk op** als de AI systematisch anders oordeelt over vergelijkbare gevallen — een leverancier, een ploeg, een productserie.
3. **Meld** vertekening als je denkt het te zien. Alleen met feedback kan het beter. Eén concrete observatie is genoeg om een gesprek te starten.
4. **Zie ook** de kansen voor inclusie. Vraag of jullie AI-tool ook iets kan voor meertalige uitleg of voorlezen.

## Waarom dit ertoe doet

Vertekening is geen ver-van-bed-show. Bij de leverancier C-casus werd de afkeur verholpen door bij te trainen met 10.000 nieuwe beelden van leverancier C. Resultaat: afkeur normaal niveau. Positief gevolg: dezelfde toolkit werd later gebruikt voor meertalige werkinstructies voor Poolse collega's. Inclusie won.

Wie vertekening herkent én inclusie-kansen ziet:

- **Voorkomt financiële schade** door onterechte afkeur of vervanging.
- **Behandelt collega's en leveranciers eerlijk** — geen systematische benadeling.
- **Maakt AI bruikbaar voor het hele team**, ook voor wie taal of leesbaarheid een drempel is.
- **Verbetert het AI-systeem** door gerichte feedback aan IT of leverancier.

## Zelf zien gebeuren?

Open op tablet of laptop het interactieve `model-bias-eerlijkheid-evaluator.jsx`. Je krijgt zes werkvloer-cases — van kwaliteitscontrole die nieuwe leveranciers oneerlijk behandelt tot een AI-vertaaltool die juist inclusie bevordert. Per case kies je: scheve trainingsdata, onvolledige data, stilzwijgende aanname — of een inclusie-kans. Per keuze directe feedback met onderbouwing. Aan het eind krijg je de vier eigen acties (vragen, opmerken, melden, kansen zien) als vuistregel mee.

## Na deze sessie

Doe deze maand één van de vier eigen acties op een AI-systeem op je werkvloer. Kies één optie en voer hem deze maand uit:

- Vraag aan IT of de leverancier welke data is gebruikt voor training — periode, machines, leveranciers, producten.
- Of: kijk twee weken lang of de AI systematisch anders oordeelt over vergelijkbare gevallen, bijvoorbeeld bij verschillende leveranciers, ploegen of productseries.
- Of: meld een vermoeden van vertekening aan kwaliteit of IT, met één concrete observatie als onderbouwing.
- Of: vraag of jullie AI-tool ook iets kan voor inclusie — meertalige werkinstructies, voorleesfunctie, visuele uitleg.

Neem de uitkomst mee naar de volgende sessie. Stel deze week ook aan één collega de open vraag: "Heb jij wel eens gezien dat onze AI iemand of iets oneerlijk behandelt?" Vaak heeft iemand een observatie die nog niet gedeeld is. Patronen in vertekening komen vaak naar voren in gesprekken met collega's, niet in de techniek zelf.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-casus-kwaliteitscontrole.md`](./werkbladen/wb-01-casus-kwaliteitscontrole.md) — Casus kwaliteitscontrole
2. [`wb-02-buurman-drie-voorbeelden.md`](./werkbladen/wb-02-buurman-drie-voorbeelden.md) — Buurman drie voorbeelden
3. [`wb-03-handout-bias-en-inclusie.md`](./werkbladen/wb-03-handout-bias-en-inclusie.md) — Handout bias en inclusie
4. [`wb-04-eigen-bias-en-inclusie.md`](./werkbladen/wb-04-eigen-bias-en-inclusie.md) — Eigen bias en inclusie

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-204`](../../kennisbank/ai_fundamentals/ai_ethics_en_bias/ko-ai-fund-204.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
