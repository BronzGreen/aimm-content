# Reflectie: Wanneer voegde het ensemble het meest toe?
*Kolb fase 2: reflecteren — buurman-check en plenaire reflectie via STARRT*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: Ensemble Learning**

---

## Over dit werkblad

Je hebt vijf cases doorlopen met één expert versus drie experts. Nu vergelijk je je antwoorden met je buurman en met de groep. Reflectie volgt het STARRT-model: Situatie, Taak, Actie, Resultaat, Reflectie, Transfer.

Doel is niet alleen turven. Doel is voelen **wanneer drie modellen samen sterker zijn — en wanneer niet.** Dat onderscheid is de hele kern van ensemble learning.

**Tijd:** 9 minuten — eerst 5 minuten in tweetallen, daarna 4 minuten plenair.

---

## 1. Situatie — welke case maakte het grootste verschil?

*In welke case veranderde het ensemble jouw antwoord het meest?*

○ Case 1 — Lager   ○ Case 2 — Spuitgietmachine   ○ Case 3 — CNC-spindel   ○ Case 4 — Pomp   ○ Case 5 — Lasrobot

*Beschrijf in eigen woorden wat er gebeurde:*

_______________________________________________

_______________________________________________

_______________________________________________

---

## 2. Taak — drie experts spraken elkaar tegen

*Wanneer er onenigheid was, waar lette je op om te beslissen?*

| Mijn afweging | Speelde dit mee? |
|---------------|:----------------:|
| Hoeveel experts hetzelfde zeiden (meerderheid) | ○ |
| Wat de meest "voorzichtige" diagnose was | ○ |
| Welke diagnose het meest gedetailleerd onderbouwd leek | ○ |
| Welke me logisch leek bij wat ik zelf wist | ○ |

---

## 3. Actie — welke "stem-strategie" gebruikte je?

*Hoe vatte je de drie meningen samen tot één antwoord?*

○ Strikte meerderheid (2 op 3 wint)
○ Voorzichtigheid: bij twijfel "actie" kiezen
○ Eigen oordeel: ik laat een expert vallen die niet logisch klinkt
○ Anders: _______________________________________________

*Toelichting:*

_______________________________________________

_______________________________________________

---

## 4. Resultaat — wat zei je buurman?

*Vergelijk met je buurman. Bij welke cases was je antwoord hetzelfde, en bij welke verschilde het?*

**Zelfde antwoord op cases:** _______________________________________________

**Verschil bij cases:** _______________________________________________

*Wat hoorde je van je buurman dat je zelf niet had gezien?*

_______________________________________________

_______________________________________________

---

## 5. Reflectie — wanneer voegde het ensemble het meeste toe?

*Markeer aan.*

- [ ] Bij twijfelgevallen (de cases waar de drie experts niet allemaal hetzelfde zeiden)
- [ ] Bij makkelijke cases (waar alle drie het al eens waren)
- [ ] Bij cases waar één expert overduidelijk fout zat
- [ ] Bij cases waar de meerderheid mij iets liet zien dat ik gemist had

*Welke vorm van toegevoegde waarde herken je het meest?*

_______________________________________________

_______________________________________________

---

## Werkvloer-voorbeeld — even doortrekken

> Stel: in jullie ERP staan drie verschillende **voorspellers** die elke maandagochtend een lijst opleveren met "machines met verhoogd risico op uitval deze week". Soms zijn de lijsten bijna identiek. Soms verschillen ze enorm. De planner moet beslissen: welke machines op de checklist?

*Wanneer is het waardevol om de drie lijsten samen te voegen tot één gewogen lijst — en wanneer juist niet?*

_______________________________________________

_______________________________________________

> **Hint:** als alle drie hetzelfde zeggen, is samenvoegen verspilde moeite. Bij twijfel daarentegen geeft de combinatie precies wat je wilt: een robuust antwoord dat niet afhangt van één model dat een slechte dag heeft.

---

## 6. Transfer — denk aan jouw PdM-data

*Heeft jullie organisatie weinig failure-cases? Een ensemble is dán juist krachtig — het is robuuster bij scheve data.*

**Hoeveel failure-cases per jaar heeft jouw machine ongeveer?**

○ 0-5  ○ 5-20  ○ 20-100  ○ > 100  ○ Onbekend

*Verwacht je dat een ensemble jullie meer waarde zou bieden dan een enkel model?*

○ Ja, vermoedelijk wel   ○ Twijfel   ○ Nee

*Waarom?*

_______________________________________________

_______________________________________________

> **Tip voor de plenaire bespreking:** kijk naar het bord — bij hoeveel cases won het ensemble bij de groep? Bij twijfelgevallen (case 2, 4, 5) zie je vaak dat de meerderheid een verstandiger antwoord oplevert dan A alleen. Bij case 3 (alle drie hetzelfde) voegde de stemming niets toe — en dat is óók een belangrijke les: ensembles helpen vooral bij twijfel, niet bij eenduidige situaties.

---

## Wat doen we hierna?

In fase 3 krijg je de theorie: ensembles hebben twee hoofdfamilies. **Bagging** (parallel — wat jullie net deden in het diagnose-spel) en **boosting** (sequentieel — modellen leren van elkaars fouten). Houd je antwoorden bij de hand. We gebruiken ze om de twee families concreet te maken aan herkenbare PdM-cases.

---
*Bron: Ensemble Learning — AIMM Curriculum | Module 2: Train | v1.1*
