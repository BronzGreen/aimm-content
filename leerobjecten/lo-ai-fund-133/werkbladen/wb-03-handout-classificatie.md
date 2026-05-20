# Werkblad 3 — Twee smaken classificatie

*Handout — Kolb fase 3 (theoretiseren)*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 10 minuten

---

## Over dit werkblad

Dit is een handout. Je leest mee met de trainer. Je markeert met je stift wat voor jou een aha-moment is.

In de eerste twee werkbladen heb je twee soorten systemen gezien. Een binair systeem op een CNC-onderdeel. Een multi-class systeem met vier foto's. Hier zetten we de theorie op een rij.

---

## Wat is classificatie?

**Classificatie** is een AI-taak. Het model plakt een **etiket** op een voorbeeld. Dat etiket heet de **klasse**. De output is een klasse. Geen getal.

Een voorbeeld: je geeft een foto aan het model. Het model geeft terug "goed" of "afgekeurd". Dat etiket is de output.

---

## Twee smaken: binair en multi-class

### Binair (twee opties)

Het model kiest uit precies twee categorieën. Voorbeelden uit de praktijk:

- **goed** of **afgekeurd** — bij eindcontrole van producten.
- **OK** of **NOK** — bij dashboard-meldingen op de werkvloer.
- **storing** of **geen storing** — bij sensorbewaking van een machine.
- **aanwezig** of **afwezig** — bij telling van pakketten op een sorteerlijn.

### Multi-class (meer dan twee opties)

Het model kiest uit drie of meer categorieën. Voorbeelden uit de praktijk:

- **kras, barst, kleurfout, vormafwijking** — bij visuele controle.
- **storing motor, storing klep, storing sensor, storing software** — bij storingsmeldingen.
- **klasse A, klasse B, klasse C** — bij sorteren naar kwaliteit.
- **regulier, prioriteit, koel, fragiel** — bij sorteren van pakketten.

---

## Wat betekent de zekerheid?

Bij elke klasse staat een percentage. Dat heet de **zekerheid** van het model. Hoog percentage betekent: het model is heel zeker.

> **Let op — veelgemaakte denkfout.**
> "78% zekerheid kras" betekent niet "78% van het product is een kras".
> Het betekent: het model is voor 78% zeker dat dit een kras is.

Het is dus een uitspraak over het model, niet over het product. Maakt verschil!

---

## Vier voorbeeldsignalen

Stel je bent operator op de werkvloer. Het dashboard geeft deze meldingen:

| Onderdeel | Klasse | Zekerheid | Wat denk je? |
|---|---|---|---|
| Plaatje 1 | goed | 96% | Hoog — gewoon doorlaten. |
| Plaatje 2 | barst | 88% | Hoog — afkeuren is logisch. |
| Plaatje 3 | kras | 71% | Midden — twijfel mogelijk. |
| Plaatje 4 | kleurfout | 52% | Laag — nakijken nodig. |

Een hoge zekerheid (>90%) volg je doorgaans. Een lage zekerheid (60% of minder) is een twijfelgeval. Daar komt jouw vakkennis kijken.

---

## Verschil met regressie

Classificatie geeft een **etiket**. Regressie geeft een **getal**.

| Type | Output | Voorbeeld werkvloer |
|---|---|---|
| **Classificatie** | Een klasse, een etiket | "Klasse: braam" |
| **Regressie** | Een getal | "Voorspelde uitval: 3 dagen" |

Regressie komt in een ander leerobject. Onthoud nu: classificatie = etiket. Geen getal.

Een **voorspeller** voor onderhoudsmomenten is regressie. Een **classifier** voor goed of afkeur is classificatie. De camera boven de band die "goed" zegt? Dat is een classifier.

---

## Mijn samenvatting

*Vul aan in eigen woorden. Een halve zin per regel is genoeg.*

**Wat geeft een classificatiemodel terug?**

________________________________________________________________

________________________________________________________________

**Wat is het verschil tussen binair en multi-class?**

________________________________________________________________

**Wat betekent 78% zekerheid?**

________________________________________________________________

**Wat is het verschil tussen classificatie en regressie?**

________________________________________________________________

---

## Vakwoorden in dit leerobject

| Vakterm | Betekenis in een zin |
|---|---|
| **Classificatie** | AI plakt een etiket op een voorbeeld. |
| **Klasse** | Een categorie waar het etiket bij hoort. |
| **Etiket (label)** | De naam van de klasse die het model geeft. |
| **Binair** | Twee mogelijke klassen, bijvoorbeeld goed of fout. |
| **Multi-class** | Drie of meer mogelijke klassen. |
| **Zekerheid** | Hoe zeker het model is over zijn keuze. |
| **Regressie** | Alternatief: model voorspelt een getal, geen etiket. |
| **Classifier** | Een model dat classificatie doet. |
| **Trainingsdata** | De voorbeelden waarmee het model leert. |

---

## Wat doen we hierna?

In het laatste werkblad krijg je een twijfelgeval. Het model zegt "goed 60%" en tegelijk "vormafwijking 40%". Jij beslist wat je daarmee doet. Hier komt jouw vakkennis aan zet.

---

## Bron

Soldatos, J. (2024). *Artificial Intelligence in Manufacturing*. Springer. Praktijkvoorbeeld CNC-controle bij metaalbewerking.

---

*AIMM x BronzGreen — AI Fundamentals · Module 1 · Classificatie (lo-ai-fund-133)*
