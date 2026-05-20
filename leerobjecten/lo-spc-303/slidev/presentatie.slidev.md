---
theme: default
title: Capability-valkuilen — drie voorwaarden vóór het getal telt
info: |
  ## SPC Module 3 — Op Maat
  Workshop-blok over capability-valkuilen: toetsen van Cp/Cpk/Pp/Ppk aan
  drie voorwaarden (meetsysteem, stabiliteit, subgroepering).
  Doelgroep: teamleiders MBO-4/HBO, 45 minuten, coachende stijl.
  Bronnen inline: AIAG MSA, Ford PPAP, NIST/SEMATECH.
  v1.0
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Capability-valkuilen

### Drie voorwaarden vóór het getal telt

<div class="mt-12 text-sm opacity-60">
  SPC Module 3 (Op Maat) · Workshop-blok · 45 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Teamleiders MBO-4 + HBO · Eigen Cpk-getal kritisch toetsen
</div>

<!--
SLIDE 1 — Cover. Open warm en direct.

"Welkom. In module 3 werken jullie aan eigen lijnen. Vorig blok de DMAIC-skeleton —
vandaag één scherpe vraag: als er straks op jouw bureau 'Cpk = 1,5' verschijnt,
weet je dan of dat getal een beslissing mag sturen? Ik ga jullie vandaag weinig vertellen —
de meeste vragen zijn aan jullie."

Toon coachend, niet doceren. De doelgroep kent Cp/Cpk al — laat ze dat voelen.

Verwijs naar draaiboek blok 1, instructie 1.
-->

---
layout: center
class: text-center
---

# "Cpk = 1,5 voor onze nieuwe productlijn."

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-80">
  Klinkt goed. <span class="font-bold">Mag je er een beslissing op baseren?</span>
</div>

<div v-click class="mt-10 grid grid-cols-3 gap-4 max-w-3xl mx-auto">
  <div class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Was het proces stabiel?</div>
    <div class="text-xs mt-2 opacity-70">Regelkaart over de meetperiode?</div>
  </div>
  <div class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Hoe waren de subgroepen?</div>
    <div class="text-xs mt-2 opacity-70">Eén bron per subgroep?</div>
  </div>
  <div class="p-4 bg-red-50 rounded-lg border-l-4 border-red-400">
    <div class="font-bold text-red-800">Is het meetsysteem gevalideerd?</div>
    <div class="text-xs mt-2 opacity-70">Gage R&amp;R volgens AIAG?</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-80 max-w-xl mx-auto">
  Eén "onbekend" = het getal stuurt nog geen beslissing.
</div>

<!--
SLIDE 2 — Trigger-slide. Coachende vraag eerst, dan pas de drie vragen tonen.

Stel coachende vraag aan de groep:
"Wie heeft ooit een Cpk-getal gezien waarvan je achteraf dacht: dat klopte niet?"

Wacht. Tel innerlijk tot 7. Vang 1-2 antwoorden.

Dan pas de drie blokjes onthullen met v-click — bevestig:
"Precies — de vraag vandaag is hoe je dat ontdekt vóór de beslissing valt, niet erna."

Daarna: deel wb-03-handout uit:
"Pak je markeerstift. Markeer wat je herkent van je eigen lijn, markeer ook wat nieuw voor je is.
We lopen samen door de drie valkuilen en de volgorde."

Verwijs naar draaiboek blok 1, instructie 2-3.
-->

---

# De drie voorwaarden

