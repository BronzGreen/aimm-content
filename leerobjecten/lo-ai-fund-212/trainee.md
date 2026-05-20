---
id: lo-ai-fund-212-trainee
knowledge_object_id: ko-ai-fund-212
version: trainee
title: Hoe weet je of een AI-model écht goed werkt? — confusion matrix, precision
  en recall
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: analyseren
knowledge_type: declaratief
competency_stage: bewust_bekwaam
kolb_start_phase: ervaren
guidance_style: instrueren
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde20-lo-ai-fund-212
---

# Hoe weet je of een AI-model écht goed werkt? — confusion matrix, precision en recall

Een AI-model dat 95 procent goed scoort klinkt prima. Maar als jouw lijn al 95 procent goede producten maakt, en het model zegt altijd "goed", dan haalt het diezelfde score. En laat het alle afkeur door. Het rapport-cijfer klopt — de werkelijkheid niet. Dit blok leert je hoe je daar doorheen prikt.

## Wat leer je?

Je kunt na deze sessie een **confusion matrix** (verwarrings-matrix) lezen, zelf **precision** (precisie) en **recall** (terugvinden) berekenen, en onderbouwd kiezen welke van de twee voor jouw werkvloer-AI het belangrijkste is.

## Waarom is "accuratesse" niet genoeg?

Stel: er lopen 100 producten over de lijn. Daarvan zijn er 20 echt afgekeurd. Een model dat altijd "goed" zegt, scoort 80 procent accuratesse. Het laat alle 20 afkeur-stuks door. Onbruikbaar.

Daarom kijken we niet alleen naar hoeveel fouten het model maakt. We kijken naar **welke** fouten. Daar is een verdeling voor in vier vakken.

## De confusion matrix in vier kwadranten

Een classificatie-model heeft per voorbeeld vier mogelijke uitkomsten:

|  | Model zegt: goed | Model zegt: afgekeurd |
|---|---|---|
| **Echt goed** | Terecht positief (juist) | Vals negatief (vals-alarm) |
| **Echt afgekeurd** | Vals positief (gemist) | Terecht negatief (juist) |

Vertaling naar de werkvloer:

- **Terecht positief** — goed product, model zegt goed. Niets aan de hand.
- **Vals negatief (vals-alarm)** — goed product, model zegt afgekeurd. Het wordt onnodig weggegooid.
- **Vals positief (gemist)** — afgekeurd product, model zegt goed. Het gaat naar de klant.
- **Terecht negatief** — afgekeurd product, model zegt afgekeurd. Klopt.

Beide soorten fouten kosten geld. Maar welke is duurder voor jouw lijn? Dat is de kernvraag.

## Precision — "als het model afkeurt, heeft het dan gelijk?"

**Precision** vertelt je hoe betrouwbaar een afkeur-signaal is.

Formule: terecht afgekeurd gedeeld door alles wat het model afkeurt.

> precision = terecht afgekeurd / (terecht afgekeurd + vals afgekeurd)

Hoge precision betekent: bijna alles wat het model afkeurt, is ook echt afgekeurd. Weinig goede producten gaan onterecht de afval-bak in.

## Recall — "vindt het model alle afkeur, of glipt er iets door?"

**Recall** vertelt je hoe compleet het model is in het terugvinden van afkeur.

Formule: terecht afgekeurd gedeeld door alle echt-afgekeurde producten.

> recall = terecht afgekeurd / (terecht afgekeurd + vals doorgelaten)

Hoge recall betekent: bijna geen afkeur glipt erdoor. Het model vangt het meeste op.

## De trade-off — je kunt niet beide tegelijk maximaal hebben

Je kunt aan de drempel van het model draaien:

- **Strenger** — het model keurt sneller af. Recall stijgt (minder gemist). Precision daalt (meer vals-alarm).
- **Soepeler** — het model laat meer door. Precision stijgt (minder vals-alarm). Recall daalt (meer gemist).

Het is een schuifregelaar. Stuur je hem naar links, dan win je op de ene kant en betaal je op de andere. Beide tegelijk maximaal kan vrijwel nooit.

## Wanneer kies je precision, wanneer recall?

Geen wiskundige regel. Een bedrijfslogica-regel.

**Hoge precision belangrijk** als vals-alarm duur is. Voorbeeld: een fabrikant van handgemaakte horloges. Een goed horloge afkeuren kost productiekosten en is jammer. Maar het echte risico is een defect product dat doorgaat — dat schaadt het merk en kost retourzendingen. Hier wil je: als het model afkeurt, dan ook echt afkeuren.

