# Handout: Vijf sensor-typen, drie trade-offs, drie fouten
*Kolb fase 3 — Theoretiseren | Sensor-keuze voor een digital twin*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | Industry 4.0**

---

> **Over deze handout**
> Dit is jouw referentiekaart. Geen invulvelden, wel jouw markeerstift erbij. Je leest mee, markeert wat opvalt en gebruikt deze kaart straks voor werkblad 4. Samen ontdekken we hoe je van vraag naar sensor komt — niet andersom.

---

## Begin bij de vraag, niet bij de sensor

*De grootste valkuil is een sensor kiezen voordat de vraag helder is. Dat geeft veel data en weinig antwoord (sensor-overdaad).*

**Goede volgorde:**

1. Welke vraag wil de digital twin (digitale tweeling) beantwoorden?
2. Welk type signaal hoort bij die vraag (trilling, hitte, geluid, beeld of druk)?
3. Welke trade-off weegt voor jouw werkvloer het zwaarst?
4. Welke fout wil je beslist vermijden?

---

## De vijf sensor-typen

*Vijf typen kom je op de werkvloer bijna overal tegen. Elk type past bij een eigen soort vraag. De richtprijzen zijn ordegrootte — vraag jouw leverancier altijd om een actuele offerte.*

| Sensor-type | Wat meet de sensor? | Typische werkvloer-vraag | Richtprijs per sensor |
|---|---|---|---|
| **Trilling** | Vibratie in lagers, motoren, ventilatoren | Welk onderdeel gaat binnenkort kapot? | €100 – €500 |
| **Temperatuur** | Hitte van een component of ruimte | Loopt deze motor te warm? | €20 – €100 |
| **Akoestiek** | Geluidpatronen (met AI-model erachter) | Klopt er iets niet met het geluid? | €500 – €2000 |
| **Beeld** | Foto of video met AI-model | Is het product afgekeurd en waarom? | €2000 – €20.000 |
| **Druk** | Druk in lucht-, hydrauliek- of vloeistof-systemen | Lekt er ergens druk weg? | €50 – €500 |

> **Bron:** Soldatos (2024) hoofdstuk 6; Bakopoulos et al. (2024) hoofdstuk 4; Anaya et al. (2024).

---

## De drie trade-offs

*Bij elke sensor-keuze wegen deze drie dingen tegen elkaar. Er is geen sensor die op alle drie het beste scoort. Kiezen betekent: één of twee laten zwaarder wegen.*

### 1. Kosten

Niet alleen de aanschaf telt mee. Ook de installatie, de bekabeling, een edge-buffer (klein tussenstation dichtbij de sensor) en het onderhoud. Een sensor van €100 met een installatie van €10.000 is nog steeds een dure sensor.

### 2. Accuratesse

Hoe fijn kan de sensor meten? Sommige trilling-sensoren meten op micrometer-niveau (één duizendste van een millimeter). Andere meten alleen op millimeter-niveau. Hoe nauwkeuriger, hoe duurder. Past de accuratesse niet bij de vraag, dan koop je te veel of te weinig.

### 3. Levensduur

In stoffige, hete of vochtige omgevingen leven sommige sensoren maar zes maanden. In milde omgevingen halen ze tien jaar. Vervangings-kosten en stilstand voor vervanging tellen op. Vraag aan de leverancier wat de levensduur is in jouw type omgeving.

---

## De vraag-driven aanpak

*Eerst de vraag, dan pas de sensor. Vier voorbeelden:*

| Werkvloer-vraag | Past bij dit signaal | Past bij dit sensor-type |
|---|---|---|
| Welk lager gaat binnenkort falen? | Vibratie | Trilling |
| Loopt deze motor te warm? | Hitte | Temperatuur |
| Waarom is dit product afgekeurd? | Beeld | Beeld |
| Lekt er ergens perslucht weg? | Druk-verlies | Druk |

> **Voorbeeld uit de praktijk:** Een fietsfabriek wil weten welke lagers in de lakstraat binnenkort falen. Twaalf trilling-sensoren van €200 plus installatie. Drie ongeplande stilstanden per jaar à €4000 verlies. De investering is in jaar 2 terugverdiend.

---

## De drie veelgemaakte fouten

*In de praktijk gaat het vooral op deze drie punten mis.*

### Fout 1 — Te veel sensoren plaatsen "voor de zekerheid"

Veel sensoren geven veel data, maar weinig antwoord. Beter: klein beginnen bij één vraag, dan uitbreiden als die werkt.

### Fout 2 — Te goedkope sensor kiezen

Een temperatuur-sensor van €20 die elke drie maanden moet worden vervangen, kost over vijf jaar meer dan een geïntegreerde sensor van €100 die vijf jaar meegaat. Reken altijd de totale kosten over de hele looptijd.

### Fout 3 — Sensor-onderhoud vergeten

Vuile of niet-geijkte sensoren (ijken = opnieuw afstellen op een bekende referentie) geven foute data. Plan vervangen en ijken direct in vanaf dag één.

---

## Snelkaart — Welke sensor bij welke vraag?

| Hoor je deze vraag op de werkvloer? | Denk eerst aan: | Let op deze fout: |
|---|---|---|
| "Wat trilt er raar?" | Trilling-sensor | Fout 1 (te veel) |
| "Wat loopt te warm?" | Temperatuur-sensor | Fout 2 (te goedkoop) |
| "Wat klinkt anders?" | Akoestiek-sensor | Fout 3 (geen onderhoud) |
| "Waarom is dit afgekeurd?" | Beeld-sensor | Fout 1 (te veel) |
| "Waar lekt het?" | Druk-sensor | Fout 3 (geen onderhoud) |

> **Onthoud:** De beste sensor is degene die past bij jouw vraag, jouw omgeving en jouw budget. Niet de duurste, niet de goedkoopste. Samen met je collega en je leverancier kies je de juiste.

---
*Bron: Soldatos (2024). Artificial Intelligence in Manufacturing, hoofdstuk 6; Bakopoulos et al. (2024). Digital-Twin-Enabled Framework, hoofdstuk 4; Anaya et al. (2024). A Manufacturing Digital Twin Framework | AIMM Industry 4.0 Module 2 | v1.0*
