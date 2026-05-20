# AI als aanvulling op SPC — wanneer klassieke regels tekortschieten — Draaiboek
*SPC Module 3 (Op Maat) | Workshop-blok 25 minuten | 6-10 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan voor één concrete eigen lijn beargumenteren wanneer klassieke SPC volstaat en wanneer een AI-laag meerwaarde heeft, met expliciete XAI-eis voor operator-vertrouwen, in een ingevuld eigen lijn-screen — minimaal de procesvraag, de aanpak-categorie en de XAI-eis correct geformuleerd. |
| **Doelgroep** | Teamleider HBO (primair), teamleider MBO-4 (secundair), 6-10 personen |
| **Voorkennis** | ko-spc-103 (multivariate variatie), ko-spc-601 (moderne SPC-aannames), lo-spc-104 + lo-spc-201 (stabiliteit + Nelson) doorlopen in module 1-2 |
| **Stadium (H&B)** | Bewust bekwaam — kent SPC-basis, weegt AI-claims kritisch |
| **Begeleidingsstijl** | Coachen — weinig sturing, veel ondersteuning; trainer stelt vragen vóór hij duidt |
| **Ruimte** | U-opstelling of clusters van 3-4, beamer + scherm, flip-over, ruimte voor onderling overleg |
| **Plek in module** | Eerste helft van workshop-blok 'AI + alarmrationalisatie ontwerpen' (50 min). Dit blok = 25 min (lo-spc-602) → direct gevolgd door 25 min (lo-spc-603) zonder pauze. |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:08 | Handout + tabel klassieke vs AI-aanpak | 📘 theoretiseren | 8 min |
| 00:08 - 00:17 | Eigen lijn-screen invullen + sparring in duo | 🟢 experimenteren | 9 min |
| 00:17 - 00:25 | Plenaire reflectie + transfer | 🟣 reflecteren | 8 min |

**Totaal:** 25 minuten — geen aparte pauze (komt direct na de module-pauze of na vorig blok).
**Buffer:** elk blok bevat 30-60 sec flexibele ruimte; gebruik die voor doorvragen of voor uitloop in fase 1 (handout).

---

## Voorbereiding

### De avond ervoor
- [ ] Print 3 werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 36 vellen bij 10 deelnemers.
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer. Let op: slide 4 (klassieke vraag vs AI-vraag) is de centrale slide — controleer leesbaarheid.
- [ ] Lees het antwoordmodel klassiek-vs-AI-tabel in dit draaiboek door (3 voorbeelden uit wb-01) en bedenk per voorbeeld of je een variant uit jouw eigen ervaring kunt inbrengen — alleen als die de boodschap versterkt, anders weglaten.
- [ ] Check of de doelgroeplijst klopt: zijn er deelnemers met AI-ervaring op hun lijn? Zo ja, voorbereid op de openingsvraag (zie blok 1, instructie 1).
- [ ] Bekijk lo-spc-603-draaiboek (volgende blok) om te zien wat je NIET moet behandelen vandaag (alarm fatigue, alarmsignaal-management — dat is daar).

### Het uur ervoor
- [ ] Leg per stoel: pen, wb-01-klassiek-vs-ai-tabel.
- [ ] Houd wb-02 (eigen lijn-screen) en wb-03 (reflectie) apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Schrijf op de flip-over alvast twee koppen naast elkaar: links **"Klassieke SPC vraagt: 'Is het proces NU anders dan normaal?'"**, rechts **"AI vraagt: 'Welk patroon leidt naar verstoring?'"** — dit wordt je vangrail bij blok 1 en de centrale visualisatie in blok 3.
- [ ] Open slide 1 op het scherm.
- [ ] Optioneel: leg één geprinte SHAP-screenshot uit publieke literatuur klaar — alleen ter hand-around als iemand vraagt 'hoe ziet dat er dan uit?'.

---

## Blok-details

### 📘 Blok 1: Handout + tabel klassieke vs AI-aanpak
**00:00 - 00:08** | 8 min | Kolb-fase: theoretiseren

**Doel:** Het kernonderscheid 'klassieke vraag vs AI-vraag' verankeren, drie tekortkomingen van klassieke SPC concreet maken, en de XAI-eis als voorwaarde introduceren — alles in 8 minuten, dus strak.

**Werkvorm:** Trainer-geleide handout-bespreking met centrale tabel + reactor-voorbeeld als anker.

**Instructie:**

