---
id: ko-smart-mfg-702
title: Vals alarm of gemist defect — welke fout kost meer?
type: framework
domain: smart_manufacturing
subdomain: computer_vision_kwaliteit
summary: 'Een AI-inspectiesysteem kan twee soorten fouten maken: een goed product
  onterecht afkeuren (vals alarm), of een defect doorlaten (gemist defect). Welke
  fout duurder is, bepaalt hoe je het systeem moet afstellen — en dat verschilt per
  product.'
source_centrality: 0.7
source_ref: Op basis van standaard confusion-matrix literatuur, aangepast naar operator-niveau
status: validated
updated_at: '2026-05-20'
correlation_id: ronde27-lo-smart-mfg-702
---

# Vals alarm of gemist defect — welke fout kost meer?

Geen enkel AI-systeem is perfect. Er zullen altijd fouten zijn — ook bij een model met goede trainingsdata. De vraag is niet *of* fouten voorkomen, maar *welke soort fouten* en *wat ze kosten*.

### De twee soorten fouten

| | Systeem zegt: goed | Systeem zegt: afkeur |
|---|---|---|
| **Product is goed** | ✅ Correct goedgekeurd | ⚠️ **VALS ALARM** (false positive) |
| **Product is defect** | ❌ **GEMIST DEFECT** (false negative) | ✅ Correct afgekeurd |

Twee soorten fouten: vals alarm en gemist defect. Allebei vervelend, maar om hele andere redenen.

### Kosten van een vals alarm

Een vals alarm betekent: een perfect product wordt afgekeurd. Wat kost dat?

- **Materiaalverlies** als het product niet opnieuw gebruikt kan worden
- **Productietijd** omdat een nieuwe unit moet worden gemaakt
- **Inspecteurs-tijd** om handmatig na te gaan of het systeem wel klopte
- **Vertrouwensverlies** bij de operators (*'dit systeem werkt toch niet'*)

### Kosten van een gemist defect

Een gemist defect betekent: een product met fouten glipt door naar de klant. Wat kost dat?

- **Klachten** en retourzendingen
- **Reparatie- of vervangingskosten**
- **Reputatieschade** bij de klant
- **In kritieke toepassingen (medicatie, luchtvaart): risico op letsel**

### Wanneer welke fout erger is

Dit hangt af van het **product en de markt**:

- **Kritieke toepassingen** (medicatie, veiligheidsonderdelen, voedsel): gemist defect is catastrofaal. Systeem streng afstellen, veel vals alarm accepteren.
- **Massaproductie goedkope goederen** (verpakkingen, inox-bestek): vals alarm kost materiaal, gemist defect kost klant-goodwill. Balans zoeken.
- **Luxe-producten** (sieraden, high-end electronica): zichtbare defecten zijn onacceptabel. Streng instellen — goodwill opgebouwd in jaren kan in één defect verdwijnen.
- **Interne halffabricaten** (onderdelen voor eigen eindproduct): afhankelijk van waar in het proces. Vroeg afkeuren is goedkoop, laat afkeuren is duur.

### Wat dit voor jou betekent

Als operator ben jij vaak degene die ziet wat een fout werkelijk kost — niet alleen in euro's, maar ook in werkbelasting, sfeer, of klantklachten. De drempel-instelling uit KO-701 hangt direct samen met deze kostenafweging:

- Vals alarm duur? → drempel strenger, model afwijzen bij twijfel
- Gemist defect duur? → drempel soepeler, model afkeuren bij twijfel

Als niemand in je organisatie deze afweging expliciet gemaakt heeft, is de drempel waarschijnlijk op 'gemakkelijk voor iedereen' ingesteld — wat meestal niet de goedkoopste uitkomst is.


## Praktijkvoorbeeld

Stel: een fabrikant van automotive-onderdelen. Elk onderdeel dat gemist wordt kan een motor laten vastlopen — dat is een recall, bij een grote serie snel €500.000 aan kosten. Vals alarm kost ~€5 materiaal plus 2 minuten inspecteur-tijd.

De afweging is hier eenvoudig: elk vals alarm dat een gemist defect voorkomt, is goud waard. Drempel streng zetten, liever 100 valse alarmen dan 1 gemist defect.

Contrast: een bakker met AI-camera voor broodvormen. Gemist defect = een misvormd brood bij de klant, klacht waarschijnlijk genegeerd. Vals alarm = een goed brood weggegooid, 60 cent materiaalverlies.

Hier is de afweging andersom: vals alarm is duurder dan gemist defect. Drempel soepel — alleen duidelijk misvormde broden laten afkeuren.

Zelfde model. Zelfde camera-opstelling. Totaal andere drempel-instelling. Dat is de kern: techniek is generiek, afwegingen zijn context-specifiek.
