# Mijn Cpk/Ppk-gap: Diagnose voor Mijn Eigen Lijn
*Pp/Ppk — langetermijn-procesbekwaamheid (ko-spc-302)*

**Naam:** ____________________  **Datum:** __________
**Lijn / proces:** ____________________  **Kritische maat:** ____________________

---

> **Over dit werkblad** *(blok 2 — experimenteren, A4 dubbelzijdig of A3)*
> Dit werkblad is jouw diagnose voor één concrete eigen lijn. Geen hypothetisch geval — jouw eigen klantkritische maat, over minimaal een week data uit meerdere shifts of batches. Wat je nog niet weet, mag blijven staan met "opzoeken week 1 bij kwaliteit". Aan het eind heb je één pagina met een getal, een hypothese en een maandag-actie.

---

## 🔵 1. Scope van mijn lijn

**Welke lijn / welk product / welke maat kies je?**
*(bijv. "Spuitgietlijn 3, onderdeel XZ-45, onderdeelgewicht in gram")*

_______________________________________________

_______________________________________________

**Klantspecificatie — tolerantiegrenzen**

| Grens | Waarde | Eenheid |
|-------|--------|---------|
| USL (bovengrens klant) | | |
| LSL (ondergrens klant) | | |
| Nominale waarde | | |

**Klantcontext** *(interne klant, externe klant, automotive/PPAP?)*

_______________________________________________

---

## 🟠 2. Cpk en Ppk — de twee getallen

*Haal op uit je kwaliteitsrapport, MES, of schat realistisch op basis van wat je weet.*

**Dataset**

| | Waarde |
|---|--------|
| Periode (van ... tot ...) | |
| Aantal meetwaarden | |
| Aantal shifts / batches in deze periode | |

**De cijfers**

| Index | Waarde | Bron / hoe bepaald |
|-------|--------|---------------------|
| Cpk (binnen-subgroep, kortetermijn) | | |
| Ppk (totale spreiding, langetermijn) | | |
| **Gap (Cpk − Ppk)** | | *(reken uit)* |

Weet je de waarde niet precies? Schat, en noteer "opzoeken bij kwaliteit week 1" erbij.

---

## 🟣 3. Gap-diagnose — wat zegt het verschil?

**Zet een kruisje bij de categorie die past**

- ☐ **Gap < 0,10** — stabiel proces, weinig tussen-subgroep-variatie. Actie (als Cpk te laag): op het proces zelf.
- ☐ **Gap 0,10 – 0,20** — merkbare tussen-subgroep-variatie. Kijk naar batches/shifts/setups.
- ☐ **Gap > 0,20** — groot gat. Actie ligt op het **systeem rondom** het proces, niet op de machine.

**Toets Ford PPAP (4th edition, eis Ppk ≥ 1,67)**

- ☐ Ja — Ppk ≥ 1,67 gehaald
- ☐ Nee — Ppk < 1,67, ontbrekend bedrag: _______
- ☐ Niet van toepassing (geen automotive-klant)

**Toets klant-eis** *(indien andere klant — vul hun drempel in)*

Klant-eis Ppk: __________ | Gehaald: ☐ Ja / ☐ Nee

---

## 🔴 4. Oorzaak-hypothesen — waar komt de gap vandaan?

**Kruis aan wat op jouw lijn speelt — minstens twee bij een gap > 0,20**

- ☐ **Materiaalbatch-wissels** — nieuwe batch heeft net andere eigenschappen
- ☐ **Shift-overdracht** — ploeg A/B/C stelt niet identiek in
- ☐ **Setup-aanpassingen** — wisseltijd tussen orders niet gestandaardiseerd
- ☐ **Temperatuur** — dag/nacht, seizoen, locatie op de vloer
- ☐ **Meetsysteem-drift** — meter wordt niet op tijd gekalibreerd
- ☐ **Anders, namelijk:** _______________________________________________

**Mijn hoofdhypothese voor deze lijn** *(één zin)*

_______________________________________________

_______________________________________________

---

## 🟢 5. Actie-beslissing

**Waar ligt de volgende actie?**

- ☐ **Op het proces zelf** (Cpk te laag — machine/parameters)
- ☐ **Op het systeem rondom** (Cpk goed, gap groot — setup, shift, batch, temperatuur)
- ☐ **Beide — eerst systeem rondom, dan proces**

**Mijn concrete maandag-actie** *(wat doe je, wanneer, met wie?)*

Wat? _______________________________________________

Wanneer? __________________________

Met wie? __________________________

Hoe weet je of het werkte? ____________________________________

---

## 🔵 6. Aandachtspunten / open vragen

*Wat moet je nog uitzoeken vóór je écht beslist?*

_______________________________________________

_______________________________________________

_______________________________________________

---

> 💡 **Onthoud:** Een grote gap tussen Cpk en Ppk is zelf een signaal. Je lost hem niet op door de machine strakker te zetten — je lost hem op door het systeem rondom (setup, shift, batch) onder controle te krijgen. Ford PPAP eist Ppk ≥ 1,67, niet alleen een mooie Cpk.

---
*Bron: ko-spc-302 (Pp/Ppk). Ford PPAP 4th edition, AIAG SPC Reference Manual, NIST/SEMATECH e-Handbook of Statistical Methods. AIMM Module 3 — SPC Op Maat | v1.0*
