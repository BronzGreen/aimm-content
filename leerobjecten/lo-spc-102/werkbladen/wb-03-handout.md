# Handout: Regelkaart lezen + reactieplan
*De klassieke gedragsregels en wat jij als operator doet*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Een regelkaart herkent signalen door patronen — niet alleen door grenzen."**

Een run, trend of zone-patroon *binnen* de controlegrenzen is óók een signaal. Wie alleen kijkt of een punt buiten UCL of LCL ligt, mist de helft van de waarschuwingen.

---

## 🔵 Jouw rol op de regelkaart

Uit ko-spc-102: SPC werkt op drie niveaus tegelijk.

| Rol | Frequentie | Wat jij/zij doet |
|-----|-----------|------------------|
| **Operator (jij)** | Dagelijks | Meten, plotten, patroon herkennen, reageren volgens reactieplan |
| Teamleider | Shift / dag / week | Patronen over shifts, machines, ploegen, matrijzen vergelijken |
| Kwaliteitsmanager | Strategisch | Limieten valideren, capability beoordelen, control plans beheren |

*Bron: AIAG SPC Reference Manual, 2e ed. (2005); ko-spc-102.*

Jouw bijdrage: **lezen + reageren in het hier-en-nu.** De teamleider kan patronen pas zien als jij ze eerst correct vastlegt.

---

## 🟣 Controlegrens versus tolerantiegrens

Dit onderscheid is **géén detail**. Een van de vaakst voorkomende fouten op de werkvloer.

| Grens | Waar vandaan? | Wat zegt het? | Code |
|-------|---------------|---------------|------|
| **UCL / LCL** | Uit het **proces zelf** — berekend op basis van variatie | "Gedraagt mijn machine zich zoals ze hoort?" | Controlegrens |
| **USL / LSL** | Van de **klant** — uit tekening of specificatie | "Is dit onderdeel bruikbaar?" | Tolerantiegrens |

Een proces kan binnen de tolerantie draaien én tóch een signaal geven op de regelkaart. Dat signaal zegt: morgen ligt het misschien buiten de tolerantie — als je niks doet.

*Bron: Shewhart (1931), Economic Control of Quality of Manufactured Product; AIAG SPC 2005; Montgomery, D.C. (2012), Introduction to Statistical Quality Control, 7e ed.*

---

## 🟢 De klassieke gedragsregels

Western Electric publiceerde in hun *Statistical Quality Control Handbook* (1956) de eerste zone-regels. Lloyd Nelson verfijnde ze in *Journal of Quality Technology* (1984) tot de set van 8 die vandaag standaard is.

### Jouw startpakket — 4 regels die een operator vooral gebruikt

| # | Regel | Wat zie je? | Waarom is dit een signaal? |
|---|-------|-------------|------------------------------|
| **1** | **Punt buiten controlegrens** | Eén punt boven UCL of onder LCL | Kans ≈ 0,27% bij stabiel proces — vrijwel zeker special cause |
| **2** | **Run** | 7 of meer opeenvolgende punten aan één kant van de middenlijn | Het procesgemiddelde is aan het verschuiven |
| **3** | **Trend** | 6 of meer opeenvolgende punten steeds hoger (of steeds lager) | Geleidelijke verschuiving: slijtage, temperatuur, gereedschap |
| **4** | **2-uit-3 in waarschuwingszone** | 2 van 3 opeenvolgende punten in zone A (tussen 2σ en 3σ, aan dezelfde kant) | Proces instabiel aan die kant |

*Bron: Western Electric (1956); Nelson, L.S. (1984), "The Shewhart Control Chart — Tests for Special Causes", Journal of Quality Technology 16(4), pp. 237–239; AIAG SPC 2005.*

### De volledige Nelson-set (referentie, voor later)

De 8 Nelson-regels in hun volledigheid:

1. Eén punt buiten 3σ (UCL/LCL) — **regel 1 uit je startpakket**
2. 9 opeenvolgende punten aan één kant van de middenlijn (Nelson gebruikt 9; sommige bronnen 7 of 8) — **basis voor regel 2**
3. 6 opeenvolgende punten steeds hoger of lager — **regel 3**
4. 14 opeenvolgende punten die afwisselend hoog-laag-hoog-laag gaan
5. 2 uit 3 opeenvolgende punten voorbij 2σ aan dezelfde kant — **regel 4**
6. 4 uit 5 opeenvolgende punten voorbij 1σ aan dezelfde kant
7. 15 opeenvolgende punten binnen 1σ van de middenlijn (beide kanten)
8. 8 opeenvolgende punten buiten 1σ (beide kanten)

*Bron: Nelson (1984); samengevat in AIAG SPC 2005 en Montgomery 2012.*

> Begin met de 4. De overige 4 leer je later — in module 3 of als je ervaring bouwt.

---

## 🟠 Het reactieplan — vier actieniveaus

