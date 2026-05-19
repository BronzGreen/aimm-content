# Handout: De zeven regelkaart-types
*Welke kaart hoort bij welke meting — keuzehulp voor operators*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale vragen (uit je hoofd waard)**  
> **1. Meet je een getal (continue) of tel je defecten?**  
> **2. Is je steekproef elke keer even groot of varieert die?**  
>
> Die twee vragen leiden je altijd naar de juiste kaart.

---

## De zeven kaart-types in één tabel

| Kaart | Wanneer gebruiken | Hoe wordt hij gemaakt | Hoe lees je hem af | Voorbeeld uit de maakindustrie |
|-------|-------------------|-----------------------|--------------------|--------------------------------|
| **X̄-R** | Continue metingen, **kleine** subgroepen (2–8, meestal 4 of 5) | Gemiddelde + range per subgroep | Boven: verschuift het gemiddelde? Onder: blijft de spreiding stabiel? | Elke 2 uur 5 onderdelen wegen op spuitgietlijn |
| **X̄-S** | Continue metingen, **grotere** subgroepen of meer precisie | Gemiddelde + standaarddeviatie per subgroep | Geschikt als n groter is en range te grof wordt | Diameter- of diktemetingen in automatische meetcel |
| **I-MR** | Eén meting per moment of batch (geen subgroep mogelijk) | Individuele waarden + moving range | Handig bij batch-, tank- of lotmetingen | Viscositeit per batch in voeding of chemie |
| **p-kaart** | Attribuutdata, **wisselende** steekproefomvang | Percentage defecte stuks | Defectpercentage en patronen in de tijd | % lekkende verpakkingen per gecontroleerde steekproef |
| **np-kaart** | Attribuutdata, **vaste** steekproefomvang | Aantal defecte stuks per vaste steekproef | Zelfde logica als p, maar in aantallen | Aantal fout-geassembleerde sets in monsters van 50 |
| **c-kaart** | Tellingen per **gelijke** eenheid | Aantal defecten per vaste eenheid | Meer fouten per object dan normaal? | Aantal krassen per vast plaatoppervlak |
| **u-kaart** | Tellingen per **wisselende** eenheid (oppervlakte of tijd) | Defecten per eenheid of inspectievolume | Defectdichtheid, niet ruwe telling | Aantal fouten per meter folie |

---

## 🔵 De beslis-stroom — gebruik deze!

```
Wat meet je?

├── Een getal (continue meting)?
│     │
│     ├── Kun je een subgroep nemen (meerdere metingen achter elkaar)?
│     │     │
│     │     ├── Kleine subgroep (2 tot 8)? .......... X̄-R
│     │     └── Grotere subgroep? ................... X̄-S
│     │
│     └── Nee, maar één meting per moment? ......... I-MR
│
└── Tellingen van defecten?
      │
      ├── Percentage defecten?
      │     │
      │     ├── Vaste steekproef? ................. np-kaart
      │     └── Wisselende steekproef? ............ p-kaart
      │
      └── Aantal defecten per eenheid?
            │
            ├── Gelijke eenheid? .................. c-kaart
            └── Wisselende eenheid? ............... u-kaart
```

---

## 🟣 Twee vuistregels om te onthouden

### Vuistregel 1 — R versus S: subgroep-grootte beslist

Gebruik **R-kaarten bij kleine** subgroepen (2–8). Bij **grotere** subgroepen wordt de range-berekening te grof en wordt een **S-kaart** (standaarddeviatie) efficiënter en nauwkeuriger.

> **NIST:** zodra de subgroep groter wordt, wordt de S-kaart efficiënter dan de R-kaart.

### Vuistregel 2 — I-MR pas als laatste keuze

Gebruik **I-MR alleen** als subgroeperen écht niet kan. Als je logische mini-steekproeven kunt nemen — zelfs maar n=2 — is **X̄-R of X̄-S meestal informatiever** dan I-MR.

> **Praktijk:** I-MR past vooral bij batch-, tank- of lotmetingen waar je per natuur maar één meting per moment hebt.

---

## 🟢 Vier voorbeelden uitgewerkt