<div class="grid grid-cols-3 gap-4 mt-8">
  <div v-click class="text-center p-4 bg-blue-50 rounded-xl border-2 border-blue-200">
    <div class="text-3xl mb-2">📏</div>
    <div class="font-bold text-blue-800">1. Meetsysteem</div>
    <div class="text-xs opacity-70 mt-2">Geschikt via Gage R&amp;R / MSA?</div>
    <div class="text-xs mt-2 font-bold text-blue-900">AIAG MSA · Ford PPAP</div>
  </div>
  <div v-click class="text-center p-4 bg-amber-50 rounded-xl border-2 border-amber-200">
    <div class="text-3xl mb-2">📈</div>
    <div class="font-bold text-amber-800">2. Stabiliteit</div>
    <div class="text-xs opacity-70 mt-2">Proces stabiel? SPC-regelkaart zonder signalen?</div>
    <div class="text-xs mt-2 font-bold text-amber-900">NIST/SEMATECH</div>
  </div>
  <div v-click class="text-center p-4 bg-purple-50 rounded-xl border-2 border-purple-200">
    <div class="text-3xl mb-2">🧩</div>
    <div class="font-bold text-purple-800">3. Subgroepen</div>
    <div class="text-xs opacity-70 mt-2">Rationeel? Eén bron, dicht in tijd?</div>
    <div class="text-xs mt-2 font-bold text-purple-900">AIAG · ko-spc-109</div>
  </div>
</div>

<div v-click class="mt-8 text-center text-sm opacity-80 max-w-2xl mx-auto p-3 bg-gray-100 rounded-lg">
  <span class="font-bold">Drie keer "ja met bron"</span> = getal bruikbaar.
  <span class="font-bold">Eén "onbekend"</span> = eerst uitzoeken.
  <span class="font-bold">Eén "nee"</span> = herrekenen na correctie.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Diagram lo-spc-303 — drie voorwaarden + %GRR-drempels
</div>

<!--
SLIDE 3 — Centrale didactische slide. Drie voorwaarden overzicht.

Wijs naar de A3-print achter in de zaal (diagram-lo-spc-303.svg).

Werkvorm: per voorwaarde niet zelf vertellen — vraag de groep.
Per voorwaarde ~2 min:

Voorwaarde 1 (meetsysteem):
Onthul met v-click. Vraag: "Wanneer werd op jouw lijn een capability berekend zonder
eerst het Gage R&R-rapport te checken?" Wacht 5-7 sec. Vang één antwoord.
Bron: "Ford PPAP eist MSA vóór capability — automotive-audit-vereiste."

Voorwaarde 2 (stabiliteit):
Onthul met v-click. Vraag: "Op jouw lijn — is er over de capability-meetperiode een
regelkaart gedraaid?" Bron: "NIST/SEMATECH — capability-formules zijn alleen geldig op
een statistisch stabiel proces."

Voorwaarde 3 (subgroepen):
Onthul met v-click. Vraag: "Hoe waren de subgroepen samengesteld bij de laatste Cpk?"
Bron: "AIAG — rationele subgroepen, één bron per subgroep. Zie ko-spc-109."

Dan laatste v-click: de gate-regel.

Verwijs naar draaiboek blok 1, instructie 4.
Verwijst naar trainee-SVG: diagram-lo-spc-303.svg.
-->

---
layout: center
class: text-center
---

# %GRR-drempels (AIAG MSA 4e)

<div class="grid grid-cols-3 gap-6 mt-10 max-w-4xl mx-auto">
  <div v-click class="p-6 bg-green-50 rounded-xl border-2 border-green-300">
    <div class="text-4xl font-bold text-green-700">&lt; 10%</div>
    <div class="text-xs uppercase opacity-60 mt-2">AIAG-norm</div>
    <div class="font-bold text-green-800 mt-3">Geschikt</div>
    <div class="text-xs opacity-70 mt-2">Bewezen bruikbaar voor capability</div>
  </div>
  <div v-click class="p-6 bg-amber-50 rounded-xl border-2 border-amber-300">
    <div class="text-4xl font-bold text-amber-700">10 – 30%</div>
    <div class="text-xs uppercase opacity-60 mt-2">AIAG-norm</div>
    <div class="font-bold text-amber-800 mt-3">Marginaal</div>
    <div class="text-xs opacity-70 mt-2">Conditioneel — verbetering overwegen</div>
  </div>
  <div v-click class="p-6 bg-red-50 rounded-xl border-2 border-red-300">
    <div class="text-4xl font-bold text-red-700">&gt; 30%</div>
    <div class="text-xs uppercase opacity-60 mt-2">AIAG-norm</div>
    <div class="font-bold text-red-800 mt-3">Niet geschikt</div>
    <div class="text-xs opacity-70 mt-2">Niet bruikbaar voor capability</div>
  </div>
