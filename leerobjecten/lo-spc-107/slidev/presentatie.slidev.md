---
theme: default
title: Control limits versus specificatiegrenzen
info: |
  ## SPC Module 1 — Gebruik
  Workshop-blok over het verschil tussen control limits (UCL/LCL) en specificatiegrenzen.
  Doelgroep: operators MBO-3, 40 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Proces-grens of product-grens?

### Control limits versus specificatiegrenzen

<div class="mt-12 text-sm opacity-60">
  SPC Module 1 (Gebruik) · Workshop-blok · 40 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
Welkom. Open de sessie.
"Op veel werkvloeren hangen regelkaarten aan de wand. Er staan lijnen op — een bovengrens,
een ondergrens. Maar wie heeft die lijnen getekend, en waarop zijn ze gebaseerd?
Dat is de vraag van deze 40 minuten."

De vraag: zijn de lijnen op de kaart de grenzen van het PROCES of van het PRODUCT?
Blok 1 (15 min): ervaren — drie voorbeeld-kaarten, welke is fout?
Blok 2 (12 min): reflecteren — hoe zit het op jouw eigen lijn?
Blok 3 (13 min): theoretiseren — de formule, de NIST-waarschuwing, de vier scenario's.
-->

---
layout: two-cols
layoutClass: gap-8
---

# De klant vraagt 100 ± 1 gram

Spuitgietlijn — onderdeelgewicht.

<v-clicks>

- **Specs van de klant:** 99 g (onder) tot 101 g (boven)
- **Dit komt uit:** contract of tekening
- **Zijn dat ook de lijnen op de regelkaart?**

</v-clicks>

<div v-click class="mt-10 p-4 bg-amber-50 rounded-lg text-sm">
Dat is de valstrik. <span class="font-bold">Specs zeggen iets over het product. De regelkaart zegt iets over het proces.</span> Twee verschillende vragen.
</div>

::right::

<div class="h-full flex items-center justify-center">
  <div class="text-center">
    <div class="text-6xl mb-4">⚖️</div>
    <div class="text-3xl font-mono font-bold text-blue-700">100 ± 1 g</div>
    <div class="text-sm opacity-60 mt-2">specs: 99 – 101 g</div>
    <div class="text-xs opacity-50 mt-4">spuitgietlijn · klantopdracht</div>
  </div>
</div>

<!--
Slide 2 — klantspecs intro.

"We kijken naar een spuitgietlijn. De klant vraagt onderdeelgewicht 100 ± 1 g.
Dus de specs zijn 99 tot 101 g. Dat is wat de klant wil.
Vraag: zijn dat ook de lijnen die op de regelkaart horen te staan?"

Laat de vraag hangen. Deel daarna wb-01-spot-the-fout uit.
"Je krijgt drie regelkaarten van dezelfde klant. Eén is fout opgezet.
Vind welke, en leg in één zin uit waarom. Bij twijfel: vraagteken."
-->

---

# Kaart A — trainer doet voor (IK DOE)

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Wat staat er op de kaart?
- Klantspecs: **99 – 101 g**
- Gemiddelde uit 100 metingen: **99,9 g**
- Standaardafwijking σ: **0,12 g**
- **UCL op de kaart:** 100,26 g
- **LCL op de kaart:** 99,54 g
- Specs staan apart aangegeven op 99 en 101

</div>

<div>

### Wat zie je?
<v-clicks>

- UCL/LCL liggen **binnen** de specs
- Berekend: 99,9 + 3 × 0,12 = **100,26**
- Berekend: 99,9 − 3 × 0,12 = **99,54**
- Specs staan er **apart** op
- **Goed opgezet**

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-3 bg-green-50 rounded-lg text-sm max-w-3xl mx-auto">
Twee vragen — twee aparte grenzen. UCL/LCL uit <span class="font-mono">gemiddelde ± 3σ</span> vertellen of het proces stabiel loopt. Specs vertellen of het stuk naar de klant mag.
</div>

<!--
Slide 3 — IK DOE voor kaart A (3 min).

Lees hardop: "Gemiddelde 99,9, sigma 0,12. UCL op 100,26 en LCL op 99,54.
Specs staan apart op 99 en 101."

"Wat valt op? De UCL/LCL liggen BINNEN de specs. Dat is geen toeval —
die zijn berekend uit 100 metingen van de eigen lijn met de formule UCL = gemiddelde + 3σ.
Deze kaart beantwoordt de vraag: loopt mijn proces stabiel?
De specs staan er apart op voor de tweede vraag: mag dit naar de klant?
Twee vragen, twee aparte grenzen. Deze kaart: goed opgezet."

