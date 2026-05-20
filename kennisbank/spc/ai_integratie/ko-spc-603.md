---
id: ko-spc-603
title: Alarm fatigue — de cry-wolf valkuil van digitale SPC
type: tip
domain: spc
subdomain: ai_integratie
summary: 'Meer sensoren = meer alarmen. Excessieve false positives leiden

  tot alarm fatigue / "cry-wolf"-effect: operators verliezen

  vertrouwen en negeren signalen. Digitale SPC zonder

  alarmrationalisatie kan slechter uitpakken dan een simpele kaart

  met een goed reactieplan.'
source_centrality: 0.7
source_ref: Recente literatuur fault detection en alarm management; medische analogie
  patient monitoring alarm fatigue
status: validated
updated_at: '2026-05-20'
correlation_id: ronde28-lo-spc-603
---

# Alarm fatigue — de cry-wolf valkuil van digitale SPC

## Het probleem
Digitale SPC + AI levert **veel meer alarmen** op dan klassieke
SPC. Bij elk alarm dat **vals** blijkt te zijn, neemt het
operator-vertrouwen af.

Eindresultaat:
- Operator negeert alarmen ("toch weer vals")
- Operator schakelt alarmen uit
- Echte verstoringen worden gemist
- Het systeem wordt **onbetrouwbaar door overbetrouwbaarheid**

Dit heet **alarm fatigue** of het **"cry-wolf"-effect** (uit het
verhaal van de jongen die "wolf" riep).

## Waarom dit kritisch is in industriële omgevingen
In medische monitoring is alarm fatigue een bekend probleem (zie
literatuur over patient monitoring). In industriële omgevingen is
het minstens zo kritisch:
- Een gemiste verstoring kan **grote afkeur** veroorzaken
- In procesindustrie: **veiligheidsrisico**
- In automotive: **klantklachten / recalls**

## Tegenintuïtieve les
> Digitale SPC zonder alarmrationalisatie kan **slechter** uitpakken
> dan een **simpele kaart** met een goed reactieplan.

Een lijn met één papieren X̄-R-kaart en een betrouwbaar reactieplan
kan effectiever zijn dan een dashboard met 30 sensoren en honderd
false positives per dag.

## Alarmrationalisatie — wat is dat?
Het ontwerpproces om alleen de **echt zinvolle alarmen** te laten
bestaan:

| Stap | Wat |
|------|-----|
| 1. Inventariseren | Welke alarmen bestaan er? |
| 2. Frequentie-analyse | Hoe vaak gaat elk alarm af? |
| 3. Validiteit | Welk % is een echte verstoring? |
| 4. Prioriteren | Welke alarmen mogen niet worden gemist? |
| 5. Drempel-tunen | Met behoud van detectie, false positives reduceren |
| 6. Documenteren | Per alarm: wat, waarom, welke actie? |

## Voor AIMM-curriculum
In Module 1 (Gebruik) moet aandacht zijn voor:
- Hoe lees je een dashboard met meerdere alarmen?
- Hoe onderscheid je echte van valse alarmen?
- Wanneer escaleer je voor alarmrationalisatie?

In Module 3 (Op Maat) hoort:
- Hoe ontwerp je een alarmsysteem dat operators wél vertrouwen?
- Hoe richt je rationalisatie-cycli in?

## Verband met klassieke ARL-discussie
Dit is dezelfde afweging als bij Nelson-rules en ARL (zie
ko-spc-202). Met AI op grote schaal wordt de afweging alleen veel
scherper: één extra signaalregel × duizenden datapunten = veel
vals alarm.


## Praktijkvoorbeeld

Een productielijn voert 30 nieuwe sensoren in. Elke sensor heeft
±3σ-grenzen. Statistisch: bij 30 onafhankelijke sensoren en
Bonferroni-correctie zou je bijna geen alarmen verwachten — maar
zonder correctie krijgt het systeem ~30 × 0,27% = ~8% kans op één
vals alarm per meting.

Met meting elke minuut, 8 uur shift = 480 metingen → ~38 valse
alarmen per shift. Operator stelt na week 2 het systeem op "alleen
kritische alarmen" — en mist daarmee een echte verstoring in week 3.

Les: investeer eerst in **alarmrationalisatie** voordat je sensoren
uitbreidt.
