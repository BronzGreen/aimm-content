---
id: ko-smart-mfg-513
title: 'Resultaten interpreteren: confusion matrix voor operators'
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Een confusion matrix toont vier uitkomsten van een AI-model in een tabel.
  Je ziet hoeveel producten het model terecht of onterecht als goed of defect beoordeelde.
  Precision en recall vertellen je hoe goed het model is.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-412
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-513
---

# Resultaten interpreteren: confusion matrix voor operators

Als je een vision-model hebt getraind en geconfigureerd, wil je weten: **hoe goed werkt het?** Daarvoor gebruik je een **confusion matrix** — een tabel met vier vakken die precies laat zien wat het model goed en fout doet.

## De vier uitkomsten

Elk product dat het model beoordeelt, valt in een van deze vier vakken:

|  | Model zegt: GOED | Model zegt: DEFECT |
|---|---|---|
| **Werkelijk GOED** | Terecht goed | Vals alarm |
| **Werkelijk DEFECT** | Gemist defect | Terecht defect |

### In gewone taal

- **Terecht goed**: het product is goed en het model zegt goed. Prima.
- **Terecht defect**: het product is defect en het model zegt defect. Prima.
- **Vals alarm**: het product is goed, maar het model zegt defect. Vervelend — je keurt een goed product onnodig af.
- **Gemist defect**: het product is defect, maar het model zegt goed. Gevaarlijk — een slecht product gaat door naar de klant.

## Precision en recall — twee getallen die ertoe doen

### Precision: "Hoe betrouwbaar zijn de alarmen?"

Van alle producten die het model als **defect** aanmerkt, hoeveel zijn er **echt** defect?

> Precision = terecht defect / (terecht defect + vals alarm)

**Hoge precision** = weinig valse alarmen. Als het model zegt "defect", is het meestal ook echt defect.

### Recall: "Hoeveel defecten vinden we?"

Van alle producten die **echt** defect zijn, hoeveel vindt het model er?

> Recall = terecht defect / (terecht defect + gemist defect)

**Hoge recall** = weinig gemiste defecten. Het model vindt bijna alle echte problemen.

### Wat is belangrijker?

Dat hangt af van je situatie:

| Situatie | Prioriteit | Waarom |
|---|---|---|
| Veiligheidsonderdelen | **Recall** | Een gemist defect kan gevaarlijk zijn |
| Cosmetische controle | **Precision** | Valse alarmen vertragen de lijn |
| Dure producten | **Beide** | Zowel afkeur als doorlating kost geld |

## Hoe lees je een confusion matrix?

**Voorbeeld:** een model controleert 100 onderdelen.

|  | Model: GOED | Model: DEFECT | **Totaal** |
|---|---|---|---|
| **Werkelijk GOED** | 55 | 5 | 60 |
| **Werkelijk DEFECT** | 3 | 37 | 40 |
| **Totaal** | 58 | 42 | 100 |

- Precision = 37 / (37 + 5) = **88%** — van de 42 afgekeurde producten waren er 37 echt defect
- Recall = 37 / (37 + 3) = **93%** — van de 40 echte defecten vond het model er 37

**Vraag jezelf af:** zijn die 3 gemiste defecten acceptabel? Zijn die 5 valse alarmen te handelen?

## Praktijkvoorbeeld

Een vision-model controleert 100 metalen onderdelen. De confusion matrix laat zien: 55 terecht goed, 5 vals alarm (goed product afgekeurd), 3 gemist defect (defect product doorgelaten), en 37 terecht defect. De precision is 37/(37+5) = 88% — van alle producten die het model afkeurde, was 88% echt defect. De recall is 37/(37+3) = 93% — van alle echte defecten vond het model 93%. De operator besluit dat 3 gemiste defecten te veel is voor veiligheidsonderdelen en verlaagt de drempelwaarde.