Na deze slide: deelnemers zelf kaart B en C beoordelen (7 min).
Daarna buurman-check (2 min). Plenaire verzamel (2 min).
Bevestig dat kaart B fout is — UCL/LCL zijn gelijk aan specs.
-->

---
layout: section
---

# Reflecteren

## Hoe zit het op jouw eigen kaart?

<!--
Overgang naar blok 2 (reflecteren, 12 min).

"Nu kijken we naar jullie eigen werkplek.
Veel operators weten niet precies hoe de lijnen op hun kaart zijn bepaald.
Dat is geen zwakte — dat is vaak gewoon nooit uitgelegd.
Eerlijk opschrijven is hier de kunst."

Deel wb-02-reflectie uit (STARRT-structuur).
7 min individueel, 3 min tweetallen, 2 min plenair handen tellen.
-->

---
layout: image-right
image: ./diagram-lo-spc-107.svg
backgroundSize: contain
---

# Twee vragen, twee grenzen

<v-clicks>

1. **Control limits (UCL / LCL)**
   Is mijn PROCES stabiel?
   Berekend uit procesdata (<span class="font-mono">gemiddelde ± 3σ</span>)

2. **Specificatiegrenzen (USL / LSL)**
   Voldoet het PRODUCT aan de eisen?
   Van de klant of uit het ontwerp

</v-clicks>

<div v-click class="mt-8 text-sm opacity-70">
Op de regelkaart: UCL/LCL altijd. Specs apart getoond — of helemaal niet op de kaart.
</div>

<div class="abs-bl m-6 text-xs opacity-40">
  Bron: NIST/SEMATECH e-Handbook · Shewhart 1931 · ISO 7870-2
</div>

<!--
Slide 4 — onthul eerst het A3-diagram achter in de zaal.
Toon dan deze slide met het diagram rechts.

"Dit is waar we naartoe werken. Links op het diagram zie je een regelkaart —
zo hoort het. UCL en LCL uit de procesdata, specs apart getoond.
Rechts zie je vier mogelijke situaties die je kaart kan laten zien.
We lopen ze zo langs."

Deel wb-03-handout-verschil-control-vs-specs uit.
"Pak je markeerstift. Markeer wat voor jou een aha-moment is.
Dit werkblad neem je mee — het is je naslagwerk."
-->

---

# De vergelijking in één tabel

<div class="mt-4 text-sm">

| | **Control limits (UCL/LCL)** | **Specificatiegrenzen (USL/LSL)** |
|---|------------------------------|-----------------------------------|
| **Welke vraag?** | Is het PROCES stabiel? | Voldoet het PRODUCT? |
| **Waar komen ze vandaan?** | Uit eigen procesdata (gemiddelde ± 3σ) | Van de klant of het ontwerp |
| **Waar op de kaart?** | Op de regelkaart | Apart — of niet op de kaart |
| **Welke beslissing?** | "Moet ik ingrijpen in het proces?" | "Mag dit naar de klant?" |
| **Verandert met?** | Procesgedrag → nieuwe data → nieuwe limits | Klantafspraak of ontwerpwijziging |

</div>

<div v-click class="mt-6 p-3 bg-red-50 rounded-lg text-sm max-w-2xl mx-auto">
Op kaart B uit de oefening stond één lijn die twee vragen tegelijk moest beantwoorden. <span class="font-bold">Dat kan niet.</span>
</div>

<!--
Slide 5 — vergelijkingstabel (3 min).

Lees hardop de vier regels langs. Per regel:
- "Welke vraag beantwoordt elke grens?"
- "Waar komen ze vandaan?"
- "Waar staan ze op de kaart?"
- "Welke beslissing volgt?"

Wijs fysiek terug naar kaart B uit blok 1:
"Op die foute kaart stond één lijn die twee vragen tegelijk moest beantwoorden.
Dat kan niet."

Schrijf op de flip-over:
- kolom PROCES (UCL/LCL): "uit data, 3σ, is proces stabiel?"
- kolom PRODUCT (USL/LSL): "van klant, mag dit naar klant?"
-->

---
layout: two-cols
layoutClass: gap-8
---

# De 3σ-formule (Shewhart, 1931)

### De oorspronkelijke formule

```
UCL = gemiddelde + 3σ
LCL = gemiddelde − 3σ
```

<v-clicks>

- Wat je nodig hebt: **25-30 metingen** van een stabiel lopend proces
- Gemiddelde + standaardafwijking σ
- Bij een stabiel normaal proces zit **99,7%** van je metingen tussen UCL en LCL
- Iets daarbuiten? Bijna zeker een echt signaal

