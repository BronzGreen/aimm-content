# CNC-frees casus — I-MR kaart en gereedschapsslijtage detecteren — Draaiboek
*SPC Module 2 (Train) | Workshop-blok 45 minuten | 6-10 deelnemers*

> 📋 DRAAIBOEK — VERTROUWELIJK

**Datum:** _______________  **Trainer:** _______________
**Locatie:** _______________  **Deelnemers:** ___ personen

---

## Sessie-informatie

| | |
|---|---|
| **Leerdoel** | Deelnemer kan een I-MR-regelkaart opzetten voor een eigen kritische maat (meetfrequentie, UCL/LCL en MR-limiet) en herkent een trend (Nelson-regel 3) als vroeg signaal dat tooling-actie nodig is — vóórdat een punt buiten de control limits valt. Degree: minimaal 2 van de 3 oefenreeksen correct geduid én op wb-03 een eigen kritische maat genoteerd met I-MR/X̄-R-motivering. |
| **Doelgroep** | Operators MBO-3/MBO-4 (primair), teamleiders MBO-4 (secundair), 6-10 personen |
| **Voorkennis** | ko-spc-108 (basis regelkaarten) en ko-spc-201 (Nelson-regels overzicht) doorlopen. Deelnemer kent 'punt buiten UCL' (regel 1) maar herkent trends (regel 3) vaak niet. |
| **Stadium (H&B)** | Bewust onbekwaam — weet dát er regelkaarten bestaan, heeft zelden zelf een kaart moeten inrichten. Herkent regel 1 wel, regel 3 vaak niet. De trend-oefening activeert die ervaren onbekwaamheid als leerbrandstof ('alles binnen de grenzen, waarom stop ik dan?'). |
| **Begeleidingsstijl** | Trainen — veel sturing én veel ondersteuning. Scaffolding via IK DOE → WIJ DOEN → JIJ DOET: trainer leest eerst één reeks voor (hardop denken), deelnemers doen daarna zelf de CNC-casus + extra oefenreeksen, reflecteren plenair, krijgen pas daarna de theorie. |
| **Ruimte** | U-opstelling of clusters van 4, beamer + scherm, flip-over, ruimte om rond te lopen |
| **Plek in module** | Workshop-blok binnen module 2 (Train) — SPC regelkaarten deel 2: na Cp/Cpk-workshop (lo-spc-301), vóór groepsreflectie configuratiebesluit |

---

## Sessie-overzicht

| Tijd | Activiteit | Type | Duur |
|------|-----------|------|------|
| 00:00 - 00:15 | Trend-oefening: lees drie I-MR-reeksen | 🟢 ervaren | 15 min |
| 00:15 - 00:27 | STARRT-reflectie op Reeks A + plenaire duiding | 🟣 reflecteren | 12 min |
| 00:27 - 00:45 | Handout: I-MR configureren + Nelson-regel 3 + eigen-lijn-actieplan | 📘 theoretiseren (+ transfer geïntegreerd) | 18 min |

**Totaal:** 45 minuten — geen aparte pauze.
**Buffer:** elk blok bevat 1-2 minuten flexibele ruimte; gebruik die voor doorvragen of voor uitloop in fase 2 (plenaire duiding).

---

## Voorbereiding

### De avond ervoor
- [ ] Print drie werkbladen × (aantal deelnemers + 2 reserve) — totaal ca. 36 vellen bij 10 deelnemers.
- [ ] Print `diagram-lo-spc-501.svg` op A3 (in kleur indien mogelijk — drie reeksen naast elkaar met trend-annotatie).
- [ ] Open de presentatie (`presentatie.slidev.md`) op je laptop en test met de beamer.
- [ ] Lees de drie meetreeksen in wb-01 door en kies welke korte voorbeeld-reeks je voor IK DOE hardop voordoet (geen van de drie uit wb-01 — gebruik een aparte 8-puntsreeks op de flip-over).
- [ ] Check of de doelgroeplijst klopt: zijn er teamleiders bij? Zo ja, voorbereid op extra vragen over escalatie en documentatie-eisen.

