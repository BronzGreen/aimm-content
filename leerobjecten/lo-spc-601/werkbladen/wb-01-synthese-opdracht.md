# Synthese-Opdracht: AI + SPC op Mijn Eigen Machine
*Hoe zou AI + klassieke SPC samenwerken op jouw lijn?*

**Naam:** ____________________  **Datum:** __________
**Machine / lijn:** ____________________  **Product:** __________

---

> **Over dit werkblad** *(blok 2 — experimenteren, A4)*
> Dit is geen theorie-oefening. Je kijkt naar **jouw** machine en beschrijft per laag wat er al is, wat er nog niet is, en waar AI wel of juist niet zou passen. Invullen wat je weet — markeren wat je moet uitzoeken is prima.

---

## 🔵 Laag 1 — Meten

*Hoe komt de data van je proces tot bij jou?*

**Wat meet je op jouw lijn? (maten / parameters)**

_______________________________________________

_______________________________________________

**Hoe meet je nu?**

- ☐ Handmatig (bv. elke shift / elke 2 uur een monster)
- ☐ Semi-automatisch (sensor meet, operator leest af)
- ☐ Continu via IoT-sensoren → dashboard
- ☐ Anders: _______________________________________________

**Kan AI hier iets toevoegen?**

- ☐ Ja — bv. meetfouten herkennen, ontbrekende data schatten
- ☐ Nee — metingen zijn betrouwbaar en compleet
- ☐ Weet ik niet — uitzoeken met: __________

---

## 🟠 Laag 2 — Signaal-detectie

*Hoe zie je nu dat er iets afwijkt?*

**Hoe herken je afwijkingen nu?**

- ☐ Ik kijk zelf naar de kaart / het scherm en pas Nelson-regels toe
- ☐ Het dashboard geeft automatisch alarm op Nelson-regels
- ☐ Er is een auto-alarm maar ik weet niet welke regels erachter zitten
- ☐ Anders: _______________________________________________

**Welke Nelson-regels zijn bij jou actief?** *(voor zover je het weet)*

_______________________________________________

_______________________________________________

**Waar zien Nelson-regels mogelijk te weinig?** *(meerdere variabelen die samen afwijken, langzame drift, combinatie-patronen)*

_______________________________________________

_______________________________________________

**Zou AI hier waarde toevoegen?**

- ☐ Ja — bv. combinatie van 2-3 variabelen die samen afwijken
- ☐ Ja — bv. patronen die Nelson-regels niet vatten
- ☐ Nee — Nelson-regels zijn genoeg voor deze lijn
- ☐ Weet ik niet — uitzoeken met: __________

---

## 🟣 Laag 3 — Beslissen

*Wie beslist er wat er gebeurt als er een signaal is?*

**Wie beslist nu bij een afwijking?**

- ☐ Ik als operator, volgens reactieplan
- ☐ Teamleider / shiftleider
- ☐ Kwaliteitsdienst
- ☐ Combinatie: __________

**Kan AI hier ondersteunen?**

- ☐ Ja — aanbeveling geven ('controleer eerst X')
- ☐ Ja — prioriteren welk alarm het belangrijkst is
- ☐ Nee — beslissingen blijven bij mens, AI voegt niks toe
- ☐ Weet ik niet

**Wat blijft altijd mijn / onze verantwoordelijkheid?**

_______________________________________________

_______________________________________________

---

## 🟢 Eén kans en één zorg

*Concreet, voor jouw werkvloer.*

**Eén kans — waar zou AI op jouw lijn echt iets toevoegen?**

_______________________________________________

_______________________________________________

**Eén zorg — waar maak je je zorgen over als AI erbij komt?**

*(bv. uitlegbaarheid, vertrouwen, rolverandering, datakwaliteit)*

_______________________________________________

_______________________________________________

---

## 📎 Referentie — fictieve chemische reactor

> *Dit is een fictief voorbeeld — gebruik het als ijkpunt, niet als sjabloon.*
>
> Een chemische reactor meet continu druk, temperatuur en debiet. Elke variabele heeft zijn eigen controlekaart met Nelson-regels. Een AI-model dat is getraind op historische batches herkent dat een **combinatie** (temperatuur iets hoog + debiet iets laag + druk normaal) vaak voorafgaat aan een off-spec batch. De AI geeft 40 minuten eerder een vroege waarschuwing dan de Nelson-regels. De operator blijft beslisser; Nelson-regels blijven actief als tweede net.

---

> 💡 **Onthoud:** niet elke lijn heeft AI nodig. Nelson-regels volstaan vaak. AI voegt waarde toe als meerdere variabelen samen spelen, als er veel historische data is, én als iemand de AI-uitkomst kan uitleggen.

---
*Bron: ko-spc-601 (Digitale SPC en sensordata) | AIMM Module 3 — SPC Op Maat | v1.0*
