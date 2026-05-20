---
theme: default
title: Autoencoder — AI leert wat normaal is
info: |
  ## Predictive Maintenance Module 2 — Train
  Workshop-blok over anomaliedetectie via autoencoder.
  Doelgroep: operators MBO-3, 30 minuten, hands-on.
author: AIMM × BronzGreen
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
---

# Autoencoder

### AI leert wat normaal is — en signaleert wat afwijkt

<div class="mt-12 text-sm opacity-60">
  Predictive Maintenance Module 2 (Train) · Workshop-blok · 30 min<br/>
  AIMM Curriculum · BronzGreen
</div>

<div class="abs-br m-6 text-xs opacity-40">
  Operators MBO-3 · spuitgieten / CNC / verpakking
</div>

<!--
"De komende 30 minuten kijken we naar een type AI dat leert wat normaal is.
Het wordt vandaag concreet: jij gaat eerst doen wat de AI doet."

Het woord 'autoencoder' valt nog niet in deze opening — bewaar voor fase 3.
-->

---
layout: center
class: text-center
---

# Storingsquiz

<div class="text-2xl mt-6 max-w-xl mx-auto leading-relaxed opacity-80">
  6 sensorgrafieken.<br/>
  Normaal of afwijkend?<br/>
  Schrijf op waaraan je het ziet.
</div>

<div v-click class="mt-10 text-base opacity-60 max-w-md mx-auto">
  Geen goed of fout. Jouw oordeel telt.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  5 min · individueel · wb-01-ervaren
</div>

<!--
Werkblad wb-01 uitdelen. Toon de 6 sensorgrafieken.
Zet timer op 5 min. Loop rond. Geen sturing.

Bij vastlopen: "Vergelijk met de andere grafieken — welke ziet er anders uit dan de rest?"

Niet voorzeggen.
-->

---
layout: section
---

# Hoe wist je het?

## Wat zag je in die grafieken?

<!--
Overgang naar blok 2.
-->

---

# Bespreek met je buurman

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-4xl mb-3">👀</div>
  <div class="text-base font-bold text-blue-700">Waar lette je op?</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-4xl mb-3">🤔</div>
  <div class="text-base font-bold text-purple-700">Wat was lastig?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-4xl mb-3">✨</div>
  <div class="text-base font-bold text-green-700">Voelde iets raar zonder uitleg?</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70 italic max-w-xl mx-auto">
  Jullie hebben een normaal-beeld in je hoofd, ook als niemand het je heeft uitgelegd.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  3 min duo · 3 min plenair · wb-02-reflecteren
</div>

<!--
Werkblad wb-02. Zet timer op 3 min duo.
Loop rond. Luister naar woorden als 'vorm', 'ritme', 'pieken'.

Plenair daarna 3 min — drie open vragen, schrijf sleutelwoorden op flap-over.

Sluit af: "Wat jullie net deden — leren wat normaal is door veel voorbeelden te zien — dat is precies wat AI doet."

Bij vraag 'is dit hetzelfde als die foto's van LO-006?': bevestig overeenkomst, benoem verschil:
'Visuele inspectie kent goed EN fout. Autoencoder kent alleen NORMAAL.'
-->

---
layout: section
---

# Theoretiseren

## Hoe werkt het — drie stappen

<!--
Overgang naar blok 3.
"Nu krijgt het een naam — en de naam klinkt erger dan het is."
-->

---
layout: center
class: text-center
---

# Auto-encoder

<div class="text-2xl mt-8 grid grid-cols-2 gap-8 max-w-2xl mx-auto">
  <div class="p-4 bg-blue-50 rounded-lg">
    <div class="text-3xl font-bold text-blue-700">auto</div>
    <div class="opacity-70 mt-2">vanzelf</div>
  </div>
  <div class="p-4 bg-purple-50 rounded-lg">
    <div class="text-3xl font-bold text-purple-700">encoder</div>
    <div class="opacity-70 mt-2">samenvatter</div>
  </div>
</div>

<div v-click class="mt-10 text-xl">
  Een <span class="font-bold">vanzelf-samenvatter.</span>
</div>

<div v-click class="mt-4 text-base opacity-60">
  Klinkt ingewikkeld. Is het niet.
</div>

<!--
Maak het woord onschadelijk. Geen drempel, geen mystiek.
"Auto = vanzelf. Encoder = samenvatter. Klaar."
-->

---

# De drie stappen

<div class="grid grid-cols-3 gap-6 mt-10">

<div class="p-6 bg-blue-50 rounded-xl border-2 border-blue-200">
  <div class="text-5xl mb-3">📥</div>
  <div class="text-xl font-bold text-blue-700 mb-2">1. Invoer</div>
  <div class="text-sm opacity-80">Sensordata van een productiecyclus — bijv. trillingscurve</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl border-2 border-purple-200">
  <div class="text-5xl mb-3">📝</div>
  <div class="text-xl font-bold text-purple-700 mb-2">2. Samenvatting</div>
  <div class="text-sm opacity-80">Het AI maakt een korte beschrijving — alsof in 5 woorden</div>
</div>

<div class="p-6 bg-green-50 rounded-xl border-2 border-green-200">
  <div class="text-5xl mb-3">📤</div>
  <div class="text-xl font-bold text-green-700 mb-2">3. Herstel</div>
  <div class="text-sm opacity-80">Vanuit de samenvatting de oorspronkelijke data terugbouwen</div>
</div>

</div>

<div v-click class="mt-10 text-center text-base opacity-70">
  Drie stappen — meer is het niet.
</div>

