# Architectuur invullen: de vier lagen van een CNN
*Kolb fase 1 — Theoretiseren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: CNN-architectuur**

---

> **Over dit werkblad**
> Je luistert naar het mini-college over een CNN (Convolutional Neural Network, oftewel een vouw-netwerk). De trainer loopt het diagram door: input, daarna de convolutielaag, dan pooling, dan fully connected, en als laatste de output. Per laag noteer je in eigen woorden wat de laag doet. Je noteert ook wat de laag zou kunnen "zien" in jouw soort werkvloer-data.
>
> **Tijd:** 17 minuten.
>
> **Waarom dit werkblad?**
> Een CNN is geen toverdoos. Het is een keten van lagen, en elke laag heeft een eigen taak. Als je die keten kunt natekenen, kun je beter meedenken met de leverancier. Je weet dan ook waarom een camera-inspectie soms een kras mist of een dashboard-melding wel of niet klopt.

---

## 1. Het lege architectuur-schema

*Vul tijdens de uitleg per laag de twee kolommen in. Gebruik korte zinnen. Bij twijfel mag je een vraagteken zetten. Die nemen we straks samen door.*

| Laag | Wat doet deze laag? | Wat zou hij kunnen "zien" of opleveren? |
|------|---------------------|------------------------------------------|
| **1. Input** | | |
| **2. Convolutielaag** (kernel = klein zoekvenster) | | |
| **3. Pooling** (samenvatten) | | |
| **4. Fully connected** (integreren) | | |
| **5. Output** | | |

---

## 2. Twee sleutelwoorden — in eigen taal

*De trainer benoemt twee kernconcepten. Die maken het verschil met een gewoon netwerk waarin alle cellen aan elkaar hangen.*

| Concept | Mijn omschrijving |
|---------|-------------------|
| **Lokale connectiviteit** (de kernel kijkt klein) | |
| **Shared weights** (gedeelde gewichten — overal hetzelfde glas) | |

*Welke van de twee was voor jou het lastigst om te volgen?*

○ Lokale connectiviteit   ○ Shared weights   ○ Allebei goed gevolgd

---

## 3. De analogie van de speurder

> Een speurder kijkt door een vergrootglas (de kernel) over een foto en markeert overal kraspatronen. Het vergrootglas is steeds hetzelfde glas. Daarom heet het "gedeelde gewichten". Het glas ziet alleen wat eronder ligt. Daarom heet het "lokale connectiviteit". Wat de speurder vindt, schrijft hij op een nieuwe kaart. Die kaart heet de feature map (kenmerk-kaart).

*Vink aan wat je hierin herkent.*

- [ ] Ik snap waarom het vergrootglas (de kernel) klein is
- [ ] Ik snap waarom hetzelfde glas overal wordt gebruikt
- [ ] Ik snap dat de feature map laat zien wat de kernel oppikte
- [ ] Ik kan dit in eigen woorden navertellen

---

## 4. Werkvloer-voorbeelden: beeld en tijdreeks

*Een CNN werkt op beelden (2D) maar ook op tijdreeksen (1D, bijvoorbeeld een trillingssignaal). Vul in:*

| Type data | Wat is een "klein patroon" dat de kernel opzoekt? |
|-----------|----------------------------------------------------|
| **Camera-inspectie** op een lasergravure-plaatje | |
| **Sorteersysteem** met camera boven een lopende band | |
| **Trillingsmeting** op een rollager (tijdreeks) | |
| **Storingsclassificatie** op een geluidsfragment | |

---

## 5. Eerste check: snap ik het?

*Vink aan wat je nu kunt.*

- [ ] Ik kan de vier lagen op volgorde benoemen
- [ ] Ik kan per laag in één zin uitleggen wat hij doet
- [ ] Ik begrijp het verschil tussen lokaal en globaal kijken
- [ ] Ik snap waarom een CNN minder parameters heeft dan een fully-connected netwerk

> **Tip:** Lukt een vraag nog niet? Markeer hem. In fase 2 ga je de architectuur toepassen op vier data-voorbeelden. Daar valt het concept vaak op zijn plek.

---

## Wat doen we hierna?

In fase 2 (Ervaren) krijg je vier korte data-voorbeelden van de werkvloer. Per voorbeeld ga je beoordelen: past een CNN hier wel of niet? Het schema dat je hier invult, neem je daar als denkraam mee. Houd je antwoorden bij de hand. We pakken straks de werkblad-pagina van fase 2 erbij.

---
*Bron: CNN-architectuur — AIMM Curriculum | Module 2: Train | v1.0*