| Niveau | Actie | Wanneer? | Voorbeeld |
|--------|-------|----------|-----------|
| **1** | Doorgaan + normaal loggen | Géén patroon — gewone variatie | Punten schommelen rond middenlijn |
| **2** | Signaal vastleggen (tijd, waarde, wat gezien) | Run of trend in rustige zone, nog niet dicht bij grens | 7 punten aan één kant, allemaal binnen 2σ |
| **3** | Bijsturen volgens procedure + vastleggen | Duidelijk oplosbaar signaal | Trend bij vulgewicht → dosering bijstellen |
| **4** | Stoppen of melden aan teamleider/engineering | Punt buiten controlegrens, twijfel over meetsysteem, herhaald signaal | Punt > UCL, of 2-uit-3 in waarschuwingszone |

> **Belangrijk:** het reactieplan **per lijn** verschilt per bedrijf en per type product. Vraag je teamleider wat voor jouw machine afgesproken is. Is er geen geschreven reactieplan? Dan is jouw observatie zelf waardevolle input voor het maken ervan.

*Bron: AIAG SPC 2005, hoofdstuk Reaction Plans; ISO 7870-2 (regelkaart-richtlijnen).*

---

## 🔴 Signaal of ruis? Drie valkuilen

*Niet elk raar ogend punt is een signaal. Pas op voor:*

| # | Valkuil | Wat is er aan de hand? |
|---|---------|--------------------------|
| 1 | **Normaal schommelen** | Een stabiel proces schommelt rond de middenlijn — dat is gezond, géén signaal |
| 2 | **Eén uitschieter** | Kan een meetfout zijn; herhaal de meting voordat je actie onderneemt |
| 3 | **Ritmische golf** | Soms is dat een bekende cyclus (dag/nacht, opwarming machine) — geen special cause |

*Bron: Montgomery (2012), hoofdstuk over patroonherkenning; Nelson (1984).*

De kunst: **signaal niet missen én ruis niet als signaal lezen.** Allebei fout kost geld.

---

## 📋 Koppeling naar de oefening (wb-01)

| Oefening-casus | Welk patroon? | Welke actie? |
|:--------------:|---------------|--------------|
| **Casus 1** (punt op 50,42 g boven UCL) | Regel 1: punt buiten controlegrens | Niveau 4: stoppen of melden |
| **Casus 2** (8 punten steeds stijgend) | Regel 3: trend van 6+ stijgend | Niveau 3: bijsturen + vastleggen |
| **Casus 3** (2 van 3 in waarschuwingszone) | Regel 4: 2-uit-3 in zone A | Niveau 3 of 4: bijsturen, bij twijfel melden |
| **Casus 4** (punten schommelen normaal) | Géén patroon — normale variatie | Niveau 1: doorgaan + normaal loggen |

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Regelkaart** | Grafiek waarop je metingen in volgorde plot met controlegrenzen |
| **X̄-kaart** | Regelkaart voor het gemiddelde van kleine subgroepen |
| **R-kaart** | Regelkaart voor de range (spreiding) binnen die subgroepen |
| **UCL / LCL** | Upper / Lower Control Limit — de 3σ-grenzen van het proces |
| **USL / LSL** | Upper / Lower Specification Limit — de tolerantiegrenzen van de klant |
| **Middenlijn** | Gemiddelde van het stabiele proces |
| **Zone A / B / C** | De banden op 1σ, 2σ en 3σ boven en onder de middenlijn |
| **Special cause** | Bijzondere oorzaak van variatie — iets is veranderd |
| **Common cause** | Gewone variatie — het proces doet wat het altijd doet |
| **Reactieplan** | Afspraak per lijn: welk patroon → welke actie |

---

## 🟢 Onthoud dit

1. **Jouw rol** = dagelijks meten, plotten, patroon herkennen, reageren.
2. **Controlegrens ≠ tolerantiegrens.** UCL/LCL komt uit het proces; USL/LSL uit de klantspecificatie.
3. **Vier klassieke patronen** — punt-buiten-grens, run (7+), trend (6+), 2-uit-3 in zone A.
4. **Vier actieniveaus** — doorgaan / vastleggen / bijsturen / stoppen-en-melden.
5. **Signaal of ruis?** Bij twijfel: meet opnieuw, vraag door, noteer wat je zag.
6. **Vraag het reactieplan.** Bestaat er een geschreven afspraak? Zo niet: jouw observatie is het begin ervan.

---

*Bronnen: Shewhart, W.A. (1931), Economic Control of Quality of Manufactured Product; Western Electric Co. (1956), Statistical Quality Control Handbook; Nelson, L.S. (1984), "The Shewhart Control Chart — Tests for Special Causes", JQT 16(4), pp. 237–239; AIAG (2005), Statistical Process Control Reference Manual, 2e ed.; ISO 7870-2 (regelkaart-richtlijnen); Montgomery, D.C. (2012), Introduction to Statistical Quality Control, 7e ed. | ko-spc-102 | AIMM Module 2 — SPC Train | v1.0*
