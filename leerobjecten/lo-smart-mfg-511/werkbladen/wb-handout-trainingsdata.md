# Handout: Best practices trainingsdata

**Leerobject:** Trainingsdata labelen en een model configureren
**Kolb-fase:** Theoretiseren
**Type:** Theorie-handout

---

## De drie stappen van trainingsdata

### Stap 1: Consistente foto's maken

| Doe dit | Doe dit niet |
|---|---|
| Altijd dezelfde belichting | Wisselend licht (schaduw = verwarring) |
| Effen achtergrond | Rommel op de achtergrond |
| Zelfde hoek en afstand | Steeds andere hoek |
| Scherpe foto's | Onscherpe of bewogen foto's |

**Vuistregel:** kun je het verschil tussen twee foto's niet zien, behalve het defect? Dan is de foto goed genoeg.

---

### Stap 2: Correct en consistent labelen

**Drie gouden regels:**

1. **Spreek criteria af** — wanneer is iets een defect? Schrijf het op. Gebruik dezelfde regels als bij je huidige controle.

2. **Label specifiek** — niet alleen "defect", maar ook het type. Denk aan kras, deuk of kleurafwijking. Hoe specifieker, hoe beter het model leert.

3. **Controleer je labels** — laat een collega steekproefsgewijs meekijken. Labels die niet kloppen zijn de grootste valkuil.

**Hoeveel foto's heb je nodig?**

| Situatie | Minimum |
|---|---|
| Goed vs. defect (eenvoudig) | 100-200 totaal |
| Meerdere defecttypes | 50-100 per type |
| Subtiele defecten | 200+ per type |

**Let op:** minimaal 30% van je foto's bevat een defect. Anders leert het model dat alles goed is.

---

### Stap 3: Verdelen in trainingsset en testset

```
Alle gelabelde foto's (100%)
├── Trainingsset (80%) → Hier leert het model van
└── Testset (20%)      → Hiermee controleer je het model
```

**Belangrijk:** de testset mag het model NOOIT zien tijdens het trainen. Anders weet je niet of het model nieuwe producten kan beoordelen.

**Vergelijk het met:** een toets maken terwijl je de antwoorden al kent. Dat is geen eerlijke test.

---

## Veelgemaakte fouten

| Fout | Gevolg | Oplossing |
|---|---|---|
| Inconsistente labels | Model raakt in de war | Criteria afspreken en opschrijven |
| Te weinig defecten in de set | Model zegt overal "goed" | Minimaal 30% defecte foto's *(vuistregel class balance)* |
| Verkeerde labels | Model leert het verkeerde | Steekproefsgewijs controleren |
| Wisselend licht op foto's | Model leert schaduw = defect | Vaste belichtingsopstelling |
| Testset te klein | Onbetrouwbare resultaten | Minimaal 20% voor testset |

---

*AIMM Pipeline | ko-smart-mfg-511 | Handout trainingsdata*
