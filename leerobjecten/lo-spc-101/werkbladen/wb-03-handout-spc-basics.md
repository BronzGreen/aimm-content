# Handout: SPC-basics — de drie componenten
*Wat staat er op die grafiek bij mijn machine?*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**
> SPC staat voor **Statistical Process Control**. Het is **geen inspectie achteraf** — het is procesgedrag in de tijd volgen via een regelkaart. De kerntaak: zien of de variatie in je proces **consistent en voorspelbaar** is, of dat er **onvoorspelbare verstoringen** optreden (bron: ASQ — Control Chart; ISO 7870-1, ISO 7870-2).

---

## De drie componenten van een regelkaart

Elke regelkaart — van spuitgietlijn tot verpakking, van CNC tot assemblage — heeft dezelfde opbouw.

| | **Wat is het?** | **Waar kijk je naar?** |
|---|---|---|
| **1. Centrale lijn (CL)** | Het gemiddelde gedrag van je proces | Ligt meestal in het midden van de grafiek |
| **2. UCL en LCL** | Upper/Lower Control Limit — grenzen van het **normale** procesgedrag. **Geen** klantspecificaties. | Boven en onder de centrale lijn, meestal op een paar standaarddeviaties afstand (bron: Shewhart 1931) |
| **3. Punten in tijd** | Meetwaarden in de volgorde waarin ze zijn gedaan | Van links naar rechts: punt 1 was eerst, daarna punt 2, enzovoort |

---

## 🔵 Wat is het verschil met klantspecificaties?

Dit is belangrijk en wordt vaak verward:

| **Regelgrenzen (UCL/LCL)** | **Klantspecificaties (USL/LSL)** |
|---|---|
| Komen uit **je proces zelf** | Komen van de **klant** of uit het ontwerp |
| Zeggen: wat is normaal voor **deze lijn**? | Zeggen: wat mag wel/niet verkocht worden? |
| Statistisch bepaald uit historische data | Bepaald door eis of tolerantie |
| Staan op de **regelkaart** | Staan op de **tekening of bestelformulier** |

Een proces kan binnen regelgrenzen draaien (stabiel) en tóch buiten klantspec raken — dan is er iets anders aan de hand. Omgekeerd kan een proces binnen klantspec draaien en tóch instabiel zijn (nu geluk, morgen niet). SPC kijkt naar het **proces**, niet naar het onderdeel.

---

## 🟣 Stabiel of onstabiel? De herkenningslijst

| **Stabiel (voorspelbaar)** | **Onstabiel (onvoorspelbaar)** |
|---|---|
| Willekeurige spreiding rond de centrale lijn | Plotselinge **sprong** omhoog of omlaag |
| Alle punten binnen UCL/LCL | Een of meer **punten buiten** UCL of LCL |
| Evenveel boven als onder de centrale lijn | **Trend**: meerdere metingen op rij omhoog of omlaag |
| Geen rare patronen | **Cluster**: 7 of meer op rij aan één kant van de lijn |

Walter Shewhart formuleerde deze basis in 1931: een centrumlijn met grenzen op enkele standaarddeviaties, en het patroon van de punten verklapt of er een andere oorzaak meespeelt (bron: Shewhart, W.A. 1931 — *Economic Control of Quality of Manufactured Product*).

---

## 🟠 Waarom geen losse meetwaarde beoordelen?

> Eén meting van 100,3 g op een spuitgietlijn zegt weinig.
> Tien opeenvolgende metingen die langzaam stijgen zegt véél meer.

**SPC is een tijdreeks-beoordeling.** Variatie zie je pas in het patroon over tijd — niet in losse waarden. Dat is precies waarom de kaart de **volgorde** van metingen bewaart.

**Vuistregel (te valideren per werkvloer):** voor een nieuwe observatie heb je minstens 5 tot 10 opeenvolgende metingen nodig voordat je een patroon zinnig kunt beoordelen.

---

## 🟢 Wat SPC níet is

- **Geen eindinspectie.** SPC keurt geen onderdelen af — dat doet de kwaliteitscontrole.
- **Geen garantie voor perfecte kwaliteit.** SPC maakt alleen zichtbaar of het proces zich voorspelbaar gedraagt.
- **Geen bijstelautomaat.** Een regelkaart vertelt je alleen *dat* er iets lijkt te spelen, niet meteen *wat* — onderzoek is altijd de volgende stap.

---

## 🔴 Onthoud dit

1. **SPC volgt procesgedrag in de tijd** — het is geen inspectie achteraf.
2. **Regelkaart = centrale lijn + UCL/LCL + punten in tijd.**
3. **UCL/LCL zijn procesgrenzen, geen klantspecificaties.**
4. **Losse waarde zegt weinig — patroon in tijd zegt veel.**
5. **Stabiel** = willekeurig binnen grenzen. **Onstabiel** = sprong, trend, cluster, punt buiten grenzen.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **SPC** | Statistical Process Control — procesgedrag in de tijd volgen |
| **Regelkaart** | Grafiek met centrale lijn, UCL/LCL en punten in tijd |
| **CL** | Centrale Lijn — het gemiddelde procesgedrag |
| **UCL** | Upper Control Limit — bovengrens van normaal procesgedrag |
| **LCL** | Lower Control Limit — ondergrens van normaal procesgedrag |
| **USL / LSL** | Klantspecificaties (ontwerpgrenzen) — iets anders dan UCL/LCL |
| **Tijdreeks** | Meetwaarden in volgorde van tijd |
| **Stabiel proces** | Variatie is consistent en voorspelbaar |
| **Onstabiel proces** | Er lijkt een extra oorzaak mee te spelen |

---

*Bron: Shewhart, W.A. (1931) Economic Control of Quality of Manufactured Product; ASQ — Control Chart definitie; ISO 7870-1, ISO 7870-2; NIST/SEMATECH Engineering Statistics Handbook | AIMM Module 1 — SPC Gebruik | v1.0*