</v-clicks>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-5xl mb-2">📐</div>
    <div class="text-base opacity-70">Bron: Shewhart, W.A. (1931)</div>
    <div class="text-xs opacity-50 mt-1"><em>Economic Control of Quality of Manufactured Product</em></div>
  </div>

  <div v-click class="p-4 bg-blue-50 rounded-lg text-sm">
    <div class="font-bold text-blue-800 mb-1">Kaart A uit de oefening:</div>
    Gemiddelde 99,9 g, σ = 0,12 g<br/>
    UCL = 99,9 + 3 × 0,12 = <span class="font-mono font-bold">100,26 g</span><br/>
    LCL = 99,9 − 3 × 0,12 = <span class="font-mono font-bold">99,54 g</span>
  </div>
</div>

<!--
Slide 6 — de 3σ-formule (3 min).

"Deze formule komt van Walter A. Shewhart. Hij werkte bij Bell Labs en schreef
in 1931 het boek waarin de regelkaart werd uitgevonden. De formule komt hiervandaan."

"UCL = gemiddelde + 3σ, LCL = gemiddelde − 3σ. Die 3σ is niet willekeurig —
bij een stabiel normaal proces zit 99,7% van je metingen binnen die grenzen.
Dus als er iets buiten komt, is dat bijna zeker een echt signaal en geen toeval."

Reken hardop voor bij kaart A:
"Gemiddelde 99,9, sigma 0,12. 3 × 0,12 is 0,36.
99,9 + 0,36 = 100,26. 99,9 − 0,36 = 99,54.
Dat zijn precies de control limits die op kaart A stonden."

NIET in de statistische diepte duiken. Geen normaalverdeling-grafiek.
De 99,7%-vuistregel is genoeg voor MBO-3.

MBO-4 differentiatie: verwijs wie verder wil naar ISO 7870-2.
-->

---
layout: two-cols
layoutClass: gap-6
---

# NIST waarschuwt

### Twee scenario's die vaak worden gemist

<div class="mt-4 p-4 bg-amber-50 rounded-lg text-sm">
<div class="font-bold text-amber-900 mb-2">Scenario 1</div>
Een proces kan <span class="font-bold">stabiel</span> zijn (binnen control limits) en toch <span class="font-bold">te dicht bij de specificatiegrens</span> zitten.
</div>

<div v-click class="mt-3 p-4 bg-red-50 rounded-lg text-sm">
<div class="font-bold text-red-900 mb-2">Scenario 2</div>
Een proces kan incidenteel <span class="font-bold">binnen specs</span> produceren terwijl het proces <span class="font-bold">al uit controle is</span>.
</div>

::right::

<div class="h-full flex flex-col justify-center">
  <div class="text-center mb-6">
    <div class="text-5xl mb-2">⚠️</div>
    <div class="text-xl font-bold">Binnen specs ≠ onder controle</div>
    <div class="text-sm opacity-70 mt-2">twee aparte vragen · twee aparte grenzen</div>
  </div>

  <div v-click class="p-3 bg-gray-50 rounded-lg text-xs">
    <div class="font-bold mb-1">Bron:</div>
    NIST/SEMATECH e-Handbook of Statistical Methods<br/>
    <em>Control Charts versus Specification Limits</em><br/>
    <span class="opacity-60">itl.nist.gov/div898/handbook</span>
  </div>
</div>

<!--
Slide 7 — NIST-waarschuwing (3 min).

"Dit is een waarschuwing uit het NIST/SEMATECH e-Handbook of Statistical Methods —
een referentiewerk voor proces- en meetbeheersing. Twee scenario's."

Lees voor:
"Een proces kan stabiel zijn én toch te dicht bij de specificatiegrens zitten.
Omgekeerd: een proces kan incidenteel binnen specs produceren terwijl
het proces al uit controle is."

Wijs naar de flip-over "Binnen specs ≠ onder controle":
"Dat is de kern. Binnen specs zegt niets over het proces.
Uit controle zegt niets over afkeur. Twee aparte dingen."

"De vier-scenario-matrix rechts op je handout laat precies zien
wat je doet in welke situatie. Die gaan we nu even langs."
-->

---

# Vier scenario's — wat doe je?

<div class="mt-6 grid grid-cols-2 gap-4 text-sm">

<div v-click class="p-4 bg-green-50 rounded-lg border-l-4 border-green-500">
<div class="font-bold text-green-800 mb-1">Stabiel + bekwaam</div>
<div class="text-xs opacity-70 mb-2">binnen UCL/LCL + binnen specs</div>
<div class="font-bold">Laat lopen</div>
<div class="text-xs opacity-70">Dit is wat je wilt.</div>
</div>

<div v-click class="p-4 bg-yellow-50 rounded-lg border-l-4 border-yellow-500">
<div class="font-bold text-yellow-800 mb-1">Stabiel + onbekwaam</div>
<div class="text-xs opacity-70 mb-2">stabiel maar vlak tegen specs</div>
<div class="font-bold">Capability verbeteren</div>
<div class="text-xs opacity-70">Minder spreiding nodig.</div>
</div>

