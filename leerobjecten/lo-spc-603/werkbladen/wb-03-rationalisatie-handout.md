# Handout: Alarmrationalisatie in 6 stappen
*Alarm fatigue voorkomen — ontwerpproces, geen quick fix*

**Module 3 — SPC Op Maat | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Minder alarmen die je vertrouwt is beter dan meer alarmen die je negeert."**

Een dashboard met 30 sensoren en 38 valse alarmen per shift kán slechter werken dan één papieren X̄-R-kaart met een goed reactieplan. Niet omdat de techniek faalt, maar omdat **vertrouwen** — niet hoeveelheid — bepaalt of een operator een alarm serieus neemt.

---

## 🔵 Wat is alarm fatigue / cry-wolf?

*Het mechanisme in vier zinnen.*

1. Meer sensoren = **meer alarmen**, waarvan een (groot) deel **vals positief** is.
2. Bij elk vals alarm neemt het **operator-vertrouwen** in het systeem af.
3. Boven een drempel: operator **negeert** of **schakelt alarmen uit**.
4. Eindresultaat: het systeem wordt **onbetrouwbaar door overbetrouwbaarheid** — een echte verstoring wordt gemist.

Dit heet **alarm fatigue** (uit medische monitoring: ICU-verpleegkundige met 700 alarmen per shift hoort niets meer) of het **"cry-wolf"-effect** (uit het verhaal van de jongen die "wolf" riep — als de echte wolf komt, gelooft niemand hem nog).

---

## 🟠 Waarom kritisch in industriële context?

*De pijn is groter dan in medische monitoring vaak — alleen minder zichtbaar.*

| Sector | Risico bij gemiste verstoring |
|--------|-------------------------------|
| **Automotive** | Klantklachten, PPM-overschrijding, recalls |
| **Procesindustrie** | Veiligheidsincident (lekkage, brand, explosie) |
| **Spuitgieten / verpakking** | Massa-afkeur (denk: 240 onderdelen op één ploeg) |
| **Medisch / farma** | Patiëntveiligheid, inspectie-issues |

**Vuistregel uit de praktijk:** elke vals positief boven 10% leidt op termijn tot vertrouwensverlies. Boven 30% wordt het systeem structureel genegeerd. Boven 50% is het effectief uitgeschakeld — ongeacht of het technisch nog 'aan' staat.

---

## 🟣 De tegenintuïtieve les

> Digitale SPC zonder alarmrationalisatie kan **slechter** uitpakken dan een **simpele kaart met een goed reactieplan**.

Eén papieren X̄-R-kaart, gemonitord door een operator die alle signalen serieus neemt, vangt vaak meer **echte verstoringen** dan een dashboard met 30 sensoren waarvan de operator er 27 negeert. Dit is geen anti-technologie-pleidooi — het is een ontwerp-principe: **minder alarmen die je vertrouwt > meer alarmen die je negeert.**

Wat je dus toevoegt aan een sensoruitbreiding moet altijd gepaard gaan met **rationalisatie** — anders haalt de uitbreiding zichzelf onderuit.

---

## 🔵 De 6 stappen van alarmrationalisatie

*Een ontwerpproces, geen one-shot. Vaak per kwartaal herhalen na uitbreidingen of veranderingen.*

### Stap 1 — Inventariseren
**Vraag:** Welke alarmen bestaan er op deze lijn?  
**Hoe:** Lijst trekken uit MES, dashboard-config of sensorleverancier. Niet alleen 'actieve' alarmen — ook de uitgeschakelde, want die vertellen wat ooit teveel werd.  
**Resultaat:** Volledige lijst met alarm-naam, sensor, type signaal, huidige status.

### Stap 2 — Frequentie-analyse
**Vraag:** Hoe vaak gaat elk alarm af?  
**Hoe:** MES-log over minimaal 4 weken doorlopen. Per alarm: aantal triggers per shift, per dag, per week.  
**Resultaat:** Top-10 meest frequente alarmen — daar zit je rationalisatiewinst.

### Stap 3 — Validiteit
**Vraag:** Welk percentage van elk alarm is een **echte** verstoring?  
**Hoe:** Steekproef van triggers koppelen aan operator-logboek of kwaliteitsrapport: was er iets aan de hand of niet? Ruwe inschatting (10%, 30%, 50%) is voldoende — exacte cijfers zijn fijn maar geen vereiste.  
**Resultaat:** Per alarm: validiteit-ratio (true positive rate).

### Stap 4 — Prioriteren
**Vraag:** Welke alarmen mogen onder géén voorwaarde gemist worden?  
**Hoe:** Combineer klantimpact (afkeur, recall), veiligheid (incident), regelgeving (audit). Top-3 of top-5 — niet meer.  
**Resultaat:** Onaantastbare set alarmen die altijd kritisch blijven, wat de frequentie ook is.

