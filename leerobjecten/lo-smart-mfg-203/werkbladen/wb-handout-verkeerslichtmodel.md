# Handout: Het Verkeerslichtmodel + 5-Staps Actieplan

**Leerobject:** lo-smart-mfg-203 | **Kolb-fase:** Theoretiseren
**Bewaar deze handout — je hebt hem nodig op de werkvloer!**

---

## Het Verkeerslichtmodel

De anomaliescore (afwijkingsscore) vertelt je hoe ongewoon de machine zich gedraagt. Hoe hoger de score, hoe meer er afwijkt van normaal.

```
  GROEN            ORANJE              ROOD
  0 ────── 30 ────── 70 ────── 100
  Normaal     Let op, monitor      Ingrijpen!
  Geen actie  extra                Plan onderhoud
```

### Groen: score 0-30

- De machine draait **normaal**.
- Alle sensoren zijn stabiel.
- **Actie:** Geen. Doorgaan.

### Oranje: score 30-70

- Er is **iets veranderd**, maar het is nog niet kritiek.
- Mogelijke oorzaken:
  - Een sensor begint langzaam af te wijken
  - De machine gedraagt zich net iets anders
  - Er is iets veranderd in de omgeving of het product
- **Actie:** Zoek uit welke sensor het is. Kijk of er een verklaring is. Check vaker. Meld het bij de overdracht.

### Rood: score 70-100

- De machine wijkt **sterk af** van normaal.
- De kans op een storing neemt toe.
- **Actie:** Zoek direct uit welke sensor afwijkt. Plan inspectie of onderhoud. Overleg met de technische dienst. Leg het vast.

---

## Het 5-Staps Actieplan (bij oranje of rood)

Gebruik dit stappenplan als de score boven de 30 komt:

| Stap | Wat doe je? | Voorbeeld |
|------|-------------|-----------|
| **1** | Kijk welke **sensor** de hoogste bijdrage levert aan de score | "De trillingssensor op de Y-as drijft de score omhoog" |
| **2** | Check of er een **logische verklaring** is | Productwissel? Recent onderhoud? Temperatuur buiten? |
| **3** | **Vergelijk** met eerdere situaties | "Heeft deze sensor eerder zo gedaan? Wat gebeurde er toen?" |
| **4** | **Beslis:** monitoren of ingrijpen? | Monitoren = vaker checken. Ingrijpen = inspectie/onderhoud plannen. |
| **5** | **Documenteer** je beslissing en het resultaat | Schrijf op wat je zag, wat je deed, en wat er gebeurde |

---

## Wanneer vertrouw je de score NIET blindelings?

De score kan misleidend zijn in drie situaties:

| Situatie | Waarom misleidend? | Wat doe je? |
|----------|--------------------|-------------|
| **Na een productwissel** | Het model kent de nieuwe instellingen nog niet | Wacht 2-3 dagen. Monitor extra. |
| **Na onderhoud** | Nieuwe onderdelen geven andere sensorwaarden | Wacht tot de machine stabiel draait (ca. 2 weken). |
| **Seizoensverandering** | De buitentemperatuur beinvloedt sensordata | Houd rekening met de context. |

**Vuistregel:** Je kunt de score vertrouwen als de machine al minimaal **2 weken stabiel** draait. En als de omstandigheden hetzelfde zijn gebleven.

---

*Bron: ko-smart-mfg-203 — Modelresultaten interpreteren*
