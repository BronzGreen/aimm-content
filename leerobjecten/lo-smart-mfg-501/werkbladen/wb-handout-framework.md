# Handout: Kosten-baten framework + datakwaliteit-checklist

**Module 3: Op Maat | Predictive Maintenance**

---

## Machine selecteren: drie criteria

| Criterium | Vraag | Hoe te meten |
|-----------|-------|-------------|
| **1. Stilstand** | Welke machine staat het vaakst ongepland stil? | Storingsregistratie: uren/jaar |
| **2. Kosten** | Wat kost elk uur stilstand? | Verloren productie + arbeid + materiaal |
| **3. Haalbaarheid** | Kan ik hiermee starten? | Sensoren aanwezig? Toegankelijk? Team mee? |

**Vuistregel:** kies de machine met de hoogste besparing. Die ook praktisch haalbaar is.

---

## Potentiele besparing berekenen

```
Besparing per jaar = uren stilstand x kosten per uur x 50%
```

- 50% is een conservatieve schatting
- In de praktijk halen bedrijven vaak 50-70% reductie *(bron: Mobley 2002, hoofdstukken 8-9 — klassieke PM-referentie)*
- Begin met 50% — als je meer haalt, is dat bonus

---

## Datakwaliteit-checklist

Voordat je een model kunt bouwen, is het goed om te checken of je data aan vier eisen voldoet:

| Criterium | Wat het betekent | Check |
|-----------|-----------------|-------|
| **Volledigheid** | Geen grote gaten in de data | ☐ Meer dan 90% van de metingen aanwezig |
| **Consistentie** | De sensor meet steeds op dezelfde manier | ☐ Geen plotselinge sprongen zonder oorzaak |
| **Nauwkeurigheid** | De waarden kloppen met de werkelijkheid | ☐ Sensor is gekalibreerd (afgelopen 12 maanden) |
| **Tijdstempel** | Elke meting heeft datum en tijd | ☐ Datum + tijd bij elke meting |

**Vuistregel:** meer dan 10% ontbrekende of onbetrouwbare data? Dan eerst de dataverzameling verbeteren.

---

## Minimale eisen voor een pilot

- Minimaal **3 maanden** historische data (liefst 6-12 maanden)
- Minimaal **1 relevante sensor** (temperatuur, trillingen of druk)
- Meetfrequentie: minimaal **elke minuut** (liefst elke 10 seconden)
- Data is **exporteerbaar** of via dashboard in te zien
