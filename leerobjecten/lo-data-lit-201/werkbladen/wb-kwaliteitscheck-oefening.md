# Werkblad 3: Kwaliteitscheck-oefening -- Vind de Fouten

**Leerobject:** Datatypes herkennen en datakwaliteit beoordelen
**Fase:** Ervaren (oefening)
**Duur:** 15 minuten

---

## Wat ga je doen?

Bekijk de productiedataset hieronder. Er zitten bewuste fouten in. Voer de drie kwaliteitschecks uit en noteer elke fout.

---

## Dataset: Productieregistratie Lijn 2 -- Week 15

| Rij | Datum | Ploeg | Machine | Productie (stuks) | Afkeur (%) | Stilstand (min) | Temperatuur (C) | Opmerking |
|-----|-------|-------|---------|------------------|-----------|----------------|----------------|-----------|
| 1 | 2026-04-06 | Ochtend | CNC-01 | 234 | 1,2% | 18 | 185 | |
| 2 | 2026-04-06 | Middag | CNC-01 | 289 | 0,8% | 12 | 188 | |
| 3 | 2026-04-06 | Nacht | cnc01 | 201 | 1,5% | 22 | 182 | "Trillingen" |
| 4 | 2026-04-07 | Ochtend | CNC-01 | 245 | 1,1% | 15 | 186 | |
| 5 | 2026-04-07 | Middag | CNC-01 | 267 | 0,9% | | 187 | |
| 6 | 2026-04-07 | Nacht | CNC-01 | 198 | 1,8% | 28 | 183 | |
| 7 | 2026-04-08 | Ochtend | CNC-01 | 251 | 1,0% | 14 | 186 | |
| 8 | 2026-04-08 | | CNC-01 | 278 | 0,7% | 11 | 2850 | |
| 9 | 2026-04-08 | Nacht | CNC-01 | 205 | 1,4% | 25 | 181 | |
| 10 | 2026-04-09 | Ochtend | CNC-01 | 248 | 1,1% | 16 | 185 | |
| 11 | 2026-04-09 | Middag | CNC-01 | 271 | 0,8% | 13 | 188 | |
| 12 | 2025-03-15 | Nacht | CNC-01 | 195 | 2,1% | 32 | 179 | |
| 13 | 2025-03-16 | Ochtend | CNC-01 | 240 | 1,3% | 17 | 184 | |
| 14 | 2025-03-16 | Middag | CNC-01 | 265 | 0,9% | 14 | 187 | |
| 15 | 2025-03-16 | Nacht | CNC-01 | 199 | 1,6% | 0,5 uur | 180 | |

---

## Jouw bevindingen

### Check 1: Volledigheid

Welke gegevens ontbreken?

1. _________________________________________________

2. _________________________________________________

### Check 2: Consistentie

Welke gegevens zijn inconsistent?

1. _________________________________________________

2. _________________________________________________

3. _________________________________________________

### Check 3: Actualiteit

Welke gegevens zijn verouderd?

1. _________________________________________________

---

## Totaal aantal fouten gevonden: _____ / 5

---

## Antwoordmodel (na bespreking invullen)

| Fout | Check | Uitleg |
|------|-------|--------|
| Rij 5: stilstand ontbreekt | Volledigheid | Lege cel, geen waarde geregistreerd |
| Rij 8: ploeg ontbreekt | Volledigheid | Geen ploeg ingevuld |
| Rij 3: "cnc01" i.p.v. "CNC-01" | Consistentie | Andere schrijfwijze voor dezelfde machine |
| Rij 8: temperatuur 2850 graden | Consistentie | Onlogische waarde (waarschijnlijk 185) |
| Rij 15: stilstand in uren i.p.v. minuten | Consistentie | Andere eenheid (0,5 uur = 30 min) |
| Rij 12-15: data van maart 2025 | Actualiteit | Meer dan een jaar oud, niet van deze week |
