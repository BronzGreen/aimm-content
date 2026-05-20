# Handout: Cp en Cpk lezen
*Cp en Cpk — wat ze zeggen over spreiding en centrering*

**Module 2 — SPC Train | Naslagwerk**

---

> **De centrale zin (uit je hoofd waard)**  
> **"Cp vertelt of de spreiding smal genoeg is. Cpk vertelt of die smalle spreiding ook goed in het tolerantievak ligt."**

Een proces kan een aardige Cp hebben (smal genoeg) en toch een lage Cpk — dat betekent: de spreiding is op zich oké, maar het gemiddelde staat te dicht bij één van de tolerantiegrenzen. **Centreren, geen spreiding-werk.**

---

## De twee formules — als referentie

> Je hoeft deze niet uit je hoofd te leren. Je hoeft ze ook niet zelf te berekenen — engineering of het MES-systeem doet dat. Maar het helpt om te zien waar de getallen vandaan komen.

| Index | Formule | Wat zegt het? |
|-------|---------|---------------|
| **Cp** | (USL − LSL) / (6 × σ) | Is de spreiding smal genoeg ten opzichte van de tolerantie? **(Potentieel)** |
| **Cpk** | min[ (USL − μ) / (3 × σ) ;  (μ − LSL) / (3 × σ) ] | Past die spreiding ook werkelijk in het tolerantievak? **(Werkelijke prestatie)** |

**Wat de letters betekenen:**

| Letter | Betekenis |
|--------|-----------|
| **USL** | Upper Specification Limit — bovengrens van de klant |
| **LSL** | Lower Specification Limit — ondergrens van de klant |
| **μ** (mu) | Procesgemiddelde — gemiddelde meetwaarde van de lijn |
| **σ** (sigma) | Procesvariatie — hoe ver wijken metingen af van het gemiddelde |

---

## 🔵 De interpretatietabel — gebruik deze!

*Dit is je werkpaard. Lees het Cpk-getal, kijk in deze tabel, weet wat het betekent.*

| Cp / Cpk | Wat betekent het? | Wat doe je? |
|----------|-------------------|-------------|
| **< 1,0** | Niet capabel — afkeur is structureel waarschijnlijk | **Stoppen of escaleren.** Proces hoort eigenlijk niet zo te draaien. |
| **= 1,0** | Theoretisch passend — kwetsbaar voor drift en meetonzekerheid | **Onderzoeken.** Eén tegenvaller en het zit fout. |
| **≥ 1,33** | Veelgebruikte industriële ondergrens — algemeen geaccepteerd | **Doorgaan, blijven monitoren.** |
| **≥ 1,67** | Zwaardere automotive of kritische eis (Ford PPAP) | **Doorgaan.** Hoog niveau van controle. |
| **≈ 2,0** | Gecentreerd kortetermijnproces op zes sigma (12σ tolerantievak) | **Uitstekend.** Klasse-A proces. |

---

## 🟣 Het centrering-vs-spreiding onderscheid

*Twee soorten problemen — en ze vragen totaal verschillende acties.*

### Geval A: Cp en Cpk zijn ongeveer gelijk
→ Spreiding is wat het is, en het ligt netjes in het midden van het tolerantievak.  
→ Beoordeel het getal via de tabel hierboven.

### Geval B: Cp is duidelijk hoger dan Cpk
→ De spreiding is op zich smal genoeg, **maar het gemiddelde staat scheef** in het tolerantievak.  
→ **Eerste actie: centreren** (procesgemiddelde verschuiven naar het midden).  
→ Niet harder proberen de spreiding te verkleinen — die is al smal genoeg.

### Geval C: Cp is laag (en daarmee ook Cpk)
→ De spreiding is **te breed** voor de tolerantie.  
→ **Eerste actie: spreiding verkleinen** (oorzaakanalyse: machine, materiaal, methode, mens, milieu, meting).  
→ Centreren helpt niet — er is gewoon te veel variatie.

---

## 🟢 Het spuitgiet-voorbeeld uitgewerkt

*Casus 1 uit de puzzel — laten we het stap voor stap zien.*

**Spuitgietmachine 3, onderdeelgewicht.**  
Tolerantie: USL = 100,5 g, LSL = 99,5 g.  
Stabiele lijn: gemiddelde μ = 99,9 g, σ = 0,12 g.

**Cp** = (100,5 − 99,5) / (6 × 0,12) = 1,00 / 0,72 ≈ **1,39**  
→ De spreiding **lijkt in potentie goed**. Volgens de tabel zou Cp ≥ 1,33 prima zijn.

