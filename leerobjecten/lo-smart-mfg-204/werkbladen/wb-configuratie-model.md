# Werkblad 1: Configuratie-werkblad -- Je Eerste Predictief Model

**Leerobject:** Je eerste predictief model configureren
**Fase:** Experimenteren (Ronde 1 -- Jij doet)
**Duur:** 15 minuten

---

## De opdracht

Je hebt een dataset van een verpakkingsmachine: 100 cycli sensordata. Je hebt de 5-stappen handleiding als naslagkaart. Doorloop alle vijf stappen en vul dit werkblad in.

---

## Stap 1: Kies je machine

**Machine:** Verpakkingsmachine (gegeven in de opdracht)

**Waarom deze machine?**

_________________________________________________

**Storingshistorie (uit de dataset):** Hoeveel ongeplande stops zie je in de data?

Aantal: _____

---

## Stap 2: Selecteer je sensoren

Bekijk de dataset. Er zijn drie sensoren beschikbaar. Kies minimaal twee.

| Sensor | Beschikbaar | Gebruik ik | Waarom wel/niet? |
|--------|-------------|-----------|-----------------|
| Temperatuur sealbalken | Ja | [ ] Ja [ ] Nee | _________________________ |
| Trillingen aandrijfmotor | Ja | [ ] Ja [ ] Nee | _________________________ |
| Druk pneumatiek | Ja | [ ] Ja [ ] Nee | _________________________ |

---

## Stap 3: Bepaal de normaalwaarden

Bekijk de normaaldata in de dataset (de eerste 50 cycli zijn "normaal"). Bereken per sensor:

**Sensor 1: ___________________________**

| Wat | Waarde | Eenheid |
|-----|--------|---------|
| Laagste meting | _______ | _______ |
| Hoogste meting | _______ | _______ |
| Gemiddelde | _______ | _______ |
| Spreiding | _______ | _______ |

**Sensor 2: ___________________________**

| Wat | Waarde | Eenheid |
|-----|--------|---------|
| Laagste meting | _______ | _______ |
| Hoogste meting | _______ | _______ |
| Gemiddelde | _______ | _______ |
| Spreiding | _______ | _______ |

**Sensor 3 (optioneel): ___________________________**

| Wat | Waarde | Eenheid |
|-----|--------|---------|
| Laagste meting | _______ | _______ |
| Hoogste meting | _______ | _______ |
| Gemiddelde | _______ | _______ |
| Spreiding | _______ | _______ |

---

## Stap 4: Stel drempelwaarden in

Gebruik de formule: waarschuwing = gemiddelde + 1,5 x spreiding, alarm = gemiddelde + 2 x spreiding.

**Sensor 1: ___________________________**

| Drempel | Berekening | Waarde |
|---------|-----------|--------|
| Waarschuwing | _______ + 1,5 x _______ = | _______ |
| Alarm | _______ + 2 x _______ = | _______ |
| Vertraging | | _______ sec |

**Sensor 2: ___________________________**

| Drempel | Berekening | Waarde |
|---------|-----------|--------|
| Waarschuwing | _______ + 1,5 x _______ = | _______ |
| Alarm | _______ + 2 x _______ = | _______ |
| Vertraging | | _______ sec |

---

## Stap 5: Draai de eerste test

Pas je drempels toe op de testdata (cycli 51-100). Tel de resultaten.

| Resultaat | Aantal |
|-----------|--------|
| Waarschuwingen | _______ |
| Alarmen | _______ |
| Valse alarmen (machine draaide prima) | _______ |
| Gemiste problemen (storing zonder alarm) | _______ |

**Ben je tevreden met dit resultaat?** [ ] Ja [ ] Nee

**Waarom?**

_________________________________________________

---

*Bewaar dit werkblad. Je hebt het nodig bij de duo-vergelijking en bij ronde 2.*
