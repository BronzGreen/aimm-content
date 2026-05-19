# Draaiboek: Datatypes herkennen en datakwaliteit beoordelen

**Leerobject:** lo-data-lit-201
**Kennisobjecten:** ko-data-lit-201 + ko-data-lit-202
**Doelgroep:** MBO-3 operator, B1 taalniveau
**Duur:** 45 minuten
**Groepsgrootte:** 6-12 deelnemers
**Opstelling:** Groepstafels (4 per tafel) of U-vorm

---

## Kernprincipe: Coachen -- de deelnemers doen het zelf

Module 2 verschuift van TRAINEN (Module 1) naar COACHEN. De deelnemers zijn na Module 1 bewust bekwaam. Ze weten wat data is, kunnen een dashboard lezen. Nu gaan ze ZELF aan de slag met datatypes en kwaliteitschecks.

| Fase | Wie doet? | Ondersteuning | Activiteit |
|------|----------|---------------|------------|
| 1. Experimenteren | **Duo's** doen zelf | Minimaal | Sorteerkaarten datatypes |
| 2. Reflecteren | **Groep** bespreekt | Medium | Twijfelgevallen bespreken |
| 3. Theoretiseren | **Trainer** legt uit | Medium | Drie kwaliteitschecks |
| 4. Ervaren | **Duo's** doen zelf | Minimaal | Fouten vinden in dataset |

---

## Voorbereiding (15 minuten voor aanvang)

### Materialen printen
- [ ] Werkblad 1: Sorteerkaarten datatypes (1x per deelnemer)
- [ ] Werkblad 2: Theorie-handout drie kwaliteitschecks (1x per deelnemer)
- [ ] Werkblad 3: Kwaliteitscheck-oefening met dataset (1x per deelnemer)
- [ ] Werkblad 4: Transferopdracht (1x per deelnemer)

### Optioneel
- [ ] Sorteerkaarten uitknippen als fysieke kaarten (leuker, kost meer voorbereiding)

### Ruimte
- [ ] Flip-over + stiften
- [ ] Groepstafels of U-vorm

---

## FEED-UP (0:00 - 0:01)

> "Na deze sessie kun je het verschil herkennen tussen vier soorten data: getallen, categorieën, tijddata en tekst. En je kunt checken of data betrouwbaar genoeg is om beslissingen op te nemen."

---

## ACTIVITEIT 1: Sorteerkaarten Datatypes (0:01 - 0:12)

### Doel
Duo's classificeren 16 datapunten in vier categorieën.

### Scaffolding-niveau: JIJ DOET (direct beginnen met oefening)

### Stap voor stap

**0:01** Deel werkblad 1 uit.

> "Jullie krijgen 16 kaarten met data uit de productie. Sorteer ze in vier groepen: getallen, categorieën, tijddata en tekst. Werk samen met je buurman. Jullie hebben 8 minuten."

**0:01-0:09** Loop rond. Stel vragen, geef GEEN antwoorden:
- "Kun je hiermee rekenen?"
- "Is het een keuze uit een vaste lijst?"
- "Gaat het over wanneer?"

**0:09** Plenaire bespreking. Focus op de 3-4 lastige kaarten:

> "Foutcode E-03 -- velen van jullie twijfelden. Is het tekst? Nee, het is een categorie. Waarom? Omdat het een keuze is uit een VASTE LIJST van foutcodes. Je kunt er niet mee rekenen, maar je kunt wel tellen hoe vaak E-03 voorkomt."

> "Storingsduur 14 minuten -- dat lijkt op tijddata, maar het is een GETAL. Je kunt ermee rekenen: gemiddelde storingsduur, totale storingsduur. Een datum (2026-04-08) is wél tijddata."

### Valkuilen
- Alle 16 kaarten nabespreken. Focus op de 3-4 lastige.
- Het antwoord geven als een duo twijfelt. Stel een tegenvraag.

### Differentiatie
- **Sterke groep:** Laat ze per datatype benoemen wat je ermee kunt doen.
- **Zwakke groep:** Schrijf de drie beslissingsvragen op het bord vooraf.

---

## ACTIVITEIT 2: Groepsbespreking Twijfelgevallen (0:12 - 0:22)

### Doel
Reflecteren op de sorteeroefening, inzichten delen.

### Scaffolding-niveau: WIJ DOEN

### Stap voor stap

**0:12** > "Welke kaarten vonden jullie lastig? Waarom?"

