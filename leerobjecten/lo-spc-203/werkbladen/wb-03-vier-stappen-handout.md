# Handout: De Vier Stappen bij een Signaal
*Operator-respons bij een out-of-control signaal — AIAG / Ford reaction plan*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**  
> Een signaal op de regelkaart vraagt om een vaste, geoefende volgorde van vier stappen — niet om een snelle oplossing. Wie de volgorde aanhoudt, voorkomt drie veelgemaakte fouten: ingrijpen op een meetfout, doorvoeren van verdachte producten, en zelf-corrigeren zonder dat iemand het weet.

---

## De vier stappen — in deze volgorde

| Stap | Wat doe je? | Waarom in deze volgorde? |
|------|-------------|--------------------------|
| **1** | **Meetfout uitsluiten** | Een verkeerde meting is geen signaal. Eerst checken voordat je iets doet aan het proces. |
| **2** | **Laatste proceswijziging checken** | Als er iets recent veranderd is, weet je vaak meteen waar je moet kijken. |
| **3** | **Verdachte output veiligstellen** | Producten gemaakt rond het signaal-moment mogen niet doorgevoerd worden tot vrijgave. |
| **4** | **Teamleider informeren** | Geen zelf-corrigeren zonder consultatie. De teamleider beslist over doorgaan, stilleggen of opschalen. |

---

## 🔵 Stap 1 — Meetfout uitsluiten

*Een signaal is alleen geldig als de meting klopt. Dus eerst: klopt mijn meting wel?*

**Check vier dingen:**

- ☐ Is mijn meetinstrument gecalibreerd?
- ☐ Heb ik gemeten volgens de juiste procedure?
- ☐ Is er een referentiestuk waarmee ik opnieuw kan meten?
- ☐ Heb ik per ongeluk de verkeerde meetmethode gebruikt?

**Als de meting fout was:** documenteer wat er mis was en herstart de meting. Doe níets aan het proces.

**Als de meting klopt:** ga door naar stap 2.

---

## 🔵 Stap 2 — Laatste proceswijziging checken

*Wat is er recent veranderd? Begin bij de laatste paar uur, werk terug.*

**Vraag jezelf af:**

- ☐ Is er een nieuwe materiaalbatch geladen?
- ☐ Is er een setup-wissel geweest?
- ☐ Is er een andere ploeg begonnen?
- ☐ Is er onderhoud uitgevoerd?
- ☐ Zijn er nieuwe of bijgeslepen tools in gebruik?
- ☐ Zijn de omgevingscondities veranderd (temperatuur, vocht)?

**Als je een wijziging vindt:** noteer wat het was. Dat helpt bij stap 4.

**Geen wijziging gevonden:** ook dat is een uitkomst — meld dat aan de teamleider.

---

## 🟠 Stap 3 — Verdachte output veiligstellen

*Producten die gemaakt zijn rond het signaal-moment mogen niet zomaar verder.*

**Wat is 'verdachte output'?**

- Alle producten gemaakt tussen het laatste 'goede' meetmoment en nu.
- Bij voorkeur: alle producten sinds de laatste in-control meting.

**Wat doe je ermee?**

- ☐ Apart zetten in een rode bak / quarantaine-rek / aangewezen plek
- ☐ Markeren met datum + tijd + reden ('signaal regelkaart 13:45')
- ☐ Niet doorvoeren naar de volgende processtap tot vrijgave
- ☐ Niet weggooien — de teamleider of kwaliteit beslist

**Geen rode bak op je lijn?** Regel een afzetplek vóór het volgende signaal.

---

## 🟠 Stap 4 — Teamleider informeren

*Geen zelf-corrigeren zonder consultatie. De teamleider beslist.*

**Wat geef je door?**

- ☐ Welke kaart een signaal gaf (welke meting, welke regel)
- ☐ Datum, tijd en de meetwaarde
- ☐ Wat je in stap 1 hebt gecheckt (meetfout uitgesloten?)
- ☐ Wat je in stap 2 hebt gevonden (welke wijziging is recent?)
- ☐ Waar de verdachte output staat (hoeveel stuks, welke plek)

**De teamleider beslist over:**

- Doorgaan na verificatie?
- Lijn stilleggen?
- Engineering inschakelen?
- 100% inspectie van verdachte output?

