---
id: ko-smart-mfg-801
title: 'Van drempel naar businesscase: de cijfers op een rij'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Een AI-camerasysteem koop je niet op gevoel. Je koopt het op cijfers. Als
  je drie getallen paraat hebt — jaarlijkse besparing, eenmalige investering, payback-periode
  — kun je een serieus gesprek voeren met de teamleider of directie.
source_centrality: 0.7
source_ref: Standaard businesscase-framework, aangepast voor operator-niveau
status: validated
updated_at: '2026-05-20'
correlation_id: ronde27-lo-smart-mfg-801
---

# Van drempel naar businesscase: de cijfers op een rij

Module 1 gaf je begrip, Module 2 gaf je toepassing. Module 3 gaat over wat je ermee doet. Dat begint bij het vertalen van alles wat je geleerd hebt naar **cijfers die een beslisser begrijpt**.

### Waarom cijfers?

Een voorstel zonder cijfers is een wens. Met cijfers is het een businesscase. Directie en teamleiders maken elke dag investeringskeuzes — ze kunnen niet álle ideeën honoreren, dus ze kiezen op basis van onderbouwing. Als operator heb jij informatie die zij niet hebben. Dat maakt jouw businesscase waardevol.

### De drie getallen

Elke businesscase voor AI-kwaliteitscontrole heeft drie kerncijfers:

**1. Jaarlijkse besparing**

Uit LO-702: vals-alarm-kosten + gemist-defect-kosten per jaar *zonder* AI. Het systeem elimineert deze niet helemaal (het maakt zelf ook fouten), maar het reduceert ze significant. **Vuistregel: reductie van 60-80% voor een ingericht systeem** *(ontwerp-schatting op basis van sector-publicaties; varieert sterk per bedrijf en volwassenheid van het systeem — in pilot te valideren).*

Formule: (huidige inspectie-tijd × uurloon) + (klachten per jaar × kosten per klacht). Dat is de **maximale besparing**.

**2. Eenmalige investering**

Wat kost het om het systeem op te zetten?

Vuistregel-bereiken *(ordes van grootte; vraag bij concrete leveranciers om offertes)*:

- Hardware (camera, verlichting, computer): €5.000-€30.000 afhankelijk van schaal
- Software-licentie: €5.000-€20.000 eenmalig, of €500-€2.000 per maand
- Labelwerk (zie KO-601!): 10-50 uur × intern uurloon
- Installatie + configuratie: 20-80 uur × technisch uurloon

Totaal: grofweg €20.000 - €80.000 voor een gemiddelde productielijn *(ontwerp-schatting)*.

**3. Payback-periode**

Hoe lang duurt het voordat de besparing de investering heeft terugverdiend?

```
Payback = Investering / Jaarlijkse besparing
```

Is payback < 1 jaar: zeer aantrekkelijk
Is payback 1-2 jaar: goede kans op investering
Is payback 2-5 jaar: gesprek, niet automatisch
Is payback > 5 jaar: waarschijnlijk andere prioriteiten

### De verborgen getallen

Deze drie zijn de basis. Slimmere businesscases voegen toe:

- **Risico-kosten vermeden:** als gemist defect een recall riskeert (zoals in LO-702 automotive-voorbeeld), is zelfs een hoge investering verantwoord.
- **Kwaliteits-improvement:** minder klachten betekent betere klanttevredenheid — moeilijk in euro's maar wel meetbaar via NPS of retentie.
- **Operator-tijd voor beter werk:** wat ga je doen met de vrijkomende tijd? Meer producten inspecteren? Complexere taken? Training? Dat is de 'verborgen' ROI.

### Wat dit voor jou betekent

Je hoeft geen financieel expert te zijn. Wel: ruwe schattingen durven maken, en die kunnen onderbouwen met wat je geleerd hebt. 'Tussen €40.000 en €60.000 investering, payback waarschijnlijk 18 maanden, gebaseerd op onze huidige inspectie-tijd van 200 uur per week' is veel bruikbaarder dan 'het zou iets met AI kunnen'.

Jouw voordeel: je kent de werkvloer beter dan de leverancier, beter dan de directie. Je weet welke kosten echt oplopen, en welke bij presentaties worden weggelaten. Een eerlijke businesscase is daarom vooral een operator-businesscase — niet een leveranciers-presentatie.


## Praktijkvoorbeeld

*Fictieve rekenvoorbeeld ter illustratie — geen gerealiseerde case.*

Stel: een fabriek voor autokabelbomen. Huidige inspectie: 3 inspecteurs × 40 uur × €35/uur × 50 weken = **€210.000/jaar**. Klachten: gemiddeld 6 per jaar × €2.500 = **€15.000/jaar**. Totale huidige kosten: **€225.000/jaar**.

AI-inspectiesysteem vermindert inspectie-uren met 70% (1 inspecteur blijft voor twijfelgevallen + onderhoud) en klachten met 80% — *de 70% en 80% zijn ontwerp-schattingen, in een echt bedrijf te meten*. Besparing: €147.000 + €12.000 = **€159.000/jaar**.

Investering: hardware €25.000 + software €15.000 + labelwerk 30 uur × €35 + installatie 40 uur × €80 = **€44.250**.

Payback = €44.250 / €159.000 = **3,4 maanden**.

Hiermee ga je naar je teamleider. Niet: 'AI zou goed zijn'. Wel: '€159.000 besparing per jaar, €44.000 investering, terugverdiend in 3,4 maanden'. Dat is een gesprek dat ergens landt.
