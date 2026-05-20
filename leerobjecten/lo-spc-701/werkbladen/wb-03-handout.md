# Handout: De Drie Kaders van SPC-Implementatie
*SPC — Shewhart (1931) · Nelson (1984) · Deming (1986)*

**Module 3 — SPC Op Maat | Naslag bij blok 1 (theoretiseren) — markeren tijdens trainersuitleg**

---

> **De centrale zin (uit je hoofd waard)**
> **"SPC werkt alleen als alle drie kaders tegelijk staan — statistisch, operationeel én organisatorisch. Eén overslaan en het valt binnen half jaar om."**

Pak je markeerstift. Markeer per kader het element dat op jouw lijn nu het zwakste is. Twee minuten.

---

## De drie kaders in één blik

```
 ┌─────────────────┐   ┌─────────────────┐   ┌──────────────────────┐
 │ 🔵 STATISTISCH   │   │ 🟠 OPERATIONEEL │   │ 🟣 ORGANISATORISCH   │
 │ (begrippen)     │ + │ (dagelijks werk)│ + │ (borging & cultuur)  │
 │ Shewhart·Nelson │   │ Wie·wanneer·hoe │   │ Training·MSA·steun   │
 └─────────────────┘   └─────────────────┘   └──────────────────────┘
        ↓                      ↓                       ↓
    zonder dit            zonder dit             zonder dit
    = pseudo-SPC          = mooie theorie        = doodbloeden na half jaar
```

Alle drie tegelijk of geen van drie. Geen tussenoplossing.

---

## 🔵 Kader 1 — Statistisch

*Begrippen die NIET vereenvoudigd mogen worden tot "binnen of buiten tolerantie".*

| Begrip | Waarom kritisch | Bron |
|--------|-----------------|------|
| **Common vs special cause** | Onderscheid bepaalt of je ingrijpt. Ingrijpen op common cause → "tampering" (Deming) → meer variatie. | Shewhart (1931) |
| **Control limits vs spec limits** | Specgrenzen van klant, controlegrenzen uit proces. Verwarren = einde SPC. | Shewhart (1931) |
| **Chart-keuze** | I-MR, X-bar/R, X-bar/S, p-, np-, c-, u-kaart. Verkeerde kaart = verkeerde signalen. | AIAG SPC |
| **Nelson-signalen 1-8** | Patroonherkenning, niet alleen punt buiten 3σ. Regel 2 (9 punten één kant) mist je anders. | Nelson (1984) |
| **Cp / Cpk / Pp / Ppk** | Cp = potentieel. Cpk = werkelijke prestatie. Pp/Ppk = langetermijn. | AIAG SPC |

**Branche-context Cpk.** MKB-maakindustrie beweegt bij gezonde SPC richting Cpk 1,33–1,50. Automotive-klanten eisen vaak ≥ 1,33 op kritische kenmerken; farma/medisch hoger. Check altijd je eigen klantspecificatie — dit zijn richtwaarden, geen universele normen.

---

## 🟠 Kader 2 — Operationeel

*De vertaling naar dagelijks werk. Zonder dit hangt de kaart, maar werkt SPC niet.*

| Element | Kernvraag |
|---------|-----------|
| **Sampling** | Wie meet, wanneer, hoe vaak? Staat het in standaardwerk? |
| **Subgroepering** | Rationele subgroepen (Shewhart): één operator, één batch, één uur. Geen gemixte bronnen. |
| **Reactieplannen** | Bij Nelson-1: containment + oorzaakcheck. Bij Nelson-2: trend-check. Op papier. |
| **Containment** | Verdachte output veiligstellen — fysiek afschermen, niet alleen "even apart". |
| **Shift-overdracht** | Signalen van ploeg 1 komen aan bij ploeg 2. Ploegboek-template. |
| **Escalatie** | Wanneer naar teamleider, wanneer naar kwaliteit, wanneer naar engineering? |

> **Typisch symptoom van zwak operationeel kader.** Signalen verdwijnen in de nachtploeg. De kaart klopt, de meting klopt, maar het signaal bereikt de juiste persoon niet — omdat het reactieplan of de shift-overdracht niet is geregeld.

---

## 🟣 Kader 3 — Organisatorisch

*De borging en cultuur. Deming (1986): "It is management's job to work on the system."*

| Voorwaarde | Wat betekent dat concreet? |
|-------------|------------------------------|
| **Training** | Iedereen die meet of beslist begrijpt SPC-basis. Onderhoud, geen eenmalige kick-off. |
| **Meetsysteembeheersing (MSA)** | Gage R&R periodiek. Anders meet je variatie van de meter, niet van het proces. |
| **Control plans** | Per kritisch kenmerk vastgelegd. Niet één plan voor hele lijn. |
| **Managementsteun** | Tijd, middelen, prioriteit. Zonder managementverantwoordelijkheid geen SPC-werking (Deming). |
| **Signaalcultuur** | Signalen worden onderzocht, niet weggepoetst. No-blame-principe expliciet. |

> **Typisch symptoom van zwak organisatorisch kader.** SPC werkt initieel. Na 3 maanden: minder aandacht. Na 6 maanden: kaarten hangen leeg, training-onderhoud is niet gedaan, operator zegt "dat doen we niet meer zo". Dit is bijna altijd een organisatorisch probleem, geen statistisch.

