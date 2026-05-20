---
theme: default
title: CNC-frees casus — I-MR en gereedschapsslijtage detecteren
info: |
  ## SPC Module 2 — Train
  Workshop-blok over I-MR-regelkaarten en Nelson-regel 3 (trend).
  Doelgroep: operators MBO-3/MBO-4 + teamleiders MBO-4, 45 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# I-MR en de stille trend

### Hoe zie je gereedschapsslijtage vóórdat de eerste uitvaller komt?

<div class="mt-12 text-sm opacity-60">
  SPC Module 2 (Train) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3/4 + teamleiders · I-MR + Nelson-regel 3
</div>

<!--
Open met de centrale vraag.
"Op jouw lijn draai je een serie van 2000 stuks. Elk punt dat jij meet ligt netjes
binnen de control limits. En tóch zitten er na 40 uur 200 stuks in de uitval-bak.
Hoe kan dat?"

Wacht. Laat 1-2 mensen speculeren. Geen lange verhalen.

Trigger: "Vandaag leer je één regel waarmee je dát scenario voorkomt: Nelson-regel 3,
de trend. Zes punten achter elkaar omhoog of omlaag — ook binnen de grenzen — is al een signaal.
We beginnen niet met theorie. We beginnen met kijken."

Verwijs naar draaiboek blok 1, instructie 1-2.
-->

---
layout: center
class: text-center
---

# IK DOE — even hardop denken

<div class="text-xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  8 metingen op een I-chart.<br/>
  UCL ≈ 10,010 mm. LCL ≈ 9,990 mm.<br/>
  <span class="font-mono text-amber-700 font-bold">10,002 · 10,003 · 10,001 · 10,003 · 10,004 · 10,005 · 10,006 · 10,007</span>
</div>

<div v-click class="mt-10 inline-block px-5 py-3 bg-amber-100 text-amber-900 rounded-lg">
  Geen punt buiten de grenzen.<br/>
  <span class="font-bold">Maar zes punten achter elkaar omhoog.</span>
</div>

<div v-click class="mt-6 text-base opacity-70 max-w-lg mx-auto">
  Nelson-regel 3 — trend.<br/>
  <span class="text-sm">Eerste actie: meten, niet direct vervangen.</span>
</div>

<!--
Trainer plot de reeks met kruisjes op de lege I-chart op de flip-over.

Denk hardop: "Geen punt buiten. Maar ik zie zes punten achter elkaar omhoog kruipen —
vanaf punt 3 tot punt 8. Dat is een trend. Nelson-regel 3.
Eerste actie: ik stop niet meteen met vervangen, ik ga eerst het gereedschap meten.
Misschien is het slijtage, misschien iets anders. Meten is de eerste stap."

Stilte van 3 sec. Dan werkblad uitdelen.

Verwijs naar draaiboek blok 1, instructie 3.
-->

---
layout: center
class: text-center
---

# 🟢 Werkblad — drie reeksen lezen

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  Drie meetreeksen.<br/>
  Per reeks: <span class="font-bold">signaal? regel? eerste actie?</span>
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Reeks A = echt (CNC-frees, ko-spc-501)<br/>
  Reeks B = oefen (fictief)<br/>
  Reeks C = oefen (fictief)
</div>

<div class="abs-br m-6 text-xs opacity-40">
  9 minuten · individueel · pen + liniaal
</div>

<!--
Deel wb-01-oefening uit (30 sec).
"Drie reeksen. Reeks A is de CNC-frees casus uit ko-spc-501 — de echte casus.
Reeks B en C zijn oefenreeksen.
Voor elke reeks: zie je een signaal? Welke Nelson-regel? Wat zou je als eerste doen?
Bij twijfel: vraagteken."

Zet timer op 9 min. Loop rond. Beantwoord praktische vragen, GEEN inhoudelijke.
Als iemand vraagt "is dit goed?": "Dat bespreken we zo plenair."

Aan het einde: "Pen neer. Handopsteking per reeks: wie zag een signaal in A? B? C?"
Tel hardop, noteer op flip-over.

Verwijs naar draaiboek blok 1, instructie 4-6.
-->

---
layout: section
---

# Reflecteren

## Wat zag je — en wat had je bijna gemist?

<!--
Overgang naar blok 2 (reflecteren).
"Handen omlaag. We gaan de drie reeksen één voor één bespreken. Eerst invullen op wb-02,
dan plenair."

Deel wb-02-reflectie uit:
"Tijdens de bespreking vul je Situatie, Taak en een begin van Actie in.
Resultaat, Reflectie en Transfer doe je thuis af — neem het werkblad mee naar de volgende sessie."