1. **Open de sessie** (45 sec) — toon slide 1. Vraag direct: *"Wie van jullie heeft al een AI-systeem op zijn lijn? Welke vraag beantwoordt het?"* Wacht. Als iemand opsteekt: *"Even kort — welke vraag?"* Vang max 90 sec, schrijf de vraag op de flip-over rechts. Als niemand opsteekt: *"Goed — dan is dit blok geen evaluatie, maar een ontwerp-oefening. Wat zou je willen vragen aan een AI-laag op jouw lijn?"* Geen paniek, dat is de meeste setting.

2. **Trigger** (45 sec) — toon slide 2. Zeg: *"In de komende 25 minuten ontwerpen we voor jouw lijn de combinatie van klassieke SPC en AI. We gaan niet leren rekenen met SHAP. We gaan leren wanneer welke aanpak past — en waarom je AI nooit zonder uitlegbaarheid moet inzetten."*

3. **Centrale slide — klassieke vraag vs AI-vraag** (1 min 30) — toon slide 4. Lees beide vragen voor van de flip-over. Zeg: *"Dit is het hart van vandaag. Klassieke SPC vraagt 'is het proces NU anders dan normaal?' — Shewhart, Nelson. AI vraagt 'welk patroon leidt naar verstoring?' — predictive monitoring. En XAI vraagt 'welke signalen dragen het meest bij?' — SHAP, LIME. Drie verschillende vragen. Geen vervangt de andere."* Stilte van 3 sec. *"Belangrijk: Nelson-rules zijn NIET verouderd. Ze beantwoorden een ándere vraag dan AI."*

4. **Deel wb-01-klassiek-vs-ai-tabel uit** (30 sec). Zeg: *"Drie voorbeelden. Per voorbeeld: een procesvraag, en je vult zelf in: kan klassieke SPC dit beantwoorden, en zo nee, waarom niet, en wat zou een AI-aanpak toevoegen — inclusief XAI-eis."*

5. **Behandel voorbeeld 1 — chemische reactor (multivariaat)** (2 min) — toon slide 5. *"Tien sensoren op een chemische reactor. Alle individueel binnen ±3σ. Geen Nelson-regel triggert. Maar de combinatie temperatuur +1σ, druk +0,5σ, debiet -0,8σ ging in 78% van de gevallen vooraf aan katalysator-degradatie. Wie ziet wat hier de tekortkoming is van klassieke SPC?"* Wacht. Iemand zegt 'multivariaat' of 'samenhang'. *"Precies. Klassieke SPC beoordeelt elk signaal apart. Multivariate AI — kernel methods, autoencoders — leert het collectieve patroon. En dan komt XAI: SHAP zegt tegen de operator: druk 45%, temperatuur 30%, debiet 25%. Operator weet wáár te kijken. Drukvalcheck. 6-uur productiestop voorkomen."*

6. **Voorbeelden 2 en 3 — kort introduceren** (2 min) — toon slide 6 of de tabel-rand. *"Voorbeeld 2 — subtiele drift. Sensor-baseline schuift langzaam over weken. Klassieke vaste limieten missen het, of triggeren te laat. AI-toevoeging: drift-aware model. Voorbeeld 3 — korte productieserie. 50 stuks per run, 3 producten per dag. Klassieke Cpk werkt niet — onvoldoende dichtheid. AI-toevoeging: transfer learning over runs heen. Deze twee ga je zo zelf afronden in je werkblad — voorbeeld 1 was de demonstratie."*

7. **XAI als voorwaarde** (1 min) — toon slide 7. *"Eén kernregel: XAI is geen luxe, het is de voorwaarde. Stel je operator krijgt een alarm zonder uitleg. Wat doet hij? Of hij negeert het — alarm fatigue. Of hij stopt de lijn op vermoeden — duur. Zonder uitlegbaarheid ondermijn je je eigen investering. Black-box-systemen krijgen geen vertrouwen, en zonder vertrouwen geen gebruik."*

8. **Overgang naar blok 2** (15 sec) — *"Nu is het kader klaar. Tijd om het op je eigen lijn los te laten — strenge realiteitscheck inclusief."*

**Materiaal:**
- [ ] wb-01-klassiek-vs-ai-tabel.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Slides 1-7
- [ ] Flip-over met de twee vragen-koppen
- [ ] Markeerstift voor flip-over

