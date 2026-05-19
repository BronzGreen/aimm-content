# Handout: Common Cause vs Special Cause
*Wanneer wel, wanneer niet aan een knop draaien*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**  
> Een productieproces varieert altijd. De vraag is niet *óf* er variatie is, maar *welk soort* variatie. Wie het verschil tussen **common cause** en **special cause** kent, weet wanneer ingrijpen helpt — en wanneer het juist schaadt.

---

## Twee soorten variatie

Variatie in een productieproces komt in twee soorten. Het verschil zien is het hele punt van deze sessie.

| | **Common cause** | **Special cause** |
|---|------------------|-------------------|
| **Wat is het?** | Variatie die in het systeem zelf zit | Iets ánders dan normaal — een invloed die er meestal niet is |
| **Hoe vaak?** | Altijd aanwezig, elke dag, elke meting | Komt en gaat — meestal traceerbaar |
| **Voorbeelden uit de praktijk** | Buitentemperatuur, materiaalvariatie binnen batch, normale slijtage, meetruis, koelwater-temperatuur | Verkeerde materiaalbatch, defecte sensor, vastlopend thermokoppel, verstopte nozzle, fout gereedschap, matrijs scheef |
| **Wat doe je?** | Niets bijstellen — het hoort erbij | Onderzoeken en de oorzaak wegnemen |

---

## 🔵 Hoe herken je het in de meetwaarden?

| **Common cause-patroon** | **Special cause-patroon** |
|--------------------------|---------------------------|
| Willekeurige spreiding rond het gemiddelde | Plotselinge **sprong** omhoog of omlaag |
| Geen onwaarschijnlijke reeksen | **Trend**: meerdere metingen op rij die stijgen of dalen |
| Beide kanten van het gemiddelde ongeveer even vaak | **Cluster**: 7 of meer metingen op rij aan één kant van het gemiddelde |
| Geen punt valt buiten je normale bereik | **Punt buiten de grenzen** van wat je gewend bent |
| | **Oscillatie** (op-en-neer-patroon): meting wisselt steeds extreem hoog–laag |

---

## 🟣 Waarom geen losse meetwaarde beoordelen?

> Eén onderdeel op 100,02 gram zegt weinig.  
> Tien opeenvolgende metingen die langzaam omhoog kruipen op een spuitgietlijn zegt véél meer.

**SPC staat voor Statistical Process Control. Dat is een manier om je proces in de tijd te volgen op een kaart. SPC beoordeelt tijdreeksen — meetwaarden in volgorde van tijd — en geen losse waardes.**

Eén afwijkende meting kan toeval zijn (common cause). Een patroon in meerdere metingen is een signaal (special cause). Daarom is bijhouden in een grafiek zo nuttig: je ziet het patroon dat je in losse waardes mist.

---

## 🟠 Wanneer wel/niet ingrijpen?

| Situatie | Wat doe je? |
|----------|-------------|
| Eén meting net buiten je gewone bereik, daarna weer normaal | **Niets doen.** Common cause — toeval hoort erbij. |
| Meerdere metingen op rij stijgen of dalen | **Onderzoeken.** Trend = special cause-signaal. |
| Plotselinge sprong na een gebeurtenis (matrijswissel, batch, nieuwe gereedschapshouder) | **Onderzoeken.** Special cause — koppel terug naar de gebeurtenis. |
| 7 of meer metingen op rij aan één kant van het gemiddelde | **Onderzoeken.** Cluster = special cause-signaal. |
| Schommeling binnen het normale patroon | **Niets doen.** Common cause — bijstellen maakt het slechter. |

---

## 🔴 De grootste valkuil: overcontrol

Bijstellen op elke afwijkende meting heet **overcontrol**. Het lijkt actief en goed, maar het maakt het proces juist instabieler. Je voegt extra variatie toe die er eerst niet was.

**Voorbeeld:** Vulgewicht is 503 gram (normaal 498–502). Je draait de doseerschroef terug. Volgende meting: 495 gram. Je draait weer omhoog. Volgende: 504 gram. Je hebt een common-cause-schommeling behandeld als special cause — en het proces dansje gemaakt.

---

## 🟢 Onthoud dit

1. Variatie is normaal — wees er niet bang voor.
2. Eén meting zegt niets — kijk naar het patroon in meerdere metingen.
3. Bij een **patroon** (sprong, trend, cluster, punt buiten bereik): onderzoek.
4. Bij **willekeurige schommeling**: laat het met rust.
5. Bij twijfel: meet een paar keer extra voordat je aan een knop draait.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Variatie** | Verschillen tussen meetwaarden van hetzelfde proces |
| **Common cause** | Normale variatie die altijd aanwezig is |
| **Special cause** | Variatie door een uitzonderlijke oorzaak |
| **Tijdreeks** | Meetwaarden in volgorde van tijd (zoals een grafiek) |
| **Trend** | Meerdere metingen op rij die dezelfde kant op gaan |
| **Cluster** | Meerdere metingen op rij aan dezelfde kant van het gemiddelde |
| **Overcontrol** | Onnodig bijstellen op normale schommeling |
| **SPC** | Statistical Process Control — kijken naar variatie in de tijd |

---
*Bron: Deming, W.E. (1986) Out of the Crisis; Wheeler, D.J. (1993) Understanding Variation | AIMM Module 1 — SPC Gebruik | v1.0*