### Het uur ervoor
- [ ] Leg per stoel: pen, liniaal, wb-01-oefening.
- [ ] Houd wb-02 en wb-03 apart op de trainer-tafel — uitdelen pas op het moment in de sessie.
- [ ] Hang de A3-versie van het diagram zichtbaar achter in de zaal (nog afdekken — pas onthullen in blok 3).
- [ ] Teken op de flip-over alvast een lege I-chart (horizontale as uren, verticale as mm) met gestippelde UCL en LCL — dit wordt je canvas voor IK DOE.
- [ ] Open slide 1 op het scherm.

---

## Blok-details

### 🟢 Blok 1: Trend-oefening — drie I-MR-reeksen lezen
**00:00 - 00:15** | 15 min | Kolb-fase: ervaren

**Doel:** De deelnemer ervaart dat een stijgende reeks binnen de control limits een echt signaal is — niet pas 'punt buiten UCL'. Verwarring ('hoezo stoppen, alles ligt toch binnen de grenzen?') wordt geactiveerd als leerbrandstof voor de I-MR-theorie in blok 3.

**Werkvorm:** IK DOE (trainer leest één voorbeeldreeks voor, hardop denkend) → JIJ DOET (deelnemers lezen zelf drie reeksen op wb-01, markeren per reeks hun inschatting + Nelson-regel + eerste actie).

**Instructie:**

1. **Open de sessie** (30 sec) — toon slide 1. Zeg: *"Op jouw lijn draai je een serie van 2000 stuks. Elk punt dat jij meet ligt netjes binnen de control limits. En tóch zitten er na 40 uur 200 stuks in de uitval-bak. Hoe kan dat?"* Wacht. Laat 1-2 mensen hardop speculeren. Geen lange verhalen.

2. **Trigger** (1 min) — *"Vandaag leer je één regel waarmee je dát scenario voorkomt: Nelson-regel 3, de trend. Zes punten achter elkaar omhoog of omlaag — ook als ze binnen de grenzen blijven — is al een signaal. We beginnen niet met theorie. We beginnen met kijken."*

3. **IK DOE** (3 min) — toon slide 2. Wijs naar de lege I-chart op de flip-over. Plot acht punten snel met de hand (kruisjes): 10,002 – 10,003 – 10,001 – 10,003 – 10,004 – 10,005 – 10,006 – 10,007 (binnen UCL ≈ 10,010 en LCL ≈ 9,990). Denk hardop: *"Geen punt buiten de grenzen. Maar ik zie zes punten achter elkaar omhoog kruipen — vanaf punt 3 tot punt 8. Dat is een trend. Nelson-regel 3. Eerste actie: ik stop niet meteen het gereedschap vervangen, ik ga eerst het gereedschap meten. Misschien is het slijtage, misschien iets anders. Meten is de eerste stap."* Stilte van 3 sec.

4. **Deel wb-01-oefening uit** (30 sec). Zeg: *"Drie reeksen. Reeks A is de CNC-frees casus uit ko-spc-501 — de echte casus. Reeks B en C zijn oefenreeksen. Voor elke reeks: zie je een signaal? Welke Nelson-regel? Wat zou je als eerste doen? Per reeks één inschatting, één regel, één actie. Bij twijfel: vraagteken. Geen theorie nodig — alleen kijken."*

5. **JIJ DOET** (9 min) — zet timer op 9 min. Loop rustig rond. Beantwoord praktische vragen (*"wat betekent UCL ook alweer?"*) maar GEEN inhoudelijke (*"is mijn antwoord goed?"*) — verwijs door: *"Dat bespreken we zo plenair — schrijf op wat jij denkt, ook als je twijfelt."*