> **💡 Tips voor de trainer:**
> - 8 minuten is krap voor handout + 3 voorbeelden + XAI. Houd het tempo. Voorbeeld 1 is je anker (gebruik volledig); voorbeelden 2 en 3 alleen aanstippen — deelnemers werken ze zo zelf uit in wb-02-koppeling.
> - Schrijf de twee centrale vragen op de flip-over voordat de sessie begint. Verwijs er voortdurend naar — het is je vangrail bij elke discussie in alle drie de blokken.
> - HBO-doelgroep wil snel naar de toepassing. Niet uitwijden over Shapley-waarden of autoencoder-architectuur — concept-niveau is genoeg.

> **🔄 Differentiatie:**
> - **Data-savvy teamleider HBO:** voeg in punt 5 of 6 een korte vraag toe: *"Wie heeft ervaring met one-class classifiers of PCA-monitoring?"* Laat hen het kort uitleggen aan de minder technische deelnemers — 2 min max, anders parkeren.
> - **Minder technische teamleider MBO-4:** sla de term 'kernel' over, gebruik alleen 'multivariate AI'. Houd de focus op 'voor welke vraag past welke aanpak'.
> - **AI-ervaring in de zaal:** vraag in opening (punt 1) door op de levende casus en gebruik die als 4e voorbeeld bij de tabel — alleen als het past bij de boodschap.

> **🔴 Valkuil — teamleider ziet AI als magisch (vk-01):**
> Bij opmerking 'AI lost dit wel op' of 'wij willen AI op onze lijn' zonder data-check: stop kort. Vraag: *"Hoeveel maanden labelled historie heb je liggen voor dit proces?"* Antwoord onduidelijk → *"Geen data, geen AI. Multivariate AI vraagt minimaal 6-12 maanden representatieve historie inclusief storingen — anders kun je het patroon niet leren."* Verwijs naar Module 1 voor data-foundation.

> **🔴 Valkuil — Nelson-rules afschaffen (vk-02):**
> Bij opmerking 'als we AI hebben, hoeven die ouderwetse regelkaarten niet meer': stop expliciet. *"Het KO is hierover ondubbelzinnig: Nelson is NIET verouderd. Klassieke SPC en AI beantwoorden verschillende vragen — beide blijven relevant."* Wijs naar de twee koppen op de flip-over. Gebruik het reactor-voorbeeld om aan te tonen dat klassiek niets miste — het beantwoordde gewoon een andere vraag.

> **🔴 Valkuil — trainer gaat te diep op SHAP/LIME (vk-05):**
> Verleidelijk om Shapley-waarden uit te leggen. Niet doen. Eén zin per term: *"SHAP geeft per signaal een bijdrage-percentage aan het alarm, LIME geeft een lokaal vereenvoudigd model rond één voorspelling."* Wie diep wil duiken: verwijs naar de Technometrics 2024 review of de SHAP-paper van Lundberg & Lee (2017).

---

### 🟢 Blok 2: Eigen lijn-screen invullen + sparring in duo
**00:08 - 00:17** | 9 min | Kolb-fase: experimenteren

**Doel:** Elke deelnemer formuleert voor één concrete lijn de procesvraag, kiest een aanpak-categorie (klassiek volstaat / klassiek + drift-aware / multivariate AI / transfer learning), en formuleert expliciet de XAI-eis. Eigenaarschap centraal — autonomie is de werkende component.

**Werkvorm:** Individueel werkblad invullen (5 min) + sparring in duo (4 min). Coaching, niet doceren.

**Instructie:**

1. **Deel wb-02-eigen-lijn-screen uit** (30 sec). Zeg: *"Kies één lijn die jij goed kent. Niet de moeilijkste — de meest representatieve. Het werkblad heeft vier secties: procesvraag, data-check, aanpak-categorie, XAI-eis."*

2. **Inventarisatie-vraag** (45 sec) — *"Even rondkijken: noem in één zin welke lijn of welk proces je kiest. Geen toelichting."* Vang 4-6 voorbeelden op (chemische dosering, vulgewicht, persdruk, lijmhechting, etc.). Niet bespreken — alleen verzamelen. Helpt deelnemers die niet weten wat ze moeten kiezen.

