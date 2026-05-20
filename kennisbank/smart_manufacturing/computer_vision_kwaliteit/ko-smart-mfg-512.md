---
id: ko-smart-mfg-512
title: 'Een vision-model configureren: parameters instellen'
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: Bij het configureren van een vision-model stel je de gevoeligheid in. Te
  streng betekent te veel valse alarmen. Te soepel betekent gemiste defecten. De testset
  helpt je de juiste balans te vinden.
source_centrality: 0.7
source_ref: Rožanec et al. (2024). Artificial Intelligence in Manufacturing, pp. 397-412
status: validated
updated_at: '2026-05-20'
correlation_id: ronde23-lo-smart-mfg-512
---

# Een vision-model configureren: parameters instellen

Als je trainingsdata hebt gelabeld en een model hebt getraind, moet je het model **configureren**. De belangrijkste instelling is de **drempelwaarde** — hoe streng het model oordeelt.

## Wat is de drempelwaarde?

Het model geeft elk product een **score** tussen 0.0 en 1.0:

- **0.0** = het model is zeker dat het product goed is
- **1.0** = het model is zeker dat het product defect is
- **0.5** = het model twijfelt

De drempelwaarde bepaalt waar je de grens legt. Alles boven de drempel wordt als "defect" aangemerkt. Alles eronder als "goed".

## De balans: streng vs. soepel

| Instelling | Drempel | Wat gebeurt er? |
|---|---|---|
| **Te streng** | 0.3 | Vindt bijna alle defecten, maar ook veel valse alarmen |
| **Gebalanceerd** | 0.5 | Goede balans tussen vinden en vals alarm |
| **Te soepel** | 0.7 | Weinig valse alarmen, maar mist echte defecten |

### Wanneer kies je streng?

- Als een gemist defect **gevaarlijk** is (veiligheidsonderdelen)
- Als een gemist defect **duur** is (recall, klachten)
- Als je genoeg capaciteit hebt om valse alarmen handmatig te checken

### Wanneer kies je soepel?

- Als valse alarmen de productielijn **stilleggen**
- Als gemiste defecten **weinig impact** hebben (cosmetisch)
- Als je te weinig mensen hebt om valse alarmen te controleren

## De testset gebruiken

Zo vind je de juiste drempelwaarde:

1. **Draai het model** op je testset (de 20% die het model nog niet heeft gezien)
2. **Probeer verschillende drempelwaarden**: 0.3, 0.4, 0.5, 0.6, 0.7
3. **Tel per drempel**: hoeveel defecten gevonden? Hoeveel valse alarmen?
4. **Kies de drempel** die past bij jouw situatie

**Vuistregel:** begin met 0.5 en pas aan op basis van wat je ziet. Stuur twijfelgevallen (score dicht bij de drempel) altijd naar een menselijke inspecteur.

## Twijfelzone instellen

Veel systemen werken met een **twijfelzone** in plaats van een harde grens:

- Score < 0.3 = automatisch goedgekeurd
- Score 0.3-0.7 = naar de operator voor handmatige controle
- Score > 0.7 = automatisch afgekeurd

Dit geeft het beste van twee werelden: het model handelt de duidelijke gevallen af, en jij bekijkt alleen de twijfelgevallen.

## Praktijkvoorbeeld

Een operator configureert een vision-model voor het detecteren van krassen op metalen onderdelen. Bij een drempelwaarde van 0.3 meldt het systeem 95% van de defecten, maar ook 40% van de goede producten als defect (valse alarmen). Bij 0.7 zijn er bijna geen valse alarmen meer, maar mist het systeem 30% van de echte defecten. De operator kiest uiteindelijk 0.5: het systeem vindt 85% van de defecten en heeft slechts 10% valse alarmen. De twijfelgevallen (score 0.4-0.6) stuurt hij naar handmatige controle.
