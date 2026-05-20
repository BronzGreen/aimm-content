---
id: ko-data-lit-202
title: 'Datakwaliteit beoordelen: drie checks die je zelf kunt doen'
type: framework
domain: data_literacy
subdomain: data_kwaliteit
summary: Goede data is volledig, consistent en actueel. Met drie simpele checks kun
  je zelf beoordelen of je data betrouwbaar genoeg is om beslissingen op te baseren.
source_centrality: 0.7
source_ref: AIMM Competentieframework Data Literacy, competentie data_kwaliteit.train
status: validated
updated_at: '2026-05-20'
correlation_id: ronde18-lo-data-lit-202
---

# Datakwaliteit beoordelen: drie checks die je zelf kunt doen

Goede data is volledig, consistent en actueel. Met drie simpele checks kun je zelf beoordelen of je data betrouwbaar genoeg is om beslissingen op te baseren.

In Module 1 heb je geleerd dat data niet altijd klopt. Nu leer je hoe je dat zelf kunt checken. Want als je beslissingen neemt op slechte data, neem je slechte beslissingen.

### De drie kwaliteitschecks

**Check 1: Volledigheid -- ontbreekt er iets?**

Kijk of alle velden zijn ingevuld. Lege cellen of ontbrekende waarden zijn een signaal.

Stel jezelf de vraag:
- Staan alle metingen erin? Of ontbreken er uren/diensten?
- Zijn alle machines meegeteld? Of ontbreekt lijn 3?
- Zijn alle velden ingevuld? Of staat er ergens "n.v.t." waar een getal hoort?

**Vuistregel:** Als meer dan 10% van de data ontbreekt, wees voorzichtig met conclusies.

**Check 2: Consistentie -- klopt het met zichzelf?**

Dezelfde meting zou op dezelfde manier moeten worden vastgelegd. Inconsistente data is onbetrouwbaar.

Let op:
- Dezelfde eenheid? (kilogram vs gram, minuten vs uren)
- Dezelfde schrijfwijze? ("CNC-01" vs "cnc01" vs "CNC 1")
- Logische waarden? (een temperatuur van 3000 graden is waarschijnlijk een fout)
- Geen dubbele registraties? (dezelfde storing twee keer gelogd)

**Vuistregel:** Als je twee systemen vergelijkt en de totalen kloppen niet, is er een consistentieprobleem.

**Check 3: Actualiteit -- is het nog geldig?**

Data verliest waarde over tijd. Een OEE-score van vorige maand zegt minder dan die van vandaag.

Vraag jezelf af:
- Wanneer is deze data verzameld?
- Is er sindsdien iets veranderd? (nieuwe machine, ander materiaal, andere ploeg)
- Gebruik je de meest recente versie?

**Vuistregel:** Hoe sneller je omgeving verandert, hoe verser je data moet zijn.

### Het drie-stappenplan

Als je data moet beoordelen, doorloop dan altijd deze drie stappen:

1. **Scan op volledigheid** -- blader door de data, zoek lege plekken
2. **Check op consistentie** -- vergelijk eenheden, schrijfwijzen, logische waarden
3. **Controleer actualiteit** -- kijk naar de datum, vraag of er iets is veranderd

Als alle drie de checks positief zijn, kun je de data gebruiken. Als een of meer checks negatief zijn, meld het en gebruik de data met een voorbehoud.

### Wat doe je als de kwaliteit niet goed is?

- **Meld het.** Niet zelf repareren zonder dat iemand het weet.
- **Gebruik het met voorbehoud.** Zeg erbij: "Let op, de data van lijn 3 ontbreekt."
- **Verbeter de bron.** Afspraken maken over hoe data wordt ingevoerd.


## Praktijkvoorbeeld

Een teamleider wil het afkeurpercentage van deze week bespreken. Hij opent het rapport en ziet:
- Maandag: 1,2% -- dinsdag: -- -- woensdag: 0,9% -- donderdag: 1,8% -- vrijdag: 1,1%

Check 1 (volledigheid): dinsdag ontbreekt. Was er geen productie? Of is het niet geregistreerd? Hij moet het navragen.

Check 2 (consistentie): alle waarden zijn in percentages. Dat klopt.

Check 3 (actualiteit): het zijn cijfers van deze week. Actueel genoeg.

Conclusie: de data is BIJNA bruikbaar, maar de ontbrekende dinsdag maakt het weekgemiddelde onbetrouwbaar. De teamleider meldt dit en rekent het gemiddelde over vier dagen.