---

## 🔴 Wat doe je NIET — de anti-regel

| Verkeerd | Waarom verkeerd |
|----------|-----------------|
| **Direct aan een knop draaien** om het gemiddelde 'terug te duwen' | Dit heet **tampering** — je behandelt common cause als special cause en maakt het proces juist instabieler (zie ko-spc-105) |
| **Het signaal negeren** omdat 'het zo wel goed komt' | Een signaal staat er niet zomaar — wegkijken laat verdachte producten doorgaan |
| **Wachten tot meerdere signalen verschijnen** | Bij het tweede signaal is je verdachte output al de poort uit |
| **Alleen de meetwaarde aanpassen** in het systeem | Dat is data-vervalsing — geen oplossing, wel een groot probleem |
| **De teamleider bellen voordat je stap 1 hebt gedaan** | De teamleider kan niets met 'er ging een lampje af' — hij heeft je check nodig |
| **Verdachte output doorvoeren** omdat 'het er goed uitziet' | Het ziet er altijd goed uit, daar gaat het juist om |

---

## 📋 De praktijkcasus — Daan op de spuitgietlijn

> **13:45** — Operator Daan meet 100,45 g op zijn X̄-R-kaart. Het punt staat buiten UCL.

**Stap 1:** Daan meet hetzelfde stuk opnieuw met een ander instrument → dezelfde uitslag. *Meetfout uitgesloten.*

**Stap 2:** Daan checkt het logboek: om 13:30 is een nieuwe materiaalbatch geladen. *Wijziging gevonden.*

**Stap 3:** Daan zet alle 30 producten gemaakt sinds 13:30 apart in een rode bak. *Verdachte output veiliggesteld.*

**Stap 4:** Daan belt teamleider Yasmin met alle informatie van stap 1, 2 en 3.

**Yasmin beslist:** 100% inspectie van de rode bak, materiaalbatch in quarantaine voor leverancier-onderzoek, lijn doorlaten met monsters van vorige batch tot validatie.

> **Resultaat:** geen verdachte producten naar de klant, oorzaak in beeld, lijn niet onnodig stilgelegd. Tijd: 15 minuten.

---

## 📝 Documentatie — wat leg je vast?

Elke signaal-respons wordt vastgelegd in het lijn-logboek of het kwaliteitssysteem:

- Datum, tijd, kaart, welke regel afging
- Genomen acties (stap 1, 2, 3)
- Gevonden oorzaak (of: nog onbekend)
- Vrijgave-besluit verdachte output (van wie?)

Deze logs zijn cruciaal: de teamleider kan op patronen letten die jij in losse signalen niet ziet (bijvoorbeeld: 'altijd een signaal na batchwissel van leverancier X').

---

## 🟢 Onthoud dit

1. **Volgorde is alles.** Stap 1 → 2 → 3 → 4. Niet door elkaar.
2. **Geen actie zonder verificatie.** Eerst meetfout uitsluiten.
3. **Geen hervatting zonder oorzaakanalyse.** Pas weer draaien als de teamleider het zegt.
4. **Niet zelf bijdraaien.** Dat is tampering — maakt het proces slechter.
5. **Verdachte output apart.** Geen producten met een vraagteken naar de klant.
6. **Bel de teamleider met informatie**, niet met een vraag. ('Ik heb 1, 2 en 3 gedaan, dit is wat ik vond.')

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Out-of-control signaal** | De regelkaart geeft aan dat er iets ánders is dan normaal |
| **UCL / LCL** | Boven- / ondergrens van het normale procesgedrag |
| **Reactieplan** | De vaste volgorde die je doorloopt bij een signaal |
| **Verdachte output** | Producten gemaakt rond het signaal-moment, status: nog niet vrij |
| **Quarantaine** | Aparte plek voor verdachte producten (rode bak, afgesloten rek) |
| **Tampering** | Onnodig aan het proces draaien — maakt het juist instabieler |
| **Vrijgave** | Officiële beslissing dat producten door mogen |
| **Escalatie** | Doorgeven aan teamleider / engineering / kwaliteit |

---
*Bron: AIAG SPC Reference Manual; Ford PPAP Reaction Plan | AIMM Module 1 — SPC Gebruik | v1.0*
