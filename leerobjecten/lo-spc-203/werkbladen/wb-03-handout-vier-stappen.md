# Handout: De Vier Stappen bij een Signaal
*Operator-respons bij een out-of-control signaal — Kolb-fase: theoretiseren*

**Module 1 — SPC Gebruik | Naslagwerk**

---

> **Kernidee**
> Een signaal op de regelkaart vraagt om een vaste volgorde van vier stappen. Geen snelle oplossing. Wie de volgorde aanhoudt, voorkomt drie veelgemaakte fouten. Eén: ingrijpen op een meetfout. Twee: doorvoeren van verdachte producten. Drie: zelf-corrigeren zonder dat iemand het weet.

---

## De vier stappen — in deze volgorde

| Stap | Wat doe je? | Waarom in deze volgorde? |
|------|-------------|--------------------------|
| **1** | **Meetfout uitsluiten** | Een verkeerde meting is geen echt signaal. Check eerst je meting voordat je iets doet aan het proces. |
| **2** | **Laatste proceswijziging checken** | Als er recent iets veranderd is, weet je vaak meteen waar je moet kijken. |
| **3** | **Verdachte output veiligstellen** | Producten gemaakt rond het signaal-moment mogen niet door tot vrijgave. |
| **4** | **Teamleider informeren** | Geen zelf-corrigeren zonder overleg. De teamleider beslist over doorgaan, stilleggen of opschalen. |

---

## 🔵 Stap 1 — Meetfout uitsluiten

*Een signaal is alleen geldig als de meting klopt. Eerste vraag: klopt mijn meting wel?*

**Check vier dingen:**

- ☐ Is mijn meetinstrument gecalibreerd?
- ☐ Heb ik gemeten volgens de juiste procedure?
- ☐ Is er een referentiestuk waarmee ik opnieuw kan meten?
- ☐ Heb ik per ongeluk de verkeerde meetmethode gebruikt?

**Als de meting fout was:** noteer wat er mis was. Herstart de meting. Doe niets aan het proces.

**Als de meting klopt:** ga door naar stap 2.

**Voorbeelden meetfouten op de werkvloer:**

- *Spuitgieten:* weegschaal niet genuld voor de meting.
- *CNC:* schuifmaat sluit niet goed op het werkstuk.
- *Verpakking:* gewicht gemeten op een trillende lopende band.
- *Voedselverwerking:* thermometer nog warm van vorige meting.
- *Metaal:* ruwheidsmeter op een natte plek.

---

## 🔵 Stap 2 — Laatste proceswijziging checken

*Wat is er recent veranderd? Begin bij het laatste uur. Werk terug in de tijd.*

**Vraag jezelf af:**

- ☐ Is er een nieuwe materiaalbatch geladen?
- ☐ Is er een setup-wissel geweest?
- ☐ Is er een andere ploeg begonnen?
- ☐ Is er onderhoud uitgevoerd?
- ☐ Zijn er nieuwe of bijgeslepen tools in gebruik?
- ☐ Zijn de omgevingscondities veranderd (temperatuur of vocht)?

**Als je een wijziging vindt:** noteer wat het was. Dat helpt bij stap 4.

**Geen wijziging gevonden:** ook dat is een uitkomst. Meld het aan je teamleider.

**Voorbeelden recente wijzigingen op de werkvloer:**

- *Spuitgieten:* nieuwe HDPE-batch van een andere leverancier.
- *CNC:* freesbeitel net bijgeslepen.
- *Verpakking:* nieuwe ploeg startte 30 minuten geleden.
- *Voedselverwerking:* koeling 's nachts uitgeschakeld voor onderhoud.
- *Metaal:* lasdraad uit een nieuwe rol.

---

## 🟠 Stap 3 — Verdachte output veiligstellen

*Producten gemaakt rond het signaal-moment mogen niet zomaar verder.*

**Wat is "verdachte output"?**

- Alle producten gemaakt tussen het laatste goede meetmoment en nu.
- Bij voorkeur: alle producten sinds de laatste in-control meting.

**Wat doe je ermee?**

- ☐ Apart zetten in een rode bak of een quarantaine-rek.
- ☐ Markeren met datum, tijd en reden ("signaal regelkaart 13:45").
- ☐ Niet doorvoeren naar de volgende processtap tot vrijgave.
- ☐ Niet weggooien — de teamleider of kwaliteit beslist.

**Geen rode bak op je lijn?** Regel een afzetplek vóór het volgende signaal.

**Voorbeelden afzetplekken op de werkvloer:**

- *Spuitgieten:* rode bak naast de pers.
- *CNC:* aparte pallet met gele tape.
- *Verpakking:* quarantaine-rek bij de inpaktafel.
- *Voedselverwerking:* afgesloten koelkar met "HOLD"-sticker.
- *Metaal:* aparte stelling met rode hangbord.

---

## 🟠 Stap 4 — Teamleider informeren

*Geen zelf-corrigeren zonder overleg. De teamleider beslist.*

**Wat geef je door?**