**Cpk** = min[ (100,5 − 99,9)/0,36 ;  (99,9 − 99,5)/0,36 ]  
&nbsp;&nbsp;&nbsp;&nbsp; = min[ 1,67 ;  **1,11** ] = **1,11**  
→ De pers staat te dicht tegen de **ondergrens** (99,5 g) aan.

> **De operatorles:** de pers schiet niet "te wijd", maar staat **scheef**.  
> De juiste actie is **centreren** (procesgemiddelde van 99,9 → naar 100,0 brengen),  
> niet harder proberen de spreiding te verkleinen.

**Resultaat na centreren:** als μ = 100,0 g blijft staan met dezelfde σ = 0,12 g,  
dan worden Cp én Cpk samen ≈ **1,39**. Klaar.

---

## 🔴 Drie veelgemaakte fouten — pas op!

*Capability-getallen zijn alleen zinvol als de basis klopt. Dit zijn de drie valkuilen waardoor een mooi getal niets zegt.*

| # | Fout | Wat is er aan de hand? |
|---|------|------------------------|
| 1 | **Capability op een instabiel proces** | Het proces draait op meerdere "toestanden" (verschillende batches, verschillende drukinstellingen, verschillende ploegen). Eén Cpk-getal middelt dat uit. → **Eerst SPC-regelkaart maken; pas capability berekenen als de lijn stabiel is.** |
| 2 | **Slechte subgroepering** | Korte-termijnvariatie en lange-termijnvariatie zitten door elkaar. Het Cpk-getal lijkt mooi maar is misleidend. → **Subgroepen moeten dicht bij elkaar gemeten worden binnen één bedrijfstoestand.** |
| 3 | **Slecht meetsysteem** | De spreiding die je ziet komt deels van de **meter**, niet van de **machine**. → **Ford eist eerst een Gage R&R / MSA, dan pas capability.** |

> **Stelregel uit de praktijk (NIST, Minitab, Ford):**  
> Eerst **stabiliteit** → dan **normaliteit** → dan pas **capability**.

---

## 🟠 Wanneer escaleren?

*Je hoeft niet alles zelf op te lossen. Dit zijn de momenten om het bij teamleider of engineering te leggen.*

| Situatie | Wat doe je? | Aan wie? |
|----------|-------------|----------|
| Cpk < 1,0 op een kritische maat | **Direct melden** + onderzoek starten | Teamleider + engineering |
| Cp duidelijk hoger dan Cpk (centreer-probleem) | Eerst zelf proberen te centreren; als het niet lukt → melden | Teamleider |
| Cp én Cpk te laag (spreidings-probleem) | Niet zelf proberen te knutselen — root-cause-analyse nodig | Engineering / kwaliteitsdienst |
| Cpk-getal komt steeds anders terug per rapport | Misschien meetsysteem of subgroepering instabiel | Engineering / kwaliteitsdienst |
| Klant vraagt automotive-eis (Cpk ≥ 1,67) en je zit op 1,33 | **Direct melden** — dit is een capability-issue | Teamleider |

---

## 📋 Vakjargon kort uitgelegd

| Term | Wat betekent het? |
|------|-------------------|
| **Capability** | Hoe goed past je proces in het tolerantievak van de klant |
| **Cp** | Capability-index: spreiding ten opzichte van tolerantie (potentieel) |
| **Cpk** | Capability-index die rekening houdt met centrering (werkelijke prestatie) |
| **Tolerantievak** | Het gebied tussen LSL (ondergrens) en USL (bovengrens) |
| **Centrering** | Hoe dicht het procesgemiddelde bij het midden van het tolerantievak ligt |
| **Stabiel proces** | Proces zonder special cause variatie — zie ko-spc-104 |
| **MSA / Gage R&R** | Meetsysteem-analyse: zegt of de meter zelf nauwkeurig genoeg is |
| **PPAP** | Production Part Approval Process — Ford-norm voor automotive |

---

## 🟢 Onthoud dit

1. **Cp = spreiding** — is je proces in potentie smal genoeg?
2. **Cpk = werkelijke prestatie** — ligt die smalle spreiding ook netjes in het midden?
3. **Cp >> Cpk** → centreer-probleem (eerst gemiddelde verschuiven).
4. **Cp en Cpk samen laag** → spreidings-probleem (oorzaak zoeken).
5. **Onder de 1,0** → eigenlijk niet OK, melden en onderzoeken.
6. **1,33 of hoger** → algemeen geaccepteerd, blijven monitoren.
7. **Eerst stabiel, dan meetsysteem, dan pas capability** — anders zegt het cijfer niets.

---
*Bron: NIST/SEMATECH Engineering Statistics Handbook; ASQ; Ford PPAP 4th ed.; Minitab documentation | ko-spc-301 | AIMM Module 2 — SPC Train | v1.0*
