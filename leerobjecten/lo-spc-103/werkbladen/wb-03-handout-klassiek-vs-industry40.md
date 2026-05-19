# Handout: Klassieke SPC vs Industry 4.0 SPC
*Wat verandert, wat blijft hetzelfde?*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**  
> Elk productieproces varieert. De vraag "is deze meting normaal of niet?" is sinds 1931 onveranderd — bedacht door Walter Shewhart (bron: Shewhart, W.A. (1931) *Economic Control of Quality of Manufactured Product*; herbevestigd in ISO 7870-2 voor Shewhart-regelkaarten). Wat wél veranderd is: hoe je die vraag stelt, hoe snel je antwoord krijgt, en wie (of wat) bij de grenzen alarm slaat.

---

## De vijf belangrijkste verschuivingen

| Aspect | Klassieke SPC (papieren kaart) | Moderne SPC (Industry 4.0 dashboard) |
|--------|-------------------------------|---------------------------------------|
| **Meten** | Handmatig, periodiek (elke shift, elk uur) | Continu via sensoren (tot meermalen per seconde) |
| **Drager** | Papier of spreadsheet | Cloud, MES- of SCADA-dashboards |
| **Detectie** | Operator scant de kaart | Automatische alarmregels, vaak aangevuld met AI |
| **Reactietijd** | Uren tot dagen | Seconden tot minuten |
| **Datavolume** | Tientallen punten per dag | Miljoenen punten per dag |

*Bron: recente literatuur Industry 4.0 SPC; zie ko-spc-103.yaml `metadata.source_ref` voor de volledige bronverwijzing.*

---

## 🔵 Wat blijft exact hetzelfde

**Het Shewhart-principe.** Onderscheid maken tussen:
- **Common cause** — normale systeemvariatie (laat met rust)
- **Special cause** — iets ánders dan normaal (onderzoek)

Een sensor die elke seconde meet verandert *niets* aan die vraag. Sneller meten betekent niet beter beslissen.

---

## 🟣 Wat verandert in jouw rol als operator

| Vroeger (kaart) | Nu (dashboard) |
|-----------------|----------------|
| Zelf meten | Sensor meet |
| Zelf plotten | Dashboard plot |
| Zelf scannen op patronen | Regel alarmeert |
| Zelf beslissen wat "buiten grenzen" is | Grens is voor-geprogrammeerd |
| Reageren in uren | Reageren in seconden of minuten |

Wat blijft jouw werk:
- Begrijpen wát het dashboard laat zien
- Weten welke regel achter een alarm zit
- Inschatten of een alarm een echt signaal is of valse alarm
- Beslissen wanneer je ingrijpt en wanneer niet

---

## 🟠 Valkuilen bij dashboards

| Valkuil | Wat gaat er mis? | Wat helpt? |
|---------|------------------|------------|
| Alarm wegklikken zonder kijken | Je mist trends onder de alarmen | Eerst 10 seconden kijken wát er afgaat |
| Sneller reageren omdat dashboard sneller is | Je gaat tamperen (overcontrol, zie ko-spc-104) | Shewhart-denken: *is dit signaal of ruis?* |
| AI-aanbeveling blind volgen | Advies past niet altijd bij jouw context | Vraag: *waar baseert dit model zich op?* |
| Geen idee welke regel eronder zit | Je kunt het alarm niet wegen | Vraag de engineer of teamleider |

---

## 🔴 Koppeling met andere AIMM-thema's

Het KO (ko-spc-103) legt drie bruggen:

- **Predictive Maintenance** gebruikt vergelijkbare sensordata en tijdreeksen
- **AI Kwaliteitscontrole (vision)** levert defectdata die in p-, np-, c-, u-kaarten passen
- **Data Literacy** is voorwaarde om een dashboard betekenisvol te lezen

---

## 🟢 Onthoud dit

1. **Het denken verandert niet.** Signaal of ruis — dat is de vraag.
2. **De snelheid verandert wel.** Dashboards alarmeren in seconden; jij hoeft niet automatisch in seconden te handelen.
3. **Jouw rol schuift.** Van *kaart tekenen* naar *dashboard lezen en wegen*.
4. **Weet wat eronder zit.** Een alarm zonder begrip is een knop die je zonder nadenken indrukt.
5. **AI is hulpmiddel, geen orakel.** Een aanbeveling ("reset nozzle 3") is een voorstel dat jij kunt wegen.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **SPC** | Statistical Process Control — proces volgen in de tijd |
| **Shewhart-principe** | Onderscheid tussen common cause en special cause variatie |
| **Regelkaart** | Grafiek in de tijd met gemiddelde, UCL en LCL |
| **UCL / LCL** | Upper / Lower Control Limit — bovengrens en ondergrens |
| **MES** | Manufacturing Execution System — productieaansturingssysteem |
| **SCADA** | Supervisory Control and Data Acquisition — systeem voor toezicht op machines |
| **Dashboard** | Scherm met meerdere grafieken, alarmen en statussen tegelijk |
| **Sensor** | Apparaat dat automatisch meet (gewicht, temperatuur, druk, positie) |
| **Alarm / alarmregel** | Automatische melding als een meetwaarde een grens overschrijdt |
| **AI-aanbeveling** | Voorstel van een algoritme op basis van patronen in data |

---

*Bronnen: Shewhart, W.A. (1931) *Economic Control of Quality of Manufactured Product*; ISO 7870-2 voor Shewhart-regelkaarten; recente literatuur Industry 4.0 SPC (zie ko-spc-103.yaml `metadata.source_ref`). Volledige bronvermelding in het onderliggende kennisobject. | AIMM Module 1 — SPC Gebruik | v1.0*
