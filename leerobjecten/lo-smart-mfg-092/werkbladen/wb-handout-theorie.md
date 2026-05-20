# Werkblad 3: Theorie-handout — Drie Soorten Anomalieen

**Leerobject:** Anomaliedetectie in de productie
**Fase:** Theoretiseren
**Duur:** 8 minuten

---

## Wat is anomaliedetectie?

Anomaliedetectie (het opsporen van afwijkingen) werkt automatisch. Een AI-systeem leert wat "normaal" is. Het slaat alarm bij iets ongewoons.

---

## Drie soorten anomalieen

### 1. Puntanomalie

**Wat is het?** Een enkel meetpunt dat afwijkt van normaal.

**Voorbeeld:** De temperatuur van een motor is 82 graden. Normaal is 65-70 graden.

**Hoe herken je het?** De waarde valt buiten de normale bandbreedte.

**In de oefening was dit:** voorbeeld 1 (trillingsniveau).

---

### 2. Contextuele anomalie

**Wat is het?** Een waarde die normaal is in de ene situatie, maar afwijkend in een andere.

**Voorbeeld:** Een druk van 4,2 bar is normaal bij opstart, maar afwijkend tijdens productie.

**Hoe herken je het?** Je moet weten WAT de machine op dat moment doet.

**In de oefening was dit:** voorbeeld 2 (energieverbruik bij zwaarder product).

---

### 3. Collectieve anomalie

**Wat is het?** Een reeks metingen die samen een afwijkend patroon laten zien.

**Voorbeeld:** Temperatuur: 68, 69, 70, 72, 74, 77, 80. Elke waarde apart is niet alarmerend. Maar het patroon stijgt.

**Hoe herken je het?** Kijk niet naar een enkel getal, maar naar de TREND.

**In de oefening was dit:** voorbeeld 3 (stijgende temperatuurreeks).

---

## Hoe werkt anomaliedetectie?

| Stap | Wat gebeurt er? | Voorbeeld |
|------|----------------|-----------|
| 1. Voorbereiding | Data wordt verzameld | Sensoren meten temperatuur, druk, trillingen |
| 2. Training | Het AI-model leert wat normaal is | 3 maanden data van een goed draaiende machine |
| 3. Detectie | Het model vergelijkt nieuwe data met normaal | "Let op: trillingsniveau is 2x hoger dan normaal" |

---

## Praktijkvoorbeeld

Bij een fabrikant van brandstoftanks bewaakt een AI-systeem meer dan 100 sensorwaarden. De sensoren meten temperatuur, druk, positie en energieverbruik. Bij een afwijkend patroon krijg je direct een melding op het scherm.

---

## Noteer voor jezelf

**Welk type anomalie komt het meest voor op jouw werkvloer?**

_________________________________________________

**Worden er op jouw afdeling al sensorwaarden gemeten?**

[ ] Ja, namelijk: _________________________________

[ ] Nee

[ ] Weet ik niet

---

*Bewaar deze handout. Je hebt hem nodig bij de volgende oefening en op je werkvloer.*