### Stap 5 — Drempel-tunen
**Vraag:** Hoe verklein je het aantal valse positieven, **zonder** dat je echte verstoringen mist?  
**Hoe:** Per alarm uit de top-10 (stap 2): drempel verhogen, samenvoegen met ander alarm (alleen triggeren als beide afgaan), tijdvenster vergroten (alleen alarm bij 3 triggers binnen 5 minuten), of uitschakelen als de validiteit-ratio < 5%. Test elke wijziging op historische data voordat je live gaat.  
**Resultaat:** Geverifieerde drempel-aanpassingen, met behoud van detectiekracht.

### Stap 6 — Documenteren
**Vraag:** Wat doe je bij elk overgebleven alarm — wat is de actie?  
**Hoe:** Per alarm: één regel met **wat** het signaleert, **waarom** het belangrijk is, **welke actie** de operator moet nemen. Dit is je reactieplan-document.  
**Resultaat:** Operators weten bij elk alarm wat ze moeten doen — vertrouwen wordt herbouwd.

---

## 🟢 Hoe vaak herhalen?

*Alarmrationalisatie is geen project, het is een proces.*

| Moment | Wat doe je? |
|--------|-------------|
| **Na elke sensoruitbreiding** | Volledige rationalisatie vóór go-live (anders krijg je het cry-wolf-patroon gegarandeerd) |
| **Per kwartaal** | Frequentie- en validiteit-check (stap 2 + 3) op de top-10 |
| **Bij operator-klacht** | Specifiek alarm bekijken — operators zijn de eerste signaalgever van fatigue |
| **Bij gemiste verstoring** | Root-cause-analyse: was het een gerationaliseerd alarm dat niet had moeten worden weggetuned? |

---

## 🔴 Drie veelgemaakte fouten — pas op!

*Rationalisatie kan ook misgaan. Dit zijn de valkuilen.*

| # | Fout | Wat gebeurt er? |
|---|------|-----------------|
| 1 | **Te agressief uitschakelen** | Je verlaagt false positives, maar mist nu ook echte verstoringen. Altijd validiteit-ratio (stap 3) leidend laten zijn — niet alleen frequentie. |
| 2 | **Operators niet betrekken** | Engineering tunet in vergaderkamer; operator weet niet welk alarm wat doet. Vertrouwen herstelt niet. → **Operator zit aan tafel bij stap 4 én stap 6**. |
| 3 | **Eenmalig project, geen proces** | Na 3 maanden lopen drempels weer scheef (procesdrift, nieuwe productlijn, andere ploegmix). → Per kwartaal herhalen, anders kruipt fatigue terug. |

---

## 🟠 Verband met andere kennisobjecten

*Alarmrationalisatie staat niet op zichzelf — het is verbonden met klassieke SPC-keuzes en met AI-uitbreidingen.*

| Onderwerp | Waar vind je dat? | Relatie |
|-----------|-------------------|---------|
| **ARL en Nelson-rules** | lo-spc-202 | Dezelfde afweging op kleinere schaal: hoe gevoelig wil je een signaalregel? Met AI op grote schaal wordt deze afweging veel scherper — één extra regel × duizenden datapunten = veel vals alarm. |
| **AI-uitbreiding van SPC** | lo-spc-602 | AI-modellen voegen veel signalen toe. Zonder rationalisatie versterkt AI het cry-wolf-effect in plaats van het op te lossen. |
| **Capability-valkuilen** | ko-spc-303 | Eerst stabiel proces, dan capability — alarmen op een instabiel proces gaan altijd af. Rationalisatie heeft geen zin als de basis niet klopt. |

---

## 🟢 Onthoud dit

1. **Vertrouwen, niet hoeveelheid**, bepaalt of een alarm wordt opgepakt.
2. **38 valse alarmen per shift** is voorspelbaar bij 30 sensoren ±3σ zonder rationalisatie — geen ongeluk.
3. **Operator zet alarmen uit** = systeem heeft gefaald, niet de operator.
4. **6 stappen** = inventariseren → frequentie → validiteit → prioriteren → drempel-tunen → documenteren.
5. **Kwartaalproces**, geen project — fatigue kruipt terug.
6. **Operators aan tafel** bij prioriteren en documenteren — anders herstelt vertrouwen niet.
7. **Simpele kaart met goed reactieplan** kan effectiever zijn dan complex dashboard zonder rationalisatie.

---
*Bron: ko-spc-603; AIAG SPC reference manual (alarm management); Hollnagel — Safety-II; medische literatuur ICU alarm fatigue (Sendelbach & Funk, 2013) | AIMM Module 3 — SPC Op Maat | v1.0*