*[Fictieve voorbeelden — bedoeld als typische situaties in de maakindustrie]*

| # | Situatie | Twee vragen | Kaart |
|---|----------|-------------|-------|
| 1 | Operator weegt elke 2 uur 5 onderdelen op spuitgietlijn | Continue meting, subgroep n=5 (klein) | **X̄-R** |
| 2 | Lasersensor meet elke seconde de dikte (n=30 per minuut) | Continue meting, subgroep n=30 (groter) | **X̄-S** |
| 3 | Voedselbedrijf meet viscositeit van elke batch (1 meting per batch) | Continue meting, geen subgroep mogelijk | **I-MR** |
| 4 | Verpakkingslijn telt lekkende pakken in steekproef van precies 100 | Telling van defecten, **vaste** n | **np** |

---

## 🔴 Drie veelgemaakte fouten — pas op!

| # | Fout | Wat is er aan de hand? |
|---|------|------------------------|
| 1 | **I-MR gebruiken terwijl subgroeperen kan** | Je verliest informatie. Zelfs n=2 geeft meer inzicht in de spreiding dan losse metingen. |
| 2 | **p en np door elkaar halen** | p = percentage (bij wisselende n), np = aantal (bij vaste n). Kies op basis van je steekproef. |
| 3 | **c en u door elkaar halen** | c = bij gelijke eenheid (zelfde plaat, zelfde stuk), u = bij wisselende eenheid (variabele lengte folie, variabele oppervlakte). |

---

## 🟠 Wanneer escaleren?

*Je hoeft niet zelf te kiezen welke kaart er komt — dat is taak van engineering of de kwaliteitsdienst. Maar deze situaties zijn een signaal.*

| Situatie | Wat doe je? | Aan wie? |
|----------|-------------|----------|
| De kaart op jouw lijn lijkt niet te passen bij de meting | Vraag waarom die kaart is gekozen | Teamleider of engineering |
| De steekproefgrootte varieert maar je gebruikt een np-kaart | Meld dit — p-kaart zou passender zijn | Engineering of kwaliteitsdienst |
| Je doet één meting per batch maar je ziet een X̄-R-kaart | Meld — waarschijnlijk hoort I-MR hier | Engineering |
| De kaart heeft geen as-titels of geen subgroep-info | Vraag om duidelijke labeling | Teamleider |

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Continue meting** | Een getal op een schaal (gewicht, diameter, temperatuur, tijd) |
| **Attribuutdata** | Tellingen (aantal defecten, ja/nee, goed/fout) |
| **Subgroep** | Kleine groep metingen kort na elkaar (bijvoorbeeld 5 onderdelen achter elkaar wegen) |
| **Steekproef** | Aantal stuks dat je controleert (bijvoorbeeld 100 pakken per uur) |
| **Range (R)** | Verschil tussen hoogste en laagste meting in een subgroep |
| **Standaarddeviatie (S)** | Nauwkeurigere maat voor spreiding dan de range |
| **Moving range (MR)** | Verschil tussen twee opeenvolgende losse metingen (bij I-MR) |
| **Defectpercentage** | Percentage afgekeurde stuks in de steekproef |
| **Defectdichtheid** | Aantal defecten per eenheid (oppervlak, lengte, tijd) |

---

## 🟢 Onthoud dit

1. **Twee vragen zijn genoeg:** continue of telling? Vaste of wisselende steekproef?
2. **Continue + subgroep klein** → X̄-R
3. **Continue + subgroep groter** → X̄-S
4. **Continue + één meting per moment** → I-MR
5. **Percentage defecten + wisselende n** → p-kaart
6. **Aantal defecten + vaste n** → np-kaart
7. **Defecten per gelijke eenheid** → c-kaart
8. **Defecten per wisselende eenheid** → u-kaart
9. **I-MR is laatste keuze** — pak subgroeperen waar het kan.

---
*Bron: NIST/SEMATECH Engineering Statistics Handbook; ISO 7870-1 en 7870-2; ASQ; Minitab documentation | ko-spc-108 | AIMM Module 2 — SPC Train | v1.0*