3. **Individueel invullen** (4 min) — zet timer op 4 min. Loop rond. Coach met deze vragen (NIET met antwoorden):
    - **Procesvraag scherp:** *"Welke vraag beantwoordt je huidige SPC nu wél? Welke vraag zou je willen kunnen beantwoorden?"*
    - **Data-check:** *"Hoeveel maanden labelled historie heb je? Hoeveel daarvan dekt storingscondities?"*
    - **Aanpak-categorie:** *"Past hier univariate uitbreiding (drift-aware kaart) of multivariate aanpak (autoencoder)? Heb je voldoende storingsvoorbeelden voor supervised, of moet het anomaliedetectie zijn?"*
    - **XAI-eis:** *"Hoe ga je je operator uitleggen waarom een alarm afgaat? Wat doet hij als er geen uitleg bij staat?"*
    Stel vooral de vragen — laat de teamleider zelf antwoorden vinden. HBO-stadium = bewust bekwaam = sparring, geen instructie.

4. **Sparring in duo** (3 min 30) — *"Zoek een buurpersoon. Wissel werkbladen. Stel je duo-partner één scherpe vraag bij zijn ingevulde screen — bij voorkeur over de aanpak-keuze of de XAI-eis. Twee keer 1 min 30, ik geef een belletje."* Loop rond, luister mee. Tussentijds belletje na 1 min 30 voor wisseling.

5. **Verzamel-moment** (15 sec) — *"Pen neer. Wie heeft een vraag waar zijn duo-partner geen goed antwoord op had? Onthoud die — die nemen we mee naar blok 3."*

**Materiaal:**
- [ ] wb-02-eigen-lijn-screen.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Timer / mobiel met geluid
- [ ] Flip-over met de twee centrale vragen (zichtbaar)

> **💡 Tips voor de trainer:**
> - Stel vragen, geef geen antwoorden. Bij blokkade: *"Welke vraag beantwoordt je huidige SPC nu wél?"* — dat ontgrendelt bijna altijd.
> - Loop niet over schouders — buig niet over werkbladen heen. Dat verhoogt prestatiedruk; HBO-doelgroep schrijft eerlijker als je op afstand blijft.
> - Bevestig dat 'ik weet de data-status nog niet' een geldig antwoord is — sterker nog: vaak is dát de eerste actie die uit het werkblad komt.
> - 'XAI-eis' is voor sommigen abstract. Help met: *"Schrijf één zin op die je tegen je operator zou zeggen om uit te leggen waarom de AI alarm sloeg."* Concreter dan dat hoeft niet.

> **🔄 Differentiatie:**
> - **Data-savvy teamleider HBO:** voeg vraag toe over modelfamilie (supervised classifier vs autoencoder vs drift-aware) en verwijs naar Technometrics 2024 review.
> - **Minder technische teamleider MBO-4:** koppel als duo-partner aan een data-savvy teamleider. De minder technische levert procesvragen, de andere de aanpak-categorie.
> - **Geen AI op de lijn nu:** *"Ontwerp dit voor een toekomstige situatie. Wat zou je willen kunnen vragen, en wat zou je leverancier moeten leveren — inclusief XAI?"*

> **🔴 Valkuil — teamleider wil multivariate AI zonder voldoende historie (vk-04):**
> Bij iemand die 'we starten volgende maand' noteert zonder historie-check: coach in plaats van corrigeer. *"Welke historie heb je nu beschikbaar? Hoeveel daarvan dekt ook storingscondities? Wat is je sensor-drift-cyclus?"* Laat hem zelf concluderen dat starten zonder fundament niet werkt. Vuistregel: 6-12 maanden representatieve historie inclusief storingen.

> **🔴 Valkuil — trainer doceert in plaats van coacht (vk-06):**
> Vooral voor HBO-doelgroep dodelijk. Adem in. Stel een vraag. Wacht. *"Welke vraag beantwoordt jouw huidige SPC nu wél?"* Stem zelf nooit mee. Tel innerlijk tot 7 bij stilte. HBO-doelgroep komt niet voor instructie, zij komt voor sparring.

---

### 🟣 Blok 3: Plenaire reflectie + transfer
**00:17 - 00:25** | 8 min | Kolb-fase: reflecteren

**Doel:** De groep deelt 2-3 cases plenair, kernonderscheid wordt versterkt door herkenning ('dit speelt bij ons ook'), en elke deelnemer formuleert één concrete transfer-actie voor de komende 2 weken.

**Werkvorm:** Plenaire bespreking 2-3 cases + reflectie-werkblad invullen + transferopdracht.

**Instructie:**

1. **Deel wb-03-reflectie uit** (15 sec). Zeg: *"Tijdens de bespreking vul je hier in: welke vraag wil je voor jouw lijn beantwoord krijgen, en welke aanpak past daarbij — klassiek, AI of beide. En één concrete actie voor de komende twee weken."*

