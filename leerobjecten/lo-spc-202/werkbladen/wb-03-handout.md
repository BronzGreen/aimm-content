# Handout: Gevoeligheid vs vals alarm
*Signaalregels op regelkaarten — wat ze opleveren en wat ze kosten*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Elke extra signaalregel maakt je regelkaart gevoeliger — maar ook vaker vals.**
> **Te veel regels = alarm-fatigue. Operators gaan signalen negeren."**

---

## Wat is ARL?

**ARL** = **A**verage **R**un **L**ength = gemiddeld aantal metingen tot er een alarm afgaat, terwijl het proces in werkelijkheid **stabiel** is. Dus: hoe vaak je een vals alarm krijgt.

> Rekensom: **vals alarm per dag = metingen per dag / ARL**

| ARL | Betekenis |
|-----|-----------|
| Hoog (bijv. 371) | Weinig vals alarm — rustig |
| Laag (bijv. 50) | Veel vals alarm — alarm-fatigue-risico |

---

## 🔵 De drie regelsets — vergelijkingstabel

| Regelset | Wat let de kaart op? | ARL | Vals alarm bij 96 metingen/dag |
|----------|----------------------|-----|-------------------------------|
| **Kale Shewhart** | Alleen 1 punt buiten ±3σ | **~371** | ~1 per 4 dagen |
| **+ WECO (4 regels)** | Ook trends en zones | **~91,75** | ~1 per dag |
| **+ Volledige Nelson (8 regels)** | Diagnostische volledig | **aanzienlijk vaker** (~40–60) | meerdere per dag |

> **Bronverantwoording:** Het getal **ARL ≈ 91,75** voor WECO komt uit **Champ & Woodall (1987, Technometrics)** — niet uit NIST zoals vaak foutief wordt doorgegeven. Let op bij citeren.

---

## 🟣 Wat zeggen die regels eigenlijk?

### Kale Shewhart (regel 1)
Eén punt buiten de ±3σ-band = alarm. Robuust, niet gevoelig voor kleine trends.

### WECO-uitbreiding (regels 2–5 kort samengevat)
Let op **patronen**: 2 van 3 punten buiten ±2σ, 4 van 5 buiten ±1σ, 8 opeenvolgende punten aan één kant van de middellijn. Pakt **trends en verschuivingen** op die kale Shewhart mist.

### Volledige Nelson (regels 6–8)
Extra diagnostische regels: oscillerende patronen, waarden te dicht bij de middellijn, enz. Gevoelig voor heel specifieke procesdiagnoses — maar geeft ook veel vals alarm.

---

## 🟢 Waarom "meer is beter" een val is

Drie redenen waarom meer regels averechts werken:

| # | Effect | Wat is er aan de hand? |
|---|--------|------------------------|
| 1 | **Alarm-fatigue** | Operators krijgen zo vaak vals alarm dat ze alle alarmen minder serieus nemen — inclusief de échte. |
| 2 | **Verloren productietijd** | Elk alarm = lijn stil of operator erheen. Vals alarm kost écht geld, niet "een beetje ruis". |
| 3 | **Verloren vertrouwen in de kaart** | Als operators het systeem niet meer geloven, werkt de kaart niet meer — dan is hij kwijt. |

> **Minitab-stelregel:** Liever drie regels die je begrijpt dan acht die je negeert.

---

## 🔴 De gefaseerde AIMM-aanpak

We leren signaalregels gefaseerd op — niet alles tegelijk:

| Module | Welke regels? | Leerdoel |
|--------|--------------|----------|
| **Module 1 — Gebruik** | Regel 1 + 2 | Basisstabiliteit. Je leert de kaart lezen en het eerste echt signaal herkennen. |
| **Module 2 — Train** *(deze sessie)* | Regels 3–6 | Trend- en mixsignalen. Je leert wat ze toevoegen én wat ze kosten (vals alarm). |
| **Module 3 — Op Maat** | Regels 7–8 | Diagnostische verdieping. Alleen bij goed begrip van subgroepering. |

Die volgorde is geen toeval: het voorkomt dat je te snel te veel tegelijk aan zet en dat de kaart onbetrouwbaar wordt.

---

## 🟠 Operator-implicatie

*Wat betekent dit concreet voor jouw werkdag?*

| Situatie | Wat doe je? |
|----------|-------------|
| Je krijgt meerdere alarmen per dag op dezelfde lijn | Vraag teamleider welke regelset actief is — misschien staan er te veel aan |
| Engineering stelt voor "meer regels aan te zetten" | Vraag om de afweging gevoeligheid vs vals alarm — de gefaseerde aanpak is een goed gesprek |
| Collega's negeren alarmen | Alarm-fatigue — meld het, want dit is een reëel productierisico, geen mentaliteitsprobleem |
| Je weet niet welke regelset actief is | Vraag het na — als niemand het weet, is dat ook informatie |

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Shewhart-regel** | De basisregel: 1 punt buiten ±3σ = alarm. Genoemd naar Walter Shewhart (grondlegger SPC). |
| **WECO** | Western Electric Company Rules (1956) — vier aanvullende signaalregels. |
| **Nelson-regels** | Lloyd Nelson (1984) — acht signaalregels. Strenger dan WECO. |
| **ARL** | Average Run Length — gemiddeld aantal metingen tot (vals) alarm bij een stabiel proces. |
| **Vals alarm** | Alarm terwijl het proces in werkelijkheid stabiel is. Niet "gratis ruis" — kost echte productietijd. |
| **Alarm-fatigue** | Het effect dat operators alarmen gaan negeren omdat er te veel valse tussen zitten. |
| **Signaalregel** | Een regel die bepaalt wanneer een regelkaart alarm geeft. |

---

## 🟢 Onthoud dit

1. **ARL = hoe vaak vals alarm** — hoger = beter.
2. **Kale Shewhart: ARL ≈ 371** — rustig, ±1 per 4 dagen op een dagelijkse lijn.
3. **+ WECO: ARL ≈ 91,75** — voelbaar, ongeveer 1 per dag.
4. **+ Volledige Nelson: aanzienlijk vaker** — alarm-fatigue-risico.
5. **Vals alarm = verloren productietijd** — niet gratis ruis.
6. **Te veel regels werkt averechts** — operators negeren dan ook echte signalen.
7. **Gefaseerd opbouwen** — Module 1 regels 1+2, Module 2 regels 3–6, Module 3 pas regels 7+8.

---
*Bron: NIST/SEMATECH Engineering Statistics Handbook; Champ & Woodall (1987) Technometrics; Minitab documentation; Western Electric Company (1956); Nelson (1984) | ko-spc-202 | AIMM Module 2 — SPC Train | v1.0*
