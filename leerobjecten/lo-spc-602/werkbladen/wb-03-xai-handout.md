# Handout: AI als aanvulling op SPC
*Wanneer schiet klassiek tekort, en wat voegt explainable AI toe?*

**Module 3 — SPC Op Maat | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Klassieke SPC vraagt: is het proces NU anders dan normaal? AI vraagt: welk PATROON leidt naar verstoring? Explainable AI vraagt: welke SIGNALEN dragen het meest bij?"**

Klassieke SPC en AI zijn geen concurrenten. Ze beantwoorden verschillende vragen. Wie het onderscheid kent, kiest gericht — en investeert alleen in AI waar klassieke regels structureel tekortschieten.

---

## Klassieke SPC versus AI — naast elkaar

> Deze tabel komt direct uit het onderliggende kennisobject. Lees hem twee keer: één keer om het onderscheid te zien, één keer om je af te vragen wélke aanname op jouw lijn realistisch is.

| Aanname klassieke SPC | Werkelijkheid moderne lijnen |
|------------------------|------------------------------|
| **Lage dimensionaliteit** (1 variabele tegelijk) | Tientallen sensoren tegelijk |
| **Lineaire verbanden** | Niet-lineaire interacties |
| **Onafhankelijke metingen** | Autocorrelatie tussen tijdspunten |
| **Stabiele baseline** | Dynamische, adaptieve processen |

---

## 🔴 Vier redenen waarom klassieke SPC tekortschiet

*Niet altijd, maar in moderne, sensorrijke lijnen wel structureel.*

| # | Reden | Wat is er aan de hand? |
|---|-------|------------------------|
| 1 | **Hoge dimensionaliteit** | Tien sensoren die ieder binnen ±3σ blijven kunnen collectief een fout-conditie aangeven. Geen Nelson-regel ziet dat — een multivariate AI wel. |
| 2 | **Niet-lineariteit** | Verstoringen ontstaan niet uit één variabele die te hoog wordt, maar uit een combinatie waarin variabele A bij hoge B en lage C een ander effect heeft dan elders. Shewhart-grenzen vangen dat niet. |
| 3 | **Autocorrelatie** | Klassieke SPC gaat ervan uit dat opeenvolgende metingen onafhankelijk zijn. Bij continue processen (chemie, energie, voedingsmiddelen) zijn metingen sterk gecorreleerd in de tijd, waardoor regelkaarten te veel of juist te weinig signalen geven. |
| 4 | **Drift / adaptieve processen** | Een 'normale' baseline schuift langzaam door slijtage, seizoensinvloeden of materiaal-batches. Een vaste UCL/LCL wordt structureel verkeerd — drift-aware modellen passen zich aan. |

---

## 🔵 Het nuttige onderscheid in vragen

| Vraag | Wie beantwoordt 'm? |
|-------|----------------------|
| "Is het proces **NU** anders dan normaal?" | **Klassieke SPC** (Shewhart, Nelson) |
| "Welk **PATROON** leidt naar verstoring?" | **AI** (predictive monitoring, multivariate) |
| "Welke **SIGNALEN** dragen het meest bij aan dit alarm?" | **Explainable AI** (SHAP, LIME) |

> **Praktisch:** Je hoeft niet één van de drie te kiezen. In een volwassen monitoring-architectuur draaien ze náást elkaar — Nelson detecteert univariate signalen kostenefficiënt, AI signaleert multivariate patronen, XAI maakt de AI-alarmen interpreteerbaar.

---

## 🟠 AI-uitbreidingen op SPC — kort overzicht

*Recente literatuur beschrijft vier hoofdtypen. Geen leveranciersvergelijking — alleen het concept.*

| Type | Wat doet het? |
|------|---------------|
| **AI-gebaseerde control charts** | Kernel methods of one-class classifiers vervangen of aanvullen Shewhart-grenzen — beter geschikt voor niet-lineaire grenzen. |
| **Deep learning** | Patroonherkenning in tijdreeksen (LSTM, Transformer) — leert lange-termijn-afhankelijkheden waar Nelson-regels blind voor zijn. |
| **Multivariate monitoring** | PCA, autoencoders — projecteren tientallen variabelen in een lager-dimensionale ruimte; afwijkingen zichtbaar maken die per variabele onzichtbaar zijn. |
| **Adaptieve detectie** | Drift-aware modellen — passen baseline en grenzen aan bij langzame procesveranderingen. |

---

## 🟣 Wat is XAI — Explainable AI?

> **In drie zinnen:**  
> Black-box AI geeft een alarm zonder te zeggen waarom. XAI legt erbij uit welke signalen het meest hebben bijgedragen aan het alarm. Daardoor kan een operator gericht handelen — en de AI vertrouwen.

**SHAP** (Shapley Additive Explanations) berekent voor elk alarm hoeveel elke variabele heeft bijgedragen aan de uitkomst van het AI-model. Het resultaat is een ranking per alarm: druk droeg 45% bij, temperatuur 30%, debiet 25%.

**Voorbeeld uit het kennisobject:**