6. **Verzamel-moment** (1 min) — *"Pen neer. Even een handopsteking per reeks: wie zag een signaal in Reeks A? En in Reeks B? En in Reeks C?"* Tel hardop, schrijf de scores op de flip-over naast de drie reeksletters. Dit is je input voor blok 2.

**Materiaal:**
- [ ] wb-01-oefening.md (1 per deelnemer + 2 reserve)
- [ ] Pen + liniaal per deelnemer
- [ ] Slide 1 (cover) en slide 2 (IK DOE)
- [ ] Flip-over met lege I-chart voor IK DOE
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Loop tijdens de oefening langs maar buig je niet over schouders — dat verhoogt prestatiedruk en maakt twijfel onzichtbaar.
> - Als iemand na 5 minuten klaar is: vraag *"Heb je bij Reeks A écht gekeken naar de volgorde, of alleen naar of iets boven UCL uitkomt?"* De volgorde-kijken is de centrale competentie.
> - Reeks A (de echte casus) is het leermoment: 6 stijgende punten, nog net binnen UCL. Reeks B is een ruisachtige reeks zonder patroon (goed antwoord: geen signaal). Reeks C bevat een punt boven UCL (regel 1) — contrast tussen regel 1 en regel 3.

> **🔄 Differentiatie:**
> - **MBO-3 per ongeluk in zaal:** beperk tot Reeks A en C (duidelijkste contrast: regel 3 vs regel 1). Zeg er bij: *"Reeks B is de bonus — als je tijd hebt."*
> - **MBO-4 standaard:** alle drie de reeksen. Geen extra uitdaging nodig — Reeks B (ruis zonder patroon) is bewust een 'nee-signaal'-oefening.
> - **Teamleider erbij:** geef extra opdracht: *"Per reeks: wat zou je in de shift-overdracht noteren? Niets, een signaal, of een escalatie?"*

> **🔴 Valkuil — deelnemer 'ziet' een trend die er niet is (Reeks B):**
> Ruis en trend zijn moeilijk te onderscheiden voor iemand die net het begrip leert. Als de helft van de zaal een trend ziet in Reeks B: niet direct corrigeren. Plenair straks: tel samen hoeveel opeenvolgende punten dezelfde kant op gaan (antwoord: maximaal 2 of 3). Regel 3 eist er 6. Zonder dat aantal → geen trend.

> **🔴 Valkuil — deelnemer vervangt meteen het gereedschap bij Reeks A:**
> Operators denken vaak 'trend gezien = gereedschap wisselen'. Stop kort. Zeg bij de plenaire duiding: *"De eerste actie is meten, niet vervangen. Anders weet je morgen niet of de trend door slijtage kwam of door iets anders."* Dit komt in blok 3 expliciet terug — hier alleen signaleren.

---

### 🟣 Blok 2: STARRT-reflectie op Reeks A + plenaire duiding
**00:15 - 00:27** | 12 min | Kolb-fase: reflecteren

**Doel:** De centrale les van ko-spc-501 ('een trend binnen de control limits is al een signaal') verankeren via eigen reflectie. Het 'aha'-moment expliciet maken: *'ik keek naar de absolute waardes en dacht: OK, tot ik zag dat het zes keer achter elkaar omhoog ging'*.

**Werkvorm:** 7 min individueel STARRT op wb-02 (Situatie + Taak + beginnetje Actie) → 5 min plenaire duiding Reeks A, B, C. De volledige STARRT (Resultaat, Reflectie, Transfer) wordt thuis afgemaakt en meegenomen naar de volgende sessie.

**Timing-note:** 12 min is krap voor drie reeksen plenair + STARRT invullen. Werkbare verdeling: 7 min STARRT (individueel, parallel aan begin plenair) + 5 min plenaire duiding. Deelnemers vullen S + T + begin A in tijdens de sessie, R + R + T worden thuis afgemaakt — dit staat ook op wb-02.

