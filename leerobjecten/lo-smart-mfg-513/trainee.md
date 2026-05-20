---
id: lo-smart-mfg-513-trainee
knowledge_object_id: ko-smart-mfg-513
version: trainee
title: 'Resultaten interpreteren: confusion matrix voor operators'
target_audience: operator
content_level: MBO-3
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: experimenteren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-513
---

# Confusion matrix en model verbeteren

> **Leervraag:** Hoe lees je de resultaten van een vision-model, en hoe maak je het model beter als het niet goed genoeg is?

---

## Waarom is dit belangrijk?

Je hebt net een model geconfigureerd. Maar hoe weet je of het goed genoeg is? De confusion matrix vertelt je precies wat het model goed en fout doet. En als het niet goed genoeg is, weet je hoe je het kunt verbeteren. Dit is precies wat er in de praktijk gebeurt — geen enkel model werkt de eerste keer perfect.

---

## Deel 1: Je confusion matrix lezen (10 min)

Je krijgt de confusion matrix van het model dat je net hebt geconfigureerd. Dit is een tabel met vier vakken:

|  | **AI zegt: goed** | **AI zegt: defect** |
|--|-------------------|---------------------|
| **Echt goed** | Terecht goed | Vals alarm |
| **Echt defect** | Gemist defect | Terecht defect |

Vul het werkblad in met de getallen uit jouw confusion matrix:
- Hoeveel **terecht goed**? Het model zei goed en het was ook goed.
- Hoeveel **vals alarm**? Het model zei defect, maar het was goed.
- Hoeveel **gemist defect**? Het model zei goed, maar het was defect.
- Hoeveel **terecht defect**? Het model zei defect en het was ook defect.

Bereken de precision en recall met de formules op het werkblad.

---

## Deel 2: Waar gaat het mis? (10 min)

Vergelijk je confusion matrix met die van een ander duo.

Bespreek:
- Wie heeft meer valse alarmen?
- Wie heeft meer gemiste defecten?
- Welke fouten zijn erger voor jullie product?

> **De kernvraag:** Wat is erger — een vals alarm (goed product wordt weggegooid) of een gemist defect (defect product gaat naar de klant)?

---

## Deel 3: Precision en recall in operatortaal (10 min)

Twee begrippen die je moet kennen:

### Precision — als het model alarm slaat, hoe vaak is het dan echt raak?

- **Hoge precision** = weinig valse alarmen. Als het model zegt "defect", is het bijna altijd echt defect.
- **Lage precision** = veel valse alarmen. Je gooit te veel goede producten weg.

### Recall — van alle echte defecten, hoeveel vindt het model?

- **Hoge recall** = weinig gemiste defecten. Het model vindt bijna alle echte problemen.
- **Lage recall** = veel gemiste defecten. Defecte producten glippen erdoor.

> **Vuistregel:** Je kunt niet allebei maximaal hebben. Strengere drempels geven hogere precision maar lagere recall. Soepelere drempels geven hogere recall maar lagere precision.

### De verbetercyclus

Het model is nooit af. Net als een machine op de lijn heeft het bijsturing nodig:

1. **Test** — Bekijk de confusion matrix
2. **Analyseer** — Waar gaat het mis?
3. **Verbeter** — Meer data, betere labels, of drempel bijstellen
4. **Hertest** — Bekijk de nieuwe confusion matrix

---

## Deel 4: Verbeteractie formuleren (15 min)

Analyseer de fouten van je model. Vul het actieplan-werkblad in:

- **Welk type fout** is het grootste probleem?
- **Welke verbeteractie** ga je doen?
  - Meer foto's van een bepaald defect toevoegen?
  - Labels verbeteren (consistenter)?
  - Drempelwaarde bijstellen?
- **Stel een nieuwe drempelwaarde in** en bekijk het resultaat
- **Is het model verbeterd?**

Presenteer je aanpak in 1 minuut aan de groep.

---

## Samenvatting

| Begrip | In operatortaal |
|--------|----------------|
| **Confusion matrix** | Een tabel die laat zien wat het model goed en fout deed |
| **Precision** | Als het model alarm slaat, hoe vaak is het dan echt raak? |
| **Recall** | Van alle echte defecten, hoeveel vindt het model? |
| **Verbetercyclus** | Test, analyseer, verbeter, hertest — en dan weer opnieuw |

---

## Transferopdracht

Doe dit voor de volgende bijeenkomst:

1. Bedenk voor het product dat je op je werkvloer controleert: wat is belangrijker — precision of recall?
2. Schrijf op waarom
3. Bespreek dit met je leidinggevende
4. Neem je antwoord mee naar Module 3

> **Doe ook:** Vraag aan je kwaliteitsafdeling: hoeveel producten worden per week onterecht afgekeurd of onterecht doorgelaten? Dat zijn de getallen voor jouw eigen confusion matrix.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-actieplan-verbetering.md`](./werkbladen/wb-actieplan-verbetering.md) — Verbetering
2. [`wb-confusion-matrix.md`](./werkbladen/wb-confusion-matrix.md) — Matrix
3. [`wb-handout-precision-recall.md`](./werkbladen/wb-handout-precision-recall.md) — Precision recall
4. [`wb-reflectie-resultaten.md`](./werkbladen/wb-reflectie-resultaten.md) — Resultaten

## Verder

- Onderliggend kennisobject: [`ko-smart-mfg-513`](../../kennisbank/smart_manufacturing/computer_vision_kwaliteit/ko-smart-mfg-513.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
- Interactief: [`interactive/model.html`](./interactive/model.html)
