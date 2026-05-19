# Handout: Rationele subgroepering
*Wat zit er in één subgroep — en waarom is dat cruciaal?*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Een goede kaart begint vóór het plotten — bij de vraag wát je samenvoegt."**

Een regelkaart die nooit alarmeert, is vaak geen mooie kaart — maar een kaart met verkeerd samengestelde subgroepen. Als de subgroep meerdere bedrijfstoestanden mengt (caviteiten, ploegen, setups), worden control limits kunstmatig breed en verdwijnen echte verstoringen in de "ruis".

---

## Wat is een rationele subgroep?

Een subgroep is een **kleine set eenheden**:

- Onder vrijwel **dezelfde omstandigheden** gemaakt
- **Dicht in de tijd** verzameld
- Bij voorkeur uit dezelfde caviteit, lijn, machine of ploeg

**Snapshot-principe:** zie een subgroep als een momentopname van het proces in één toestand.

---

## 🔵 Twee soorten variatie — en waar ze horen

*Dit is de kern van waarom rationele subgroepering werkt.*

| Variatiebron | Waar moet die zichtbaar worden? |
|--------------|----------------------------------|
| Kortetermijn-variatie (gewone ruis) | **Binnen** de subgroep |
| Shifts, drift, verstoringen | **Tussen** subgroepen |

Als je dat omdraait, krijg je het tegenovergestelde effect:

- Subgroep over meerdere shifts → control limits worden kunstmatig **breed**
- Subgroep over meerdere caviteiten → caviteit-verschillen verdwijnen in "ruis"
- Subgroep over setup-condities → setup-effecten worden onzichtbaar

**Resultaat:** de kaart geeft geen alarmen meer, ook niet bij echte verstoringen.

---

## 🟣 De vier veelgemaakte fouten

*Dit zijn de valkuilen — herken ze op je eigen lijn.*

| # | Fout | Wat is er aan de hand? | Hoe herken je het? |
|---|------|------------------------|--------------------|
| 1 | **Subgroep over shifts** | Operator-effecten + procesvariatie worden vermengd | Subgroep loopt over ploegwissel heen |
| 2 | **Subgroep over caviteiten** | Caviteit-specifieke problemen verdwijnen | Eén subgroep bevat stuks uit meerdere caviteiten |
| 3 | **Te kleine n (<3)** | Variatieschatting wordt instabiel, kaart reageert grillig | Subgroepen van 1 of 2 stuks |
| 4 | **Mengen van setup-condities** | Verschil vóór en ná setup-wissel wordt "ruis" | Subgroep loopt over setup-wissel of materiaalbatch-wissel heen |

---

## 🟢 Branche-normen voor subgroep-grootte

*De getallen hieronder zijn **branche-normen** — afspraken uit de industrie, geen wiskundige wetten. Ze geven je een werkbaar startpunt.*

| Bron | Aanbeveling | Wanneer relevant? |
|------|-------------|-------------------|
| **NIST / Minitab** *(branche-norm)* | Initiële studie: **4-5 stuks per uur**, ongeveer **100 metingen** of **25 subgroepen** | Algemene capabilitystudies |
| **Ford PPAP** *(branche-norm Ford PPAP)* | Capabilitydemonstratie: **minimaal 25 subgroepen** van **minimaal 5** stuks | Automotive-leveringen, Production Part Approval Process |
| **Snapshot-principe** | Subgroep = momentopname van proces in één toestand | Altijd |

> **Let op:** de Ford PPAP-eis is specifiek voor automotive (MBO-4-laag). Jij hoeft de studie niet zelf uit te voeren, maar je moet wel begrijpen waarom die 25 × 5 subgroepen níét over ploegen of caviteiten heen mogen lopen — anders is de uitkomst misleidend.

---

## 🟠 Wat betekent dit op jouw lijn?

*Drie concrete situaties waarin je iets kunt doen.*

### Situatie A — Meerdere caviteiten op één kaart
**Probleem:** de kaart middelt caviteit-verschillen uit.  
**Oplossing:** aparte kaarten per caviteit, **óf** subgroepen uit één caviteit per keer (op rotatie: uur 1 caviteit 1, uur 2 caviteit 2, enzovoort).

### Situatie B — Subgroep loopt over ploegwissel
**Probleem:** operator-verschillen worden vermengd met procesvariatie.  
**Oplossing:** plan subgroepen zó dat ze binnen één ploeg blijven. Rond de ploegwissel: liever geen subgroep, of een aparte markering.

### Situatie C — Subgroep loopt over setup-wissel of batch-wissel
**Probleem:** setup-effect wordt "ruis".  
**Oplossing:** na elke setup-wissel een nieuwe meetreeks starten. Markeer de wissel op de kaart.

---

## 🔴 Wanneer escaleren?

*Je hoeft niet alles zelf op te lossen. Dit zijn de momenten om het bij teamleider of kwaliteitsdienst te leggen.*

| Situatie | Wat doe je? | Aan wie? |
|----------|-------------|----------|
| Kaart geeft nooit alarm maar op de lijn zie je wél problemen | Controleer hoe subgroepen worden samengesteld | Teamleider / kwaliteitsdienst |
| Lijn heeft meerdere caviteiten en één gezamenlijke kaart | Vraag of aparte kaarten per caviteit mogelijk zijn | Teamleider |
| Ford PPAP-capabilitystudie loopt en subgroepen lopen over ploegen of setups | **Direct melden** | Teamleider / kwaliteitsdienst |
| n in de subgroep is 2 of lager | Vraag of er ruimte is voor minimaal 3-5 stuks | Teamleider |
| Verdenking dat materiaal-batch-wissels binnen één subgroep vallen | Bespreken met kwaliteitsdienst | Kwaliteitsdienst |

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Subgroep** | Kleine set eenheden samen gemeten; basis van een X̄-R- of X̄-S-kaart |
| **Rationele subgroep** | Subgroep onder één bedrijfstoestand, dicht in de tijd |
| **Caviteit** | Één "holte" in een spuitgietmatrijs — bij 4 caviteiten komen er per shot 4 stuks uit |
| **Shift / ploeg** | Werkperiode met één operatorteam (dag/avond/nacht) |
| **Setup-wissel** | Overstap van één product of instelling naar een andere |
| **Control limits** | Boven- en ondergrens van de regelkaart — gebaseerd op binnen-subgroep-variatie |
| **PPAP** | Production Part Approval Process — Ford-norm voor automotive |
| **Gage R&R / MSA** | Meetsysteem-analyse — test of de meter zelf nauwkeurig genoeg is |

---

## 🟢 Onthoud dit

1. **Dezelfde omstandigheden, dicht in de tijd** — dat is een rationele subgroep.
2. **Binnen subgroep** = kortetermijn-ruis; **tussen subgroepen** = shifts en drift.
3. **Vier valkuilen:** shifts mengen, caviteiten mengen, n<3, setup mengen.
4. **Een kaart die nooit alarmeert** is meestal geen mooie kaart maar een slecht gesubgroepeerde kaart.
5. **Branche-normen** (NIST/Minitab, Ford PPAP) geven startpunten voor aantal en grootte — geen wetten.
6. **Snapshot-principe:** subgroep = momentopname, geen samenvatting van een uur.
7. **Eerst rationele subgroepering** — dan pas capability-getallen uit die data geloven.

---
*Bron: NIST/SEMATECH Engineering Statistics Handbook; Minitab documentation; Ford PPAP 4th ed. (branche-norm Ford PPAP); AIAG SPC Reference Manual | ko-spc-109 | AIMM Module 2 — SPC Train | v1.0*
