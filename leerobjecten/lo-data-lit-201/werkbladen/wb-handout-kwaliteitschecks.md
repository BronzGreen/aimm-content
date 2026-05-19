# Werkblad 2: Theorie-handout -- Drie Kwaliteitschecks

**Leerobject:** Datatypes herkennen en datakwaliteit beoordelen
**Fase:** Theoretiseren
**Duur:** 8 minuten

---

## De drie kwaliteitschecks

Voordat je data gebruikt voor een beslissing, check je drie dingen:

---

### Check 1: Volledigheid

**Vraag:** Ontbreekt er iets?

**Waar let je op:**
- Lege cellen of ontbrekende waarden
- Diensten of dagen die niet geregistreerd zijn
- Machines die niet meegeteld zijn

**Vuistregel:** Als meer dan 10% ontbreekt, wees voorzichtig met conclusies.

**Voorbeeld:** Een weekrapport met alleen maandag t/m donderdag. Vrijdag ontbreekt. Het weekgemiddelde klopt niet.

---

### Check 2: Consistentie

**Vraag:** Klopt het met zichzelf?

**Waar let je op:**
- Dezelfde eenheid? (kg vs gram, minuten vs uren)
- Dezelfde schrijfwijze? ("CNC-01" vs "cnc01")
- Logische waarden? (temperatuur 3000 graden = fout)
- Geen dubbele registraties?

**Vuistregel:** Vergelijk twee systemen. Kloppen de totalen? Nee = inconsistentie.

**Voorbeeld:** In het MES staat "45 minuten stilstand". In het logboek staat "1 uur stilstand". Wie heeft gelijk?

---

### Check 3: Actualiteit

**Vraag:** Is het nog geldig?

**Waar let je op:**
- Wanneer is de data verzameld?
- Is er sindsdien iets veranderd? (nieuwe machine, ander materiaal)
- Gebruik je de meest recente versie?

**Vuistregel:** Hoe sneller je omgeving verandert, hoe verser je data moet zijn.

**Voorbeeld:** Je vergelijkt je OEE met het gemiddelde van vorig jaar. Maar vorig jaar had je een andere machine. De vergelijking klopt niet meer.

---

## Het drie-stappenplan

Bij elke dataset die je gebruikt:

1. **Scan op volledigheid** -- zoek lege plekken
2. **Check op consistentie** -- vergelijk eenheden en schrijfwijzen
3. **Controleer actualiteit** -- kijk naar de datum

Alle drie positief? --> Data is bruikbaar.
Een of meer negatief? --> Meld het en gebruik met voorbehoud.

---

## Wat doe je als de kwaliteit niet goed is?

- **Meld het.** Niet zelf repareren zonder dat iemand het weet.
- **Gebruik het met voorbehoud.** Zeg erbij wat er niet klopt.
- **Verbeter de bron.** Maak afspraken over hoe data wordt ingevoerd.
