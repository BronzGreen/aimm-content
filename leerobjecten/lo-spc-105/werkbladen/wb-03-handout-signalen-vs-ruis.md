# Handout: Signalen vs Ruis — wel of niet ingrijpen?
*Tampering vermijden op de werkvloer*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**  
> Niet elke afwijkende meetwaarde is een signaal. Soms is het gewoon **ruis** — de normale schommeling van je proces (common cause). Ingrijpen op ruis heet **tampering** en maakt je proces slechter. Wacht op een **signaal** voordat je draait. En als het systeem zelf te instabiel is: escaleren.

---

## 🔵 Het funnel-experiment van Deming (kort)

W. Edwards Deming zette een trechter boven een tafel en probeerde een kogel op een doel te laten vallen. Hij testte vier strategieën:

| Strategie | Wat je doet | Resultaat |
|-----------|-------------|-----------|
| **1. Niets doen** | Trechter staat stil | **Laagste spreiding (winnaar)** |
| **2. Compenseren naar doel** | Trechter verschuiven om de vorige afwijking goed te maken | Spreiding verdubbelt |
| **3. Compenseren naar punt** | Trechter verplaatsen naar waar de kogel viel | Exponentieel afdrijven |
| **4. Compenseren naar meting** | Reageren op elke nieuwe waarde | Random walk — totaal geen controle |

> **Zolang het proces stabiel is (alleen common cause), wint "niets doen" altijd.**  
> Het Deming Institute beschrijft dit als de klassieke les over aanpassen zonder oorzaakbegrip.

Joiner's kernzin: **"Overreageren verhoogt variatie én kosten."**

---

## 🟢 WEL ingrijpen bij (dit is een signaal)

| Signaal | Wat je ziet | Wat je doet |
|---------|-------------|-------------|
| **Punt buiten de grenzen** | Eén meting valt buiten UCL of LCL | Stoppen, onderzoeken, oorzaak zoeken |
| **Trend** | Meerdere metingen op rij stijgen of dalen | Kijken naar recente gebeurtenissen (matrijs, batch, gereedschap) |
| **Sprong of cluster** | Plotselinge verschuiving, 7+ metingen aan één kant van het gemiddelde, of Nelson-patroon | Koppelen aan wat er is veranderd; onderzoeken |

---

## 🔴 NIET ingrijpen bij (dit is ruis)

| Situatie | Wat je ziet | Wat je doet |
|----------|-------------|-------------|
| **Eén losse afwijking** | Eén meting net hoger of lager dan je gewend bent — daarna weer normaal | **Niets.** Noteer alleen. |
| **Schommeling binnen bandbreedte** | Metingen gaan op en neer rond het gemiddelde, binnen specs | **Niets.** Dit is het normale gedrag. |
| **Onderbuikgevoel** | Je "voelt" dat er iets niet klopt, maar je data zegt het niet | **Niets** aan de knop. Wel extra meten. |

---

## 🟠 Wat als je tóch zorgen hebt?

Soms is de common cause variatie zelf te groot. De metingen zijn binnen specs, maar je klanten klagen, of de uitval loopt op. Dan is er iets mis met het **systeem**, niet met een losse meting.

> **Belangrijke regel:** Systeemvariatie verbeter je niet met een operator-knopje.

**Wat dan wel?**

1. Leg het patroon vast: 10–20 metingen met datum/tijd
2. Meld het bij je **teamleider**
3. Betrek **engineering** als het om matrijs, sensor, materiaal of machine gaat
4. Blijf zelf meten zoals je gewend bent — niet zelf gaan experimenteren

Dit is geen "probleem doorschuiven" — het is de juiste route. Een operator lost operator-problemen op. Een systeem lost systeemproblemen op.

---

## 🟣 De valkuil: tampering in de praktijk

*Fictieve illustratie:*

| Meting | Waarde | Operator doet | Volgende meting |
|--------|--------|---------------|-----------------|
| 1 | 502 g | Draait pomp 0,2 g terug | 498 g |
| 2 | 498 g | Draait pomp 0,4 g omhoog | 503 g |
| 3 | 503 g | Draait pomp 0,3 g terug | 497 g |
| 4 | 497 g | Draait pomp 0,5 g omhoog | 504 g |

**Na vier "correcties" is de spreiding verdubbeld.** Niet door de machine — door de operator zelf. Dit is strategie 2 of 4 uit Deming's funnel. Puur tampering.

Wat had moeten gebeuren: niets. Alle waardes zaten ruim binnen specs (500 ± 5 g) en binnen het normale patroon.

---

## 🟢 Onthoud dit

1. **Ruis ≠ signaal.** Schommeling binnen de normale bandbreedte is ruis.
2. **Wacht op een signaal.** Punt buiten grenzen, trend, cluster, Nelson-patroon.
3. **Tampering verdubbelt spreiding.** Elke "correctie" op ruis maakt het slechter.
4. **Systeemvariatie escaleer je.** Teamleider of engineering — geen operator-knopje.
5. **Niets doen is een vaardigheid.** Professionele discipline, geen luiheid.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Tampering** | Ingrijpen op normale variatie alsof het een signaal is |
| **Common cause** | Normale variatie die altijd in het proces zit |
| **Special cause** | Variatie door een uitzonderlijke oorzaak (iets ánders dan normaal) |
| **Signaal** | Aanwijzing dat er écht iets is veranderd (trend, sprong, punt buiten grenzen) |
| **Ruis** | Normale schommeling die erbij hoort — geen reden tot actie |
| **Escaleren** | Doorgeven aan teamleider of engineering voor systeemverbetering |
| **Funnel-experiment** | Deming's demonstratie: corrigeren op common cause verdubbelt de spreiding |

---
*Bronnen: Deming, W.E. (1986) *Out of the Crisis*, MIT Press (funnel-experiment, hoofdstuk 11). Het Deming Institute (deming.org) beschrijft het experiment als klassieke illustratie van aanpassen zonder oorzaakbegrip. Joiner, B.L. (1994) *Fourth Generation Management*, McGraw-Hill — "overreageren verhoogt variatie én kosten". | AIMM Module 1 — SPC Gebruik | v1.0*
