---
id: lo-industry40-301-trainee
knowledge_object_id: ko-industry40-301
version: trainee
title: Sensor-keuze voor een digital twin — vijf typen en drie trade-offs
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_bekwaam
kolb_start_phase: ervaren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde15-lo-industry40-301
---

# Sensor-keuze voor een digital twin — welke sensor past bij welke vraag?

Een digital twin (digitale tweeling) leeft van data. Geen data, geen tweeling. En de data komt uit sensoren. Welke sensoren je kiest, bepaalt wat de twin kan zien — en wat niet. Een lager dat trilt zonder trilling-sensor? De twin merkt niks. Een product dat verkleurt zonder beeld-sensor? De twin ziet geen probleem. In deze sessie leer je hoe je een passende sensor kiest. Niet op gevoel, maar met een procedure.

## Wat leer je?

Je kunt na deze sessie voor een werkvloer-vraag een passend sensor-type kiezen. Je kent de vijf typen die je het vaakst tegenkomt. Je kunt de drie trade-offs tegen elkaar afwegen. En je herkent drie veelgemaakte fouten die je beter kunt vermijden.

## Begin bij de vraag — niet bij de sensor

De grootste valkuil bij sensor-keuze is dit: je begint bij de sensor. "Welke sensor zal ik kopen?" Verkeerde vraag. De goede vraag is: "Welke vraag wil ik beantwoorden met de digital twin?"

Voorbeelden van zulke vragen op de werkvloer:

- "Welke lagers gaan binnenkort kapot?"
- "Loopt de machine te warm?"
- "Wat is de reden van afkeur op de inpaklijn?"
- "Lekt er ergens perslucht weg?"
- "Klopt er iets niet met het geluid van de pomp?"

Pas als jouw vraag helder is, kies je een sensor. Anders krijg je sensor-overdaad: veel data, weinig antwoord.

Bron: Soldatos (2024), Artificial Intelligence in Manufacturing, hoofdstuk 6.

## Vijf typen sensoren op de werkvloer

Je komt op de werkvloer vijf typen sensoren (meetapparaten) bijna overal tegen. Elk type past bij een eigen soort vraag.

### Trilling

Meet vibratie in lagers, motoren en ventilatoren. Een vroegtijdig signaal van slijtage of onbalans. Richtprijs ongeveer €100 tot €500 per sensor. Heel geschikt voor voorspellend onderhoud.

### Temperatuur

Meet hitte van een component, een product of een ruimte. Simpel, goedkoop en robuust. Richtprijs ongeveer €20 tot €100 per sensor. Past bij vragen over oververhitting of warmteverlies.

### Akoestiek

Meet geluid. Patronen in machine-geluid wijzen op slijtage of fouten. Specialistisch. Richtprijs ongeveer €500 tot €2000 per sensor plus een AI-model dat de patronen herkent.

### Beeld

Een industriële camera met een AI-model. Geschikt voor kwaliteitsinspectie, montage-check en veiligheid. Een complete opstelling kost ongeveer €2000 tot €20.000.

### Druk

Meet druk in pneumatiek, hydrauliek of vloeistof-systemen. Robuust en betrouwbaar. Richtprijs ongeveer €50 tot €500 per sensor.

## De drie trade-offs

Bij elke sensor-keuze wegen drie dingen tegen elkaar.

### Kosten

Niet alleen aanschaf. Ook installatie, bekabeling, een edge-buffer (tussenstation bij de sensor), onderhoud en data-verwerking. Een sensor van €100 met een installatie van €10.000 is nog steeds een dure sensor.

### Accuratesse

Wat kan de sensor onderscheiden? Sommige trilling-sensoren meten op micrometer-niveau (1/1000 millimeter). Andere alleen op millimeter-niveau. Hoe nauwkeuriger, hoe duurder. Past de accuratesse niet bij jouw vraag, dan koop je te veel of te weinig.

### Levensduur

In stoffige, hete of vochtige omgevingen leven sommige sensoren maar zes maanden. In milde omgevingen halen ze tien jaar. Vervangings-kosten en stilstand voor vervanging tellen op. Vraag aan de leverancier wat de levensduur is in jouw type omgeving.

## Drie veelgemaakte fouten

In de praktijk gaat het vooral op deze drie punten mis.

1. **Te veel sensoren plaatsen "voor de zekerheid"**. Leidt tot data-overdaad zonder inzicht. Beter: klein beginnen en uitbreiden als nodig.
2. **Te goedkope sensor kiezen**. Een temperatuur-sensor van €20 die elke drie maanden vervangen moet worden, kost over vijf jaar méér dan een geïntegreerde sensor van €100 die vijf jaar meegaat.
3. **Sensor-onderhoud vergeten**. Vuile of niet-geijkte sensoren geven foute data. Plan vervangen en ijking direct in vanaf dag één.

## Een werkvloer-voorbeeld

Een fietsfabriek wil weten welke lagers in de lakstraat binnenkort falen. De engineer heeft twee opties bekeken.

**Optie A**: twaalf trilling-sensoren van €200 per stuk. Installatie €5.000. Onderhoud €1.500 per jaar. Totaal in jaar 1: €9.400. Daarna €1.500 per jaar.

**Optie B**: geen sensoren. Een operator loopt eenmaal per week een inspectie-ronde. Kosten van de operator-tijd ongeveer €8.000 per jaar.

Wat lijkt goedkoop? Optie B in jaar 1. Wat is goedkoop op de lange termijn? Optie A. De fabriek heeft drie ongeplande lager-stilstanden per jaar. Eén stilstand kost €4.000 aan productie-verlies. Drie stilstanden samen kosten €12.000. Optie A vangt die op met voorspellend onderhoud. De investering is in jaar 2 terugverdiend.

De keuze was niet "welke sensor is het mooist?" maar "wat kost stilstand ons echt?" — een vraag-driven aanpak in actie.

## Na deze sessie

Doe deze week drie kleine stappen op je eigen werkvloer. Geen extra budget nodig.

1. **Kies één machine of proces** waar jullie nu nog geen digital twin (digitale tweeling) hebben. Schrijf in één zin op welke vraag een digital twin daar zou kunnen beantwoorden.

2. **Loop langs de machine en kijk welke sensoren er al hangen.** Noteer per sensor het type (trilling, temperatuur, akoestiek, beeld of druk) en wat hij meet. Vraag bij twijfel aan onderhoud of teamleider.

3. **Bedenk twee vragen voor je teamleider of leverancier.** Bijvoorbeeld: "Welke data leveren onze huidige sensoren al?" En: "Welke trade-off (kosten, accuratesse of levensduur) is voor onze omgeving het belangrijkste?"

Neem alle drie de uitkomsten mee naar de volgende sessie.

Praat deze week ook één keer met een collega over één van de drie veelgemaakte fouten. Vraag of jullie die ergens herkennen. Vaak ontdek je dat dit gesprek nog niet is gevoerd.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-componenten-verkennen.md`](./werkbladen/wb-01-componenten-verkennen.md) — Componenten verkennen
2. [`wb-02-duo-vraag-bij-component.md`](./werkbladen/wb-02-duo-vraag-bij-component.md) — Duo vraag bij component
3. [`wb-03-handout-sensor-keuze.md`](./werkbladen/wb-03-handout-sensor-keuze.md) — Handout sensor keuze
4. [`wb-04-jouw-sensor-keuze.md`](./werkbladen/wb-04-jouw-sensor-keuze.md) — Jouw sensor keuze

## Verder

- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
