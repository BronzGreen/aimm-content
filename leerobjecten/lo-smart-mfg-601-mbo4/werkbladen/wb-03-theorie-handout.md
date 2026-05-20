# Handout: gelabelde data is de bottleneck — én de variatie-factor
*Kolb-fase: theoretiseren — vuistregels achter de ervaring*

**Module 1 — AI Vision Gebruik (MBO-4) | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**
> **"Het model is niet het probleem. Jouw data is het probleem."**

Je hebt nu zelf tien foto's gelabeld. Je hebt de seconden per foto gemeten. Je hebt de jaarlijkse inspectietijd op de flipover gezien. Nu de vuistregels achter wat je deed — én één extra inzicht dat de MBO-4-versie van deze sessie maakt: de **variatie-factor**. Zonder die factor wordt jouw ROI-rekensom te optimistisch.

---

## Waar gaat het over?

*Het mechanisme in vier zinnen.*

1. Een AI-camerasysteem leert alleen van **voorbeelden** met **labels**.
2. Geen voorbeelden = geen leren. Het model dat klaarstaat is gratis.
3. Wat tijd kost is iemand die jouw foto's labelt. Dat is **labelwerk**.
4. Eindresultaat: data is de **bottleneck**, niet het model.

Je kunt YOLO of een ander model in 10 minuten downloaden. Maar zonder duizenden labels van **jouw** producten leert het niets over **jouw** lijn.

---

## Drie cijfers om te onthouden

| Cijfer | Wat het betekent |
|--------|------------------|
| **150 per klasse** | Minimum aantal foto's per defect-type voor een werkbaar model — bij uniforme producten |
| **1-3 minuten** | Tijd per foto om zorgvuldig te labelen — afhankelijk van complexiteit |
| **5-20 uur** | Totale labeltijd voor 450 foto's (3 typen × 150) — range hangt af van strengheid |

*Vuistregels. In de praktijk te valideren per bedrijf.*

---

## Waarom werkt het zo?

Een AI-model leert van voorbeelden. Geen voorbeelden = geen leren. Vergelijk met een nieuwe collega op de werkvloer. Iemand die nog nooit een goede van een afgekeurde beugel heeft gezien, kan ook niet beoordelen. Pas na honderden goede én afgekeurde voorbeelden ontstaat patroonherkenning.

### Wat moet er in die voorbeelden zitten?

1. **Genoeg foto's** — honderden, niet tien.
2. **Labels die consistent zijn** — "kras" betekent elke keer hetzelfde.
3. **Variatie** — verschillende hoeken, lichtomstandigheden, productieseries.

### Wie kan dit het best?

De **operator**. Niet de IT-afdeling. Niet de leverancier. Jij ziet de defecten elke dag. Jij weet het verschil tussen een kras die ertoe doet en een glans die geen probleem is. Daarom is dit een sessie voor de werkvloer, niet voor het kantoor.

---

## De variatie-factor — nieuw voor MBO-4

*De vuistregel "150 foto's per klasse" geldt voor de eenvoudigste situatie. Echte productlijnen variëren. Hoe meer variatie, hoe meer foto's je nodig hebt.*

| Type productlijn | Foto's per klasse | Voorbeeld |
|------------------|-------------------|-----------|
| **Strakke, uniforme producten** | 150 *(basisvuistregel)* | Metalen connectoren, identieke beugels, één batch per jaar |
| **Productlijn met variatie** | 300-500 | Verschillende kleuren, batches, lichtcondities, posities |
| **Sterk wisselend assortiment** | 500+ | Veel productseries, regelmatig nieuwe defect-typen, sterke seizoenvariatie |

### Wat is "variatie" concreet?

Variatie zit in dingen die op het oog soms onschuldig lijken, maar die het model verwart:

- **Kleur** — een groene beugel ziet er voor het model anders uit dan een grijze, ook al heeft dezelfde defect-categorie
- **Belichting** — ochtendzon door het raam vs TL-licht 's avonds geeft andere pixels
- **Positie** — een product in het midden vs links onder in beeld
- **Achtergrond** — schone transportband vs band met olie- of stofresten
- **Hoek** — camera precies boven product vs onder een lichte hoek
- **Productserie** — serie A van leverancier X vs serie B van leverancier Y

> **Vuistregel voor MBO-4**: als jouw lijn meer dan twee van bovenstaande aspecten varieert, ga uit van **300 foto's per klasse**. Vier of meer aspecten: **500 of meer**.

---

## De consistentie-valstrik

*Twee labelaars leveren niet automatisch dubbele data. Soms minder bruikbare. Daar moet je op letten.*

### Wat gebeurt er bij inconsistente labels?

Stel: labelaar A noemt elk klein streepje "kras". Labelaar B noemt alleen diepe groeven "kras", en de oppervlakkige labelt hij als "goed". Wat krijgt het model?

- 1000 foto's getiteld "kras", waarvan de helft eigenlijk niets bijzonders is
- 1000 foto's getiteld "goed", waarvan de helft eigenlijk een lichte beschadiging heeft

Het model leert dan: "kras lijkt soms op niets, soms op iets". Het wordt **slechter**, niet beter. Eén consistente labelaar levert vaak meer bruikbare data dan twee ongecoördineerde.

### Hoe voorkom je dit?

| Maatregel | Wat doe je? |
|-----------|-------------|
| **Labelgids met foto's** | Voor elk label één eenduidig voorbeeld + één twijfelgeval met motivatie |
| **Kalibratie-sessie** | Eerste 50 foto's samen labelen, verschillen bespreken, gids aanvullen |
| **Steekproef-check** | Elke 100 foto's: andere labelaar reviewt 10 willekeurig — discussie bij verschil |
| **Eén eindverantwoordelijke** | Bij conflict: één persoon beslist hoe de gids wordt gebruikt |