<div v-click class="p-4 bg-red-50 rounded-lg border-l-4 border-red-500">
<div class="font-bold text-red-800 mb-1">Onstabiel + bekwaam</div>
<div class="text-xs opacity-70 mb-2">buiten UCL/LCL, toevallig binnen specs</div>
<div class="font-bold">Ingrijpen — nu</div>
<div class="text-xs opacity-70">Hier bewijst SPC zijn waarde.</div>
</div>

<div v-click class="p-4 bg-orange-50 rounded-lg border-l-4 border-orange-500">
<div class="font-bold text-orange-800 mb-1">Onstabiel + onbekwaam</div>
<div class="text-xs opacity-70 mb-2">stabiel maar buiten specs</div>
<div class="font-bold">Centreren</div>
<div class="text-xs opacity-70">Proces draait op verkeerde instelling.</div>
</div>

</div>

<div v-click class="mt-6 text-center text-sm max-w-2xl mx-auto opacity-80">
Het <span class="font-bold text-red-700">rode scenario</span> is waar SPC zijn waarde bewijst: <span class="font-bold">je grijpt in voordat de klant klaagt.</span>
</div>

<!--
Slide 8 — de 4-scenario-matrix (2 min).

Per vak één zin:
1. "Proces stabiel én binnen specs: laat lopen."
2. "Proces stabiel, maar vlak tegen de specs: capability verbeteren, minder spreiding."
3. "Proces niet meer stabiel, producten toevallig nog binnen specs:
    ingrijpen — DIT is het scenario waar SPC zijn waarde bewijst."
4. "Proces stabiel, maar producten buiten specs: centreren —
    je proces draait op een verkeerde instelling."

Benadruk scenario 3 — dat is waar het onderscheid tussen control limits en specs
écht betaalt. Alleen met correcte control limits (niet = specs) zie je dit gebeuren.

Korte vraagronde (30 sec): "Welke regel op de vergelijkingstabel had je niet zo scherp?"
Laat 1-2 mensen delen.
-->

---
layout: center
class: text-center
---

# Deze week op de werkvloer

<div class="text-xl mt-6 max-w-2xl mx-auto leading-relaxed opacity-90">
  Ga naar <span class="font-bold">één regelkaart op jouw lijn.</span><br/>
  Kijk welke lijnen erop staan. Noteer de waarden.
</div>

<div v-click class="mt-8 p-4 bg-blue-50 text-blue-900 rounded-lg text-base max-w-2xl mx-auto">
  Vraag aan je teamleider of SPC-coördinator:<br/>
  <span class="font-bold italic">"Komen deze grenzen uit klantspecs, of uit 3σ-berekening?"</span>
</div>

<div v-click class="mt-6 text-sm opacity-70 max-w-2xl mx-auto">
  Bonus: hangen er kaarten met specs én control limits allebei? <br/>
  <span class="opacity-90">Dat is juist goede praktijk. Neem de notitie mee naar de volgende sessie.</span>
</div>

<!--
Slide 9 — afsluiting en transfer (1 min).

"Deze week: ga naar één regelkaart op jouw lijn. Kijk welke lijnen erop staan.
Noteer de waarden. Vraag aan je teamleider of SPC-coördinator:
komen deze uit de klantspecs of uit 3σ-berekening?
Noteer het antwoord.

Bonus: kijk of er kaarten hangen met specs én control limits allebei —
dat is juist goede praktijk.

Neem je notitie mee naar de volgende sessie."

Vergeet niet werkbladen 1 en 2 in te nemen of foto's te maken voor learning analytics.
Werkblad 3 (handout) gaat MEE naar de werkvloer — niet innemen.
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop-blok: <span class="font-bold">procesbekwaamheid (Cp, Cpk) — lo-spc-108</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · SPC Module 1 (Gebruik)<br/>
  Bronnen: NIST/SEMATECH e-Handbook · Shewhart 1931 · ISO 7870-2
</div>

<!--
Bedank de groep. Kondig het volgende blok aan (lo-spc-108: procesbekwaamheid).

Notitie voor jezelf na afloop:
- Hoeveel deelnemers wisten in blok 2 zeker waar hun eigen UCL/LCL vandaan komen?
- Welke vragen bleven hangen — meestal: "hoe bereken ik σ zelf?"
  (Antwoord: Excel STDEV, of SPC-software. Niet met de hand.)
- Heeft iemand tijdens blok 1 luidop gezegd dat kaart B "wel handig" is?
  Dat is een signaal dat het onderscheid in deze groep nog niet diep geland is —
  overweeg een korte herhaling in de volgende sessie.
-->
