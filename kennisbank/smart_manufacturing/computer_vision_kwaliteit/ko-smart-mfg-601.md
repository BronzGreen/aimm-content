---
id: ko-smart-mfg-601
title: Gelabelde data is de echte bottleneck bij computer vision
type: concept_uitleg
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Het model is niet het probleem bij computer vision. Jouw data is het probleem.
  En niemand anders gaat dat voor jou oplossen.
source_centrality: 0.7
source_ref: RLC-Oost (2026). Workshop w00 — Waarom computer vision? (AI Vision Learning
  Community)
status: validated
updated_at: '2026-05-19'
correlation_id: ronde28-lo-smart-mfg-601-mbo4
---

# Gelabelde data is de echte bottleneck bij computer vision

Veel mensen denken dat een AI-model voor beeldherkenning 'vanzelf leert' als je het lang genoeg laat draaien. Dat beeld klopt niet. Een model leert alleen van de **voorbeelden** die je het geeft. Zonder voorbeelden leert het niets.

### Wat betekent 'gelabelde data'?

Een **label** is een aanduiding bij een beeld die zegt wat er te zien is. Bijvoorbeeld:

- 'Dit is een kras' (bij een foto van een metalen onderdeel)
- 'Dit is goed' (bij een foto zonder defect)
- 'Dit is een scheurtje langs de rand'

Elk beeld dat je aan het model geeft om van te leren, moet zo'n label hebben. Het model leert namelijk van voorbeelden waarvan jij als mens al weet wat het goede antwoord is. Geen voorbeelden betekent: geen leren.

### Waarom is dit de bottleneck?

De modellen bestaan al, kant-en-klaar. Je kunt ze gratis downloaden. Dat is het makkelijke deel.

Het moeilijke deel is de data:

- **Je hebt honderden beelden nodig per type defect** — vuistregel 100-300 per klasse, afhankelijk van de variatie in je product *(ontwerp-schatting, te valideren per bedrijf)*
- **Elk beeld moet gelabeld worden** — dat kost 1-3 minuten per beeld *(vuistregel)*
- **De labels moeten consistent zijn** — wat de ene inspecteur 'kras' noemt, mag de andere niet 'deuk' noemen

Reken maar eens: 500 beelden labelen kost tussen de 2 en 6 uur. En dat is nog maar één type product, één type defect.

### Het data flywheel

Er bestaat een patroon dat laat zien waarom data strategisch zo belangrijk is:

```
Meer gebruikers
    -> Meer gelabelde data
        -> Beter model
            -> Beter product
                -> Meer gebruikers
```

Dit heet een **data flywheel**. Google gebruikte de reCAPTCHA-puzzels (die je invult om te bewijzen dat je geen robot bent) mede om hun beeldherkenningsmodellen te trainen. Miljoenen mensen leverden onbewust labels voor Google — en die data was voor Google een strategisch voordeel, niet het model.

### Wat dit voor jou betekent

Als je op de werkvloer iets wil automatiseren met beeldherkenning — een camera die krassen op producten herkent, bijvoorbeeld — begin je **niet** met het model. Je begint met foto's. En labels. En de vraag: *is mijn data goed genoeg?*

Want als de data niet klopt, klopt het model ook niet.


## Praktijkvoorbeeld

Stel: een bedrijf maakt metalen beugels. Soms zit er een kras op, soms een scheurtje, soms een verkeerde maat. Je wil een camerasysteem dat dat automatisch herkent.

Stap 1 is niet 'download YOLO en train het model'. Stap 1 is: maak honderden foto's van die beugels. Label elk beeld. 'Kras op positie linksboven.' 'Geen defect.' 'Scheurtje langs de rand.' Pas daarna heeft het model iets om van te leren.

Bij Philips in Drachten werkt dit al zo *(bron: Rožanec et al. 2024 — academisch gedocumenteerd praktijkvoorbeeld)*: drie aparte modellen voor drie producten, elk getraind met honderden voorbeeldfoto's. De operator bekijkt alleen nog de twijfelgevallen — maar zonder die voorbeeldfoto's vooraf had het systeem niks kunnen doen.