- ☐ Welke kaart een signaal gaf (welke meting, welke regel).
- ☐ Datum, tijd en de meetwaarde.
- ☐ Wat je in stap 1 hebt gecheckt (meetfout uitgesloten?).
- ☐ Wat je in stap 2 hebt gevonden (welke wijziging is recent?).
- ☐ Waar de verdachte output staat (hoeveel stuks, welke plek).

**De teamleider beslist over:**

- Doorgaan na verificatie?
- Lijn stilleggen?
- Engineering inschakelen?
- 100% inspectie van verdachte output?

**Tip:** bel met informatie, niet met een vraag. Dus niet "er ging een lampje af". Wel: "ik heb stap 1, 2 en 3 gedaan, dit is wat ik vond".

---

## 🔴 Wat doe je NIET — de anti-regel

| Verkeerd | Waarom verkeerd |
|----------|-----------------|
| **Direct aan een knop draaien** om het gemiddelde "terug te duwen". | Dit heet **tampering**. Je behandelt common cause als special cause. Je maakt het proces juist instabieler (zie ko-spc-105). |
| **Het signaal negeren** omdat "het zo wel goedkomt". | Een signaal staat er niet zomaar. Wegkijken laat verdachte producten doorgaan. |
| **Wachten tot meerdere signalen verschijnen.** | Bij het tweede signaal is je verdachte output al de poort uit. |
| **Alleen de meetwaarde aanpassen** in het systeem. | Dat is data-vervalsing. Geen oplossing. Wel een groot probleem. |
| **De teamleider bellen voordat je stap 1 hebt gedaan.** | De teamleider kan niets met "er ging een lampje af". Hij heeft je check nodig. |
| **Verdachte output doorvoeren** omdat "het er goed uitziet". | Het ziet er altijd goed uit. Daar gaat het juist om. |

---

## 📋 De praktijkcasus — Daan op de spuitgietlijn

> **13:45** — Operator Daan meet 100,45 gram op zijn X̄-R-kaart. Het punt staat buiten UCL.

**Stap 1:** Daan meet hetzelfde stuk opnieuw met een ander instrument. Dezelfde uitslag komt eruit. *Meetfout uitgesloten.*

**Stap 2:** Daan checkt het logboek. Om 13:30 is een nieuwe materiaalbatch geladen. *Wijziging gevonden.*

**Stap 3:** Daan zet alle 30 producten gemaakt sinds 13:30 apart in de rode bak. *Verdachte output veiliggesteld.*

**Stap 4:** Daan belt teamleider Yasmin. Hij geeft alle info van stap 1, 2 en 3 door.

**Yasmin beslist:** 100% inspectie van de rode bak. De materiaalbatch gaat in quarantaine voor leverancier-onderzoek. De lijn mag doorgaan met monsters uit de vorige batch tot validatie.

> **Resultaat:** geen verdachte producten naar de klant. De oorzaak is in beeld. De lijn is niet onnodig stilgelegd. Tijd: 15 minuten.

---

## 📝 Documentatie — wat leg je vast?

Elke signaal-respons wordt vastgelegd in het lijn-logboek of het kwaliteitssysteem:

- Datum, tijd, kaart en welke regel afging.
- Genomen acties (stap 1, 2 en 3).
- Gevonden oorzaak (of: nog onbekend).
- Vrijgave-besluit verdachte output (door wie?).

Deze logs zijn belangrijk. De teamleider ziet patronen in losse signalen die jij niet ziet. Bijvoorbeeld: "altijd een signaal na een batchwissel van leverancier X".

---

## 🟢 Onthoud dit

1. **Volgorde is alles.** Stap 1 → 2 → 3 → 4. Niet door elkaar.
2. **Geen actie zonder verificatie.** Sluit eerst meetfouten uit.
3. **Geen hervatting zonder oorzaakanalyse.** Pas weer draaien als de teamleider het zegt.
4. **Niet zelf bijdraaien.** Dat is tampering. Dat maakt het proces slechter.
5. **Verdachte output apart.** Geen producten met een vraagteken naar de klant.
6. **Bel met informatie.** Niet met een vraag.

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Out-of-control signaal** | De regelkaart geeft aan dat er iets anders is dan normaal. |
| **UCL / LCL** | Bovengrens / ondergrens van het normale procesgedrag. |
| **Reactieplan** | De vaste volgorde die je doorloopt bij een signaal. |
| **Verdachte output** | Producten gemaakt rond het signaal-moment. Status: nog niet vrij. |
| **Quarantaine** | Aparte plek voor verdachte producten (rode bak of afgesloten rek). |
| **Tampering** | Onnodig aan het proces draaien — maakt het juist instabieler. |
| **Vrijgave** | Officiële beslissing dat producten door mogen. |
| **Escalatie** | Doorgeven aan teamleider, engineering of kwaliteit. |

---

## Wat doen we hierna?

Je hebt nu de vier stappen gelezen. Pak het volgende werkblad: het eigen reactieplan voor jouw lijn. Daar vul je in welk meetinstrument jij gebruikt. Wie jouw teamleider is. En waar jij verdachte output apart zet. Klein beginnen mag. Eén signaal-type tegelijk is genoeg.

---
*Bron: AIAG SPC Reference Manual; Ford PPAP Reaction Plan | AIMM Module 1 — SPC Gebruik | v1.0*