**Instructie:**

1. **Deel wb-02-reflectie uit** (30 sec). Zeg: *"Tijdens de plenaire bespreking vul je in: Situatie, Taak en een begin van Actie. Resultaat, Reflectie en Transfer doe je thuis af — tijdens de bespreking kun je daar aantekeningen voor maken. Dit werkblad neem je mee naar de volgende sessie, zodat we de Transfer kunnen bespreken."*

2. **STARRT-start** (7 min) — zet timer op 7 min. Zeg: *"Schrijf op wb-02 bij S en T wat Reeks A was (CNC-frees casus, boorgat 10,00 ± 0,02 mm, I-MR-kaart) en wat je opdracht was. Bij A: welke inschatting schreef je op wb-01, welke Nelson-regel koos je, welke eerste actie?"* Loop rond. Bevestig: *"Je eigen eerste inschatting — ook als die niet klopte — is precies waar we zo op doorgaan."*

3. **Plenaire duiding Reeks A** (2 min) — *"Reeks A. Acht uurmetingen, van uur 35 tot 42: 9,996 — 9,998 — 9,999 — 10,001 — 10,003 — 10,005 — 10,007 — 10,008."* Teken deze reeks op de flip-over over je eerdere lege I-chart heen. *"Geen enkel punt boven UCL (10,010). Maar — kijk mee — tel van uur 35 naar uur 42: dat zijn acht stijgende punten. Regel 3 eist er 6. We zitten ruim over de drempel. Dit is een trend."* Stilte van 3 sec. *"In de echte casus bleek: 0,015 mm gereedschapsslijtage. Tooling vervangen voorkwam dat de volgende 200 stuks out-of-spec gingen. Wachten op regel 1 (een punt boven 10,020 USL) had uren gescheeld — en uitvallers."*

4. **Plenaire duiding Reeks B** (1 min) — *"Reeks B — wie zag een signaal?"* Vang de handopsteking. *"Laten we tellen: 10,002 — 9,997 — 10,004 — 9,999 — 10,001 — 9,998 — 10,003 — 10,000. Ga van links naar rechts: hoeveel punten gaan achter elkaar dezelfde kant op?"* Laat iemand meetellen: max 2 op een rij. *"Regel 3 eist er 6. Dit is ruis — geen signaal. Goed nieuws: niet elk schommelend patroon is een trend."*

5. **Plenaire duiding Reeks C** (1 min 30) — *"Reeks C. Wie zag een signaal?"* Vang handopsteking. *"Reeks C is de makkelijkste: 10,001 — 10,000 — 10,003 — 9,998 — 10,004 — 10,013 — 10,002 — 9,999. Uur 6 geeft 10,013 — boven UCL (10,010) én boven USL (10,020 is de klantgrens, maar UCL is de procesgrens). Punt buiten UCL = Nelson-regel 1. Direct signaal, direct actie. Geen trend — wél een special cause."*

6. **Sluit blok 2 af** (30 sec) — wijs naar de flip-over. Zeg: *"Drie reeksen, drie verschillende verhalen: Reeks A is de stille trend (regel 3, nog binnen grenzen), Reeks B is ruis (geen signaal), Reeks C is de klap buiten (regel 1). We gaan nu naar de theorie — maar jullie hebben het zojuist al gezien. De theorie bevestigt."*

**Antwoordmodel — gebruik dit als basis voor de plenaire duiding (exact gesynchroniseerd met wb-01):**