2. **Plenaire deel-ronde — 2 cases** (5 min) — *"Wie wil zijn eigen lijn-screen plenair bespreken? Vrijwilliger eerst — geen aanwijzen."* Vang 2 cases. Per case max 2 min. Laat de teamleider:
    - In één zin de procesvraag vertellen.
    - Aangeven welke aanpak hij heeft gekozen.
    - Aangeven welke XAI-eis hij heeft geformuleerd.
    Coach met vraag aan de groep: *"Wie zou hier iets anders aanpakken? Waarom?"* Maximaal 1 reactie per case. Zelf alleen duiden bij verwarring tussen klassiek en AI, of bij ontbrekende XAI.

3. **Centrale terugkoppeling** (1 min 30) — wijs naar de flip-over met de twee vragen. Zeg: *"Wat we vandaag hebben gedaan — niet kiezen tussen klassiek of AI, maar weten welke vraag je beantwoordt en welke aanpak daarbij past. En XAI is geen optie. Eén voorbeeld dat we hebben gezien — de chemische reactor — maakt zichtbaar wat klassieke SPC niet ziet en wat multivariate AI mét XAI wel kan. De Nelson-routine van je operators verandert NIET. Wel verandert hun rol: van detector naar interpreteerder. Daar moet je hen op voorbereiden."*

4. **Implicatie operator-rol** (45 sec) — toon slide 11. *"Operator-rol verandert: van regelvolger naar systeem-bewaker. Data Literacy is voorwaarde. Wie traint dat bij jou — eigen lijn of via Module 1? Onthoud: AI vervangt operators niet, het verandert hun rol."*

5. **Transferopdracht** (45 sec) — toon slide 12. *"Deze twee weken: voer één concrete actie uit op je eigen lijn-screen. Drie opties — kies één:*
    - *Doe een data-check: hoeveel labelled historie heb je echt, hoeveel dekt storingen?*
    - *Voer een gesprek met je operators: wat zouden zij willen kunnen vragen aan een AI-laag — en hoe zouden ze willen dat het wordt uitgelegd?*
    - *Beoordeel een leverancier-pitch (huidige of vorige): vroeg die om XAI? Zo nee, wat ontbrak?*
    *Schrijf je actie in één zin op je werkblad. Volgende sessie bespreken we de uitkomsten."*

6. **Overgang naar lo-spc-603** (15 sec) — *"Alarmen zijn nu het thema. We gaan zo door met alarmrationalisatie — wat moet er met al die alarmen gebeuren als ze afgaan?"*

**Materiaal:**
- [ ] wb-03-reflectie.md (1 per deelnemer + 2 reserve)
- [ ] Pen per deelnemer
- [ ] Slides 9-12
- [ ] Flip-over met centrale vragen (zichtbaar)
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Niet aanwijzen voor de plenaire deel-ronde. Vraag vrijwilligers. HBO-doelgroep deelt zelf als de veiligheid er is — dwingen verbreekt die.
> - Bewaak je tijd strak: 8 minuten gaat sneller dan je denkt. Als case 1 uitloopt, kort case 2 in tot 90 sec.
> - De flip-over met de twee centrale vragen is je belangrijkste anker bij de terugkoppeling. Verwijs er expliciet naar — herhaling versterkt verankering.
> - Bevestig het 'transfer-doe-het-in-twee-weken' karakter. Zonder deadline geen actie.

> **🔄 Differentiatie:**
> - **Data-savvy teamleider HBO:** vraag in deel-ronde naar de modelfamilie-keuze (waarom autoencoder en niet supervised?). Operators registeren niet, andere HBO-teamleiders herkennen wel.
> - **Minder technische teamleider MBO-4:** in transferopdracht zwaartepunt op gesprek met operators (optie 2) — daar zijn ze sterk in. Optie 3 (leverancier-pitch) is HBO-territorium.
> - **Gemengde groep:** kies bewust 1 case van een MBO-4 teamleider en 1 van een HBO-teamleider voor plenaire bespreking.

> **🔴 Valkuil — teamleider slaat XAI over (vk-03):**
> Bij iemand die in zijn case geen XAI-eis noemt: stop kort. *"Stel je operator krijgt een alarm zonder uitleg. Wat doet hij? Of hij negeert het — alarm fatigue. Of hij stopt de lijn op vermoeden — duur. XAI is geen luxe."* Verwijs naar het reactor-voorbeeld: SHAP gaf 'druk 45%, temperatuur 30%, debiet 25%' — operator wist wáár te kijken.

