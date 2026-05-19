# Handout: Control limits versus specificatiegrenzen
*Het verschil, de 3σ-formule, en de NIST-waarschuwing*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**  
> Control limits zeggen of je **proces** stabiel loopt. Specificatiegrenzen zeggen of je **product** voldoet aan wat de klant vraagt. Dat zijn twee verschillende vragen. Wie die twee door elkaar haalt, verliest de hele signaalwaarde van SPC.

---

## Het verschil in één tabel

| | **Control limits (UCL/LCL)** | **Specificatiegrenzen** |
|---|------------------------------|-------------------------|
| **Welke vraag?** | Is het PROCES stabiel? | Voldoet het PRODUCT aan de eisen? |
| **Waar komen ze vandaan?** | Uit eigen procesdata (gemiddelde ± 3σ) | Van de klant of het ontwerp |
| **Waar staan ze op de kaart?** | Op de regelkaart | NIET op de regelkaart (apart, of helemaal niet) |
| **Welke beslissing?** | "Moet ik ingrijpen in het proces?" | "Mag dit onderdeel naar de klant?" |
| **Verandert met?** | Procesgedrag (nieuwe data → nieuwe limits) | Klantafspraak of ontwerpwijziging |

---

## 🔵 De 3σ-formule (Shewhart, 1931)

Control limits bereken je uit de **werkelijke procesmetingen** van je eigen lijn. De formule komt van Walter A. Shewhart (Bell Labs, 1931) — de uitvinder van de regelkaart.

```
UCL = gemiddelde + 3σ
LCL = gemiddelde − 3σ
```

Wat je nodig hebt:
- Een reeks opeenvolgende metingen (minimaal 25-30) van een **stabiel lopend proces**
- Het gemiddelde (optelsom gedeeld door aantal)
- De standaardafwijking σ (meestal door Excel of SPC-software berekend)

**Voorbeeld:** bij een spuitgietlijn is het gemiddelde gewicht 99,9 g en σ = 0,12 g.
- UCL = 99,9 + 3 × 0,12 = **100,26 g**
- LCL = 99,9 − 3 × 0,12 = **99,54 g**

---

## 🔴 NIST waarschuwt expliciet

Het Amerikaanse NIST/SEMATECH is een referentie-instituut voor meet- en procesbeheersing. In het *NIST/SEMATECH e-Handbook of Statistical Methods* staat zwart op wit gewaarschuwd:

> Een proces kan **stabiel** zijn (binnen control limits) en toch **te dicht bij de specificatiegrens** zitten (lage capability).  
> Omgekeerd: een proces kan incidenteel **binnen specs** produceren terwijl het proces **al uit controle** is.

Met andere woorden: de twee zijn onafhankelijk.
- Binnen specs → goed product, zegt niets over het proces.
- Binnen control limits → stabiel proces, zegt niets over of het product de klant tevreden stelt.

Je hebt ze **allebei** nodig, maar op **aparte** manieren.

---

## 🔴 De kritieke fout

Op veel werkvloeren gebeurt dit: iemand maakt een regelkaart en zet de specs (bv. 99-101) als UCL/LCL neer. Klaar. De kaart ziet er goed uit.

Wat is er fout aan?

1. Het is **geen procesbeeld meer** — je hebt een pass/fail-grafiek getekend.
2. Je **verbergt signalen** die binnen specs blijven maar wel op procesverandering wijzen.
3. Een trend van 99,8 → 99,9 → 100,0 → 100,1 geeft **nooit** een signaal in deze opzet — terwijl het een duidelijk procesverloop laat zien.
4. Je mist het **vroege signaal** — en dus het goedkoopste moment om in te grijpen.
5. Je verliest de **hele waarde van SPC**: vroeg signaleren in plaats van achteraf afkeuren.

**De regel:** nooit control limits uit klanttoleranties afleiden.

---

## 🟢 Hoe wel?

1. Verzamel **25-30 opeenvolgende metingen** van een stabiel lopend proces.
2. Bereken gemiddelde + standaardafwijking σ (Excel of SPC-software).
3. Bereken **UCL = gemiddelde + 3σ** en **LCL = gemiddelde − 3σ**.
4. Teken UCL en LCL op de regelkaart.
5. Specs? **Apart weergeven** of **helemaal niet op de kaart** — sommige bedrijven houden specs bewust weg van de regelkaart om verwarring te voorkomen.
6. Herbereken de control limits bij procesverandering (nieuwe matrijs, nieuwe instelling, groot onderhoud).

---

## 🟠 Drie scenario's naast elkaar

| Situatie | Proces stabiel? | Product binnen specs? | Wat moet je doen? |
|----------|-----------------|----------------------|--------------------|
| Binnen UCL/LCL én binnen specs | Ja | Ja | Laat lopen — dit is wat je wilt |
| Binnen UCL/LCL, maar vlak tegen specs | Ja | Krap | Capability verbeteren (minder spreiding) |
| Buiten UCL/LCL, maar nog binnen specs | Nee | Ja (toevallig) | Ingrijpen — proces is al aan het afwijken, alleen nog niet zichtbaar bij de klant |
| Binnen UCL/LCL, buiten specs | Ja | Nee | Proces opnieuw afstellen / centreren |

Het derde scenario is precies waar SPC zijn waarde bewijst: je grijpt in vóór de klant klaagt. Dat kan alleen als je control limits **echte** control limits zijn.

---

## 🟢 Onthoud dit

1. **Control limits ≠ specificatiegrenzen.** Twee verschillende vragen, twee verschillende grenzen.
2. **Control limits bereken je uit procesdata** (3σ-regel van Shewhart).
3. **Specificatiegrenzen komen van de klant of het ontwerp** — niet uit metingen.
4. **NIST waarschuwt: verwar ze niet**, want dan verlies je signaaldetectie.
5. **Bij twijfel over je eigen kaart**: vraag aan je teamleider of SPC-coördinator hoe de grenzen bepaald zijn.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **UCL** | Upper Control Limit — bovenste grens waarbinnen een stabiel proces normaal blijft |
| **LCL** | Lower Control Limit — onderste grens waarbinnen een stabiel proces normaal blijft |
| **σ (sigma)** | Standaardafwijking — maat voor de normale spreiding van je proces |
| **3σ-regel** | UCL/LCL liggen op 3 × σ afstand van het gemiddelde (Shewhart 1931) |
| **Specificatiegrens** | Grens die de klant of het ontwerp aan het product stelt |
| **Capability** | Mate waarin het proces (UCL-LCL) binnen de specs past |
| **Tolerantie** | Ander woord voor specificatiegrens (plus/min rond het doel) |

---

## Bronnen

- **NIST/SEMATECH** *e-Handbook of Statistical Methods* — sectie over Control Charts en Specification Limits. Vrij toegankelijk: https://www.itl.nist.gov/div898/handbook/
- **Shewhart, W.A. (1931)** *Economic Control of Quality of Manufactured Product.* — oorspronkelijke publicatie waarin de 3σ-regel is geïntroduceerd.
- **ISO 7870-2** — internationale standaard voor Shewhart-regelkaarten.

---

*AIMM Module 1 — SPC Gebruik | v1.0*
