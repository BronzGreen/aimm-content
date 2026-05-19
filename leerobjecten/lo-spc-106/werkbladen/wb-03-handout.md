# Handout: Signaal of ruis — en de eerste blik van de teamleider
*Operator-regel en teamleider-regel bij de SPC-regelkaart*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Reageer op signalen, niet op ruis. Niets doen bij ruis is geen luiheid — het is vakmanschap."**

Een regelkaart laat zien wat er op jouw lijn gebeurt. Maar niet elke schommeling is een teken om iets te doen. Sterker nog: bij de meeste schommelingen is **niets doen** het juiste antwoord.

---

## 🔵 De operator-regel (voor jou, elke shift)

*Dit is jouw werkpaard. Lees je kaart. Weet wanneer je reageert en wanneer niet.*

| Situatie | Wat is het? | Wat doe je? |
|----------|-------------|-------------|
| Een punt **buiten** een controlegrens | **Signaal** | **Stop → onderzoek → documenteer.** |
| **7 of meer punten op rij** aan dezelfde kant van het midden | **Signaal** (run) | **Stop → onderzoek → documenteer.** |
| **6 of meer stijgende of dalende punten op rij** (trend) | **Signaal** | **Stop → onderzoek → documenteer.** |
| Losse schommeling, alles binnen de grenzen, geen patroon | **Ruis** | **Niets doen.** Blijven monitoren. |
| Twee punten dicht bij de grens, maar geen patroon | **Ruis** (tenzij dit vaker gebeurt) | **Blijven monitoren**, niet bijstellen. |

> **Kernregel:** bij een signaal is er een oorzaak die **niet bij de normale variatie hoort**. Die zoek je op. Bij ruis ga je niet aan de knoppen draaien — je maakt de variatie dan alleen groter.

---

## 🟣 Waarom ingrijpen bij ruis fout is: tampering

*Stel: je ziet een meting iets boven het midden. Je stelt de machine ietsje naar beneden bij. De volgende schommeling komt en die gaat nu óók iets naar beneden — maar jouw bijstelling zit er boven op. Resultaat: de spreiding wordt groter, niet kleiner.*

**Dit heet tampering.** Het is één van de vaakst gemaakte fouten op de vloer — niet uit onkunde, maar uit de verleiding om "iets te doen". Zie ook ko-spc-105.

---

## 🟠 De teamleider-regel (voorproefje — Module 3 werkt dit uit)

*De operator ziet zijn/haar eigen kaart. De teamleider ziet patronen boven het individuele niveau uit. Dat vraagt om data uitsplitsen — stratified analysis.*

| Patroontype | Wat zie je? |
|-------------|-------------|
| Verschil tussen **shifts** | Ploeg A en C produceren stabiel, B niet |
| Verschil tussen **caviteiten** | Caviteit 4 systematisch hoger dan 1-3 |
| Verschil tussen **matrijzen** | Matrijs M2 geeft consistent meer variatie |
| Verschil tussen **gereedschappen** | Specifieke tool faalt na X stuks |
| Verschil tussen **recepturen** | Variant Z heeft hogere afkeur |

> Voor vandaag: je hoeft dit niet zelf uit te voeren. Het gaat om **bewustwording**: je eigen regelkaart vertelt niet het hele verhaal.

---

## 🟢 Karim & Sophie — het voorbeeld uit het kennisobject

*Fictief, illustratief voorbeeld uit ko-spc-106.*

**Karim** is operator op shift A. Hij kijkt maandag naar zijn regelkaart: alle punten netjes binnen de grenzen, geen opvallend patroon. Karim volgt de operator-regel correct en produceert door — **terecht**.

**Sophie** is teamleider. Aan het eind van de week zet ze de data van alle drie de shifts naast elkaar en ontdekt dat shift A **systematisch 0,3 mm hoger** meet dan shift C. Geen enkele losse meting uit shift A is out-of-control. Maar het **verschil tussen** shifts is een patroon dat alleen zichtbaar wordt als je de data uitsplitst.

Sophie escaleert naar engineering voor een calibratie-check — misschien meet shift A met een andere meter of een andere methode.

**Wat leert dit ons?**
- Karim deed het goed: op zijn kaart geen signaal → niet reageren.
- Sophie ziet iets wat Karim op zijn kaart **niet kan zien**. Dat is geen tekortkoming van Karim; dat is de logica van uitsplitsen.
- De twee regels vullen elkaar aan: de **operator-regel** zegt *wat doe ik met deze losse kaart?* De **teamleider-regel** zegt *welk patroon zie ik over alle kaarten heen?*

---

## 🔴 Waar SPC verschuift van techniek naar denken

- De **operator-regel** maakt SPC een **uitvoeringsdiscipline**: lezen wat er staat, reageren op signalen, niet reageren op ruis.
- De **teamleider-regel** maakt SPC een **analytische discipline**: data uitsplitsen, patronen ontdekken, oorzaken traceren naar factoren die boven één shift of één machine uitstijgen.

Module 1 ging over de operator-regel. **Module 2** (deze sessie) scherpt het signaal/ruis-onderscheid aan en introduceert de teamleider-regel. **Module 3** (Op Maat) gaat vol op stratified analysis: je leert zelf patronen ontwerpen voor je eigen fabriek.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Regelkaart** | Grafiek van meetwaarden in de tijd, met controlegrenzen |
| **Controlegrens** | Statistische grens die aangeeft wat normale variatie is (meestal ±3σ) |
| **Signaal** | Patroon dat statistisch onwaarschijnlijk is bij normale variatie — reageren |
| **Ruis** | Normale schommeling binnen de bandbreedte — niet reageren |
| **Tampering** | Bijstellen op ruis; maakt variatie groter (ko-spc-105) |
| **Stratified analysis** | Data uitsplitsen naar factoren (shift, caviteit, matrijs, gereedschap, receptuur) |
| **Stabiel proces** | Proces zonder special cause variatie (ko-spc-104) |

---

## 🟢 Onthoud dit

1. **Reageer op signalen, niet op ruis.** Dat is de operator-regel.
2. Een **signaal** = een patroon dat statistisch onwaarschijnlijk is → stop, onderzoek, documenteer.
3. **Ruis** = normale schommeling → niets doen. Aan de knop draaien maakt het erger.
4. Je **eigen kaart** vertelt wat er op jouw lijn gebeurt — maar niet het hele verhaal.
5. Je **teamleider** ziet patronen tussen shifts, caviteiten, matrijzen die jij op individueel niveau niet ziet.
6. In Module 3 ga je zelf leren hoe stratified analysis werkt. Voor nu: **wees bewust dat die laag bestaat**.
7. **Kernvaardigheid vandaag:** durven 'niets doen' bij ruis. Dat is geen luiheid — het is vakmanschap.

---
*Bron: ko-spc-106 (AIAG SPC Reference Manual; ASQ); zie ook ko-spc-104 (stabiel proces), ko-spc-105 (tampering), ko-spc-102 (gerelateerd). | AIMM Module 2 — SPC Train | v1.0*