Verwijs naar draaiboek blok 2, instructie 1-2.
-->

---

# Reeks A — de stille trend

<div class="font-mono text-lg mt-6 text-center bg-amber-50 p-4 rounded-lg">
  9,996 · 9,998 · 9,999 · 10,001 · 10,003 · 10,005 · 10,007 · 10,008
</div>

<div v-click class="mt-6 grid grid-cols-2 gap-4">
  <div class="p-4 bg-green-50 rounded-lg border-2 border-green-200">
    <div class="font-bold text-green-800 mb-2">Wat zie je binnen de grenzen?</div>
    <div class="text-sm opacity-80">UCL = 10,010 · LCL = 9,990<br/>Geen enkel punt buiten.</div>
  </div>
  <div class="p-4 bg-red-50 rounded-lg border-2 border-red-200">
    <div class="font-bold text-red-800 mb-2">Wat zie je in de volgorde?</div>
    <div class="text-sm opacity-80">Acht punten — allemaal stijgend.<br/><span class="font-bold">Regel 3 eist er 6. Ruim over.</span></div>
  </div>
</div>

<div v-click class="mt-6 p-4 bg-blue-50 text-blue-900 rounded-lg text-center">
  In de echte casus: <span class="font-bold">0,015 mm gereedschapsslijtage</span>.<br/>
  Tooling vervangen voorkwam <span class="font-bold">200 out-of-spec stuks</span>.
</div>

<!--
Teken deze reeks over de lege I-chart op de flip-over heen.

"Acht uurmetingen, uur 35 tot 42. Geen enkel punt boven UCL (10,010).
Maar tel mee — acht stijgende punten op een rij. Regel 3 eist er 6. We zitten ruim over."

Stilte van 3 sec.

"In de echte casus: 0,015 mm gereedschapsslijtage.
Tooling vervangen voorkwam dat de volgende 200 stuks out-of-spec gingen.
Wachten op regel 1 (punt boven 10,010) had uren gescheeld — met afkeur."

Verwijs naar draaiboek blok 2, instructie 3.
-->

---

# Reeks B — geen patroon

<div class="font-mono text-lg mt-6 text-center bg-gray-50 p-4 rounded-lg">
  10,002 · 9,997 · 10,004 · 9,999 · 10,001 · 9,998 · 10,003 · 10,000
</div>

<div v-click class="mt-8 text-center text-base opacity-80">
  Tel van links naar rechts:<br/>
  <span class="font-bold">hoeveel opeenvolgend dezelfde kant op?</span>
</div>

<div v-click class="mt-6 inline-block mx-auto block text-center px-5 py-3 bg-green-100 text-green-900 rounded-lg">
  Maximaal 2 op een rij.<br/>
  <span class="font-bold">Regel 3 eist er 6. Geen signaal.</span>
</div>

<div v-click class="mt-6 text-sm opacity-70 text-center max-w-lg mx-auto">
  Goed nieuws: niet elk schommelend patroon is een trend.<br/>
  Regel 3 is streng — met reden.
</div>

<!--
"Reeks B — wie zag een signaal?" Vang handopsteking.

Laat iemand meetellen: omhoog, omlaag, omhoog, omlaag — maximaal 2 op een rij.

"Regel 3 eist er 6. Dit is ruis — geen signaal. Goed nieuws: niet elk schommelend patroon is een trend."

Bevestig de deelnemers die 'geen signaal' hadden. Die hebben de regel goed toegepast.

Verwijs naar draaiboek blok 2, instructie 4.
-->

---

# Reeks C — punt buiten UCL

<div class="font-mono text-lg mt-6 text-center bg-red-50 p-4 rounded-lg">
  10,001 · 10,000 · 10,003 · 9,998 · 10,004 · <span class="text-red-700 font-bold">10,013</span> · 10,002 · 9,999
</div>

<div v-click class="mt-8 text-center text-base">
  Uur 6: <span class="font-mono font-bold text-red-700">10,013</span> — <span class="font-bold">boven UCL (10,010)</span>
</div>

<div v-click class="mt-6 inline-block mx-auto block text-center px-5 py-3 bg-red-100 text-red-900 rounded-lg">
  Nelson-regel 1 — punt buiten UCL.<br/>
  <span class="font-bold">Stop onmiddellijk. Zoek special cause.</span>
</div>

<div v-click class="mt-6 text-sm opacity-70 text-center max-w-lg mx-auto">
  Contrast met Reeks A: regel 1 is <span class="font-bold">duidelijk maar laat</span>.<br/>
  Regel 3 had eerder gewaarschuwd — als er een trend vóór had gezeten.
