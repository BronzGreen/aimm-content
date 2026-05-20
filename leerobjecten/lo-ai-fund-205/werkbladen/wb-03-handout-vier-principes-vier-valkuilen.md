# Werkblad 3 — Vier principes en vier valkuilen (handout)
*Data labelen — Activiteit: Theoretiseren*

**Naam:** ____________________  **Datum:** __________

**Tijdsindicatie:** 13 minuten

---

> **De kern**
> Goede labels zijn de basis voor een goed AI-model. Vier principes maken een labelschema bruikbaar. Vier valkuilen maken labelwerk lastiger dan het lijkt. Hieronder vind je beide blokken op één A4. Markeer met je stift wat voor jou nieuw is. Markeer ook wat je vandaag bij jezelf hebt gemerkt.

---

## Blok 1 — Vier principes van goed labelen

### 1. Consistentie

Hetzelfde voorbeeld krijgt altijd hetzelfde label. Dat geldt voor jou over de hele dag. Het geldt ook tussen jou en je collega.

Hoe meet je dit? Door inter-rater agreement (inter-beoordelaar-overeenkomst) — precies wat jullie net deden.

> *Hoog inter-rater agreement = bruikbare labels. Laag = signaal dat het schema scherper kan.*

### 2. Helderheid

Labels staan vooraf vast. Met grenswaarden. Geen ambiguïteit (geen ruimte voor twijfel).

Test: kan een nieuwe collega het schema lezen en direct toepassen? Lukt dat? Dan is je schema helder genoeg.

### 3. Dekking

Alle relevante situaties zitten in de trainingsdata (leerdata). Niet alleen de makkelijke voorbeelden.

Voorbeelden die er vaak in ontbreken:

- Zeldzame defecten op het zichtvlak.
- Producten van een nieuwe leverancier.
- Foto's gemaakt in nachtploeg-licht.

Test: zijn de zeldzame defecten ook gelabeld? Of alleen de duidelijke?

### 4. Domeinkennis

Jij weet wat een label betekent in de praktijk. Een operator met tien jaar ervaring ziet een grensgeval direct. Een buitenstaander niet.

Zonder vakkennis valt label-werk uit elkaar. Daarom is labelen werk voor mensen op de werkvloer — niet voor mensen achter een bureau.

---

## Blok 2 — Vier valkuilen bij labelwerk

### a. Vermoeidheids-drift

Na 100 foto's word je minder consistent. Je kijkt sneller. Je twijfelt minder.

**Wat je kunt doen:** pauzeer elk uur. Vijf minuten weg van het scherm helpt al.

### b. Confirmation bias (bevestigings-valkuil)

Je verwacht een label. Daardoor zie je het ook. Na tien keer GOED verwacht je nog een GOED.

**Wat je kunt doen:** wissel periodiek met een collega. Laat hem af en toe meekijken.

### c. Gemak boven precisie

Een twijfelproduct krijgt soms GOED. Omdat dat sneller is dan TWIJFEL invullen.

**Wat je kunt doen:** twijfel hoort het label TWIJFEL te krijgen. Niet GOED. Het schema is daar precies voor.

### d. Operator-verschillen

Twee operators kiezen niet altijd hetzelfde. Sommige mensen denken: één van de twee zit fout. Dat is meestal niet zo.

**Wat je kunt doen:** verschillen zijn signaal voor het schema. Niet voor de operator. Breng ze naar wie het schema beheert.

---

## Terug naar jullie buurman-vergelijking

*Welk principe heeft jullie verschillen het beste verklaard?*

- [ ] Principe 1 — Consistentie (we waren niet hetzelfde).
- [ ] Principe 2 — Helderheid (het schema-woord was vaag).
- [ ] Principe 3 — Dekking (dit type voorbeeld ontbrak).
- [ ] Principe 4 — Domeinkennis (een van ons keek met andere ervaring).

*En welke valkuil herken jij van vandaag?*

- [ ] a. Vermoeidheids-drift (na voorbeeld 15 keek ik anders).
- [ ] b. Confirmation bias (ik verwachtte vooral GOEDs te zien).
- [ ] c. Gemak boven precisie (ik koos soms GOED in plaats van TWIJFEL).
- [ ] d. Operator-verschillen (mijn buurman zag het echt anders).

---

## Mijn aha-moment

Welk principe was voor mij vandaag nieuw of het scherpst?

________________________________________________________________

________________________________________________________________

Welke valkuil ga ik mezelf op betrappen, vanaf vandaag?

________________________________________________________________

________________________________________________________________

---

## Vakwoorden in dit werkblad

| Vakterm | Betekenis in één zin |
|---|---|
| **Label (etiket)** | Het juiste antwoord bij een voorbeeld, bijvoorbeeld GOED of AFGEKEURD. |
| **Labelschema** | De afspraak welke labels er zijn en wanneer je ze gebruikt. |
| **Inter-rater agreement (inter-beoordelaar-overeenkomst)** | Hoe vaak twee mensen hetzelfde label kiezen, in procenten. |
| **Confirmation bias (bevestigings-valkuil)** | Je ziet wat je verwacht, niet wat er staat. |
| **Vermoeidheids-drift** | Na veel labelen kies je minder zorgvuldig. |
| **Domeinkennis** | Vakkennis over het product en het proces. |

---

> **Onthoud:** een labelschema is een levend document. Het start simpel. Het wordt scherper door jullie verschillen. Jullie ervaring van vandaag is waardevolle input voor de versie van volgende week.

---

*Bron: AIMM praktijklessen labelwerk + ko-ai-fund-002, ko-ai-fund-003, ko-ai-fund-023.*
*AIMM x BronzGreen — AI Fundamentals · Module 2 · Data labelen (lo-ai-fund-205) — v1.0*
