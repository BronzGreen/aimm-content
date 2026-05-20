# Vier data-voorbeelden — past CNN hier?
*Kolb fase 2 — Ervaren*

**Naam:** ____________________  **Datum:** __________
**Module 2 — Train | AI Fundamentals: CNN-architectuur**

---

> **Over dit werkblad**
> Je krijgt vier korte data-voorbeelden van de werkvloer. Per voorbeeld bepaal je: past een CNN hier wel of niet? Doorslaggevend is of er **lokale structuur** in de data zit. Dat kan ruimtelijke ordening zijn (bij een beeld) of volgordelijke ordening (bij een tijdreeks). Geen "misschien", kies een richting en leg het uit.
>
> **Tijd:** 12 minuten.
>
> **Waarom dit werkblad?**
> Niet elke meting past bij een CNN. Een tabel met onderdeelnummers heeft geen lokale structuur. Een trillingssignaal of een oppervlaktefoto wel. Wie dat verschil ziet, kan beter meekijken met de leverancier en weet waarom een dashboard-melding bij de ene case zinvol is en bij de andere niet.

---

## Voorbeeld A — Camera-inspectie op een lasergravure

> Een productiecel produceert metalen plaatjes met een lasergravure. Een 5-megapixel-camera neemt na elke gravure een beeld op. Het kwaliteitsteam wil een AI-model dat krassen, deuken en verkleuringen herkent in het beeld. Voorbeeld: een kras is een dun, lokaal lijntje van enkele pixels breed.

**Past CNN hier?**   ○ Ja   ○ Nee

*Welk concept is doorslaggevend?*

○ Lokale structuur (ruimtelijk)   ○ Lokale structuur (volgordelijk)   ○ Geen lokale structuur

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

---

## Voorbeeld B — Oppervlaktefoto van een gespoten plaat

> Een lakcabine spuit autodelen. Na het drogen wordt elk deel gefotografeerd onder gestandaardiseerd licht. Het systeem moet pinholes (microscopisch kleine luchtbelletjes), druipranden en verkleuring detecteren. De defecten zitten op verschillende plekken op het deel.

**Past CNN hier?**   ○ Ja   ○ Nee

*Welk concept is doorslaggevend?*

○ Lokale structuur (ruimtelijk)   ○ Lokale structuur (volgordelijk)   ○ Geen lokale structuur

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

---

## Voorbeeld C — Trillingssignaal van een rollager

> Een trillingssensor op een rollager meet 200 samples per beslissing. Dat is ongeveer 0,2 seconden bij een meetsnelheid van 1 kHz. Bij beginnende lagerschade verschijnt een terugkerend frequentiepatroon. Dat patroon kan overal in het venster zitten, niet per se aan het begin of einde.

**Past CNN hier?**   ○ Ja   ○ Nee

*Welk concept is doorslaggevend?*

○ Lokale structuur (ruimtelijk)   ○ Lokale structuur (volgordelijk)   ○ Geen lokale structuur

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

---

## Voorbeeld D — ERP-tabel met onderdeelnummer en leverdatum

> Het ERP-systeem (voorraad-beheer) heeft een tabel met kolommen: onderdeelnummer, leverancier, leverdatum, prijs, kwaliteitsklasse. Het kwaliteitsteam wil voorspellen welke onderdelen waarschijnlijk afgekeurd worden. De volgorde van de kolommen heeft geen betekenis. Leverancier had net zo goed in kolom 1 of 5 kunnen staan.

**Past CNN hier?**   ○ Ja   ○ Nee

*Welk concept is doorslaggevend?*

○ Lokale structuur (ruimtelijk)   ○ Lokale structuur (volgordelijk)   ○ Geen lokale structuur

*Onderbouwing in eigen woorden:*

_______________________________________________

_______________________________________________

---

## Mijn samenvatting

| # | Mijn antwoord | Welk woord uit fase 1 hielp het meest? |
|---|---------------|----------------------------------------|
| A | ○ Ja  ○ Nee | |
| B | ○ Ja  ○ Nee | |
| C | ○ Ja  ○ Nee | |
| D | ○ Ja  ○ Nee | |

---

## Welke laag deed het belangrijkste werk?

*Voor het voorbeeld waar CNN volgens jou het beste past — welke van de vier CNN-lagen doet daar waarschijnlijk het belangrijkste werk?*

○ Convolutielaag (lokale patronen oppikken)
○ Pooling (samenvatten en robuust maken)
○ Fully connected (eindoordeel vellen)

*Toelichting:*

_______________________________________________

_______________________________________________

> **Tip:** A, B en C hebben lokale structuur. CNN past daar. D heeft die structuur niet. Daar is een tabular model (bijvoorbeeld random forest, een beslis-bossen-model) geschikter. Klopt jouw redenering daarmee?

---

## Wat doen we hierna?

In fase 3 (Reflecteren) vergelijk je je antwoorden eerst met je buurman. Daarna stemt de groep plenair per voorbeeld, en bespreekt de trainer vooral voorbeeld D als contrast met A, B en C. Houd je antwoorden bij de hand. We pakken straks de werkblad-pagina van fase 3 erbij.

---
*Bron: CNN-architectuur — AIMM Curriculum | Module 2: Train | v1.0*