</div>

<!--
"Reeks C is de makkelijkste. Uur 6 geeft 10,013 — boven UCL (10,010).
Punt buiten UCL = Nelson-regel 1. Direct signaal, direct actie. Geen trend — wel special cause."

Contrast: regel 1 is duidelijk maar je pakt pas het signaal als de uitval er al is.
Regel 3 pakt de drift erheen.

Sluit blok 2 af: "Drie reeksen, drie verhalen. A = stille trend (regel 3), B = ruis (geen signaal),
C = de klap buiten (regel 1). Nu de theorie."

Verwijs naar draaiboek blok 2, instructie 5-6.
-->

---
layout: section
---

# Theoretiseren

## Van kijken naar configureren

<!--
Overgang naar blok 3 (theoretiseren).
"Jullie hebben het zojuist al gezien — drie soorten signalen. De theorie bevestigt wat jullie deden.
We kijken nu naar: wanneer kies je I-MR, hoe werkt de kaart, en wat doe je bij een trend."

Onthul het A3-diagram achter in de zaal (slide 7 + diagram-lo-spc-501.svg).

Deel wb-03-handout uit: "Pak je markeerstift. Markeer wat voor jou nieuw is.
Onderaan zit jouw eigen-lijn-actieplan — dat vul je over 8 minuten zelf in."

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---
layout: two-cols
layoutClass: gap-6
---

# X̄-R of I-MR?

### 🟢 X̄-R
<div class="mt-3 text-sm opacity-80">

- Meerdere stuks tegelijk
- Uit **dezelfde** machinetoestand
- Bijv. 4 cavitieten per cyclus

</div>

<div class="mt-4 p-3 bg-green-50 rounded-lg text-xs">
Natuurlijke subgroep → plot het gemiddelde
</div>

::right::

### 🟠 I-MR
<div class="mt-3 text-sm opacity-80">

- **Eén meting** per meetmoment
- Of stukken met **tijd tussen**
- Destructieve of dure meting

</div>

<div class="mt-4 p-3 bg-amber-50 rounded-lg text-xs">
Elke meting uniek → plot de individuele meting + MR
</div>

<div v-click class="mt-8 text-center text-base p-3 bg-blue-50 text-blue-900 rounded-lg">
  CNC-casus: drie stuks per uur, <span class="font-bold">sequentieel gefreesd</span> — elke meting uniek → <span class="font-bold">I-MR</span>
</div>

<!--
Teken op flip-over twee kolommen: X̄-R en I-MR.

"Kernvraag: hebben jullie één stuk per meetmoment, of meerdere stuks tegelijk uit dezelfde toestand van de machine?

CNC-casus: drie stuks per uur, maar sequentieel gefreesd, niet parallel. Elke meting uniek. Dus I-MR.
Spuitgieten met 4 cavitieten: wél X̄-R — 4 parallelle stuks uit één cyclus."

Verwijs naar draaiboek blok 3, instructie 3.
-->

---
layout: two-cols
layoutClass: gap-6
---

# I-MR heeft twee chart-lijnen

### 📊 I-chart
<div class="mt-3 text-sm opacity-80">

- Plot **elke individuele meting**
- Bewaakt **proces-niveau**
- Hier kijk je naar Nelson-regels

</div>

::right::

### 📉 MR-chart
<div class="mt-3 text-sm opacity-80">

- Plot **verschil opeenvolgende metingen**
- Bewaakt **korte-termijn-variatie**
- Piek = plotse verandering

</div>

<div v-click class="mt-6 text-center">
  <div class="font-mono text-base text-amber-700 bg-amber-50 p-3 rounded-lg inline-block">
    UCL = X̄ + 2,66 · M̄R
  </div>
</div>

<div v-click class="mt-4 text-sm opacity-70 text-center max-w-lg mx-auto">
  De factor 2,66 komt uit de statistische tabel.<br/>
  MES rekent — jij hoeft alleen te onthouden:<br/>
  <span class="font-bold">UCL ≠ USL.</span>
</div>

<!--
"De I-MR heeft twee chart-lijnen onder elkaar.
De bovenste — I-chart — plot elke meting. Daarop kijk je naar proces-niveau en Nelson-regels.
De onderste — MR-chart — plot het verschil tussen opeenvolgende metingen.
Daarop kijk je of de korte-termijn-variatie rustig blijft. Een MR-piek zegt: iets is plots veranderd.
Een I-trend zegt: iets verandert geleidelijk."

