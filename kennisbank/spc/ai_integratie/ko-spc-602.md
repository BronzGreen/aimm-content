---
id: ko-spc-602
title: AI als aanvulling op SPC — wanneer klassieke regels tekortschieten
type: concept_uitleg
domain: spc
subdomain: ai_integratie
summary: 'AI vult SPC vooral aan waar klassieke aannames zwakker worden:

  hoge dimensionaliteit, niet-lineariteit, autocorrelatie, complexe

  interacties. Klassieke SPC: "is het proces nu anders dan normaal?"

  AI: "welk patroon leidt naar verstoring?" Explainable AI is voorwaarde

  voor operator-vertrouwen.'
source_centrality: 0.7
source_ref: Recente literatuur AI in process monitoring (2023-2024); explainable AI
  overzichten
status: validated
updated_at: '2026-05-20'
correlation_id: ronde27-lo-spc-602
---

# AI als aanvulling op SPC — wanneer klassieke regels tekortschieten

## Wanneer schiet klassieke SPC tekort?
Traditionele control charts gaan uit van aannames die in moderne
productieomgevingen zwakker worden:

| Aanname klassieke SPC | Werkelijkheid moderne lijnen |
|------------------------|------------------------------|
| Lage dimensionaliteit (1 variabele) | Tientallen sensoren tegelijk |
| Lineaire verbanden | Niet-lineaire interacties |
| Onafhankelijke metingen | Autocorrelatie tussen tijdspunten |
| Stabiele baseline | Dynamische, adaptieve processen |

## AI-toevoegingen
Recente literatuur beschrijft AI-uitbreidingen op SPC:
- **AI-gebaseerde control charts** (kernel methods, one-class
  classifiers)
- **Deep learning** voor patroonherkenning in tijdreeksen
- **Multivariate monitoring** (PCA, autoencoders)
- **Adaptieve detectie** (drift-aware modellen)

## Het nuttige onderscheid voor operators

| Vraag | Wie beantwoordt 'm? |
|-------|----------------------|
| "Is het proces NU anders dan normaal?" | **Klassieke SPC** (Shewhart, Nelson) |
| "Welk PATROON leidt naar verstoring?" | **AI** (predictive monitoring) |
| "Welke SIGNALEN dragen het meest bij?" | **Explainable AI** (SHAP, LIME) |

## Nelson is niet "verouderd"
Het betekent **niet** dat Nelson-rules verouderd zijn. Het betekent
wel dat ze in moderne lijnen soms te weinig zien van **multivariate
en niet-lineaire patronen**.

Voorbeeld: tien sensoren die ieder binnen ±3σ blijven kunnen
collectief een fout-conditie aangeven. Geen Nelson-regel ziet dat,
maar een multivariate AI wel.

## Explainable AI (XAI) — voorwaarde, geen optie
Black-box-systemen zonder uitlegbaarheid **ondermijnen vertrouwen**,
vooral in omgevingen met hoge proces- of veiligheidsimpact.

Daarom veel aandacht voor:
- **SHAP** (Shapley Additive Explanations)
- **LIME** (Local Interpretable Model-agnostic Explanations)
- **Hybride interpretabele modellen**

Operators moeten begrijpen **waarom** een AI-alarm afgaat, niet
alleen dát het afgaat.

## Implicatie voor AIMM
AI vervangt operators niet, maar verandert hun rol:
- Van **detector** (zelf signalen scannen) naar **interpreteerder**
  (alarm beoordelen)
- Van **regelvolger** (Nelson-rules toepassen) naar **systeem-bewaker**
  (alarmen rationaliseren)
- Data Literacy is voorwaarde — zonder dat geen zinvolle interpretatie


## Praktijkvoorbeeld

*Fictieve illustratie van AI-assisted SPC — het scenario laat het samenspel zien tussen klassieke Nelson-regels en een AI-laag; geen specifieke casus.*

Bij een chemische reactor monitort een traditioneel SPC-systeem
temperatuur: alle waarden binnen ±3σ, geen Nelson-regels triggeren.
Maar de AI-laag detecteert dat de combinatie van **temperatuur**
(+1σ) + **druk** (+0,5σ) + **debiet** (-0,8σ) een patroon vormt dat
historisch in 78% van de gevallen vooraf ging aan een
katalysator-degradatie binnen 4 uur.

De operator krijgt een alarm met SHAP-verklaring: "Druk is
hoofdcontributor (45%), temperatuur tweede (30%), debiet derde
(25%)." Operator begrijpt waarom, kan gericht actie ondernemen
(drukvalcheck), voorkomt 6-uur productiestop.