| Reeks | Patroon | Nelson-regel | Eerste actie | Pedagogische tip |
|-------|---------|--------------|--------------|------------------|
| A (CNC-casus, ko-spc-501) | 8 uurmetingen, allemaal stijgend van 9,996 → 10,008; alles binnen UCL 10,010 | **Regel 3 — trend** | Stop, meet gereedschap (niet direct vervangen), documenteer | Dit is dé casus; laat de 'stille' aard expliciet zien — geen punt buiten, toch signaal |
| B (oefen, fictief) | 8 uurmetingen rond 10,000, maximaal 2 opeenvolgend dezelfde kant | **Geen signaal (ruis)** | Niets — blijven monitoren | Leert 'niet elk schommelend patroon is een trend' — Regel 3 eist 6 op een rij |
| C (oefen, fictief) | 8 uurmetingen, uur 6 = 10,013 (boven UCL 10,010) | **Regel 1 — punt buiten UCL** | Stop onmiddellijk, zoek special cause | Contrast met Reeks A — duidelijk signaal maar te laat, Regel 3 had eerder gewaarschuwd |

**Materiaal:**
- [ ] wb-02-reflectie.md (1 per deelnemer)
- [ ] Flip-over met de drie reeksen uitgeplot (laat staan voor blok 3)
- [ ] Markeerstift voor flip-over-annotaties
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Bij Reeks A: laat de stilte vallen na 'acht stijgende punten'. Niet direct invullen. Het ongemak ('ik had dit gemist') ís het leereffect.
> - De flip-over-annotatie bij Reeks A — omcirkel uur 35 en uur 42, trek er een pijl tussen met 'regel 3 trend' erbij — is je krachtigste visuele middel.
> - Tel innerlijk tot 5 bij stilte in de plenaire duiding. Vul stilte niet in. Operators kijken pas naar volgorde als je ze dwingt te kijken.

> **🔴 Valkuil — trainer legt regel 3 te snel uit:**
> Het is verleidelijk om direct 'regel 3 = 6 opeenvolgende dezelfde kant op' te zeggen. Laat eerst deelnemers meetellen op de flip-over. De tel-ervaring verankert de regel sterker dan de definitie.

> **🔴 Valkuil — deelnemer verwart UCL met USL:**
> Iemand zegt bij Reeks A: 'maar alles zit binnen de spec (10,02 mm)'. Stop kort. *"Belangrijk verschil: USL = 10,020 mm = klantgrens. UCL = 10,010 mm = processignaal-grens, berekend uit je proceshistorie. Cp/Cpk gebruikt USL/LSL — regelkaarten gebruiken UCL/LCL. Andere meting, andere doel."* Verwijs naar ko-spc-107.

> **🔄 Differentiatie:**
> - **Teamleider erbij:** voeg na Reeks A een korte vraag toe: *"Wanneer documenteer je bij jullie een trend? Alleen bij punt buiten, of ook bij regel 3?"* Vang 1-2 antwoorden — niet uitdiepen, parkeren voor blok 3.

---

### 📘 Blok 3: Handout — I-MR configureren + Nelson-regel 3 + eigen-lijn-actieplan
**00:27 - 00:45** | 18 min | Kolb-fase: theoretiseren (+ transfer geïntegreerd)

**Doel:** Het I-MR-kaart-keuzecriterium ('unieke metingen, geen natuurlijke subgroep') en de zeven Nelson-regels (focus op 1 + 3) expliciet maken. Direct daarop het transfer-moment: deelnemer kiest één eigen kritische maat en beargumenteert I-MR vs X̄-R. Lean-scope: fase 4 geïntegreerd in de handout — geen apart werkblad.

**Werkvorm:** 10 min trainer-geleide handout-bespreking + 8 min individueel eigen-lijn-actieplan onderaan wb-03.

**Instructie:**

1. **Onthul het diagram** (1 min) — verwijder de afdekking van de A3-versie achter in de zaal. Toon slide 7. Zeg: *"Drie reeksen naast elkaar — precies die van wb-01. Links de CNC-trend (regel 3, stille stijging). Midden de ruis (geen signaal). Rechts de special cause (regel 1, punt boven UCL). Dit plaatje hang je in je hoofd."*

