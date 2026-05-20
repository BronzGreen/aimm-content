# Cry-Wolf-Casus: 30 sensoren, week 3
*Alarm fatigue — analyse vóór de theorie*

**Naam:** ____________________  **Datum:** __________  
**Module 3 — SPC Op Maat | Workshop: AI + alarmrationalisatie ontwerpen**

---

> **Over dit werkblad**  
> Je krijgt één korte casus uit een productieomgeving. Lees rustig, analyseer vóór we de theorie behandelen. Je mag op je gevoel afgaan — twee vragen te beantwoorden, geen 'goed' antwoord. Je eigen analyse is leerstof. Bij twijfel zet je een vraagteken — dat bespreken we straks samen.

---

## 🔵 De casus

> **Lijn 7 — eindmontage automotive-onderdelen**
>
> Voorjaar 2026. De plant manager keurt een investering goed: **30 nieuwe sensoren** op lijn 7 — temperatuur, trilling, druk, vochtigheid, akoestiek. Levertijd 6 weken, eerste alarmen actief vanaf **week 1**. Elke sensor heeft standaard ±3σ-grenzen, samples elke minuut, 8-uur shift.
>
> **Week 1 (maandag-vrijdag).** De drie operators van lijn 7 krijgen een korte instructie van de leverancier. Het dashboard toont gemiddeld **38 alarmen per shift**. De eerste week worden alle alarmen door de operator opgepakt: meting verifiëren, log invullen, doorgaan. De meeste blijken niets aan de hand — sensor-ruis, kortstondige drift, een vrachtwagen die buiten een trilling veroorzaakt.
>
> **Week 2 (dinsdag).** Daan, één van de operators, zegt in de koffiepauze: *"Het is niet te doen. Ik krijg geen werk meer gedaan met al die meldingen — en het is altijd vals."* Hij stelt het dashboard die dag in op **'alleen kritische alarmen'**. Niemand heeft hem gevraagd dit te doen, niemand verbiedt het. De andere twee operators volgen binnen drie dagen.
>
> **Week 3 (donderdag, 14:20).** Een echte verstoring: een lager in de schroefinstallatie loopt heet. De temperatuursensor signaleert dit om 14:20, maar het alarm staat op 'niet-kritisch' en wordt niet getoond op het hoofdscherm. Pas om 16:45 — bij de eindcontrole — wordt afkeur ontdekt: **240 onderdelen** moeten worden gerejecteerd. De klant (autobouwer) krijgt een melding; dit telt mee voor de PPM-rapportage van het kwartaal.
>
> **Vrijdag.** Crisis-overleg. Iemand vraagt: *"Hadden we die sensoren wel moeten installeren?"*

---

## 🟠 Vraag 1 — Wat is hier eigenlijk gebeurd?

*Beschrijf in eigen woorden het patroon. Niet 'wie heeft schuld', maar: welk mechanisme zorgde ervoor dat een dure sensoruitbreiding eindigde in een gemiste verstoring?*

_______________________________________________

_______________________________________________

_______________________________________________

_______________________________________________

_______________________________________________

---

## 🟣 Vraag 2 — Wat had jíj als teamleider anders kunnen doen?

*Niet als operator (Daan), maar als teamleider die de lijn-eigenaar is. Op welk moment in dit verhaal had je voor het eerst kunnen ingrijpen — en wat was die ingreep geweest?*

**Eerste moment van ingrijpen:** (week 1 / week 2 / vóór week 1 / anders, namelijk:)

_______________________________________________

**De ingreep zelf:** (concreet — welke handeling, welk gesprek, welk besluit?)

_______________________________________________

_______________________________________________

_______________________________________________

_______________________________________________

---

## 🟢 Vóór de bespreking

*Eén laatste vraag voor jezelf, voordat we plenair gaan:*

**Heb je dit patroon — in welke vorm dan ook — al op je eigen lijn zien ontstaan?**

- ☐ Ja, exact zo
- ☐ Ja, in afgezwakte vorm (operator klaagt, dashboard wordt deels genegeerd)
- ☐ Nee, nog niet — maar ik zie het risico bij komende uitbreidingen
- ☐ Nee, en ik weet ook niet zeker of het bij ons zou gebeuren

**Korte toelichting (1 zin):**

_______________________________________________

_______________________________________________

---

## 📝 Notities tijdens plenaire bespreking

*Ruimte om kort te noteren wat collega's vertellen — vooral het signaal dat jij op je eigen lijn ook herkent:*

_______________________________________________

_______________________________________________

_______________________________________________

_______________________________________________

---

> **Volgende stap:** We bespreken dit plenair (6 minuten). Daarna komt de handout met het 6-stappen rationalisatieproces — en je gaat zien dat dit casus geen ongelukkige uitzondering is, maar een **statistisch voorspelbaar patroon** bij elke sensoruitbreiding zonder rationalisatie.

---
*Bron: ko-spc-603 (Alarm fatigue / cry-wolf); medische literatuur patient monitoring; AIAG-richtlijn alarm management | AIMM Module 3 — SPC Op Maat | v1.0*