</div>

<div v-click class="mt-10 text-base opacity-80 max-w-2xl mx-auto p-3 bg-gray-100 rounded-lg">
  <span class="font-bold">Ford PPAP:</span> geen capability-indiening zonder voorafgaande MSA.
</div>

<!--
SLIDE 4 — %GRR-drempelwaarden. De harde AIAG-norm.

Onthul per zone met v-click.

"%GRR zegt: hoeveel van je gemeten variatie komt uit de meter, niet uit het proces?
AIAG MSA 4e zet de drempels. Onder 10 procent: meter is bewezen geschikt.
Tussen 10 en 30: marginaal — conditioneel te gebruiken, maar verbetering overwegen.
Boven 30: niet bruikbaar voor capability — je meet de ruis van je meter."

Vraag coachend: "Wie weet hier het %GRR van het meetsysteem waarop de laatste
Cpk op zijn lijn berekend is?" Stilte. Dat is het leermoment.

Bevestig: "Dit is het punt. Ford PPAP eist Gage R&R expliciet vóór capability."

Verwijs naar draaiboek blok 1, instructie 4 (valkuil 3 — Slecht meetsysteem).
-->

---

# De juiste volgorde

<div class="mt-6 space-y-2 max-w-3xl mx-auto">

<div v-click class="flex items-center gap-4 p-3 bg-blue-50 rounded-lg">
  <div class="text-xl font-bold text-blue-700 w-8">1</div>
  <div class="flex-1">
    <div class="font-bold">Meetsysteem geschikt?</div>
    <div class="text-xs opacity-70">Gage R&amp;R / MSA volgens AIAG MSA 4e</div>
  </div>
  <div class="text-blue-400">↓ Ja</div>
</div>

<div v-click class="flex items-center gap-4 p-3 bg-amber-50 rounded-lg">
  <div class="text-xl font-bold text-amber-700 w-8">2</div>
  <div class="flex-1">
    <div class="font-bold">Proces stabiel?</div>
    <div class="text-xs opacity-70">SPC-regelkaart — geen out-of-control signalen</div>
  </div>
  <div class="text-amber-400">↓ Ja</div>
</div>

<div v-click class="flex items-center gap-4 p-3 bg-purple-50 rounded-lg">
  <div class="text-xl font-bold text-purple-700 w-8">3</div>
  <div class="flex-1">
    <div class="font-bold">Verdeling redelijk?</div>
    <div class="text-xs opacity-70">Normaliteit-check (histogram / I-chart)</div>
  </div>
  <div class="text-purple-400">↓ Ja</div>
</div>

<div v-click class="flex items-center gap-4 p-3 bg-green-50 rounded-lg">
  <div class="text-xl font-bold text-green-700 w-8">4</div>
  <div class="flex-1">
    <div class="font-bold">Capability berekenen</div>
    <div class="text-xs opacity-70">Cp, Cpk, Pp, Ppk</div>
  </div>
  <div class="text-green-400">↓</div>
</div>

<div v-click class="flex items-center gap-4 p-3 bg-gray-100 rounded-lg">
  <div class="text-xl font-bold text-gray-700 w-8">5</div>
  <div class="flex-1">
    <div class="font-bold">Beslissingen nemen — nu onderbouwd</div>
    <div class="text-xs opacity-70">Vrijgave · investering · escalatie</div>
  </div>
</div>

</div>