2. **Deel wb-03-handout uit** (30 sec). *"Pak je markeerstift. Markeer wat voor jou nieuw of verrassend is. Onderaan zit jouw eigen-lijn-actieplan — dat vul je over 8 minuten zelf in."*

3. **Behandel I-MR vs X̄-R** (2 min) — slide 5. Teken op de flip-over twee kolommen: **X̄-R** (meerdere stuks uit dezelfde machinetoestand, natuurlijke subgroep) en **I-MR** (unieke meting, geen natuurlijke subgroep). *"Kernvraag: hebben jullie één stuk per meetmoment, of meerdere stuks tegelijk uit dezelfde toestand van de machine? De CNC-casus heeft drie stuks per uur meten, maar die zijn sequentieel gefreesd, niet parallel. Elke meting is uniek. Dus I-MR. In spuitgieten met vier cavitieten kun je wél X̄-R doen — want vier parallelle stuks uit één cyclus."*

4. **Behandel I-chart + MR-chart** (3 min) — slide 6. *"De I-MR heeft twee chart-lijnen onder elkaar. De bovenste — I-chart — plot elke meting. Daarop kijk je naar het proces-niveau én je Nelson-regels. De onderste — MR-chart — plot het absolute verschil tussen opeenvolgende metingen. Daarop kijk je of de korte-termijn-variatie rustig blijft. Een MR-piek zegt: iets is plotseling veranderd. Een I-trend zegt: iets verandert geleidelijk."* Schrijf de vuistformule op de flip-over: *"UCL = X̄ + 2,66 · MR̄. Je hoeft 2,66 niet uit je hoofd — het MES rekent. Maar onthoud: UCL/LCL zijn niet de klantspec. Het zijn statistische grenzen uit jouw proces zelf."*

5. **Behandel Nelson-regels tabel** (2 min) — slide 8. Loop snel door:
    - *"Regel 1 — punt buiten UCL of LCL. Heb je gezien in Reeks C."*
    - *"Regel 2 — 9 opeenvolgende aan dezelfde kant van de middellijn. Lange-termijn verschuiving."*
    - *"Regel 3 — 6 opeenvolgende stijgend of dalend. **De trend.** Heb je gezien in Reeks A."*
    - *"Regel 4 tot 7 — varianten op zone-gedrag. In deze sessie houden we het bij regel 1 en regel 3."*

6. **Regel 3 uitgelicht** (2 min) — slide 9. *"Waarom 6? Statistisch is de kans dat 6 punten toevallig op rij stijgen ongeveer 1 op 64 — 1,5%. Dan is het geen toeval meer. In de CNC-casus: 0,0004 mm slijtage per uur, 40 uur = 0,016 mm drift. Start 9,990 mm, eind 10,006 mm. Nog binnen spec (≤ 10,020). Maar de trend stond al uren op de kaart. Dat is het hele idee van regel 3: je ziet de drift aankomen."*

7. **De vijf operator-stappen + valkuil** (1 min 30) — slide 10. *"Bij een trend: Stop. Meet gereedschap. Vervang pas ná meten. Documenteer signaal-oorzaak-actie-effect. Hervat met monitoring. De belangrijkste stap die operators overslaan: meten. Direct vervangen lijkt efficiënt, maar dan weet je morgen niet of de trend door slijtage kwam of door temperatuur of materiaal. Meten is leren."*

8. **Eigen-lijn-actieplan** (8 min) — wijs naar wb-03, onderste helft. Zeg: *"Acht minuten. Kies één kritische maat van je eigen lijn. Noteer: machine, maat, USL en LSL, huidige meetfrequentie. Beargumenteer: meet je één stuk per keer of meerdere tegelijk uit dezelfde machinetoestand? Op basis daarvan: I-MR of X̄-R? Geef één trend-veroorzaker die je op die maat zou verwachten (slijtage / temperatuur / materiaal / anders). Deze week ga je in het MES of kwaliteitsrapport naar de laatste 20 metingen kijken: zie je een trend?"* Zet timer op 8 min. Loop rond. Help bij blokkades met:
    - *"Welke maat controleer je sowieso al elke shift?"*
    - *"Kun je met de hand vaststellen of er 5 stuks tegelijk uit dezelfde machinetoestand komen, of zitten er momenten tussen?"*
    - *"Welke van de trend-veroorzakers past bij jouw lijn — heeft jouw gereedschap een slijtagecurve?"*
    Bevestig dat *'ik moet dit eerst opvragen'* een geldig antwoord is — vaak het juiste.

