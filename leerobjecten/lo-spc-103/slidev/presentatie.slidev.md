---
theme: default
title: Van papieren kaart naar dashboard — wat verandert er echt?
info: |
  ## SPC Module 1 — Gebruik
  Workshop-blok over de overgang van klassieke papieren SPC-kaarten
  naar Industry 4.0 dashboards. Kern: het Shewhart-principe blijft.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Van kaart naar dashboard

### Wat verandert er echt — en wat blijft hetzelfde?

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom bij workshop-blok 2 van SPC Module 1.
"In het vorige blok hebben we geleerd dat elk proces varieert — common cause en special cause.
Vandaag kijken we: hoe zie je die variatie eigenlijk?
Vroeger op een papieren kaart. Nu op een dashboard.
In de komende 40 minuten ontdek je wat er echt verandert — en wat onder de motorkap
exact hetzelfde blijft."

Niet vooraf de vijf verschuivingen noemen. Dat is de leerstof — die ontdekken ze in blok 1.
-->

---
layout: two-cols
layoutClass: gap-8
---

# Twee beelden, naast elkaar

Op je stoel liggen twee voorbeelden.

<v-clicks>

- **Voorbeeld A** — papieren X-bar-R-kaart, 20 punten, fictief (uit 2010)
- **Voorbeeld B** — MES/SCADA-dashboard, screenshot, fictief (uit 2026)
- **Eerst 2 min kijken** — pen neer
- **Daarna 10 min** de vergelijkingstabel invullen
- **Werkblad:** wb-01-vergelijk-papieren-en-digitaal

</v-clicks>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="flex gap-6 items-center justify-center">
      <div>
        <div class="text-6xl">📋</div>
        <div class="text-xs opacity-60 mt-2">Voorbeeld A<br/>papier</div>
      </div>
      <div class="text-3xl opacity-40">vs</div>
      <div>
        <div class="text-6xl">📊</div>
        <div class="text-xs opacity-60 mt-2">Voorbeeld B<br/>dashboard</div>
      </div>
    </div>
    <div class="text-xs opacity-50 mt-6">fictieve voorbeelden · ter illustratie</div>
  </div>
</div>

<!--
Slide 2 — introductie vergelijking.

"Hier naast je stoel liggen twee beelden. Voorbeeld A is een papieren regelkaart uit 2010,
20 meetpunten, met de hand ingevuld. Voorbeeld B is een screenshot van een MES-dashboard
van een vergelijkbare lijn uit 2026. Allebei fictief, ter illustratie."

Deel wb-01-vergelijk-papieren-en-digitaal uit (of check of het op de stoel ligt).
"2 minuten rustig kijken — geen pen op papier. Daarna vul je de tabel in. Totaal 12 min."

Zet timer op 2 min stil-kijken. Houd de stilte vol.
Daarna timer op 10 min. Loop rond. Beantwoord alleen praktische vragen.
NIET beoordelen wat "goed" is — alleen wat ze herkennen.

Geen theorie vooraf — dat komt pas in blok 3.
-->

---
layout: section
---

# Reflecteren

## Mijn dashboards, mijn reactietijd

<!--
Overgang naar blok 2 (reflecteren).
"Nu gaan we van Voorbeeld A en B naar jouw werkvloer. Welke schermen gebruik jij?
Wat gebeurde er bij het laatste alarm? Hoe snel reageerde je?
En — eerlijk — weet je wát er onder die alarmregel zit?"

15 min totaal: 10 min STARRT individueel, 5 min plenair op vraag 5.
-->

---
layout: two-cols-header
---

# STARRT — over jezelf

::left::

### Wat vul je in?
<v-clicks>

- **S**ituatie — welke schermen op jouw werkvloer?
- **T**aak — wat werd bij het laatste alarm verwacht?
- **A**ctie — wat deed je precies?
- **R**esultaat — hoe snel reageerde je?
- **R**eflectie — wat weet jij onder het scherm?
- **T**ransfer — welke vraag stel je morgen?

</v-clicks>

::right::

### Hoe vul je in?
<v-clicks>

- Over **jezelf**, niet over Voorbeeld B
- In jouw eigen woorden
- Eerlijk — *"ik weet het niet"* is goud
- Twijfel mag — zet een vraagteken