<div v-click class="mt-4 text-center text-sm opacity-70">
  Elke stap overgeslagen = elke beslissing minder onderbouwd.
</div>

<!--
SLIDE 5 — Stroomschema juiste volgorde. Verwijs naar A3-diagram achter in zaal.

"Vier poortjes: MSA, stabiliteit, verdeling, capability. Elke poort overgeslagen =
elke beslissing daarna minder onderbouwd. De fictieve case in je handout:
iemand claimt Cpk = 1,5 — drie vragen onthullen dat alle drie de poortjes niet
gecheckt zijn. Je gaat zo hetzelfde doen met jouw eigen getal."

Markeer expliciet bij het noemen: "Dit is een fictieve case ter illustratie —
niet uit één specifiek bedrijf."

Verwijs naar draaiboek blok 1, instructie 5.
-->

---
layout: section
---

# Experimenteren

## Eigen capability-getal toetsen — 20 min

<div class="text-base mt-8 opacity-80 max-w-2xl mx-auto">
  Tot zover de structuur. Nu de echte vraag: jouw eigen getal.<br/>
  <span class="font-bold mt-4 block">Pak wb-01 uit je stapel. Laat wb-03 open op tafel als naslag.</span>
</div>

<!--
SLIDE 6 — Overgang naar blok 2 (experimenteren).

"Tot zover de structuur. Nu de echte vraag: jouw eigen getal. Pak wb-01 uit je stapeltje.
Laat wb-03 open op tafel als naslag."

Maak de pedagogische overgang expliciet: van "we lopen samen door" (blok 1, geleide coaching)
naar "jij doet, ik vraag" (blok 2, individueel coaching).

Verwijs naar draaiboek blok 2, instructie 1.
-->

---

# Wat ga je nu doen?

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Het werkblad (wb-01)
<v-clicks>

1. Schrijf bovenaan: **welk getal, welke bron, welke beslissing**
2. Werk **top-down**: voorwaarde 1 → 2 → 3
3. Per voorwaarde: **ja / nee / onbekend + bron**
4. Formuleer **drie vragen** aan de rapporteur
5. Eindig met **één maandag-actie**

</v-clicks>

</div>

<div>

### Hulpvragen
<v-clicks>

- Wanneer was de laatste Gage R&amp;R op deze meter?
- Is er over dezelfde periode een regelkaart gedraaid?
- Was er één bron per subgroep?
- Welke beslissing hangt af van dit getal?
- Wie is de rapporteur — wie bel je?

</v-clicks>

</div>

</div>

<div class="abs-br m-6 text-xs opacity-40">
  15 min · individueel · A3 werkblad · wb-03 als referentie
</div>

<!--
SLIDE 7 — wb-01-instructie. Toon de instructie. Zet timer op 15 min.

Belangrijke instructie aan jezelf als trainer:
- Loop rond, buig je niet over schouders.
- Bij stagnatie: stel ÉÉN doorvraag per voorwaarde uit de bibliotheek in het draaiboek.
- GEEF GEEN OPLOSSINGEN. Vervang elke neiging tot voorbeeld door een vraag.
- Bij blokkade: drie-zinnen-aanpak — vraag → wacht 5 sec → bevestig wat hij al heeft → stilte.

PLAN-B (zie draaiboek blok 2, gele box):
Bij 10 min visuele check. Als > 50 % nog bij voorwaarde 1 hangt:
"Focus op de voorwaarde die voor jouw getal het meest onbekend is — de andere twee kun je
na de sessie afmaken."

Deelnemer zonder eigen getal:
"Pak de fictieve case uit wb-03 als werkmateriaal."

Halverwege (7,5 min): zachte tafelklap.
"Halverwege. Heb je alle drie de voorwaarden aangeraakt? Als voorwaarde 3 nog leeg is,
ga er nu naartoe — die wordt het vaakst vergeten."

Eindsignaal:
"Pen neer. Drie vragen aan de rapporteur + één maandag-actie — dat is het harde resultaat."