**Hoge recall belangrijk** als doorlaten duur is. Voorbeeld: een vleesverwerker. Goed vlees afkeuren kost productiekosten. Maar afgekeurd vlees dat naar de klant gaat, kost mogelijk levens of grote schade. Hier wil je: vind alle afkeur, ook als dat betekent dat je vaker vals-alarm krijgt.

## Werkvloer-voorbeeld — een vleesverwerker draait aan de drempel

Een vleesverwerker traint een camera om "geschikt" versus "afgekeurd" te beoordelen. 100 producten, waarvan 20 echt afgekeurd.

**Eerste instelling (strenge drempel):**

- Terecht afgekeurd: 17
- Vals doorgelaten: 3
- Vals afgekeurd: 5
- Terecht goed: 75

Precision = 17 / (17 + 5) = **77 procent**.
Recall = 17 / (17 + 3) = **85 procent**.

Drie afgekeurde stuks glippen erdoor. Onaanvaardbaar voor voedselveiligheid.

**Tweede instelling (soepelere drempel — vanger groter):**

- Terecht afgekeurd: 20
- Vals doorgelaten: 0
- Vals afgekeurd: 15
- Terecht goed: 65

Precision = 20 / (20 + 15) = **57 procent**.
Recall = 20 / (20 + 0) = **100 procent**.

Geen enkel afgekeurd stuk glipt erdoor. Maar 15 goede stuks gaan onterecht naar herinspectie. Dat kost werk — niet levens.

Voor deze werkvloer is de tweede instelling de juiste keuze. Recall weegt hier zwaarder.

## Waarom dit ertoe doet

Wie deze twee maten kent, kan een evaluatie-rapport van zijn AI-leverancier kritisch lezen:

- **Voorkomt blind vertrouwen** in een rapport-cijfer dat niet de werkelijkheid op de lijn dekt.
- **Spaart discussies uit** met collega's, kwaliteit of leverancier over "wat is een goed model".
- **Maakt zijn vakkennis zichtbaar** — je weet als operator welke fout op jouw lijn duurder is.

Dit gaat niet over wiskunde. Het gaat over de vraag: welke fout kan ik níet hebben op deze lijn?

## Zelf zien gebeuren?

Twee extra hulpmiddelen die bij dit leerobject horen — beide tonen de trade-off live in beweging:

- **Video (~90 seconden):** confusion matrix met 4 kwadranten, drempel-slider die live beweegt, en het verschil tussen defectinspectie (recall belangrijk) en spam-filter (precision belangrijk). Bestand: `video/composition.tsx`.
- **Interactief "Drempel-slider":** schuif aan een drempel (0-1) op een fictieve dataset van 50 voorbeelden, kies een scenario (kwaliteitsinspectie of spam-filter), en zie precision/recall + totale kosten live veranderen. Bestand: `model-precision-recall-drempel.jsx`.

Vraag je trainer welke variant in jouw sessie gebruikt wordt.

## Na deze sessie

Kies deze week één AI-toepassing op je eigen lijn. Een inspectiecamera. Een sorteersysteem. Een afkeur-AI.

Beantwoord schriftelijk drie vragen:

1. Wat is een **vals positief** op deze lijn — wat gaat er fout en wie merkt het?
2. Wat is een **vals negatief** — wat gaat er fout en wie merkt dat?
3. Welke van de twee is **duurder** voor jouw werkvloer?

Kies daarna één: precision of recall. Schrijf één onderbouwende zin op.

Stel deze week één concrete vraag aan leverancier, IT of kwaliteit. Bijvoorbeeld: "Wat is de recall van onze afkeur-camera op de zomerlijn?"

Neem het antwoord mee naar de volgende sessie.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-twee-confusion-matrices-vleesverwerker.md`](./werkbladen/wb-01-twee-confusion-matrices-vleesverwerker.md) — Twee confusion matrices vleesverwerker
2. [`wb-01-twee-matrices-lezen.md`](./werkbladen/wb-01-twee-matrices-lezen.md) — Twee matrices lezen
3. [`wb-02-precision-recall-formules.md`](./werkbladen/wb-02-precision-recall-formules.md) — Precision recall formules
4. [`wb-02-vals-positief-vals-negatief-in-duo.md`](./werkbladen/wb-02-vals-positief-vals-negatief-in-duo.md) — Vals positief vals negatief in duo
5. [`wb-03-precision-recall-handout.md`](./werkbladen/wb-03-precision-recall-handout.md) — Precision recall handout
6. [`wb-03-werkvloer-keuze-precision-of-recall.md`](./werkbladen/wb-03-werkvloer-keuze-precision-of-recall.md) — Werkvloer keuze precision of recall
7. [`wb-04-eigen-werkvloer-ai-doorlichten.md`](./werkbladen/wb-04-eigen-werkvloer-ai-doorlichten.md) — Eigen werkvloer ai doorlichten

## Verder

- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
