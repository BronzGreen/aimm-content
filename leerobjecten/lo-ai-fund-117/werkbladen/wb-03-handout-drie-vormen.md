# Werkblad 3 — Drie vormen van machine learning (handout)
*Drie vormen van machine learning — Activiteit: Theoretiseren*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 10 minuten

---

> **De kern**
> Machine learning kent drie basisvormen. Elke vorm past bij een ander type vraag. De vorm hangt af van wat voor data of feedback er beschikbaar is. **De data-vorm kan heel verschillen** — denk aan foto's tegenover een tabel — **maar het leerprincipe kan toch gelijk zijn**.

---

## De drie vormen op een rij

### Supervised learning (leren met voorbeelden waarbij iemand het juiste antwoord erbij heeft gezet)

**Wat doet het?** Het systeem leert van voorbeelden met antwoord.

**Welke data heb je nodig?** Voorbeelden waarbij een expert vooraf goed of fout heeft aangegeven. Dat heet een **label (antwoord dat een mens heeft toegevoegd)**.

**Twee toepassingen op Lijn B:**
- **InspectAI** — 4.000 foto's van zijpanelen, gelabeld door Joyce als GOED, TWIJFEL of AFGEKEURD.
- **CycleAdvise** — 4.000 rijen meetdata (temperatuur, druk, cyclustijd, uitval), gelabeld door Karim als BIJSTELLEN of NIET BIJSTELLEN.

**Vuistregel:** Heb je voorbeelden mét antwoord? Dan past deze vorm — of de data nu uit foto's of uit een tabel komt.

---

### Unsupervised learning (leren zonder dat iemand een antwoord erbij heeft gezet)

**Wat doet het?** Het systeem zoekt patronen of groepen in de data.

**Welke data heb je nodig?** Veel data, maar geen labels. Niemand heeft vooraf goed of fout aangegeven.

**Typische toepassing in de maakindustrie:** Anomaliedetectie (het opsporen van afwijkingen). Bijvoorbeeld dagen vinden waarop de **CNC-frees (Computer Numerical Control — computergestuurde freesmachine)** anders draait dan andere dagen.

**Vuistregel:** Heb je data, maar geen antwoorden? Dan past deze vorm.

---

### Reinforcement learning (leren door zelf te proberen en daarna te zien wat het oplevert)

**Wat doet het?** Het systeem probeert iets. Daarna ziet het wat er gebeurt. Het past zich aan voor de volgende keer.

**Welke data heb je nodig?** Een omgeving waarin het systeem mag uitproberen. Plus een manier om uitkomsten te meten.

**Typische toepassing in de maakindustrie:** Een lasersnijder die zelf zijn snijsnelheid aanpast. Een verpakkingsrobot die zijn grijpkracht optimaliseert.

**Vuistregel:** Kan het systeem zelf proberen en meet je het resultaat? Dan past deze vorm.

---

## Vier cases uit blok 1 — antwoorden

| Case | Vorm | Waarom? |
|------|------|---------|
| Case 1A — InspectAI met 4.000 foto's | Supervised | Joyce heeft bij elke foto het antwoord gezet. Het systeem leert van die voorbeelden. |
| Case 1B — CycleAdvise met 4.000 rijen | Supervised | Karim heeft bij elke rij het antwoord gezet. Andere data-vorm, zelfde leerprincipe. |
| Case 2 — Lasrobot zonder administratie | Unsupervised | 50.000 lasnaden, geen antwoorden. Het systeem zoekt zelf patronen — bijvoorbeeld afwijkende dagen. |
| Case 3 — Verpakkingsrobot met grijpkracht | Reinforcement | De robot probeert een instelling. Hij ziet het resultaat. Hij past zich aan. |

*Markeer met je stift wat voor jou een aha-moment is.*

---

## Het contrast tussen 1A en 1B — waarom is dit belangrijk?

InspectAI en CycleAdvise leven op dezelfde lijn. Maar de data verschilt totaal:

| | InspectAI | CycleAdvise |
|---|---|---|
| Data-vorm | Foto's | Tabel met meetwaarden |
| Wie labelt? | Joyce (kwaliteit) | Karim (onderhoud) |
| Wat doet het systeem? | Beoordeelt zijpaneel | Geeft cyclustijd-advies |
| Leerprincipe | **Supervised** | **Supervised** |

Het leerprincipe is gelijk. De data-vorm verschilt. Dat is belangrijk om te onthouden: **als bij elk voorbeeld een antwoord staat, is het supervised — wat voor data het ook is**.

---

## Welke vorm kom je vaakst tegen?

Op de werkvloer komen supervised en unsupervised het vaakst voor. Reinforcement learning is zeldzamer. Dat is een vuistregel — per bedrijf kan dit anders zijn.

---

## Vakwoorden uit deze sessie

| Vakterm | Betekenis in een zin |
|---------|---------------------|
| **ML (machine learning)** | Een systeem leert uit data. |
| **Supervised (toezicht-leren)** | Leren met voorbeelden waarbij iemand het juiste antwoord erbij heeft gezet. |
| **Unsupervised (zonder toezicht)** | Leren zonder dat iemand een antwoord erbij heeft gezet. |
| **Reinforcement (versterkings-leren)** | Leren door zelf te proberen en daarna te zien wat het oplevert. |
| **Label** | Het antwoord dat een mens vooraf bij een voorbeeld heeft gezet. |
| **Tabulaire data** | Data in een tabel, met rijen en kolommen. Bijvoorbeeld meetwaarden per cyclus. |
| **CNC-frees** | Computergestuurde freesmachine. |
| **Anomaliedetectie** | Het opsporen van afwijkingen in data. |

---

*Bron: Russell & Norvig (2010). Artificial Intelligence — A Modern Approach. Pearson.*
*AIMM x BronzGreen — Module 1: Drie vormen van ML (lo-ai-fund-117) — v2.0*