Schrijf vuistformule op flip-over. "Je hoeft 2,66 niet uit je hoofd — MES rekent.
Wat je wel moet onthouden: UCL/LCL zijn statistische grenzen uit je proces zelf. Niet de klantspec."

Verwijs naar draaiboek blok 3, instructie 4.
-->

---

# De zeven Nelson-regels — kort

| Regel | Signaal |
|-------|---------|
| **1** | 1 punt buiten UCL of LCL · *zoals Reeks C* |
| **2** | 9 opeenvolgende aan dezelfde kant van middellijn |
| **3** | **6 opeenvolgende stijgend of dalend — trend** · *zoals Reeks A* |
| **4** | 14 opeenvolgende afwisselend op en neer |
| **5-7** | Zone-regels (A, B, C) — module 3 |

<div v-click class="mt-8 text-center text-base p-4 bg-blue-50 text-blue-900 rounded-lg max-w-xl mx-auto">
  Vandaag focus op <span class="font-bold">regel 1 en regel 3</span>.<br/>
  <span class="text-sm opacity-80">95% van je dagelijkse beslissingen.</span>
</div>

<!--
Loop snel door:
- Regel 1 — punt buiten. Gezien in Reeks C.
- Regel 2 — lange-termijn verschuiving.
- Regel 3 — de trend. Gezien in Reeks A.
- Regel 4-7 — zone-gedrag, komt terug in module 3.

Vandaag focus op 1 en 3. De twee die 95% van dagelijkse beslissingen dekken.

Verwijs naar draaiboek blok 3, instructie 5.
-->

---
layout: center
class: text-center
---

# Waarom 6? — Regel 3 uitgelicht

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Kans dat 6 punten toevallig op rij stijgen:<br/>
  <span class="font-mono text-3xl text-amber-700 font-bold">≈ 1 op 64</span><br/>
  <span class="text-sm opacity-70">Ongeveer 1,5%. Geen toeval meer.</span>
</div>

<div v-click class="mt-10 p-5 bg-amber-50 rounded-xl max-w-2xl mx-auto">
  <div class="text-sm opacity-80 mb-2">CNC-casus — doorrekening</div>
  <div class="text-base">0,0004 mm slijtage/uur · 40 uur = <span class="font-bold">0,016 mm drift</span></div>
  <div class="text-sm mt-2 opacity-80">Start <span class="font-mono">9,990 mm</span> → eind <span class="font-mono">10,006 mm</span></div>
  <div class="text-sm mt-1 opacity-70">Nog binnen spec (≤ 10,020). <span class="font-bold">Maar de trend stond uren op de kaart.</span></div>
</div>

<!--
"Waarom 6? Statistisch is de kans dat 6 punten toevallig op rij stijgen ongeveer 1 op 64 — 1,5%.
Dan is het geen toeval meer."

"In de CNC-casus: 0,0004 mm slijtage per uur, 40 uur = 0,016 mm drift.
Start 9,990 mm, eind 10,006 mm. Nog binnen spec (≤ 10,020).
Maar de trend stond al uren op de kaart.

Dat is het hele idee van regel 3: je ziet de drift aankomen."

Verwijs naar draaiboek blok 3, instructie 6.
-->

---

# Wat doe je bij een trend? — 5 operator-stappen

<div class="grid grid-cols-1 gap-3 mt-6">

<div v-click class="p-3 bg-blue-50 rounded-lg border-l-4 border-blue-400">
  <div class="font-bold text-blue-900">1. Stop de machine</div>
  <div class="text-sm opacity-80 mt-1">Of signaleer en laat bevoegde collega stoppen.</div>
</div>

<div v-click class="p-3 bg-amber-50 rounded-lg border-l-4 border-amber-400">
  <div class="font-bold text-amber-900">2. Meet het gereedschap</div>
  <div class="text-sm opacity-80 mt-1">CNC-casus: 0,015 mm slijtage bevestigd. <span class="font-bold">Niet overslaan.</span></div>
</div>

<div v-click class="p-3 bg-green-50 rounded-lg border-l-4 border-green-400">
  <div class="font-bold text-green-900">3. Vervang tooling</div>
  <div class="text-sm opacity-80 mt-1">Of laat vervangen — <span class="font-bold">pas ná meten</span>.</div>
</div>

<div v-click class="p-3 bg-purple-50 rounded-lg border-l-4 border-purple-400">
  <div class="font-bold text-purple-900">4. Documenteer</div>
  <div class="text-sm opacity-80 mt-1">Signaal + oorzaak + actie + effect. Voor jezelf én je collega's.</div>
