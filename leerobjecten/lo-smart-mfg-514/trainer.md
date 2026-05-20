---
id: lo-smart-mfg-514-trainer
knowledge_object_id: ko-smart-mfg-514
version: trainer
title: Het model verbeteren — meer data, betere labels — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 60
status: validated
updated_at: '2026-05-20'
correlation_id: ronde24-lo-smart-mfg-514
---

# Vision-model verbeteren — meer data, betere labels — voor de trainer

**Leerobject:** lo-smart-mfg-514
**Kennisobject:** ko-smart-mfg-514
**Doelgroep:** MBO-3/4 operator (Module 2 tweede helft), B1 taalniveau
**Duur:** 60 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Foutenanalyse confusion matrix, duo-reflectie patroon, handout iteratie-cyclus + lakdefect-casus, eigen iteratie uitvoeren |
| Kolb-startfase | Ervaren — bewust bekwame doener met werkend model start met directe foutenanalyse |
| Begeleidingsstijl | Coachen — peer-check voor veiligheid, label-consistentie controleren maar niet overnemen |
| Materialen | Vier werkbladen, simulator (model-lo-smart-mfg-514.html), eigen vision-dashboard of demo, camera/smartphone voor productfoto's, foto-opstelling |

## Wat de deelnemer leert

De deelnemer kan de fouten van een vision-model analyseren en gericht trainingsdata + labels toevoegen om de modelprestatie te verbeteren. Bij een getest vision-model met confusion matrix identificeert hij minimaal 2 zwakke categorieën, voegt 30+ gerichte foto's met correcte labels toe, en kan na hertraining de prestatieverbetering kwantificeren in recall/precision.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:12 | Fouten zoeken in confusion matrix — recall <80% per categorie | Individueel |
| Reflecteren | 0:12-0:20 | Duo: wat zegt foutenpatroon over trainingsdata? | Duo |
| Theoretiseren | 0:20-0:30 | Iteratie-cyclus + lakdefect-casus (krassen 95%, kleur 60→85%) | Trainer + diagram |
| Experimenteren | 0:30-1:00 | 30+ foto's labelen + peer-check + (optioneel) hertrainen | Individueel + duo |

## Tips voor de trainer

- **"Meer data is altijd beter" scherpen aan.** "Meer data is goed — gerichte data is beter. 30 foto's van de zwakste categorie zijn waardevoller dan 200 willekeurige." Verwijs naar de confusion matrix.
- **Peer-check geeft veiligheid.** Bij "ik durf niets toe te voegen — straks gaat het slechter": "Laat een collega 5 willekeurige labels controleren. Minder dan 1 op 10 inconsistent kan erin. En het model is altijd revertbaar."
- **Concretiseer fase 4 in dag, shift, camera, peer.** "Welke dag? Welke shift? Welke camera? Welke 5 labels laat je peer-checken?" Liever drie haalbare stappen dan één vage.
- **Houd technische diepte achter.** Transfer learning, augmentation en hyperparameters niet vandaag — verwijs naar leverancier of LO-006 voor theorie. Twee acties: gerichte foto's + consistente labels.
- **Geen toegang tot eigen model? Demo-model gebruiken.** Vraag operator wel om hypothese: "Welke categorie is bij jullie waarschijnlijk de zwakste?" — schrijf op werkblad als transferopdracht.

## Valkuilen

- **Operator denkt 'meer data is altijd beter'.** Ongericht 200 foto's toevoegen helpt niet; verwijs naar matrix.
- **Bang om model te verergeren door 'foute' labels.** Peer-check normaliseert; benadruk revertbaarheid.
- **Iteratie-fase 4 wordt gepland maar nooit uitgevoerd.** Eis concrete dag, shift, camera, peer-naam op werkblad.

## Voorbereiding (45 min vooraf)

- [ ] Vier werkbladen printen, n + 2 reserve
- [ ] SVG-diagram iteratie-cyclus + simulator op beamer
- [ ] Toegang tot eigen vision-dashboard per deelnemer (demo als backup)
- [ ] Camera/smartphone per deelnemer
- [ ] Foto-opstelling als beschikbaar (verlichting, achtergrond)
- [ ] Flap-over (iteratie-kapstok + parkeerlijst)
- [ ] Clusters van 4 met laptops

## Transferopdracht

Geef de deelnemer mee om binnen één week zijn iteratie uit te voeren: 30+ foto's van de zwakste categorie maken, labelen met peer-check (collega controleert 5 willekeurige), in trainingsset plaatsen en (laten) hertrainen. Hij vergelijkt recall/precision per categorie voor en na, en deelt het resultaat met de groep in de volgende sessie.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