> **🔴 Valkuil — verwarring met alarmrationalisatie (vk-07):**
> Een teamleider stelt vragen over alarm fatigue, alarm-prioritering of alarmsignaal-management — onderwerpen van het volgende blok. Park het: *"Goede vraag — alarmrationalisatie is precies wat we hierna behandelen. Schrijf je vraag op, we komen er over enkele minuten op terug."* Houd dit blok zuiver bij wanneer-welke-aanpak en XAI.

> **🔴 Valkuil — geen tijd voor de transferopdracht:**
> Als blok 3 dreigt uit te lopen (deel-ronde te lang): kort case 2 in en sla de implicatie-slide (instructie 4) over — die staat ook in slide 11 zelfstandig leesbaar. Sla de transferopdracht NOOIT over — dat is wat de workshop verbindt met de werkvloer.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-klassiek-vs-ai-tabel.md | n + 2 | A4 dubbelzijdig — handout met 3 voorbeelden + lege invul-kolommen |
| ☐ | wb-02-eigen-lijn-screen.md | n + 2 | A4 enkelzijdig — 4 secties: procesvraag, data-check, aanpak, XAI-eis |
| ☐ | wb-03-reflectie.md | n + 2 | A4 enkelzijdig — terugblik + transferopdracht |
| ☐ | Pennen | n + 5 | Reserve op trainer-tafel |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Flip-over + dikke stiften | 1 set | Voor de twee centrale vragen-koppen (klassiek vs AI) |
| ☐ | Timer / mobiel met geluid | 1 | Voor 4-min individueel + 3 min 30 sparring |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 4 (centrale onderscheid) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |
| ☐ | SHAP-screenshot uit publieke literatuur | 1 (optioneel) | Alleen ter hand-around als iemand vraagt 'hoe ziet dat eruit?' |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel klassiek-vs-AI-tabel

| Voorbeeld | Klassieke aanpak | Klassiek zwak omdat | AI-toevoeging | XAI-eis |
|-----------|------------------|---------------------|---------------|---------|
| 1. Chemische reactor (10 sensoren, multivariaat patroon) | Shewhart per sensor + Nelson | Univariate aannames; multivariate samenhang onzichtbaar | Autoencoder of one-class classifier op gecombineerde sensorvector | SHAP per alarm: 'druk 45%, temperatuur 30%, debiet 25%' |
| 2. Subtiele drift over weken | Vaste limieten of Nelson-rule 5 | Aanname stabiele baseline; niet drift-aware | Drift-aware model (online learning of adaptieve CUSUM) | Trend-attributie: 'baseline schuift 0,15σ/week op signaal X — sensor-recalibratie' |
| 3. Korte productieserie (50 stuks/run, high-mix-low-volume) | Per-run Cpk onbetrouwbaar; aggregatie vermengt processen | Aanname stabiele lange-run-context | Transfer learning of meta-modellen over runs | Per-product attributie: 'voor product X spreiding-issue, voor product Y centrering' |

**Slagingscriterium:** wb-02 ingevuld met minimaal procesvraag + aanpak-categorie + XAI-eis correct geformuleerd = leerdoel behaald (ABCD-degree). Voorbeeld 1 is de toetssteen voor het multivariate inzicht.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Vraag-statistiek genoteerd (welke aanpak-categorieën kozen deelnemers het vaakst?)
- [ ] Centrale vragen-flip-over gefotografeerd
- [ ] Notitie voor volgende workshop: welke lijnen hebben deelnemers gekozen voor de eigen-lijn-screen?
- [ ] xAPI-statements verstuurd: `experienced` (klassiek-vs-AI-tabel), `completed` (eigen lijn-screen + reflectie)
- [ ] Warm overdragen naar lo-spc-603 (alarmrationalisatie) — geen pauze, directe doorloop
- [ ] Bij data-savvy teamleider: korte handover naar Module 3 (Op Maat) — werkbladen voor verdiepingsstap

---

*AIMM Curriculum | SPC Module 3 (Op Maat) | AI als aanvulling op SPC — wanneer klassieke regels tekortschieten*
*Bronnen: Recente review AI in process monitoring, Technometrics (2023-2024) | Lundberg & Lee (2017) SHAP | Ribeiro, Singh & Guestrin (2016) LIME | NIST/SEMATECH e-Handbook | Wheeler, D.J. (2010) Quality Digest*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
