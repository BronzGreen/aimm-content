# Handout: Precision, recall en de verbetercyclus

**Leerobject:** Resultaten interpreteren en het model verbeteren
**Kolb-fase:** Theoretiseren
**Type:** Theorie-handout

---

## Confusion matrix — de vier uitkomsten

|  | Model zegt: GOED | Model zegt: DEFECT |
|---|---|---|
| **Werkelijk GOED** | Terecht goed | Vals alarm |
| **Werkelijk DEFECT** | Gemist defect | Terecht defect |

---

## Precision en recall in operatortaal

### Precision (trefzekerheid): "Hoe betrouwbaar zijn de alarmen?"

> Van alle producten die het model afkeurt: hoeveel zijn er ECHT defect?

**Hoge precision** = als het model "defect" zegt, klopt dat bijna altijd. Weinig onnodig afgekeurde producten.

### Recall (vangst): "Hoeveel defecten vangen we?"

> Van alle producten die ECHT defect zijn: hoeveel vindt het model?

**Hoge recall** = het model mist bijna geen echte defecten. Weinig slechte producten gaan door.

---

## Wanneer kies je wat?

| Jouw situatie | Prioriteit | Richtlijn |
|---|---|---|
| Veiligheidsonderdelen | **Recall > 95%** | Liever een vals alarm dan een gemist defect |
| Cosmetische controle | **Precision > 90%** | Liever een gemist cosmetisch foutje dan de lijn stilleggen |
| Dure producten | **Allebei > 85%** | Zowel afkeur als doorlating kost geld |
| Standaard kwaliteitscontrole | **Recall > 85%, Precision > 80%** | Goede balans |

---

## De verbetercyclus

Een model is nooit "af". Verbeteren gaat in vier stappen:

```
    ┌──────────┐
    │  1. TEST  │ ← Draai het model op testset
    └────┬─────┘
         │
    ┌────▼──────────┐
    │  2. ANALYSEER  │ ← Bekijk de confusion matrix
    └────┬──────────┘
         │
    ┌────▼─────────┐
    │  3. VERBETER  │ ← Kies een van de drie strategieen
    └────┬─────────┘
         │
    ┌────▼─────────┐
    │  4. HERTEST   │ ← Draai opnieuw, vergelijk
    └────┬─────────┘
         │
         └──── Herhaal tot goed genoeg
```

---

## Drie verbeterstrategieen

### 1. Meer data toevoegen

- Welk type defect mist het model? Maak meer foto's van dat type.
- Model verwart schaduwen met defecten? Meer foto's met variatie in belichting.
- Nieuw type defect? Label foto's van het nieuwe defect en hertrainen.

**Vuistregel:** voeg GERICHTE foto's toe van wat het model fout doet.

### 2. Labels verbeteren

- Controleer of alle labels correct en consistent zijn.
- Spreek duidelijke criteria af met je team.
- Laat een collega steekproefsgewijs meekijken.

### 3. Drempelwaarde bijstellen

- Te veel gemiste defecten? Drempel verlagen (strenger).
- Te veel valse alarmen? Drempel verhogen (soepeler).
- Of: twijfelzone breder maken.

---

## Wanneer is het "goed genoeg"?

Niet als het perfect is. Maar als het **beter is dan de huidige situatie**.

Vraag jezelf af:
- Vindt het model meer defecten dan een operator na 6 uur?
- Wegen de gemiste defecten op tegen de kosten van valse alarmen?
- Is de recall hoog genoeg voor mijn product?

---

*AIMM Pipeline | ko-smart-mfg-513/514 | Handout precision, recall en verbetercyclus*
