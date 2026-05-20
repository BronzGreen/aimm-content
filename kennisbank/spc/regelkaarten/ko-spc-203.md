---
id: ko-spc-203
title: Operator-respons bij een out-of-control signaal — vier stappen
type: tip
domain: spc
subdomain: regelkaarten
summary: 'Bij elk out-of-control signaal volgt de operator vier stappen:

  meetfout uitsluiten, recente proceswijziging checken, verdachte

  output veiligstellen, teamleider informeren. Geen actie zonder

  verificatie; geen hervatting zonder oorzaakanalyse.'
source_centrality: 0.7
source_ref: AIAG SPC Reference Manual; Ford PPAP Reaction Plan
status: validated
updated_at: '2026-05-20'
correlation_id: ronde17-lo-spc-203
---

# Operator-respons bij een out-of-control signaal — vier stappen

## De vier stappen bij elk signaal

### Stap 1: Meetfout uitsluiten
Een signaal is alleen geldig als de meting klopt. Check eerst:
- Is het meetinstrument gecalibreerd?
- Is de meting volgens procedure uitgevoerd?
- Is er een referentiestuk om opnieuw te meten?
- Gebruikt iemand misschien een verkeerde meetmethode?

Als de meting fout was: documenteer en herstart meten. Geen ingreep
op het proces.

### Stap 2: Laatste proceswijziging checken
Wat is er **recent** veranderd?
- Nieuwe materiaalbatch
- Setup-wissel
- Andere ploeg
- Onderhoud uitgevoerd
- Nieuwe of bijgeslepen tools
- Veranderde omgevingscondities (temperatuur, vocht)

### Stap 3: Verdachte output veiligstellen
Producten gemaakt **rond het signaal-moment** (en bij voorkeur sinds
het laatste in-control punt) moeten apart worden gezet. Niet
doorvoeren naar volgende processtap tot vrijgave.

### Stap 4: Teamleider informeren
Geen pogingen tot zelf-corrigeren zonder consultatie. Teamleider
besluit:
- Doorgaan na verificatie?
- Lijn stilleggen?
- Engineering inschakelen?
- 100% inspectie van verdachte output?

## De anti-regel: NIET doen
- **Niet** zomaar het proces "terugduwen" naar het gemiddelde —
  dat is tampering (zie ko-spc-105)
- **Niet** het signaal negeren omdat "het zo wel goed komt"
- **Niet** wachten tot meerdere signalen verschijnen
- **Niet** alleen de meetwaarde aanpassen in het systeem

## Documentatie
Elke signaal-respons wordt vastgelegd:
- Datum, tijd, kaart, regel die afging
- Genomen acties
- Gevonden oorzaak (of: nog onbekend)
- Vrijgave-besluit verdachte output

Deze logs zijn cruciaal voor patroonanalyse op teamleider-niveau.


## Praktijkvoorbeeld

Operator Daan meet om 13:45 een waarde buiten UCL op zijn X̄-R-kaart.
Hij doet:

1. Hij meet hetzelfde stuk opnieuw met een ander instrument →
   dezelfde uitslag (meetfout uitgesloten)
2. Hij checkt: om 13:30 is een nieuwe materiaalbatch geladen
   (wijziging gevonden)
3. Hij zet alle producten gemaakt sinds 13:30 apart in een rode bak
4. Hij belt teamleider Yasmin

Yasmin besluit: 100% inspectie van rode bak, materiaalbatch in
quarantaine voor leverancier-onderzoek, lijn doorlaten met monsters
van vorige batch tot validatie.