</v-clicks>

<div class="abs-br m-6 text-xs opacity-40">
  10 min · individueel · wb-02-reflectie
</div>

<!--
Deel wb-02-reflectie uit.
"Dit werkblad volgt de STARRT-structuur. Je vult het in over jezelf en jouw werkvloer —
niet meer over papier en Voorbeeld B. Welke schermen gebruik jij, wat gebeurde er bij het
laatste alarm, hoe snel reageerde je, en — eerlijk — weet je wát er onder die alarmregel zit?"

Zet timer op 10 min. Loop rond.
Help bij blokkades:
- Vraag 1: "Bij je machine, in de supervisor-kamer, op je mobiel?" Drie schermen is normaal.
- Vraag 4: "Geen prestatiemeting — het gaat om beseffen. Snel is niet automatisch goed."
- Vraag 5: "'Ik weet alleen dat het rood wordt' is prima. Dan weet je tenminste waar je staat."
-->

---

# Wat weet jij onder het scherm?

<div class="mt-8 grid grid-cols-3 gap-6 text-base">

<div class="p-5 bg-green-50 rounded-lg">
  <div class="font-bold text-green-700 mb-2">✅ Ik weet de regel</div>
  <div class="text-xs opacity-70">UCL/LCL, Nelson-regel, AI-model — ik weet wat er onder zit</div>
  <div class="text-xs opacity-50 mt-3">turfje</div>
</div>

<div class="p-5 bg-amber-50 rounded-lg">
  <div class="font-bold text-amber-700 mb-2">⚠️ Ik weet dat er een grens is</div>
  <div class="text-xs opacity-70">... maar niet precies welke of welk model</div>
  <div class="text-xs opacity-50 mt-3">turfje</div>
</div>

<div class="p-5 bg-red-50 rounded-lg">
  <div class="font-bold text-red-700 mb-2">🔴 Ik weet alleen dat het rood wordt</div>
  <div class="text-xs opacity-70">Alarm = reset. Meer weet ik niet.</div>
  <div class="text-xs opacity-50 mt-3">turfje</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-80">
  <span class="font-bold">Geen schaamte.</span> Dit is het vertrekpunt — niet het eindpunt.
</div>

<!--
Plenaire ronde (4 min): "Pen neer. We gaan rond bij vraag 5 — wat weet jij onder het scherm?
Drie keuzes. Eerlijke antwoorden graag."

Turf op flip-over in drie kolommen.
Laat 4-6 deelnemers snel hun keuze noemen (30 sec per persoon).

Duiding (30 sec): laat de cijfers zien.
"Heel normaal dat je niet weet wat er onder zit — dat heeft niemand je geleerd.
Maar zolang je het niet weet, ben je operator van het scherm in plaats van operator
van het proces. Dat gaan we straks rechtzetten."

Valkuilen:
- Deelnemer schaamt zich voor "ik weet het niet" → benoem het als eerlijkste start.
- Deelnemer zegt alles te weten → vraag concreet: "Welke regel zit onder het alarm van dat scherm?"
- "Bij ons hangen geen schermen" → gebruik hem als verkenner voor transferopdracht.

Stem zelf NIET mee — jij bent facilitator.
Tel tot 7 na elke vraag. Vul stilte niet in.
-->

---
layout: section
---

# Theoretiseren

## Klassiek vs Industry 4.0

<!--
Overgang naar blok 3.
"We hebben twee beelden vergeleken en onze eigen schermen op tafel gelegd.
Nu gaan we ordenen: wat je in blok 1 zag heeft officiële namen.
Wat jou opviel aan snelheid heet 'reactietijd'. Wat jou opviel aan alarmen heet 'detectie'."

Onthul nu het A3-diagram achter in de zaal. Dat is de brug voor de volgende slide.
-->

---
layout: image-right
image: ../../trainee/lo-spc-103/diagram-lo-spc-103.svg
backgroundSize: contain
---

# De brug: Shewhart

<v-clicks>

- **Links:** papieren kaart — 20 punten, handmatig
- **Rechts:** dashboard — miljoenen punten, automatisch
- **Midden:** dezelfde vraag — signaal of ruis?

</v-clicks>