> **MBO-4-inzicht**: hoeveelheid foto's is één variabele. Consistentie is een **tweede**, vaak onderschatte variabele. Beide tellen, niet alleen het aantal.

---

## De ROI-impact — wat doet de variatie-factor met jouw rekensom?

*Eén voorbeeld, om het concreet te maken.*

| Scenario | Foto's per klasse | Totaal foto's (3 typen) | Labeltijd bij 2 min per foto |
|----------|-------------------|-------------------------|------------------------------|
| **Uniform product** | 150 | 450 | 15 uur eenmalig |
| **Variatie middel** | 300 | 900 | 30 uur eenmalig |
| **Hoge variatie** | 500 | 1500 | 50 uur eenmalig |

Stel jouw jaarlijkse handmatige inspectie kost 200 uur. Dan is de terugverdientijd:

| Scenario | Eenmalig | Jaarlijks | Terugverdientijd |
|----------|----------|-----------|------------------|
| Uniform | 15 uur | 200 uur | ~4 weken |
| Variatie middel | 30 uur | 200 uur | ~8 weken |
| Hoge variatie | 50 uur | 200 uur | ~13 weken (3 maanden) |

Alle drie gunstig. Maar het verschil tussen 4 weken en 13 weken bepaalt of de productiemanager "ja" of "later" zegt. **Eerlijk inschatten van de variatie is dus geen detail. Het is de kern van een geloofwaardig voorstel.**

---

## Het data flywheel

*Waarom data steeds belangrijker wordt — een patroon dat zichzelf versterkt.*

```
Meer foto's gelabeld
    -> Beter model
        -> Meer vertrouwen in het systeem
            -> Systeem wordt op meer plekken ingezet
                -> Nog meer foto's verzameld
                    -> (cyclus opnieuw, sterker)
```

Dit heet een **data flywheel**. Google heeft er miljarden mee verdiend (via reCAPTCHA-puzzels waarmee bezoekers onbewust foto's labelden voor Google's modellen). In een fabriek werkt het kleiner, maar precies zo: hoe meer jullie het systeem voeden, hoe beter het wordt voor jullie product.

Strategisch voordeel zit dus in **de data**, niet in het model. Het model kun je kopen of downloaden. De data niet.

---

## De test bij elke leverancier

Als een leverancier komt met *"slimme camera's die defecten herkennen"*, stel dan deze vraag:

> *"Welke foto's zijn gebruikt om dit te trainen, en wie heeft die gelabeld?"*

Als de leverancier het niet weet, of als het antwoord is *"foto's uit een database"*, weet je genoeg. Voor jouw product, jouw defecten, jouw kwaliteitseisen — dan moet iemand labelwerk doen op **jouw** foto's. Dat staat los van de demo van de leverancier.

---

## De drie kernbegrippen — meer is niet beter

*Op MBO-4-niveau: maximaal vier nieuwe woorden per sessie. Hou je aan deze drie.*

| Begrip | Wat het betekent |
|--------|------------------|
| **Gelabelde data** | Foto's met een aanduiding wat erop staat — de echte bottleneck |
| **Data flywheel** | Patroon waarin meer data leidt tot beter model leidt tot meer data |
| **Variatie-factor** | Hoeveel meer foto's je nodig hebt naarmate je product/lijn varieert |

Andere termen die je tegenkomt — YOLO, transfer learning, F1-score, hyperparameters — kun je voor nu negeren. Cijfers werken in een ROI-gesprek beter dan jargon.

---

## Voor jouw teamleider-gesprek

*Drie zinnen die werken in een gesprek met productie-management.*

1. **"Het kernrisico is niet de techniek. Het is of we genoeg gelabelde foto's hebben voor onze productvariatie."**
2. **"Met onze variatie schat ik [300/500] foto's per defect-type — dat is [X] uur eenmalig labelwerk."**
3. **"Onze jaarlijkse handmatige inspectie is [Y] uur. De terugverdientijd op het labelwerk is dan [Z] weken — vóór hardware en licenties meetellen."**

Drie zinnen. Geen jargon. Concrete getallen. Dat is hoe een MBO-4-operator opschuift van uitvoerder naar beslissings-ondersteuner.

---

## Onthoud dit

1. **Data is de bottleneck**, niet het model. Het model is gratis.
2. **150 foto's per klasse** is een minimum — voor uniforme producten.
3. **Variatie-factor**: bij meerdere bronnen van variatie schaal je naar 300-500 foto's per klasse.
4. **Consistentie van labels** telt minstens zo zwaar als hoeveelheid.
5. **Eén goede labelaar** beats twee ongecoördineerde.
6. **Data flywheel**: hoe meer foto's, hoe beter — een zichzelf versterkend patroon.
7. **De operator labelt**, niet de IT-afdeling — jij ziet de defecten elke dag.

---

> **Wat doen we hierna?**
> Je gaat voor jouw eigen product de ROI-tabel invullen op werkblad 4. Drie getallen: labeltijd eenmalig, jaarlijkse inspectietijd, ratio terugverdientijd. Hou de variatie-factor in je achterhoofd — zonder die wordt jouw rekensom te rooskleurig. En aan het eind van dit werkblad ga je benoemen wie je de getallen voor wilt leggen op jouw werkvloer.

---

*Bron: ko-smart-mfg-601 (gelabelde data is de bottleneck); Ng, A. — Data-centric AI; Davenport & Ronanki — AI for the Real World (HBR 2018); Philips Drachten case (Rožanec et al. 2024) | AIMM Module 1 — AI Vision Gebruik (MBO-4) | v1.0*
