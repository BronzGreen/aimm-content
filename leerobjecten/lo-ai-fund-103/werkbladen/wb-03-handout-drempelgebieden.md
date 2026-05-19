# Werkblad 3 — Drie drempelgebieden (handout)
*Hoe AI met kansen werkt — Activiteit: Theoretiseren*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 13 minuten

---

> **De kern**
> Een AI-systeem werkt bijna altijd met onzekere informatie. Een camerabeeld is nooit honderd procent helder. Een sensor heeft ruis. Daarom geeft AI geen vast "ja" of "nee", maar een *waarschijnlijkheid* (kanspercentage). Dat percentage zegt hoe zeker het systeem is — op basis van duizenden eerdere voorbeelden.

---

## Wat betekent "87 procent kans op defect"?

Het systeem heeft veel eerdere beelden gezien. Bij beelden die op deze leken bleek **87 op de 100 keer** echt een defect. Bij 13 op de 100 niet. Het systeem rapporteert eerlijk: ik ben hier vrij zeker van, maar niet absoluut.

Bron: Russell & Norvig (2010). Artificial Intelligence — A Modern Approach.

---

## De drie drempelgebieden

*Markeer met je stift de drie gebieden. Hou ze de rest van de sessie bij de hand.*

| Defect-kans | Drempelgebied | Typische actie |
|---|---|---|
| **0 - 30 procent** | Laag | Doorlaten, eventueel steekproef |
| **30 - 70 procent** | Midden | Handmatig controleren |
| **70 - 100 procent** | Hoog | Direct afkeuren of stop |

> **Let op:** dit zijn vuistregels. De exacte grenzen verschillen per bedrijf en per product. Ze hangen af van twee dingen: wat een gemiste fout kost, en wat een onnodige check kost.

---

## Terug naar de drie producten van werkblad 1

*Klopten jouw keuzes met de drie gebieden? Vink aan.*

| Product | Defect-kans | Gebied | Mijn keuze paste hierbij |
|---|---|---|:--:|
| **A** | 87 procent | Hoog | Ja / Nee |
| **B** | 15 procent | Laag | Ja / Nee |
| **C** | 50 procent | Midden | Ja / Nee |

*Bij welk product week jouw keuze af van de vuistregel? Waarom?*

_______________________________________________

_______________________________________________

---

## De afweging — twee kosten

*Een drempel zetten is altijd een afweging.*

| Vraag | Wat het betekent voor de drempel |
|---|---|
| **Wat kost een gemiste fout?** Veiligheid? Klant die terugroept? Productie-batch verpest? | Hoe duurder de gemiste fout, hoe **lager** je drempel zet. |
| **Wat kost een onnodige check?** Tijd van een operator? Onderbreking van de lijn? | Hoe duurder de check, hoe **hoger** je drempel zet. |

*Korte oefening: voor jullie product — welke kost is groter?*

- [ ] Gemiste fout kost meer. Drempel moet eerder gaan naar "controleren" of "afkeur".
- [ ] Onnodige check kost meer. Drempel kan iets hoger liggen.
- [ ] Beide ongeveer gelijk. Standaard-drempel werkt.
- [ ] Ik weet het niet zeker. Vraag voor kwaliteit of IT.

---

## Vakwoorden in dit werkblad

*Onthoud deze termen voor de rest van de sessie.*

| Vakterm | Betekenis in een zin |
|---------|---------------------|
| **AI (Artificial Intelligence, kunstmatige intelligentie)** | Een systeem dat leert van voorbeelden en zelf beslist. |
| **Waarschijnlijkheid (kanspercentage)** | Hoe zeker het systeem is van zijn oordeel, in procenten. |
| **Drempel (grens-percentage)** | Het percentage waarboven je een andere actie kiest. |
| **Vuistregel** | Een richtlijn die meestal werkt, maar per situatie kan verschillen. |

---

*Bron: Russell & Norvig (2010). Artificial Intelligence — A Modern Approach. Pearson.*
*AIMM x BronzGreen — Module 1: Hoe AI met kansen werkt (lo-ai-fund-103) — v1.0*