<div v-click class="mt-8 text-sm opacity-80">
  Het gereedschap verandert. <span class="font-bold">De vraag niet.</span>
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: Shewhart (1931); ISO 7870-2 voor Shewhart-regelkaarten
</div>

<!--
Slide 7 — het centrale diagram.

"Hier staan ze naast elkaar — links de papieren kaart, rechts het dashboard.
Wat in het midden zit — het gele strookje — is het Shewhart-principe.
Dat is de brug: onder beide gereedschappen dezelfde vraag."

Deel wb-03-handout-klassiek-vs-industry40 uit.
"Pak je markeerstift. We gaan door de vijf verschuivingen.
Markeer wat je in blok 1 ook al had opgeschreven, en zet een sterretje bij wat je nieuw vindt."

Wijs meerdere keren naar het diagram tijdens de volgende slides.
-->

---

# Vijf verschuivingen

<div class="mt-6 grid grid-cols-[1fr_2fr_2fr] gap-3 text-sm">

<div class="font-bold p-2 bg-gray-100 rounded">Aspect</div>
<div class="font-bold p-2 bg-blue-100 rounded">Klassiek (papier)</div>
<div class="font-bold p-2 bg-green-100 rounded">Industry 4.0 (dashboard)</div>

<div v-click class="p-2 font-bold">Meten</div>
<div v-click class="p-2 bg-blue-50 rounded">Handmatig, per uur</div>
<div v-click class="p-2 bg-green-50 rounded">Continu via sensor</div>

<div v-click class="p-2 font-bold">Drager</div>
<div v-click class="p-2 bg-blue-50 rounded">Papier / spreadsheet</div>
<div v-click class="p-2 bg-green-50 rounded">Cloud / MES / SCADA</div>

<div v-click class="p-2 font-bold">Detectie</div>
<div v-click class="p-2 bg-blue-50 rounded">Operator scant</div>
<div v-click class="p-2 bg-green-50 rounded">Regel + soms AI</div>

<div v-click class="p-2 font-bold">Reactietijd</div>
<div v-click class="p-2 bg-blue-50 rounded">Uren tot dagen</div>
<div v-click class="p-2 bg-green-50 rounded">Seconden tot minuten</div>

<div v-click class="p-2 font-bold">Datavolume</div>
<div v-click class="p-2 bg-blue-50 rounded">Tientallen / dag</div>
<div v-click class="p-2 bg-green-50 rounded">Miljoenen / dag</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  Bron: recente literatuur Industry 4.0 SPC — ko-spc-103
</div>

<!--
Slide 8 — de vergelijkingstabel.

Per rij één korte uitleg + koppeling naar wat de groep in blok 1 of 2 al noemde:

METEN (1 min):
"Voorbeeld A: 1 punt per uur, 20 totaal. Voorbeeld B: honderden per minuut. Meetfrequentie."

DRAGER (1 min):
"Papier in de ordner vs scherm dat iedereen overal ziet — ook teamleider, kwaliteitsmanager."
Bron: recente literatuur Industry 4.0 SPC.

DETECTIE (1 min):
"Vroeger: jij met je ogen over 20 punten. Nu: regel die automatisch telt, soms AI."
Terugkoppeling blok 2: "De derde kolom turfjes — 'ik weet alleen dat het rood wordt' —
gaat over deze rij. De regel onder jouw alarm is wat je hoort te kennen."

REACTIETIJD (1 min):
"Vroeger uren, nu 30 seconden. BELANGRIJK: sneller piepen ≠ sneller handelen.
Eerst Shewhart-vraag, dan actie."

DATAVOLUME (1 min):
"20 punten per shift vs 3,6 miljoen per dag. Niet alleen meer — fundamenteel andere data."

Schrijf tijdens dit blok op flip-over VROEGER/NU een korte samenvatting per rij.

Tempo-check na 3 min: indien krap, "Datavolume" in één zin afronden.

Differentiatie MBO-4: bij Detectie toevoegen: "Regel = formule die jij kunt lezen;
AI-model = getraind op data, niet altijd uitlegbaar."
-->

---
layout: center
class: text-center
---

# Wat verandert niet?

<div class="mt-6 text-2xl font-bold">
  Het Shewhart-principe
</div>