9. **Afsluiting + transfer** (30 sec) — slide 12. *"Deze week: kijk in het MES naar de laatste 20 metingen van jouw gekozen maat. Zie je een regel-3-trend? En praat één keer met je teamleider: 'Gebruiken we op onze lijn al Nelson-regels, of alleen punt-buiten-UCL?' Het antwoord vertelt je vaak of je organisatie reactief of proactief werkt. Volgende sessie bespreken we per persoon."*

**Materiaal:**
- [ ] wb-03-handout.md (1 per deelnemer + 2 reserve)
- [ ] Markeerstiften (1 per deelnemer)
- [ ] diagram-lo-spc-501.svg — op A3 én op slide 7
- [ ] Slides 5-12
- [ ] Flip-over voor I-MR vs X̄-R-kolommen en de UCL-vuistformule
- [ ] Timer

> **💡 Tips voor de trainer:**
> - Houd het tempo in blok 3. 18 min is krap voor theorie + actieplan. Niet vertragen door eigen anekdotes — bewaar die voor blok 2 (reflectie).
> - De I-MR vs X̄-R-kolommen op de flip-over zijn je krachtigste visuele middel bij de keuzebegeleiding in het actieplan.
> - Laat het actieplan-gedeelte écht 8 minuten duren. De transfer is waar de sessie werk wordt — niet iets om af te raffelen.

> **🔴 Valkuil — trainer gaat over naar Pp/Ppk of andere Nelson-regels:**
> Een MBO-4'er met voorkennis vraagt naar regel 5 (zone A) of long-term capability. *"Goede vraag — regel 5 en zone-gedrag komen terug in module 3. Vandaag regel 1 en regel 3 — de twee die 95% van je dagelijkse beslissingen dekken."* Schrijf op parkeerflip.

> **🔴 Valkuil — trainer legt de UCL-formule berekenend uit:**
> Verleidelijk om 2,66 en d2-constanten uit te leggen. Niet doen. *"De factor 2,66 komt uit de statistische tabel voor I-MR — je hoeft 'm niet te onthouden. Het MES rekent. Wat je moet onthouden: UCL ≠ USL."* Klaar. Statistiek-verdieping is HBO-niveau.

> **🔴 Valkuil — deelnemer wil X̄-R waar I-MR passend is:**
> Iemand zegt: 'ik meet elk uur drie stuks dus dat is subgroep van 3, dus X̄-R'. Vraag terug: *'Komen die drie stuks achter elkaar uit de machine, met tijd tussen? Of uit één slag, één caviteit, één cyclus?'* Sequentieel = elke meting uniek = I-MR. Simultaan = natuurlijke subgroep = X̄-R mogelijk.

> **🔄 Differentiatie:**
> - **MBO-3 per ongeluk in zaal:** bij actieplan volstaat: machine + maat + I-MR/X̄-R-keuze. Sla de trend-veroorzaker-vraag over, en sla de bonus-vraag ('praat met teamleider') over.
> - **MBO-4 standaard:** volg het draaiboek precies. Volledig actieplan inclusief trend-veroorzaker.
> - **Teamleider:** dubbele rol — eigen analyse + één opdracht voor team ('operator X gaat deze week maat Y opvragen, ik bespreek het vrijdag').
> - **Gemengde groep:** maak bewust gemengde duo's bij het actieplan. Operator levert procesgedrag, teamleider levert tolerantie-context en escalatie-regels.

