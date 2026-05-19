# Handout: Hoe werkt AI-visuele inspectie?

**Leerobject:** Visuele kwaliteitscontrole met AI
**Kolb-fase:** Theoretiseren
**Type:** Theorie-handout
**Bewaar dit blad** — je kunt het later nog gebruiken.

---

## AI-visuele inspectie in 4 stappen

```
    Stap 1           Stap 2           Stap 3           Stap 4
  ┌─────────┐     ┌─────────┐     ┌─────────┐     ┌─────────┐
  │  Camera  │────>│   AI    │────>│ Goed of │────>│Twijfel? │
  │maakt foto│     │bekijkt  │     │ defect? │     │Operator!│
  └─────────┘     └─────────┘     └─────────┘     └─────────┘
```

| Stap | Wat gebeurt er? | Voorbeeld |
|------|----------------|-----------|
| 1. Camera maakt foto | De camera maakt van elk product een foto | De camera boven de band fotografeert elke behuizing |
| 2. AI analyseert | Het AI-model bekijkt de foto op defecten | Het model zoekt krassen, deuken en kleurafwijkingen |
| 3. Classificatie (indeling) | De AI geeft een score: hoe groot is de kans op een defect? | Score 0.92 = waarschijnlijk defect. Score 0.12 = waarschijnlijk goed. |
| 4. Twijfelgevallen | Bij twijfel bekijkt een inspecteur het product | Score tussen 0.40 en 0.70 = jij bekijkt het |

---

## Wat kan de AI wel en niet?

| De AI kan... | De AI kan niet... |
|---|---|
| Duizenden producten per dag bekijken | Zelf nieuwe defecten leren herkennen |
| Altijd hetzelfde oordelen (consistent) | Begrijpen waarom een defect erg is |
| Kleine defecten zien die je oog mist | Werken zonder voorbeeldfoto's |
| 24/7 werken zonder moe te worden | Omgaan met onverwachte situaties |

---

## Soorten defecten die AI kan detecteren

- Krassen en deuken op oppervlakken
- Foutieve opdrukken (bijv. logo's)
- Ontbrekende onderdelen
- Kleurafwijkingen
- Maatafwijkingen

---

## Praktijkvoorbeeld: Philips Drachten

*(Bron: Rožanec et al. 2024, Artificial Intelligence in Manufacturing — Philips visuele kwaliteitscontrole scheerapparaten, kapjes, tandenborstelschachten.)*

| Product | Wat controleert de AI? | Resultaat |
|---|---|---|
| Scheerapparaten | Logo compleet en scherp? | Minder controles met de hand |
| Decoratieve kapjes | Vloeisporen in het plastic? | Snellere detectie |
| Tandenborstelschachten | Deuken of strepen? | Consistenter oordeel |

**De inspectietijd daalde met 60%.** De operator bekijkt alleen nog de twijfelgevallen.

---

## Belangrijk om te onthouden

1. **De AI vervangt je niet** — de AI helpt je
2. **Elk product heeft een eigen model nodig** — er is geen universele AI
3. **Het model leer je aan** met honderden voorbeeldfoto's
4. **Jij blijft nodig** voor moeilijke gevallen en nieuwe defecten

---

## Noteer voor jezelf

Welk type defect op jouw werkvloer zou een AI goed kunnen herkennen?

_____________________________________________________________

Welk type defect juist niet? Waarom niet?

_____________________________________________________________

---

*AIMM Pipeline | ko-smart-mfg-095 | Handout theorie*