<div class="mt-8 text-xl opacity-90 max-w-2xl mx-auto">
  <span class="font-bold">Is dit signaal</span> — iets anders dan normaal?<br/>
  Of <span class="font-bold">is dit ruis</span> — normale spreiding?
</div>

<div v-click class="mt-10 text-base opacity-70 max-w-xl mx-auto">
  Een sensor die elke seconde meet, verandert niets aan die vraag.<br/>
  Sneller meten betekent niet beter beslissen.
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Shewhart (1931); ISO 7870-2
</div>

<!--
Slide 9 — Shewhart expliciet.

"Wat verandert niet? Dit."
Wijs naar het gele strookje in het diagram achter in de zaal.
Wijs naar de zin op de flip-over.

"Shewhart bedacht in 1931: is dit signaal, of is dit ruis?
Die vraag zit onder elke regelkaart én onder elk dashboard.
Bron: Shewhart 1931, vandaag nog de basis van ISO 7870-2."

Eén-zins-afsluiter (1.5 min):
"Iedereen — één zin: wat verandert volgens jou het meest, én wat blijft exact hetzelfde?"
Laat 3-4 deelnemers kort delen.

Slagingscriterium: minstens één noemt detectie/reactietijd als verandering,
minstens één noemt Shewhart/signaal-ruis als gelijkblijvend.

Valkuil: "Shewhart is 100 jaar oud":
"Precies — en daar is-ie nog. ISO 7870-2 is van 2013, bevestigt letterlijk wat hij in 1931 opschreef.
Het gereedschap verandert, de vraag niet."

Valkuil: "Dus alarmen moet ik altijd vertrouwen":
"Andersom — een te streng ingestelde regel piept ook zonder reden.
Dat heet valse alarmen. Shewhart-vraag blijft ook bij een dashboard-alarm."
-->

---
layout: center
class: text-center
---

# Deze week op de werkvloer

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Loop <span class="font-bold">één keer bewust langs de schermen</span> op je werkvloer.<br/>
  Noteer per scherm: welke meting? Welke grens? Welk alarm?
</div>

<div v-click class="mt-10 inline-block px-6 py-3 bg-blue-50 text-blue-900 rounded-lg text-base max-w-xl mx-auto">
  Weet je het niet? <span class="font-bold">Schrijf op wat je ziet</span><br/>
  <span class="text-sm opacity-70">en wat je je afvraagt.</span>
</div>

<div v-click class="mt-6 text-sm opacity-60 max-w-xl mx-auto">
  Bonus: vraag een collega of teamleider — <span class="italic">"Wie bepaalt wanneer dit dashboard alarm geeft?"</span>
</div>

<!--
Transferopdracht (30 sec) + afsluiter.

"Deze week één keer bewust langs de schermen op je werkvloer.
Per scherm: welke meting zie ik? Welke grens of alarm zit eronder?
Als je het niet weet — schrijf op wat je ziet en wat je je afvraagt."

"In module 2 (Train) ga je hier zelf een regel op instellen. Begin dus met jouw lijstje.
Neem je handout (wb-03) mee."

"Bonus-vraag aan collega of teamleider: 'Wie bepaalt eigenlijk wanneer dit dashboard alarm geeft?'
Het antwoord is leerzaam — soms een operator, soms een leverancier, soms een AI.
Dat maakt uit voor hoe je het alarm moet lezen."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop-blok: <span class="font-bold">common cause vs special cause — herkennen</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik) · ko-spc-103
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (lo-spc-104 — common/special cause herkennen, 45 min).

Werkbladen 1 en 2 innemen of foto's maken voor learning analytics.
Werkblad 3 (handout) gaat MEE naar de werkvloer — niet innemen.

Notities voor jezelf na afloop:
- Hoeveel turfjes kreeg elke kolom bij vraag 5 (wat weet jij onder het scherm)?
- Welke verschuiving herkenden deelnemers het snelst?
- Welk eigen voorbeeld van de werkvloer kwam vaak terug?
- Welke valkuil viel op (Shewhart-oud / dashboard-is-beter / alarmen-altijd-vertrouwen)?

Verstuur xAPI-statements:
- experienced (vergelijking wb-01)
- completed (STARRT wb-02, handout wb-03)
- attempted (transferopdracht — dashboard-inventarisatie)
-->