Laat 3-4 duo's hun twijfelgeval noemen. Begeleid naar inzichten.

**0:20** Maak de overgang naar kwaliteit:

> "Jullie kunnen nu datatypes herkennen. Maar zelfs als je weet WAT voor data het is -- klopt de data ook? Daar gaan we nu naar kijken."

### Valkuilen
- Te lang blijven hangen bij de sorteeroefening. Max 10 minuten.
- De overgang naar kwaliteitschecks vergeten.

---

## ACTIVITEIT 3: Drie Kwaliteitschecks (0:22 - 0:30)

### Doel
Kort theoretisch kader: volledigheid, consistentie, actualiteit.

### Stap voor stap

**0:22** Deel werkblad 2 uit.

> "In Module 1 heb je geleerd dat data niet altijd klopt. Nu leer je drie checks om dat zelf te controleren."

Loop de drie checks door met voorbeelden uit de sorteerkaarten:

> 1. "**Volledigheid:** stel dat je set maar 14 kaarten had. Dan mis je informatie."
> 2. "**Consistentie:** op de ene kaart staat CNC-01, op de andere cnc01. Dat is inconsistent."
> 3. "**Actualiteit:** als de kaarten data van vorig jaar bevatten terwijl je deze week wilt analyseren."

### Valkuilen
- Langer dan 8 minuten praten. De oefening is het leerpunt, niet de theorie.
- Formules of statistiek introduceren.

---

## ACTIVITEIT 4: Kwaliteitscheck op Dataset (0:30 - 0:45)

### Doel
Duo's vinden fouten in een bewust vervuilde productiedataset.

### Scaffolding-niveau: JIJ DOET

### Stap voor stap

**0:30** Deel werkblad 3 uit.

> "Jullie krijgen een dataset van een productielijn. Er zitten fouten in. Voer de drie checks uit en noteer elke fout. 10 minuten."

**0:30-0:40** Loop rond. Minimale ondersteuning. Stel alleen vragen:
- "Hoeveel rijen heb je gecheckt?"
- "Wat is de eenheid in deze kolom? En in die rij?"
- "Van wanneer is deze data?"

**0:40** Antwoordmodel bespreken:

> | Fout | Check | Uitleg |
> |------|-------|--------|
> | Rij 5: stilstand leeg | Volledigheid | Ontbrekende waarde |
> | Rij 8: ploeg leeg | Volledigheid | Ontbrekend gegeven |
> | Rij 3: cnc01 | Consistentie | Andere schrijfwijze |
> | Rij 8: temp 2850 | Consistentie | Onlogische waarde |
> | Rij 15: 0,5 uur | Consistentie | Andere eenheid |
> | Rij 12-15: 2025 | Actualiteit | Data van vorig jaar |

Succesfeedback: "3 of meer gevonden? Goed gedaan. Je kunt nu zelf datakwaliteit beoordelen."

**0:43** Deel werkblad 4 (transferopdracht) uit.

> "Neem deze week een dataset van je eigen afdeling. Bepaal de datatypes en voer de drie checks uit. Neem je bevindingen mee naar de volgende bijeenkomst."

### Valkuilen
- De temperatuur van 2850 als enige fout bespreken. Er zijn er meer.
- De transferopdracht vergeten.

---

## Tijdsoverzicht

| Tijd | Activiteit | Scaffolding | Duur |
|------|-----------|-------------|------|
| 0:00-0:01 | Feed-up | n.v.t. | 1 min |
| 0:01-0:09 | Sorteerkaarten (duo's) | JIJ DOET | 8 min |
| 0:09-0:12 | Nabespreking sorteerkaarten | WIJ DOEN | 3 min |
| 0:12-0:22 | Groepsbespreking twijfelgevallen | WIJ DOEN | 10 min |
| 0:22-0:30 | Theorie drie kwaliteitschecks | n.v.t. | 8 min |
| 0:30-0:40 | Kwaliteitscheck op dataset (duo's) | JIJ DOET | 10 min |
| 0:40-0:43 | Antwoordmodel + feedback | n.v.t. | 3 min |
| 0:43-0:45 | Transferopdracht | n.v.t. | 2 min |
| **Totaal** | | | **45 min** |

---

## Noodplan: tijd te kort

Als je bij activiteit 4 minder dan 10 minuten over hebt:
- Verkort de dataset-oefening naar 6 minuten (alleen check 1 en 2)
- Bespreek het antwoordmodel mondeling
- Geef de transferopdracht altijd