<!--
Loop ze één voor één langs. Wijs naar de flap-over-kapstok.
Geen wiskunde. Het diagram (slide 6) helpt visueel.
-->

---

# Reconstructiefout = het verschil

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Klein verschil
<v-clicks>

- AI kent het patroon
- "Dit lijkt op wat ik eerder zag"
- **Normaal**

</v-clicks>

</div>

<div>

### Groot verschil
<v-clicks>

- AI kan het niet goed terugbouwen
- "Dit ken ik niet"
- **Alarm**

</v-clicks>

</div>

</div>

<div v-click class="mt-8 p-5 bg-amber-50 rounded-lg">

### Voorbeeld — spuitgietmachine
- Cyclus 1 t/m 100 = normaal — AI leert die patronen
- Cyclus 101: matrijs raakt los — trillingscurve afwijkend
- AI kan het niet goed terugbouwen — **alarm**

</div>

<!--
Reconstructiefout = verschil tussen plaatje vóór en plaatje ná.
Geen wiskunde, geen MSE, geen Euclidische afstand.

Concreet voorbeeld werkt altijd: spuitgietmachine met trillingen.
-->

---
layout: quote
---

# Jij deed wat de AI doet

<div class="text-xl mt-6 opacity-80">
  Jullie wisten wat <span class="font-bold">normaal</span> eruitziet.
</div>

<div v-click class="mt-8 text-base opacity-70">
  Bij grafieken die <span class="font-bold">afweken</span>, voelde dat raar.
</div>

<div v-click class="mt-8 text-sm opacity-50">
  Dat is wat de autoencoder doet —<br/>
  alleen sneller en zonder vermoeidheid.
</div>

<!--
Het didactische scharnier.
"Wat jullie deden in de quiz: jullie wisten wat normaal eruitziet, en bij grafieken die afweken voelde dat raar. Dat is wat de autoencoder doet."

Bij MBO-4 die latente ruimte vraagt: parkeer ('daar gaan we dieper op in als je interesse hebt — bron Goodfellow').
-->

---
layout: section
---

# Experimenteren

## Waar zou dit op jouw machine helpen?

<!--
Overgang naar blok 4.
-->

---

# Drie vragen voor jouw lijn

<div class="grid grid-cols-3 gap-6 mt-8">

<div class="p-6 bg-blue-50 rounded-xl text-center">
  <div class="text-4xl mb-3">⚙️</div>
  <div class="text-lg font-bold text-blue-700 mb-2">Welke machine?</div>
  <div class="text-sm opacity-70">Wees specifiek</div>
</div>

<div class="p-6 bg-purple-50 rounded-xl text-center">
  <div class="text-4xl mb-3">📊</div>
  <div class="text-lg font-bold text-purple-700 mb-2">Welke sensor?</div>
  <div class="text-sm opacity-70">Temperatuur, druk, trillingen, geluid?</div>
</div>

<div class="p-6 bg-green-50 rounded-xl text-center">
  <div class="text-4xl mb-3">⚠️</div>
  <div class="text-lg font-bold text-green-700 mb-2">Verdacht-moment?</div>
  <div class="text-sm opacity-70">Wat voel je nu al?</div>
</div>

</div>

<div v-click class="mt-8 text-center text-base opacity-70 italic">
  De AI kan leren wat jij voelt — als jij het kunt benoemen.
</div>

<div class="abs-br m-6 text-xs opacity-40">
  3 min individueel · 1.5 min duo · wb-04-experimenteren
</div>

<!--
Werkblad wb-04. Zet timer op 3 min individueel.
Loop rond. Help concretiseren:
- "Welke machine merk je vaak iets raars aan?"
- "Welke sensor zou je kunnen waarschuwen?"
- "Wat is voor jou een verdacht-moment dat je nu al voelt zonder dat een sensor het meet?"

Daarna 1.5 min duo, daarna 1.5 min plenair (2-3 mensen).
-->

---

# Deze week

<div class="grid grid-cols-2 gap-8 mt-6">

<div>

### Let op patronen
<v-clicks>

- Noteer een moment waar je zelf denkt: dit is niet normaal
- Welke sensor zou dat kunnen pakken?
- Wat voel/hoor jij dat geen dashboard ziet?

</v-clicks>

</div>

<div>

### Vraag rond
<v-clicks>

- Vraag je teamleider:<br/>"Wordt er sensordata verzameld op mijn machine?"
- Vraag een collega:<br/>"Wanneer voel jij dat een machine niet lekker draait?"

</v-clicks>

</div>

</div>

<div v-click class="mt-10 p-4 bg-blue-50 rounded-lg text-center">
  Volgende sessie: <span class="font-bold">SHAP — welke sensor draagt bij aan het alarm? — LO-108</span>
</div>

<!--
Sluit af met de transferopdracht.
"De autoencoder slaat alarm. Maar bij WELKE sensor zit het probleem? Dat is de vraag van LO-108."
-->

---
layout: end
---

# Vragen?

<div class="mt-8 text-base opacity-70">
  Volgende workshop: <span class="font-bold">SHAP — welke sensor draagt bij? — LO-108</span>
</div>

<div class="abs-br m-6 text-xs opacity-40">
  AIMM × BronzGreen · Predictive Maintenance Module 2 (Train)
</div>

<!--
Bedank de groep.
Werkbladen innemen of foto's maken.

Notitie:
- Welke sensoren werden genoemd? (input voor LO-108 en LO-201)
- Wie noemde een 'verdacht-moment dat geen dashboard ziet'? (waardevolle data)
- Bron: Goodfellow et al. (2016). Deep Learning, hfdst 14. | Sakurada & Yairi (2014).
-->
