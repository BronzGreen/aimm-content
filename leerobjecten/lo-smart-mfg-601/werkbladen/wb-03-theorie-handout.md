---
werkblad: wb-03
titel: "Samenvatting — waarom gelabelde data de bottleneck is"
behorend_bij: lo-smart-mfg-601-trainee
kolb_fase: theoretiseren
type: handout
duur: voor na de sessie
---

# Samenvatting — Waarom gelabelde data de bottleneck is

*Dit is een handout. Je hoeft hem nu niet te lezen. Stop hem in je tas, lees hem als je thuiskomt of op een later moment.*

---

## De kernboodschap

**Het model is niet het probleem. Jouw data is het probleem.**

Een AI-camerasysteem dat defecten herkent? De software bestaat al. Je kunt 'm gratis downloaden. Wat ontbreekt zijn jouw foto's, met jouw labels.

---

## Drie cijfers om te onthouden

| Cijfer | Wat het betekent |
|--------|------------------|
| **150 per klasse** | Aantal voorbeeldfoto's per type defect dat je minimaal nodig hebt (100 bij simpele producten, 300+ bij veel variatie) *— vuistregel, in de praktijk te valideren* |
| **1-3 minuten** | Tijd om één foto zorgvuldig te labelen (inclusief bounding box tekenen) *— ontwerp-schatting* |
| **5 tot 20 uur** | Totale labeltijd voor 450 foto's (150 × 3 klassen): ~5 uur bij snel labelen zoals in de sessie, tot 20 uur bij strikt productiewerk *— range varieert per complexiteit* |

---

## Waarom werkt het zo?

Een AI-model leert van voorbeelden. Geen voorbeelden = geen leren. Net zoals een nieuwe collega die nog nooit een goede van een afgekeurde beugel heeft gezien, niet kan beoordelen wat er mis is.

### Wat moet er in die voorbeelden zitten?

1. Genoeg foto's — honderden, niet tien
2. Labels die **consistent** zijn — "kras" betekent elke keer hetzelfde
3. Variatie — foto's van verschillende hoeken, lichtomstandigheden, productieseries

### Wie kan dit het best?

De **operator**. Niet de IT-afdeling. Niet de leverancier. Jij ziet de defecten elke dag. Jij weet het verschil tussen een kras die ertoe doet en een glans die geen probleem is.

---

## Het data flywheel

Waarom wordt data steeds belangrijker? Kijk naar dit patroon:

```
Meer foto's gelabeld
    →  Beter model
        →  Meer vertrouwen in het systeem
            →  Systeem wordt op meer plekken ingezet
                →  Nog meer foto's verzameld
```

Dit heet een **data flywheel** — een cirkel die zichzelf versterkt. Google heeft er miljarden mee verdiend (via reCAPTCHA-puzzels waarmee bezoekers onbewust foto's labelden voor Google's modellen). In een fabriek werkt het kleiner, maar precies zo.

---

## De test bij elke leverancier

Als een leverancier komt met een verhaal over "slimme camera's die defecten herkennen", stel dan deze vraag:

> *"Welke foto's zijn gebruikt om dit te trainen, en wie heeft die gelabeld?"*

Als de leverancier dat niet weet, of als het antwoord is "foto's uit een database", weet je genoeg. Voor jouw product, jouw defecten, jouw kwaliteitseisen — dan moet iemand labelwerk doen op jouw foto's.

---

## Wat neem je hieruit mee?

- Het ontwerp van een camera-inspectiesysteem begint **niet** met het model. Het begint met foto's en labels.
- De **kwaliteit** van het systeem hangt af van de **kwaliteit van het labelwerk**.
- De operator is **centraal** in dit proces — niet de IT.
- Een systeem dat niet traint op jouw foto's, werkt niet optimaal voor jouw product.

---

*Bron: AIMM × BronzGreen Curriculum Pipeline | Module 1: Gebruik | Onderliggend kennisobject: ko-smart-mfg-601*
