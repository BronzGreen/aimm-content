---
id: lo-ai-fund-ml-001-trainer
knowledge_object_id: ko-ai-fundamentals-ml-001
version: trainer
title: Vier ML-leerklassen — welke past bij welk PdM-probleem? — trainer-pakket
target_audience: operator
content_level: MBO-3
language_level: B2
bloom_level: begrijpen
knowledge_type: declaratief
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 50
status: validated
updated_at: '2026-05-12'
correlation_id: sprint3-acceptance-5
---

# Vier ML-leerklassen voor PdM — voor de trainer

**Leerobject:** lo-ai-fund-ml-001
**Kennisobject:** ko-ai-fundamentals-ml-001
**Doelgroep:** MBO-4 operator/teamleider, B2 taalniveau
**Duur:** 50 min
**Bloom:** toepassen

## In één oogopslag

| | |
|---|---|
| Werkvormen | Vier scenario-cases, duo-vergelijking met stemkaartjes, trainer-handout, individueel actieplan |
| Kolb-startfase (de fase in de leercyclus waarmee de sessie begint) | Ervaren (vier cases zelf beoordelen) |
| Begeleidingsstijl (instrueren / trainen / coachen / mentoren) | Trainen — IK DOE worked example, daarna zelf werken |
| Materialen | 4 werkbladen, diagram (4 leerklassen × 3 PdM-probleemtypen), 4-kleur stemkaartjes |

## Wat de deelnemer leert

De deelnemer kan de vier ML-leerklassen benoemen — supervised, unsupervised, semi-supervised, reinforcement — en uitleggen welke leerklasse past bij welke datasituatie en bij welk PdM-probleemtype (classification, regression, clustering). In vier scenario's kiest hij de juiste leerklasse met onderbouwing op basis van label-beschikbaarheid en probleemtype. Vereist data-lit-101 afgerond. **Leg dit LO bij voorkeur eerst** — voor FL/CNN/RNN/Ensemble.

## Sessie-opbouw

| Fase | Tijd | Activiteit | Werkvorm |
|---|---|---|---|
| Ervaren | 0:00-0:14 | Vier scenario-cases beoordelen | Individueel + IK DOE op case A |
| Reflecteren | 0:14-0:25 | Buurman-check + plenaire stemming | Duo + 4-kleur stemkaartjes |
| Theoretiseren | 0:25-0:38 | Handout: 4 leerklassen + 3 PdM-probleemtypen | Trainer + handout |
| Experimenteren | 0:38-0:50 | Welke leerklasse past bij ons? | Individueel actieplan |

## Tips voor de trainer

- **Doe case A voor (worked example).** *"Gelabelde data + voorspelling van een getal → supervised regression."* Hardop denken — daarna lossen ze B-D zelf op.
- **Twijfel toestaan in blok 1.** Vraagteken zetten mag. Het verschil tussen semi-supervised en de andere is precies wat we straks scherp maken.
- **Stemkaartjes-techniek.** Vier kleuren voor vier leerklassen — plenair stemmen is sneller en zichtbaarder dan één-voor-één antwoorden.
- **Gebruik scenario-A-D als rode draad in blok 3.** *"Casus A — RUL — dat is regression, supervised. Casus B — afwijkende patronen zonder labels — clustering, unsupervised."* Theorie verankerd in eigen werk.
- **Adresseer de "supervised is de echte AI"-misvatting expliciet.** 80% van de fabrieken heeft geen systematische uitvalhistorie. Andere leerklassen zijn dan geen *minder*, maar de enige optie.

## Valkuilen

- **Supervised wordt gezien als de "echte AI", anderen als minderwaardig.** Bevestig dat supervised vaak het meest accuraat IS — maar alleen als de labels er zijn. Leerklasse moet aansluiten op data-realiteit.
- **Semi-supervised wordt gemist of verward met "weak supervision".** Maak expliciet: het is een COMBINATIE van klein gelabeld + groot ongelabeld. Recent populair, niet hetzelfde als supervised of unsupervised.
- **Reinforcement wordt gezien als "voor robots".** Bevestig de associatie, maar verbind aan onderhoudsbeleid: uitstellen vs preventief vervangen — reinforcement leert die balans optimaliseren.

## Voorbereiding (15 min vooraf)

- [ ] 4 werkbladen printen (4 scenario-cases, reflectie, handout leerklassen, actieplan), 1 per deelnemer + 2 reserve
- [ ] Stemkaartjes in 4 kleuren (rood/blauw/geel/groen), 1 set per deelnemer
- [ ] SVG-diagram (4×3 matrix) op A3 zichtbaar
- [ ] Beamer + Slidev, HDMI testen
- [ ] Pen + markeerstift per deelnemer
- [ ] Flipover voor parkeerlijst + 4 leerklassen-overzicht

## Transferopdracht

Sluit af met: deelnemers onderzoeken deze week binnen de eigen organisatie hoeveel gelabelde uitvalhistorie er werkelijk is. Vraag bij onderhoud, IT of kwaliteit: registreren we systematisch failure-events? Hoeveel cases over 1-3 jaar? Categorisatie aanwezig? Antwoord meenemen — dat bepaalt welke leerklasse past.

## Verdere details

- **Volledig draaiboek:** [`draaiboek.md`](./draaiboek.md)
- **Slidev presentatie:** [`slidev/presentatie.slidev.md`](./slidev/presentatie.slidev.md)
- **Trainee-versie:** [`trainee.md`](./trainee.md)