Verwijs naar draaiboek blok 2, volledige instructie.
-->

---
layout: section
---

# Reflecteren

## STARRT op wb-02 — 13 min

<!--
SLIDE 8 — Overgang naar blok 3 (reflectie + deelronde).

"STARRT — zes velden. Situatie, Taak, Actie, Resultaat, Reflectie, Transfer.
Kort en concreet. Eindig met de maandag-actie op de laatste pagina.
Dat is de zin die je zo plenair uitspreekt."

Zet timer op 9 min voor individueel schrijven.
Loop rustig rond, kijk niet mee — geef rust.

Verwijs naar draaiboek blok 3, instructie 1-2.
-->

---
layout: center
class: text-center
---

# Eén zin — maandag-actie

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Wat doe je <span class="font-bold">maandagochtend</span> om 9:00?
</div>

<div v-click class="mt-8 grid grid-cols-3 gap-3 max-w-3xl mx-auto">
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag vraag ik het Gage R&amp;R-rapport op bij kwaliteit voor lijn 3."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag haal ik de regelkaart-uitdraai over de capability-periode op."</div>
  </div>
  <div class="p-3 bg-blue-50 rounded-lg text-sm text-left">
    <div class="font-bold text-blue-900 text-xs uppercase opacity-70 mb-1">Voorbeeld</div>
    <div>"Maandag vraag ik hoe de subgroepen in het SPC-plan zijn gedefinieerd."</div>
  </div>
</div>

<div v-click class="mt-8 text-base opacity-80 max-w-xl mx-auto">
  Niet 'ik ga nadenken' — <span class="font-bold">één concrete actie</span>.<br/>
  <span class="text-sm opacity-70">Bellen, mailen, opvragen. Klein en uitvoerbaar.</span>
</div>

<!--
SLIDE 9 — Maandag-actie en één-zin-deelronde.

"Pen neer. Plenair rondje. Eén zin per persoon: wat ga je maandag anders doen —
concreet, met naam en datum. Ik begin."

Trainer eerst, modelleert de kortheid.
Dan kring rond. Knik naar volgende. Strak: 15 sec per persoon.
Geen reactie, geen vervolgvraag.

VALKUIL: één-zin-ronde wordt drie-zinnen-ronde.
Zacht handgebaar bij 15 sec. "Dank — volgende."

Bij "ik weet het nog niet":
"Wat is de kleinste stap die je morgen nog kunt zetten? Bellen, mailen, vragen —
niet oplossen, één stap."

Verwijs naar draaiboek blok 3, instructie 3.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende blok in module 3: <span class="font-bold">Six Sigma belt-rollen</span> (ko-spc-403)<br/>
  <span class="text-sm opacity-60">Wie heb je nodig in je team om MSA of DMAIC goed uit te voeren?</span>
</div>

<div class="mt-6 text-sm opacity-60 max-w-xl mx-auto">
  Neem wb-01 mee — de maandag-actie onderaan is je werkdocument voor deze week.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 3 (Op Maat) · Capability-valkuilen · v1.0
</div>

<!--
SLIDE 10 — Afsluiter. Bedank de groep. Kondig het volgende blok aan (Six Sigma belt-rollen, ko-spc-403).

"Wat jullie net hebben gedaan: één echt getal langs drie voorwaarden leggen.
Dat is het verschil tussen getallen napraten en er grip op hebben.
Neem wb-01 mee — maandag-actie onderaan is het werkdocument voor deze week."

Notities voor jezelf na afloop:
- Foto's gemaakt van alle wb-01 (met toestemming)?
- Welke voorwaarde bleek het vaakst 'onbekend' (input voor follow-up)?
- Welke maandag-acties zijn opgeschreven (input voor opvolg-coaching)?
- Parkeerflip-vragen overgedragen aan trainer ko-spc-403?

Verwijs naar draaiboek "Checklist na de sessie".
-->
