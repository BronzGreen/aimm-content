# Eigen Lijn-Screen: Past AI-uitbreiding hier?
*Vijf criteria voor één concrete lijn — randvoorwaarden vóór de business-case*

**Naam:** ____________________  **Datum:** __________  
**Module 3 — SPC Op Maat | Workshop: AI + alarmrationalisatie ontwerpen**

---

> **Over dit werkblad**  
> Een AI-uitbreiding op klassieke SPC kost geld, mensen en tijd — en mislukt vaak op randvoorwaarden, niet op techniek. Voordat je een leverancier of intern team een business-case laat schrijven, screen je je eigen lijn op vijf criteria. Aan het eind formuleer je een onderbouwde voorlopige conclusie: AI nu zinvol, eerst meer voorbereiden, of klassieke SPC blijft passend voor deze lijn.

---

## 🔵 De lijn die je screent

**Welke productielijn / installatie?**

_______________________________________________

**Welke concrete vraag wil je hier beantwoorden?** (uit wb-01 of nieuw)

_______________________________________________

_______________________________________________

---

## 🟠 Criterium 1 — Aantal sensoren / variabelen

*Hoeveel variabelen worden of kunnen worden gemonitord op deze lijn?*

- ☐ Eén of twee variabelen (klassieke SPC dekt dit goed)
- ☐ Drie tot tien variabelen (multivariate analyse begint waarde toe te voegen)
- ☐ Meer dan tien variabelen (klassieke regels missen structureel patronen)

*Korte toelichting — welke variabelen, en hoe gerelateerd zijn ze?*

_______________________________________________

_______________________________________________

---

## 🟣 Criterium 2 — Multivariate verbanden

*Vermoed je dat verstoringen ontstaan uit **combinaties** van variabelen die elk apart binnen ±3σ blijven?*

- ☐ Ja, ik heb daar concrete aanwijzingen voor (geef voorbeeld)
- ☐ Vermoeden, maar geen bewijs
- ☐ Nee, verstoringen zijn meestal terug te voeren op één variabele

*Welke aanwijzing of welk vermoeden?*

_______________________________________________

_______________________________________________

_______________________________________________

> **Let op:** Zonder concrete aanwijzingen voor multivariate patronen biedt AI vaak geen meerwaarde boven klassieke SPC met goede stratificatie.

---

## 🟢 Criterium 3 — Beschikbare historische data

*Heb je voldoende én betrouwbare historische data om een AI-model te trainen?*

- ☐ Minder dan 6 maanden, of grote gaten in de data
- ☐ 6–12 maanden, maar de procesinstellingen zijn ondertussen veranderd
- ☐ Meer dan 12 maanden, stabiele instellingen, weinig gaten

*Korte toelichting — periode, kwaliteit, eventuele wijzigingen in instellingen of materiaal:*

_______________________________________________

_______________________________________________

_______________________________________________

> **Let op:** Historische data van 6 maanden zegt niets als de procesinstellingen ondertussen zijn veranderd. Een AI-model leert dan een werkelijkheid die niet meer bestaat.

---

## 🟠 Criterium 4 — Concrete meerwaarde versus Nelson

*Wat zou een AI-systeem op deze lijn kunnen zien dat een Nelson-regel nu niet ziet?*

*Wees concreet. Niet 'AI ziet patronen' — maar: welk patroon, in welke variabelen, dat nu structureel gemist wordt.*

_______________________________________________

_______________________________________________

_______________________________________________

_______________________________________________

*Hoe vaak per maand zou dit een verschil maken?* (geschat aantal voorkomens)

_______________________________________________

> **Let op:** Als je deze vraag niet concreet kunt beantwoorden, is een AI-business-case nog niet rijp. Dan eerst zelf de vraag scherp krijgen — bijvoorbeeld door op één concrete verstoring achteraf te analyseren wat de Nelson-regel had moeten zien.

---

## 🟣 Criterium 5 — Behoefte aan explainable AI (XAI)

*Wie moet straks een AI-alarm interpreteren — en in welke taal?*

**Wie?** (operator, teamleider, kwaliteitsmanager, engineering)

_______________________________________________

**Wat moet die persoon van het AI-alarm begrijpen om er actie op te ondernemen?**

_______________________________________________

_______________________________________________

_______________________________________________

*Heeft je organisatie XAI-tooling beschikbaar (SHAP, LIME of ingebouwd in het AI-platform)?*

- ☐ Ja, ingebouwd of beschikbaar
- ☐ Onbekend, moet uitgezocht worden
- ☐ Nee, alleen black-box modellen

> **Let op:** Zonder uitlegbaarheid (wáárom dit alarm afgaat) ondermijnt een AI-systeem het operator-vertrouwen. In hoge proces- of veiligheidsimpact-omgevingen is XAI géén optie maar een voorwaarde.

---

## 🔴 Voorlopige conclusie

*Op basis van bovenstaande screen — wat is op dit moment je voorlopige conclusie voor déze lijn?*

- ☐ **AI-uitbreiding nu zinvol** — meerwaarde concreet, randvoorwaarden op orde
- ☐ **Eerst meer voorbereiden** — meerwaarde plausibel maar randvoorwaarde X of Y nog niet op orde
- ☐ **Klassieke SPC blijft passend** — geen concrete multivariate patronen, Nelson dekt dit goed (eventueel + stratificatie)

*Onderbouwing met minstens twee argumenten:*

1. _______________________________________________

   _______________________________________________

2. _______________________________________________

   _______________________________________________

*Wat is de eerste vervolgactie?* (concreet — bijv. "data-historie checken bij IT", "met operator A bespreken welke patronen hij/zij vermoedt", "leverancier vragen om XAI-demo")

_______________________________________________

_______________________________________________

_______________________________________________

---

## 📅 Mee naar de plenaire bespreking

| Onderdeel | Klaar? |
|-----------|:------:|
| Vijf criteria gescoord | ☐ |
| Voorlopige conclusie ingevuld | ☐ |
| Twee onderbouwingsargumenten | ☐ |
| Eerste vervolgactie geformuleerd | ☐ |

> 💡 **Onthoud:** AI is geen wonderoplossing. Voor univariate vragen blijft een Nelson-regel kostenefficiënt. AI voegt waarde toe daar waar klassieke regels structureel multivariate of niet-lineaire patronen missen — en alleen als de randvoorwaarden op orde zijn.

---
*Bron: ko-spc-602 (AI als aanvulling op SPC) | AIMM Module 3 — SPC Op Maat | v1.0*
