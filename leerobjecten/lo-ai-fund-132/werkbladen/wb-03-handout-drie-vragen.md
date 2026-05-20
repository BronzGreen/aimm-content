# Werkblad 3 — Drie vragen aan elke dataset
*Trainingsdata (leerdata) — Theorie-handout*

**Tijdsindicatie:** 12 minuten

---

## De drie eigenschappen van goede trainingsdata

Een AI-model leert uit voorbeelden. Drie eigenschappen bepalen of het goed leert.

### 1. Kwantiteit (hoeveelheid)

Hoeveel voorbeelden heb je per categorie?

Vuistregel: start met 100 tot 300 foto's per klasse. Dit is een richtlijn. Niet een wet. Per bedrijf kan het anders zijn.

### 2. Kwaliteit (kloppen de labels?)

Een label (antwoord) is het juiste antwoord bij een voorbeeld. Bij een foto: is dit 'goed' of 'kras'?

Klopt 1 op de 10 labels niet? Dan leert het model verkeerde patronen.

> "Garbage in, garbage out (rommel erin is rommel eruit)."
> — Russell & Norvig (2021)

### 3. Diversiteit (genoeg variatie?)

Zitten alle situaties erin? Denk aan:

- Dagploeg, avondploeg en nachtploeg.
- Kleine en grote defecten.
- Oude en nieuwe machines.

Mist een situatie? Dan herkent het model die straks niet.

---

## Terug naar fase 1

| Set | Kwantiteit | Kwaliteit | Diversiteit | Conclusie |
|---|---|---|---|---|
| A | OK | OK | Zwak (alleen ochtend) | Faalt op variatie |
| B | OK | Zwak (15% fout) | OK | Faalt op labels |
| C | Krap | OK | OK | Werkt — kleiner maar beter |

---

## Mijn aha-moment

Welke eigenschap had ik in fase 1 het minst meegewogen?

☐ Kwantiteit   ☐ Kwaliteit   ☐ Diversiteit

Wat nam ik nieuw mee uit deze handout? Markeer dit in de tekst hierboven.

---

## Vakwoorden in dit leerobject

- **Trainingsdata (leerdata)** — voorbeelden waarvan het juiste antwoord bekend is.
- **Label** — het antwoord bij een voorbeeld.
- **Kwantiteit** — hoeveelheid voorbeelden.
- **Kwaliteit** — kloppen de labels?
- **Diversiteit** — zit er genoeg variatie in?

---

*AIMM × BronzGreen — AI Fundamentals · Module 1 · Trainingsdata*
