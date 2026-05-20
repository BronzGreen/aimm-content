# Handout: AI + SPC — Samenspel, Geen Concurrentie
*Shewhart-principe, Nelson-regels en AI-aanvulling op één pagina*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"Shewhart bedacht in 1924 het onderscheid tussen signaal en ruis. Dat onderscheid is in het AI-tijdperk belangrijker dan ooit — juist omdat sensoren miljoenen punten per dag leveren."**

Pak je markeerstift. Markeer wat bij jouw machine al zo is — en wat nog niet. Twee minuten.

---

## Het Shewhart-principe blijft

> **Een sensor die elke seconde meet, verandert niets aan de vraag: "is dit signaal of ruis?"**

Wat Shewhart in 1924 zag, geldt in 2026 nog steeds:
- Ieder proces heeft **normale variatie** (ruis) — daar doe je niks mee
- Een **speciale oorzaak** produceert een **signaal** — daar onderzoek je
- Het verschil herkennen is de kern van procesbeheersing

Klassiek, digitaal of met AI — dit onderscheid blijft het fundament.

---

## De drie lagen — wat verandert, wat blijft

| Laag | Klassiek (vroeger) | Digitaal (nu) | AI-aanvulling (wanneer zinvol) |
|------|--------------------|----------------|--------------------------------|
| **1. Meten** | Handmeting elke 2 uur | Continu via IoT | AI kan gaten vullen, meetfouten herkennen |
| **2. Signaal-detectie** | Operator scant kaart, past Nelson-regels toe | Dashboard met auto-alarm op Nelson | AI vangt complexe patronen die Nelson-regels missen |
| **3. Beslissen** | Operator beslist | Operator beslist | AI geeft aanbeveling; operator beslist |

**De beslis-laag blijft bij de mens.** Dat is geen technische beperking — het is een ontwerpkeuze en verantwoordelijkheid.

---

## Nelson-regels — nog steeds correct

De regels die je kent werken gewoon door:
- Punt buiten de controlegrenzen → onderzoek
- 7 of meer punten aan dezelfde kant → trend
- 6 of meer stijgend/dalend → drift
- Andere patronen volgens ISO 7870-2

**Kracht:** helder, uitlegbaar, werkt op één variabele.

**Zwakte:** kijkt naar één variabele tegelijk. Ziet geen combinatie-patronen.

---

## Wat AI **wel** toevoegt

| Situatie | Wat AI doet | Wat Nelson niet ziet |
|----------|------------|----------------------|
| Meerdere variabelen samen | Herkent *combinatie* die afwijkt terwijl elke variabele op zich nog binnen de grenzen is | Mono-variabel blikveld |
| Veel historische data | Leert typische batch-patronen en geeft vroege waarschuwing | Alleen het nu vs de grenzen |
| Complexe patronen | Detecteert langzaam kantelende verhoudingen | Te subtiel voor statistische regels |
| Onzekere metingen | Schat ontbrekende data, markeert verdachte waarden | Gaat uit van correcte meting |

---

## Wat AI **niet** toevoegt

Eerlijk verhaal. Sla AI over als:

- **Meetsysteem onbetrouwbaar** — garbage in = garbage out
- **Weinig historische data** — model kan niks leren
- **Probleem is simpel** — Nelson-regels zien het prima
- **Geen uitleg mogelijk** — klant/auditor snapt de AI-beslissing niet
- **Proces is stabiel en capabel** — er is niks te verbeteren

**Niet iedere lijn heeft AI nodig.**

---

## Fictieve referentiecasus — chemische reactor

> *Dit voorbeeld is fictief — als ijkpunt voor schaal en aanpak.*

**De casus.** Chemische reactor meet continu druk, temperatuur en debiet. Elke variabele heeft controlekaart + Nelson-regels.

- **Klassiek / digitaal:** auto-alarm als één variabele buiten de grenzen komt.
- **AI-toevoeging:** model herkent dat *combinatie* 'temperatuur iets hoog + debiet iets laag + druk normaal' vaak vooraf gaat aan een off-spec batch — 40 minuten eerder dan de Nelson-regel zou triggeren.
- **Beslissing:** operator ziet vroege waarschuwing, controleert visueel, beslist.
- **Nelson-regels blijven actief** als tweede net.

Dit is het samenspel: **vroege signalen van AI + harde grenzen van Nelson + beslissing door mens.**

---

## Jouw rol verschuift — niet weg

**Van:** kaart tekenen, punten plotten, regels herkennen.

**Naar:** procesgedrag begrijpen, signalen duiden, beslissen.

Wat blijft **altijd** jouw verantwoordelijkheid:

1. **Meting betrouwbaar houden** — kalibratie, onderhoud
2. **Reactieplan kennen en uitvoeren** — wat doe je bij alarm
3. **Rationele subgroepering begrijpen** — welke ploeg, batch, grondstof
4. **Uitleg geven** — aan collega, klant, auditor

Een AI-model kan signaleren. Het beslist niet of het proces vandaag veilig door mag.

---

## Wanneer welke laag? — Snelle checklist

| Vraag | Actie |
|-------|-------|
| Is je meting betrouwbaar? | Zo nee: eerst meetsysteem fixen, pas dan AI overwegen |
| Volstaan Nelson-regels? | Zo ja: niet ingewikkelder maken |
| Speelt combinatie van variabelen? | Dan is AI-aanvulling kandidaat |
| Heb je veel historische data? | Nodig om een model te trainen |
| Kan iemand de AI-uitkomst uitleggen? | Zo nee: niet inzetten (audit, klant, proces-eigenaar) |
| Blijft de operator beslisser? | Zo nee: ontwerp aanpassen |

---

## Onthoud dit

1. **Shewhart blijft** — signaal vs ruis is het fundament
2. **Nelson-regels blijven correct** — helder en uitlegbaar
3. **AI is aanvulling, geen vervanging** — combinatie-patronen, vroege waarschuwing
4. **Beslissen blijft bij de mens** — ontwerpkeuze, niet toevallig
5. **Meten moet eerst kloppen** — garbage in = garbage out
6. **Niet elke lijn heeft AI nodig** — eerlijk antwoord mag "nee" zijn

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Shewhart-principe** | Onderscheid tussen normale variatie (ruis) en een echt signaal (speciale oorzaak) |
| **Nelson-regels** | Statistische patronen op een controlekaart die op een speciale oorzaak wijzen |
| **SPC** | Statistical Process Control — procesbeheersing met controlekaarten |
| **IoT-sensor** | Internet-connected meter — stuurt data continu naar een dashboard |
| **MES / SCADA** | Productie-software die data van machines verzamelt en toont |
| **Multivariaat** | Meerdere variabelen tegelijk bekijken in plaats van één |
| **Off-spec** | Buiten de specificatie — product voldoet niet aan de eis |
| **Uitlegbare AI** | AI waarvan een mens kan begrijpen waarom het model een bepaalde uitkomst geeft |

---

> **Volgende stap.** In blok 2 vul je het synthese-werkblad (wb-01) in voor jouw eigen machine. Houd deze handout open als referentie.

---
*Bron: ko-spc-601 (Digitale SPC en sensordata); Technometrics-review 2024 over Industry 4.0 SPC; ISO 7870-2; Shewhart (1924) | AIMM Module 3 — SPC Op Maat | v1.0*
