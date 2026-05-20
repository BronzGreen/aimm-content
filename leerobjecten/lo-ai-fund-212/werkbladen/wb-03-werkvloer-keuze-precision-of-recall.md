# Werkblad 3: Welke fout is duurder? — werkvloer-keuze precision of recall
*Twee scenario's, één regel, en je eigen werkvloer — fase 3 (reflecteren)*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train**

---

> **Over dit werkblad**
> Welke maat — precision of recall — telt zwaarder op een lijn? Dat is geen wiskundige vraag. Het is een **bedrijfslogica-vraag**: welke fout is duurder op deze lijn?
> Je analyseert eerst twee scenario's die aan elkaars tegengestelden staan. Daarna draai je de vraag om naar **jouw** werkvloer. Een eerste keuze is genoeg — twijfel mag.

---

## Scenario 1 — Luxe-segment: handgemaakte horloges

*Een fabrikant maakt horloges van 4000 euro per stuk. Een AI-camera controleert visueel bij de eindcontrole.*

**Wat is een vals positief (gemist) in dit scenario?**

*Het model zegt "goed" terwijl het horloge defect is — gaat naar de klant.*

Wat zijn de kosten? (denk aan retourzending, merkschade, ontevreden klant)

___________________________________________________________

___________________________________________________________

**Wat is een vals negatief (vals-alarm) in dit scenario?**

*Het model zegt "afgekeurd" terwijl het horloge eigenlijk goed is — gaat opnieuw door inspectie.*

Wat zijn de kosten? (denk aan productiekost, materiaal, arbeid)

___________________________________________________________

___________________________________________________________

**Welke fout is duurder bij dit luxe-segment-scenario?**

⃝ Vals positief (gemist) — defect naar klant kost meer dan een afgekeurd horloge dat goed bleek

⃝ Vals negatief (vals-alarm) — onnodig afkeuren kost meer dan een soms doorgelaten defect

**Welke maat hoort daarbij — precision-hoog of recall-hoog?**

⃝ **Precision hoog** — als het model afkeurt, moet het écht afgekeurd zijn

⃝ **Recall hoog** — vind alle afkeur, ook al gooi je goede stuks weg

**Korte onderbouwing (1-2 zinnen):**

___________________________________________________________

___________________________________________________________

---

## Scenario 2 — Voedselveiligheid: vleesverwerker

*Een vleesverwerker scant elk stuk met een afkeur-camera op de eindlijn.*

**Wat is een vals positief (gemist) in dit scenario?**

*Het model zegt "goed" terwijl het vlees afgekeurd hoort — gaat naar de consument.*

Wat zijn de kosten? (denk aan recall-actie, boete, gezondheidsschade, mogelijk levens)

___________________________________________________________

___________________________________________________________

**Wat is een vals negatief (vals-alarm) in dit scenario?**

*Het model zegt "afgekeurd" terwijl het vlees eigenlijk goed is — gaat in de afval-bak of naar herinspectie.*

Wat zijn de kosten? (denk aan productiekost, dubbele inspectie, geen consument-schade)

___________________________________________________________

___________________________________________________________

**Welke fout is duurder bij dit voedselveiligheid-scenario?**

⃝ Vals positief (gemist) — defect vlees naar consument kost meer dan een afgekeurd stuk dat goed bleek

⃝ Vals negatief (vals-alarm) — onnodig afkeuren kost meer dan een soms doorgelaten defect

**Welke maat hoort daarbij — precision-hoog of recall-hoog?**

⃝ **Precision hoog** — als het model afkeurt, moet het écht afgekeurd zijn

⃝ **Recall hoog** — vind alle afkeur, ook al gooi je goede stuks weg

**Korte onderbouwing (1-2 zinnen):**

___________________________________________________________

___________________________________________________________

---

## De bedrijfslogica-regel — schrijf hem op

*Beide scenario's hadden dezelfde duurste fout (vals positief — defect naar klant of consument). Toch valt de keuze anders uit. Waarom? Omdat het bij luxe-segment gaat om **onterechte afkeur minimaliseren** en bij voedsel om **alle afkeur vinden**. De maat die je kiest verschilt.*

**De bedrijfslogica-regel in je eigen woorden:**

> **Precision** belangrijk als ____________________________
>
> **Recall** belangrijk als _______________________________

*Voorbeeldformulering (gebruik je eigen woorden):* "Precision belangrijk als vals positief duurder is dan vals negatief. Recall belangrijk als vals negatief duurder is dan vals positief."

---

## Jouw eigen werkvloer — welke kant kies jij?

*Nu de echte vraag. Welke AI-toepassing ken je op jouw eigen werkvloer? Een inspectiecamera, een sorteersysteem, een afkeur-camera, een eindcontrole-AI? Heb je er geen, kies dan een toepassing waarvan je weet dat hij komt of waar de leverancier mee bezig is.*

**AI-toepassing op mijn werkvloer (naam, plek, wat doet hij):**

___________________________________________________________

___________________________________________________________

___________________________________________________________

**Wat zou een vals positief (gemist) op mijn werkvloer betekenen?**

___________________________________________________________

___________________________________________________________

**Wat zou een vals negatief (vals-alarm) op mijn werkvloer betekenen?**

___________________________________________________________

___________________________________________________________

**Welke fout is duurder op mijn lijn?**

⃝ Vals positief (gemist)

⃝ Vals negatief (vals-alarm)

**In welke categorie zit die kost vooral?** *(je mag meer dan één aankruisen)*

- [ ] Geld (directe kosten, marge, materiaal)
- [ ] Tijd (lijn-stilstand, dubbele inspectie, hertest)
- [ ] Merk (klanttevredenheid, reputatie, ontevreden buurman op LinkedIn)
- [ ] Veiligheid (mens, voedsel, gezondheid, compliance)
- [ ] Iets anders: _____________________________________

---

## Mijn keuze voor de eigen werkvloer

*Op basis van het bovenstaande kies je nu één maat. Eerste versie is genoeg — twijfel mag.*

**Voor mijn werkvloer-AI krijgt prioriteit:**

⃝ **Hoge precision** — als het model afkeurt, moet het écht afgekeurd zijn

⃝ **Hoge recall** — alle afkeur moet gevonden worden

**Waarom past dit bij MIJN werkvloer? (minimaal één onderbouwing in geld, tijd, merk of veiligheid)**

___________________________________________________________

___________________________________________________________

___________________________________________________________

---

## Spiegel-moment — voor de plenaire ronde

*Trainer haalt drie deelnemers op met contrasterende keuzes. Schrijf hieronder vast je samenvattende zin voor de groep.*

**Mijn één-zin-keuze voor de groep:**

*"Voor mijn werkvloer kies ik ___________ omdat ___________ duurder is op onze lijn."*

___________________________________________________________

___________________________________________________________

---

*Bron: Werkvloer-keuze precision of recall | AIMM Module 2 — Train | lo-ai-fund-212 | v1.0*
