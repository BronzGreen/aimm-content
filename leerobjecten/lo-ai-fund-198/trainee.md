---
id: lo-ai-fund-198-trainee
knowledge_object_id: ko-ai-fund-198
version: trainee
title: Kritisch denken over AI — bias en fouten herkennen
target_audience: operator
content_level: MBO-4
language_level: B1
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: trainen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde16-lo-ai-fund-198
---

# Hoe check je een AI-advies in 2-3 minuten — zonder álles te hoeven wantrouwen?

Een AI-systeem geeft je een advies. Cyclustijd verhogen. Voorraad bestellen. Onderhoud plannen. Je hebt twee opties: blind opvolgen of álles wantrouwen. Allebei fout. Tussen die uitersten ligt een werkbare aanpak. Drie checks. Vier vragen. Samen twee tot drie minuten. In deze sessie leer je het.

## Wat leer je?

Je leert drie checks toepassen op elke AI-output (de uitkomst die het systeem geeft). Je herkent een voorbeeld van vertekening (bias) in de context van de maakindustrie. En je kunt vier kritische vragen formuleren die je deze week aan IT of de leverancier kunt stellen.

## Casus — een advies in juli

Een operator bij een spuitgietmachine krijgt deze week een AI-advies: "verhoog cyclustijd met 1,2 seconde om afkeur te verminderen". Het advies is duidelijk en specifiek. Volgen?

De operator twijfelt. Vorige maand werd het advies ook opgevolgd en bleek het niet te kloppen. Hij stelt zichzelf drie vragen.

1. **Klopt dit met wat ik weet?** Vorige maand klopte het advies niet. Sinds toen veranderde er iets. Eind juni werd het buiten plotseling warmer. De fabriek warmt op. Warmere mallen hebben juist *kortere* cyclustijden nodig — niet langere.
2. **Is het advies compleet?** Er staat geen datum bij. Geen vermelding waarop het advies is gebaseerd. Geen score van zekerheid.
3. **Wat als ik het volg en het tegenvalt?** Verlies van 30 minuten productie per shift. Mogelijke kwaliteitsproblemen.

Hij stelt de vraag aan IT: op welke periode is dit systeem getraind? Antwoord: data van december (koude fabriek). Vertekening (bias)! De AI miste de zomer.

Bron: Npuls (2025), Raamwerk NL AI-Geletterdheid in het Onderwijs.

## De drie checks — in 2-3 minuten

Bij elke AI-output kun je drie korte checks doen.

### Check 1 — Betrouwbaarheid

Klopt het advies met wat jij weet uit ervaring? Heeft een collega iets vergelijkbaars meegemaakt? Is er recent iets veranderd dat de AI niet kon zien?

Bij de spuitgietmachine kwam check 1 als eerste: vorige maand klopte het advies niet, dat is een hint.

### Check 2 — Kwaliteit

Is het advies compleet en precies genoeg om actie te ondernemen? Staat er bij waarop het gebaseerd is? Is er een waarschijnlijkheid of zekerheidsscore meegegeven?

Bij de spuitgietmachine ontbrak de datum van de trainingsdata. Geen kwaliteits-info.

### Check 3 — (On)bedoelde effecten

Wat gebeurt er als je het advies volgt en het zou tegenvallen? Wat verlies je dan — tijd, geld, kwaliteit, veiligheid? Hoe groot is dat risico?

Bij de spuitgietmachine: 30 minuten productieverlies per shift was de uitkomst van een opgevolgd onjuist advies.

## Wat is vertekening (bias) eigenlijk?

Vertekening (bias) is *scheefheid*. AI leert uit data. Als die data scheef is, is de AI ook scheef. Niet omdat iemand het zo wilde — maar omdat de wereld waarin de AI is opgegroeid niet de hele wereld was.

In de maakindustrie zijn er drie typische bronnen van vertekening:

1. **Trainingsdata (leerdata) uit één ploeg.** AI werkt slecht in andere ploeg.
2. **Trainingsdata van één machine.** AI schat een andere machine verkeerd in.
3. **Trainingsdata van één seizoen.** AI mist winter- of zomereffecten — zoals bij de spuitgietmachine.

Vertekening is niet altijd zichtbaar. Vaak ontdek je het pas als de AI structureel anders oordeelt over vergelijkbare gevallen. Dat is het moment om door te vragen.

## Vier kritische vragen

Train jezelf om deze vier vragen altijd te stellen bij AI-output. Je hoeft ze niet allemaal te beantwoorden — een vraag stellen aan IT is óók een antwoord.