---

## 📦 Materiaallijst

| ✓ | Item | Aantal | Opmerkingen |
|---|------|--------|-------------|
| ☐ | wb-01-oefening.md | n + 2 | A4 enkelzijdig, 1 per deelnemer + reserve |
| ☐ | wb-02-reflectie.md | n + 2 | A4 enkelzijdig |
| ☐ | wb-03-handout.md | n + 2 | A4 dubbelzijdig (handout + actieplan) |
| ☐ | diagram-lo-spc-501.svg | 1 | Print A3 in kleur, hang achter in zaal (drie reeksen) |
| ☐ | Markeerstiften | n | Voor handout-blok |
| ☐ | Pennen + linialen | n + 5 | Reserve op trainer-tafel |
| ☐ | Flip-over + dikke stiften | 1 set | Voor lege I-chart (IK DOE) + I-MR/X̄-R-kolommen |
| ☐ | Timer / mobiel met geluid | 1 | Voor 9-min oefening + 7-min STARRT + 8-min actieplan |
| ☐ | Laptop + beamer + HDMI | 1 set | Vooraf testen — slide 7 (SVG) is cruciaal |
| ☐ | presentatie.slidev.md geopend | 1 | In presenter-modus voor speaker notes |

n = aantal deelnemers

---

## Snel-overzicht antwoordmodel trend-oefening

| Reeks | Gegeven (uit wb-01) | Patroon | Nelson-regel | Eerste actie |
|-------|---------------------|---------|--------------|--------------|
| A (ko-spc-501 — echt) | 8 uur, 9,996 → 10,008 mm, alles < UCL (10,010) | 6+ opeenvolgend stijgend | **Regel 3 — trend** | Stop, meet gereedschap, vervang pas ná meten |
| B (oefen — fictief) | 8 uur rond 10,000 mm, max 2 opeenvolgend zelfde kant | Ruis — geen patroon | **Geen signaal** | Niets — blijven monitoren |
| C (oefen — fictief) | 8 uur, uur 6 = 10,013 mm (> UCL 10,010) | Punt buiten UCL | **Regel 1** | Stop onmiddellijk, zoek special cause |

**Slagingscriterium (ABCD-degree):** minimaal 2 van de 3 reeksen correct geduid én op wb-03 kritische maat genoteerd met I-MR/X̄-R-motivering. Reeks A is de toetssteen voor regel 3 (stille trend). Reeks B test of deelnemer niet over-diagnosticeert. Reeks C is het regel-1-contrast.

---

## Checklist na de sessie

- [ ] Werkbladen ingenomen of foto's gemaakt (voor learning analytics)
- [ ] Handopsteking-statistiek genoteerd (hoeveel deelnemers zagen een signaal in A, B, C)
- [ ] Flip-over met plotjes van Reeks A/B/C gefotografeerd
- [ ] Notitie voor volgende workshop: welke kritische maten hebben deelnemers gekozen voor het actieplan?
- [ ] xAPI-statements verstuurd: `experienced` (trend-oefening), `attempted` (reflectie), `completed` (handout + actieplan)
- [ ] Bij teamleider-deelnemers: korte handover naar de groepsreflectie configuratiebesluit (volgend blok in module 2)

---

*AIMM Curriculum | SPC Module 2 (Train) | CNC-frees casus — I-MR en gereedschapsslijtage*
*Bronnen: ko-spc-501 (CNC-frees casus) | AIAG SPC Reference Manual, 2nd ed. | Nelson, L.S. (1984). Technical Aids: The Shewhart Control Chart — Tests for Special Causes. Journal of Quality Technology, 15(4), 237-239 | NIST/SEMATECH e-Handbook, sectie 6.3.2*
*© BronzGreen × AIMM, 2026 | Draaiboek v1.0*
