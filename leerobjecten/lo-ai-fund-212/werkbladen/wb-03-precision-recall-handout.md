# Handout: Precision en recall — twee maten, één afweging
*Theorie-handout — Module 2 Train*

**Naam:** ____________________  **Datum:** __________

---

> **Over deze handout**
> Dit blad is geen invulblad. Het is een naslagblad. Je kunt het bewaren, meenemen naar de werkvloer en gebruiken om een evaluatie-rapport van een AI-leverancier kritisch te lezen.
> Op één pagina staan de twee maten — **precision** (precisie) en **recall** (terugvinden) — de formules, de werkvloer-vertaling en de afweging tussen beide.

---

## De vier vakjes — kort opgefrist

|                       | Model zegt: goed       | Model zegt: afgekeurd  |
|-----------------------|------------------------|------------------------|
| **Echt goed**         | Terecht goed (juist)   | Vals-alarm (vals afgekeurd) |
| **Echt afgekeurd**    | Gemist (vals doorgelaten) | Terecht afgekeurd (juist) |

Twee soorten fouten: **vals-alarm** (goed product weggegooid) en **gemist** (afgekeurd product doorgelaten).

---

## Precision — "als het model afkeurt, klopt het dan?"

**In woorden:**
Van alle producten die het model heeft afgekeurd, hoeveel waren er ook echt afgekeurd?

**Formule:**

> precision = terecht afgekeurd / (terecht afgekeurd + vals afgekeurd)

**Hoge precision** betekent: bijna alles wat het model afkeurt, is ook echt afgekeurd. Weinig vals-alarm. Weinig onnodig weggegooid product.

**Lage precision** betekent: het model keurt vaak af, maar veel daarvan is eigenlijk goed product. Veel vals-alarm.

---

## Recall — "vindt het model alle afkeur?"

**In woorden:**
Van alle producten die echt afgekeurd horen te worden, hoeveel heeft het model er gevonden?

**Formule:**

> recall = terecht afgekeurd / (terecht afgekeurd + vals doorgelaten)

**Hoge recall** betekent: bijna geen afkeur glipt erdoor. Het model vangt het meeste op.

**Lage recall** betekent: het model laat afgekeurde producten doorlopen naar de klant. Misser.

---

## De trade-off — je kunt niet beide tegelijk maximaal hebben

Je kunt aan de drempel van het model draaien:

| Drempel        | Wat doet de camera/het model? | Recall          | Precision       |
|----------------|-------------------------------|-----------------|-----------------|
| **Strenger**   | Keurt sneller af              | Stijgt          | Daalt           |
| **Soepeler**   | Laat meer door                | Daalt           | Stijgt          |

Stel het voor als een schuifregelaar. Je schuift naar de ene kant, en je wint op recall maar betaalt op precision. Je schuift naar de andere kant, en het is andersom.

**Beide tegelijk maximaal — kan vrijwel nooit.**

---

## Wanneer kies je precision, wanneer recall?

Geen wiskundige regel. Een bedrijfslogica-regel.

| Situatie                                              | Welke fout is duurder?        | Belangrijkste maat |
|-------------------------------------------------------|-------------------------------|--------------------|
| **Luxe-segment** (handgemaakte horloges, premium)     | Gemist (defect bij de klant) is duurder | **Precision hoog** |
| **Voedselveiligheid** (vlees, zuivel, allergenen)     | Gemist (afkeur naar consument) kan levens kosten | **Recall hoog**    |
| **Sortering met lage marge**                          | Vals-alarm (goed product weggegooid) eet de marge | **Precision hoog** |
| **Veiligheid-kritisch onderdeel** (luchtvaart, auto)  | Gemist (defect doorgelaten) heeft grote schade | **Recall hoog**    |

De vraag die je jezelf telkens stelt:

> **Wat kan ik níet hebben op deze lijn — vals-alarm of gemist?**

Het antwoord op die vraag bepaalt op welke maat je stuurt.

---

## Voorbeeld — vleesverwerker, twee instellingen

100 producten, waarvan 20 echt afgekeurd.

**Strenge drempel:**
- Terecht afgekeurd: 17 | Vals doorgelaten: 3
- Vals afgekeurd: 5  | Terecht goed: 75
- Precision = 17 / (17 + 5) = **77 procent**
- Recall = 17 / (17 + 3) = **85 procent**

**Soepelere drempel:**
- Terecht afgekeurd: 20 | Vals doorgelaten: 0
- Vals afgekeurd: 15 | Terecht goed: 65
- Precision = 20 / (20 + 15) = **57 procent**
- Recall = 20 / (20 + 0) = **100 procent**

Voor een vleesverwerker weegt voedselveiligheid zwaarder dan marge. Recall belangrijker. **Tweede instelling is hier de juiste keuze.**

---

## Drie vragen voor elk evaluatie-rapport

Als je een evaluatie-rapport krijgt van een leverancier of van IT, stel deze drie vragen:

1. **Wat is de precision en wat is de recall?** (Niet alleen accuratesse.)
2. **Op welke data is dit gemeten — testset of werkelijke productie?**
3. **Welke fout is duurder op onze lijn, en is daar bij de instelling rekening mee gehouden?**

Die drie vragen scheiden een goed AI-rapport van een mooi-praatje.

---

*Bron: Verwarrings-matrix, precision, recall | AIMM Module 2 — Train | lo-ai-fund-212 | v1.0*