1. **Welke data heeft de AI gezien om hier te komen?** Welke periode, welke machines, welke ploegen, welke producten?
2. **Waarin lijkt mijn situatie op die data, waarin niet?** Een nieuwe leverancier? Een ander seizoen? Een andere machine? Een ander product?
3. **Welke fouten maakt dit type AI meestal?** Inspectie-AI mist soms zeldzame defecttypes. Onderhouds-AI raadt soms te vroege vervanging aan. Vraag het na.
4. **Welke rol wil ik dat AI speelt?** Suggestie (ik beslis zelf), bewaking (alarmeer me alleen bij grote afwijking), of beslisser (de AI doet het zelf)?

De laatste vraag is de belangrijkste. Niet elk AI-systeem hoort beslisser te zijn. Bij hoge gevolgen — veiligheid, terugroepactie — is "suggestie" vaak gepaster dan "beslisser".

## Kritisch denken is geen wantrouwen

Een veelgemaakte denkfout: kritisch denken betekent "alles wantrouwen". Dat klopt niet.

Kritisch denken is de **slimme-collega-houding**. Je luistert naar een collega met goede ervaring. Je checkt of wat hij zegt past in jouw situatie. Bij twijfel vraag je door. En je beslist zelf.

Precies dat doe je met een AI-output. Luister, check (drie keer), beslis zelf.

## Waarom dit ertoe doet

Een operator die in juli een advies uit december opvolgt zonder check, verliest 30 minuten productie per shift. Per maand: tien uur. Een teamleider die niet vraagt op welke periode het systeem is getraind, mist een vertekening die het hele kwartaal doorwerkt. Drie checks plus vier vragen kosten samen twee tot drie minuten. Ze voorkomen dure misverstanden.

Wie deze procedure routine maakt:

- **Volgt niet blind**, ook niet wanneer de AI specifiek klinkt.
- **Wantrouwt niet alles**, voorkomt onnodige discussies en verspilling.
- **Stelt gerichte vragen** aan IT of leverancier — geen vage zorgen, wel concrete punten.
- **Bouwt een team-routine** waarin checken normaal wordt — niet alleen jouw zorg.

## Zelf zien gebeuren?

Open op tablet of laptop het interactieve `model-kritisch-denken-ai.jsx`. Je krijgt zes AI-adviezen — van een spuitgietmachine in de zomer tot een planningsassistent die het juist goed doet. Per advies kies je welke van de drie checks alarm geeft: betrouwbaarheid, kwaliteit, bedoelde effecten — of: het advies lijkt OK. Per case zie je welke bias-bron speelt (ploeg, machine, seizoen). Aan het eind krijg je de vuistregel: drie checks in 2-3 minuten besparen vaak uren.

## Na deze sessie

Kies deze week één AI-advies of melding die je krijgt op de werkvloer. Bijvoorbeeld van de inspectiecamera, het onderhoudsdashboard, of een planningssysteem. Pas in 2-3 minuten de drie checks toe voordat je het opvolgt:

- Betrouwbaarheid — klopt dit met wat jij weet uit ervaring?
- Kwaliteit — is het compleet, weet je waarop het gebaseerd is?
- Bedoelde effecten — wat als je dit volgt en het zou tegenvallen?

Kies daarna één van de vier kritische vragen om deze week aan IT of de leverancier te stellen. Bijvoorbeeld: "welke data heeft het systeem gezien?" of "welke fouten maakt dit type AI meestal?" Neem het antwoord mee naar de volgende sessie. Vraag ook aan één collega: "Hoe check jij eigenlijk een AI-advies voordat je het opvolgt?" Je hoort vaak verschillende routines. Daar leer je beiden van.

---

## Werkbladen (Kolb-cyclus)

1. [`wb-01-casus-spuitgietmachine.md`](./werkbladen/wb-01-casus-spuitgietmachine.md) — Casus spuitgietmachine
2. [`wb-02-buurman-drie-checks.md`](./werkbladen/wb-02-buurman-drie-checks.md) — Buurman drie checks
3. [`wb-03-handout-checks-vragen.md`](./werkbladen/wb-03-handout-checks-vragen.md) — Handout checks vragen
4. [`wb-04-eigen-advies-checks.md`](./werkbladen/wb-04-eigen-advies-checks.md) — Eigen advies checks

## Verder

- Onderliggend kennisobject: [`ko-ai-fund-198`](../../kennisbank/ai_fundamentals/ai_ethics_en_bias/ko-ai-fund-198.md)
- Voor de begeleider: [`trainer.md`](./trainer.md) + [`draaiboek.md`](./draaiboek.md)