</div>

<div v-click class="p-3 bg-gray-50 rounded-lg border-l-4 border-gray-400">
  <div class="font-bold text-gray-900">5. Hervat met monitoring</div>
  <div class="text-sm opacity-80 mt-1">Wordt de kaart weer rustig? Dan klopte je diagnose.</div>
</div>

</div>

<!--
Loop snel door. Nadruk op stap 2: meten, niet direct vervangen.

"De belangrijkste stap die operators overslaan: meten.
Direct vervangen lijkt efficiënt, maar dan weet je morgen niet
of de trend door slijtage kwam of door temperatuur of materiaal.
Meten is leren."

Verwijs naar draaiboek blok 3, instructie 7.
-->

---
layout: section
---

# Experimenteren — geïntegreerd

## Eén kritische maat van jouw lijn

<!--
Overgang naar het actieplan-gedeelte van wb-03 (lean-scope: geen apart werkblad).

"Acht minuten. Kies één kritische maat van je eigen lijn.
Noteer machine, maat, USL/LSL, meetfrequentie.
Kies: I-MR of X̄-R — en beargumenteer waarom.
Noem één trend-veroorzaker die je op die maat zou verwachten."

Deze fase is bewust kort en geïntegreerd in de handout — lean-ontwerp.

Verwijs naar draaiboek blok 3, instructie 8.
-->

---

# Jouw actieplan — onderaan wb-03

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Vijf vragen
<v-clicks>

1. Machine + kritische maat?
2. USL en LSL?
3. Meet ik 1 stuk of meerdere tegelijk?
4. I-MR of X̄-R — <span class="font-bold">waarom?</span>
5. Welke trend-veroorzaker verwacht ik?

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Welke maat controleer ik elke shift al?
- Komen de stuks sequentieel of parallel?
- Heeft mijn gereedschap een slijtagecurve?
- Temperatuur? Materiaal? Afstelling?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  8 min · individueel · wb-03-handout onderaan
</div>

<!--
Zet timer op 8 min.

Loop rond. Help met:
- "Welke maat controleer je sowieso al elke shift?"
- "Kun je met de hand vaststellen of er 5 stuks tegelijk uit dezelfde machinetoestand komen?"
- "Welke van de trend-veroorzakers past bij jouw lijn?"

Bevestig dat 'ik moet dit eerst opvragen' een geldig antwoord is — vaak het juiste.
NIET zelf meedenken over instellingen — autonomie is de werkende component.

Verwijs naar draaiboek blok 3, instructie 8.
-->

---
layout: center
class: text-center
---

# Transferopdracht — deze week

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Kijk in het <span class="font-bold">MES</span> of kwaliteitsrapport<br/>
  naar de laatste <span class="font-bold">20 metingen</span> van jouw gekozen maat.
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-2xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Zie je regel 3?</div>
    <div class="text-xs opacity-70 mt-1">6 opeenvolgend?</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Zie je regel 1?</div>
    <div class="text-xs opacity-70 mt-1">Punt buiten?</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-900">Niets?</div>
    <div class="text-xs opacity-70 mt-1">Ook een antwoord.</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-70 max-w-lg mx-auto">
  Bonus: vraag je teamleider of engineer:<br/>
  <span class="font-mono text-sm">"Gebruiken we al Nelson-regels, of alleen punt-buiten-UCL?"</span>
</div>

<!--
"Deze week: kijk in het MES naar de laatste 20 metingen van jouw gekozen maat.
Zie je een regel-3-trend? Zie je een regel-1-punt-buiten? Of niets? Alle drie zijn geldige antwoorden.

Bonus: praat één keer met je teamleider.
'Gebruiken we al Nelson-regels, of alleen punt-buiten-UCL?'
Het antwoord vertelt je vaak of je organisatie reactief of proactief werkt.

Volgende sessie bespreken we per persoon."

Verwijs naar draaiboek blok 3, instructie 9.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgend blok in module 2: <span class="font-bold">groepsreflectie configuratiebesluit eigen lijn</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 2 (Train) · I-MR + Nelson-regel 3
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (groepsreflectie configuratiebesluit).

Vergeet niet werkbladen in te nemen of foto's te maken voor learning analytics.

Notities voor jezelf na afloop:
- Bij welke reeks (A, B, C) had deze groep het meeste moeite?
- Welke kritische maten hebben deelnemers gekozen voor het actieplan?
- Bij teamleider-deelnemers: warm overdragen naar groepsreflectie configuratiebesluit.

Verwijs naar draaiboek "Checklist na de sessie".
-->
