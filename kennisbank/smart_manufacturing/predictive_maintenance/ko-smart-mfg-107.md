---
id: ko-smart-mfg-107
title: Anomaliedetectie op CNC-machines met Isolation Forest
type: voorbeeld
domain: smart_manufacturing
subdomain: predictive_maintenance
summary: Een AI-systeem leert wat normaal is voor een CNC-machine en slaat alarm als
  er iets afwijkt. Bij CNH Industrial in Modena voorkomt dit onverwachte stilstand.
source_centrality: 0.7
source_ref: Sesana et al. (2024). Artificial Intelligence in Manufacturing, pp. 474-475
status: validated
updated_at: '2026-05-20'
correlation_id: ronde19-lo-smart-mfg-107
---

# Anomaliedetectie op CNC-machines met Isolation Forest

Bij de productie van tractortransmissies bij CNH Industrial in Modena valt een CNC-machine regelmatig onverwacht uit *(bron: Sesana et al. 2024, Artificial Intelligence in Manufacturing — CNH Industrial Modena anomaliedetectie)*. Een AI-systeem helpt om deze storingen eerder te ontdekken.

### Hoe werkt het?

Stel je voor dat je 1000 knikkers hebt. 990 knikkers zijn blauw — dat is normaal machinegedrag. 10 knikkers zijn rood — dat zijn afwijkingen. Het AI-systeem leert de blauwe knikkers te herkennen. Alles wat niet blauw is, krijgt een waarschuwing.

Het systeem heet **Isolation Forest**. Je hoeft niet te weten hoe het technisch werkt. Wat je wel moet weten:

- Het systeem **leert zelf** wat normaal is voor jouw machine
- Het **vergelijkt** nieuwe sensordata met dat normale patroon
- Het **markeert** alles wat afwijkt — zodat jij kunt ingrijpen

### Wat meet het systeem?

Het systeem kijkt naar sensordata: temperatuur, trillingen, energieverbruik, druk. Het kan naar **een enkele sensor** kijken, maar ook naar **een groep sensoren tegelijk**. Dat laatste is belangrijk: soms is elke sensor apart nog normaal, maar de combinatie wijkt af.

### Wat levert het op?

- Storingen eerder ontdekken (uren of dagen van tevoren)
- Minder ongeplande stilstand
- Minder beschadigde producten
- Gerichter onderhoud: je weet waar je moet kijken


## Praktijkvoorbeeld

*(Bron: Sesana et al. 2024, Artificial Intelligence in Manufacturing — CNH Industrial Modena, Heller 400 CNC-anomaliedetectie.)*

Bij de Heller 400 CNC-machine in het CNH-plant monitort het AI-systeem 76 sensoren. Op een dinsdag merkt het systeem iets op: drie temperatuursensoren bij het koelsysteem geven samen een ongewoon patroon. Elke sensor apart is nog binnen de grenzen, maar de combinatie klopt niet.

De operator krijgt een melding op zijn scherm. Hij controleert het koelsysteem en vindt een gedeeltelijk verstopte koelleiding. Reparatie duurt 20 minuten. Zonder de waarschuwing was de machine pas stilgevallen bij een volledige blokkade — met uren stilstand en mogelijke schade aan het werkstuk.