---

## De onlosmakelijkheid

| Wat je overslaat | Wat je krijgt | Voorbeeld |
|-------------------|----------------|-----------|
| Geen statistisch | Pseudo-SPC: routine zonder onderscheidingsvermogen | Operator reageert op elk punt dat "raar lijkt", ook common cause → tampering |
| Geen operationeel | Mooie theorie, geen werking | Kaart hangt, signaal in nachtploeg wordt niet opgepakt |
| Geen organisatorisch | Werkt half jaar, valt dan in | Eerste uitrol met energie, geen onderhoud, na 6 mnd leegloop |

**De drie kaders zijn onlosmakelijk.**

---

## Fictieve illustratie — kunststofverwerker

> *Fictieve illustratie met plausibele getallen voor een MKB-kunststofbedrijf; geen specifieke casus. Bedoeld als ijkpunt voor schaal en tempo, niet als sjabloon.*
>
> 12 spuitgietlijnen. SPC-uitrol per kader:
>
> - **🔵 Statistisch** — 4 dagdelen training operators (basis + Nelson 1+2); 8 dagdelen teamleiders (volledige Nelson + Cpk + DMAIC-basis).
> - **🟠 Operationeel** — control plan per machine; reactieplan per signaaltype; monsterstrategie per productlijn; signaalregel in ploegoverdracht-template.
> - **🟣 Organisatorisch** — kwartaalse Gage-R&R; maandelijkse kwaliteitsbespreking met operators; signalen expliciet op ploegoverdracht-agenda; "no-blame"-afspraak bij signaalmelding.
>
> **Plausibel resultaat na 6 maanden:** ~23% afkeurreductie; gemiddelde Cpk van circa 1,15 naar 1,42; hoog operatorvertrouwen (intern gemeten). Beweging 1,15 → 1,42 is voor MKB-spuitgieten realistisch binnen half jaar — mits alle drie kaders tegelijk.
>
> **Cruciaal.** Deze cijfers zouden het gevolg zijn van alle drie de kaders tegelijk, niet van één. Eén overslaan breekt het patroon.

---

## Hoe herken je welk kader het zwakste is?

| Signaal op je lijn | Vermoedelijk zwakste kader |
|---------------------|------------------------------|
| "We grijpen vaak in zonder dat het echt helpt" | 🔵 Statistisch (common vs special cause onhelder) |
| "Signaal in de nachtploeg zien we niet meer terug" | 🟠 Operationeel (shift-overdracht, reactieplan) |
| "SPC wordt bij drukte als eerste losgelaten" | 🟣 Organisatorisch (managementsteun, signaalcultuur) |
| "Iedereen weet dat de meter niet klopt, maar MSA is er niet" | 🟣 Organisatorisch (MSA-onderhoud) |
| "We hebben kaarten, maar niemand zegt wat bij een Nelson-2" | 🟠 Operationeel (reactieplan ontbreekt) |
| "Cpk-getallen staan in het rapport maar niemand interpreteert ze" | 🔵 Statistisch + 🟣 Organisatorisch (training + cultuur) |

---

## Onthoud dit

1. **Statistisch zonder operationeel** = mooie theorie, geen praktijk
2. **Operationeel zonder statistisch** = pseudo-SPC, schijnzekerheid
3. **Beide zonder organisatorisch** = werkt initieel, valt na half jaar in
4. **Alle drie tegelijk** = duurzame werking, blijvende winst
5. **Zwakste kader eerst versterken** — niet het kader dat je al beheerst
6. **Signalen zijn geen statistiek, maar cultuur** — no-blame of weggepoetst

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **SPC** | Statistical Process Control — Shewhart (1931) |
| **Common cause** | Normale variatie in een stabiel proces — niet ingrijpen |
| **Special cause** | Afwijkende oorzaak — wél ingrijpen, oorzaak wegnemen |
| **Tampering** | Ingrijpen op common cause → meer variatie (Deming) |
| **Nelson-regels** | 8 signaalregels voor patroonherkenning op controlekaart (Nelson, 1984) |
| **Cp / Cpk** | Procesbekwaamheid: potentieel (Cp) vs werkelijke prestatie (Cpk) |
| **Pp / Ppk** | Langetermijn-procesbekwaamheid (inclusief drift) |
| **Gage R&R / MSA** | Meetsysteem-analyse (Repeatability & Reproducibility) |
| **Rationele subgroepen** | Samenhangende meetgroepen (één operator, één batch, één uur) |
| **Containment** | Verdachte output fysiek afschermen bij signaal |
| **No-blame** | Principe: signaal melden ≠ operator fout. Cultuur, geen regel. |

---

> **Volgende stap.** In blok 2 vul je wb-01 in: per kader drie afspraken + zwakste-kader-diagnose + maandag-actie. Hou deze handout open als referentie.

---
*Bronnen: Shewhart (1931) "Economic Control of Quality of Manufactured Product"; Nelson (1984) "The Shewhart Control Chart — Tests for Special Causes"; Deming (1986) "Out of the Crisis"; AIAG SPC Reference Manual; ISO 7870-1; Ford PPAP; Wheeler implementatie-essays | AIMM ko-spc-701 | Module 3 — SPC Op Maat | v1.0*
