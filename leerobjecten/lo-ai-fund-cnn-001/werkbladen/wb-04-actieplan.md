# Actieplan: waar zou een CNN op mijn lijn passen?
*Kolb fase 4 — Experimenteren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: CNN-architectuur**

---

> **Over dit werkblad**
> Je hebt nu de CNN-architectuur en vier voorbeelden doorlopen. Tijd om het op je eigen lijn te leggen. Zoek één plek waar visuele inspectie, een sorteersysteem of een trillingsmeting plaatsvindt. Of het er al een AI-systeem heeft, maakt niet uit. Beschrijf welk patroon jij nu zelf met oog of oor herkent. Bepaal daarna welke CNN-laag dat patroon waarschijnlijk zou oppikken.
>
> **Tijd:** 11 minuten.
>
> **Waarom dit werkblad?**
> Een module beklijft pas als je het op je eigen werk legt. Dit actieplan is geen toets. Het is de eerste schets van een eigen use-case die je deze week bij de leverancier of bij IT toetst.

---

## 1. De plek op mijn lijn

**Mijn machine of werkstation:** _______________________________________________

**Soort meting of inspectie:**

○ Camera-inspectie (oppervlakte, kras, kleur, vorm)
○ Sorteersysteem met camera boven een lopende band
○ Trillingssensor of akoestische meting
○ Storingsclassificatie op een audiosignaal
○ Ander beeld of tijdreeks: _______________________________________________

**Korte omschrijving van wat er gemeten wordt:**

_______________________________________________

_______________________________________________

---

## 2. Welk patroon herken je nu zelf?

*Welk patroon zie je met je eigen ogen of hoor je met je oren? Beschrijf het zo concreet mogelijk.*

_______________________________________________

_______________________________________________

_______________________________________________

*Zit dit patroon op een specifieke plek (rand, midden, hoek), of overal in de input?*

○ Op een specifieke plek   ○ Overal verspreid   ○ Beide (afhankelijk van situatie)

---

## 3. Welke CNN-laag doet hier het belangrijkste werk?

*Op basis van de architectuur uit fase 1.*

| Laag | Wat zou hij voor jouw patroon doen? | ✓ |
|------|-------------------------------------|:-:|
| **Convolutielaag** — pikt lokale patronen op (kras, frequentie-band) | | ☐ |
| **Pooling** — maakt het robuust voor verschuiving (waar het patroon zit, maakt minder uit) | | ☐ |
| **Fully connected** — combineert alle patronen tot één eindoordeel (defect of oké) | | ☐ |

*Welke laag zou bij jouw use-case het zwaarst werk doen, en waarom?*

_______________________________________________

_______________________________________________

---

## 4. Past CNN — eerlijk gekeken?

| Vraag | Mijn antwoord |
|-------|---------------|
| Heeft mijn data ruimtelijke of volgordelijke structuur? | ○ Ja  ○ Nee  ○ Onbekend |
| Is het patroon lokaal (klein, maar overal mogelijk)? | ○ Ja  ○ Nee  ○ Onbekend |
| Heb ik genoeg gelabelde voorbeelden van "defect" én "oké"? | ○ Ja  ○ Nee  ○ Onbekend |
| Is er nu al een AI-systeem actief op deze plek? | ○ Ja  ○ Nee  ○ Onbekend |

*Mijn oordeel:*  ○ CNN is hier passend   ○ Twijfel — hangt af van data-beschikbaarheid   ○ CNN is hier niet passend

---

## 5. Concrete acties — deze week

| # | Actie | Wanneer | Met wie | ✓ |
|---|-------|---------|---------|---|
| 1 | Mijn use-case in 5 zinnen op papier zetten | | | ☐ |
| 2 | Vraag aan leverancier of IT: gebruikt het systeem een CNN? | | | ☐ |
| 3 | Vraag aan leverancier of IT: wat is de input — beeld of tijdreeks? | | | ☐ |
| 4 | Vraag aan leverancier of IT: welk type defect herkent het, en welk juist niet? | | | ☐ |

---

## 6. Mogelijke obstakels

*Wat zou dit gesprek of dit project kunnen tegenhouden?*

_______________________________________________

_______________________________________________

---

## 7. Een korte video als geheugensteun

> **Bekijk deze week één keer:** zoek op YouTube naar "CNN feature map visualization". Je ziet dan letterlijk wat de convolutielaag oppikt. Dat maakt het abstracte concept tastbaar.

- [ ] Video bekeken — datum: __________

---

## Mijn use-case — vijf zinnen om mee te nemen

1. **Welke plek op mijn lijn:** _______________________________________________

2. **Welk patroon ik zelf herken:** _______________________________________________

3. **Welke CNN-laag doet het zwaarste werk:** _______________________________________________

4. **CNN passend?** _______________________________________________

5. **Eerste vraag aan leverancier of IT:** _______________________________________________

---

## Wat doen we hierna?

In de volgende workshop bespreken we kort per deelnemer wat je terughoorde van de leverancier of IT. De trainer helpt je verbinden wat je hoorde aan de architectuur. Welke laag doet waarschijnlijk het zwaarste werk voor jouw use-case? Neem dit actieplan mee.

**Review-datum:** __________  **Buddy of coach:** __________

---
*Bron: CNN-architectuur — AIMM Curriculum | Module 2: Train | v1.0*