> Bij een chemische reactor monitort klassieke SPC alleen de temperatuur — alle waarden binnen ±3σ, geen Nelson-regels triggeren. De AI-laag detecteert dat de combinatie temperatuur (+1σ) + druk (+0,5σ) + debiet (-0,8σ) een patroon vormt dat historisch in 78% van de gevallen vooraf ging aan een katalysator-degradatie binnen 4 uur.
>
> De operator krijgt een alarm met SHAP-verklaring: **"Druk is hoofdcontributor (45%), temperatuur tweede (30%), debiet derde (25%)."** Operator begrijpt waarom, kan gericht actie ondernemen (drukvalcheck), voorkomt 6-uur productiestop.

> **Stelregel:** In omgevingen met hoge proces- of veiligheidsimpact is XAI **geen optie maar een voorwaarde**. Zonder uitlegbaarheid ondermijnt een AI-systeem het operator-vertrouwen, en vertrouwen is de bottleneck — niet de techniek.

---

## ⚠️ Nelson is NIET verouderd — een waarschuwing

*Een veelgemaakte fout in AI-discussies: aannemen dat klassieke regels achterhaald zijn.*

> Het feit dat AI bepaalde patronen ziet die Nelson-regels niet zien, betekent **niet** dat Nelson-regels verouderd zijn. Het betekent wel dat ze in moderne lijnen soms te weinig zien van multivariate en niet-lineaire patronen.

**Waar Nelson-rules onverminderd nuttig zijn:**

- Univariate vragen ("is variabele X NU buiten controle?")
- Lijnen met weinig sensoren of beperkte data-historie
- Kostenefficiëntie: geen training, geen tuning, vanaf dag één bruikbaar
- Begrijpelijkheid: elke operator kan een Nelson-regel uitleggen
- Audit en regelgeving: veel kwaliteitsstandaarden eisen klassieke regelkaarten

**Stelregel:** Vervang Nelson niet — vul aan waar het tekortschiet. Een volwassen monitoring-architectuur gebruikt beide, ieder voor de vraag waarvoor het ontworpen is.

---

## 🟢 Implicatie voor de operator-rol

*Als AI-monitoring goed wordt ingericht, verandert het operator-werk wezenlijk.*

| Van | Naar |
|-----|------|
| **Detector** — zelf signalen scannen, regelkaarten lezen | **Interpreteerder** — alarm beoordelen, context wegen |
| **Regelvolger** — Nelson-rules toepassen | **Systeem-bewaker** — alarmen rationaliseren, foute alarmen markeren |
| **Reactief** — ingrijpen als grens overschreden wordt | **Anticiperend** — patroon-alarm gebruikt om eerder te handelen |

> **Belangrijk:** Deze rolverandering vraagt **data-literacy**. Zonder dat geen zinvolle interpretatie — alleen alarm-moeheid en wantrouwen. Voordat je AI uitrolt, investeer je in de data-literacy van het team dat ermee gaat werken.

---

## 🟢 Onthoud dit

1. **Klassieke SPC** beantwoordt: "Is het proces NU anders dan normaal?"
2. **AI** beantwoordt: "Welk PATROON leidt naar verstoring?"
3. **XAI** beantwoordt: "Welke SIGNALEN dragen het meest bij?"
4. Klassieke SPC schiet tekort bij hoge dimensionaliteit, niet-lineariteit, autocorrelatie en drift.
5. Nelson-rules zijn **niet verouderd** — vul aan, vervang niet.
6. **XAI is voorwaarde**, geen optie — zonder uitlegbaarheid geen operator-vertrouwen.
7. **Data-literacy** is de bottleneck van AI-uitbreiding, niet de techniek.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Univariaat** | Eén variabele tegelijk geanalyseerd |
| **Multivariaat** | Meerdere variabelen gezamenlijk geanalyseerd |
| **Autocorrelatie** | Opeenvolgende metingen hangen met elkaar samen — niet onafhankelijk |
| **Drift** | Langzame verschuiving van het procesgemiddelde of de variantie |
| **PCA** | Principal Component Analysis — wiskundige techniek om tientallen variabelen samen te vatten in een paar hoofdcomponenten |
| **Autoencoder** | Type AI-model dat 'normaal' gedrag leert reconstrueren — afwijkingen worden zichtbaar als reconstructiefout |
| **One-class classifier** | AI-model dat alleen 'normaal' kent, alles anders is een afwijking |
| **SHAP** | Shapley Additive Explanations — methode om per alarm uit te leggen welke variabelen het meest bijdroegen |
| **LIME** | Local Interpretable Model-agnostic Explanations — vergelijkbare uitlegmethode op basis van lokale benaderingen |
| **XAI** | Explainable AI — verzamelnaam voor uitlegbare AI-methoden |
| **Black-box model** | AI-model dat een uitkomst geeft zonder uitleg — voor productiemonitoring meestal onwenselijk |

---
*Bron: ko-spc-602 (AI als aanvulling op SPC); recente literatuur AI in process monitoring (2023–2024); Lundberg & Lee (SHAP, 2017); Ribeiro et al. (LIME, 2016) | AIMM Module 3 — SPC Op Maat | v1.0*
