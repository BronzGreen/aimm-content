# Werkblad 2: Precision en recall — twee formules, narekenen
*Narekening-werkblad — fase 2 (theoretiseren)*

**Naam:** ____________________  **Datum:** __________
**Buurman / buurvrouw:** ____________________
**Module 2 — Train**

---

> **Over dit werkblad**
> Je hebt net twee matrices geteld. Nu komen er twee formules bij. Geen abstracte wiskunde — twee vragen die je elke evaluatie-rapport stelt:
> 1. **Precision** — *"Als het model afkeurt, klopt het dan?"*
> 2. **Recall** — *"Vindt het model alle afkeur, of glipt er iets door?"*
> Je schrijft de formules over, rekent samen matrix A na met de trainer, en daarna reken je matrix B na met je buurman of buurvrouw. Eén regel: **check elkaars breuk, niet je intuïtie.**

---

## De vier woorden die je nodig hebt

Voordat je rekent, zet je de vier getallen klaar uit je matrices:

| Vakje in matrix                                        | Korte naam              | Matrix A | Matrix B |
|--------------------------------------------------------|-------------------------|:--------:|:--------:|
| Echt afgekeurd, camera zegt afgekeurd                   | **terecht afgekeurd**   |   ___    |   ___    |
| Echt goed, camera zegt afgekeurd                        | **onterecht afgekeurd** |   ___    |   ___    |
| Echt afgekeurd, camera zegt goed                        | **doorgelaten afkeur**  |   ___    |   ___    |
| Echt goed, camera zegt goed                             | terecht goed            |   ___    |   ___    |

*Tip: de eerste drie woorden — terecht afgekeurd, onterecht afgekeurd, doorgelaten afkeur — heb je zo dadelijk nodig voor beide formules.*

---

## De twee formules — schrijf ze over

*Schrijf hieronder beide formules in je eigen handschrift. Bij voorkeur náást elkaar, niet onder elkaar — dan houd je ze visueel uit elkaar.*

**Precision (precisie):**

> precision = terecht afgekeurd / (terecht afgekeurd + onterecht afgekeurd)

Werkvloer-vraag: *"Als het model afkeurt — heeft het dan echt gelijk?"*

___________________________________________________________

___________________________________________________________

**Recall (terugvinden):**

> recall = terecht afgekeurd / (terecht afgekeurd + doorgelaten afkeur)

Werkvloer-vraag: *"Vindt het model alle afkeur — of glipt er iets door?"*

___________________________________________________________

___________________________________________________________

---

## Matrix A — samen narekenen met de trainer

*Vul de breuk in en schrijf het percentage erbij. Rond af op één procentpunt.*

**Precision A:**

```
precision A =  ___  / ( ___  +  ___ )  =  ___  /  ___  =  ___ %
```

**Recall A:**

```
recall A    =  ___  / ( ___  +  ___ )  =  ___  /  ___  =  ___ %
```

**Wat zeggen deze twee getallen in werkvloer-taal?** (één zin per maat)

precision A: ______________________________________________

recall A:    ______________________________________________

---

## Matrix B — narekenen in duo

*Vijftien minuten geleden zag matrix B er gunstig uit op het oog. Reken nu en kijk of dat gevoel klopt. Check elkaars breuk.*

**Precision B:**

```
precision B =  ___  / ( ___  +  ___ )  =  ___  /  ___  =  ___ %
```

**Recall B:**

```
recall B    =  ___  / ( ___  +  ___ )  =  ___  /  ___  =  ___ %
```

**Veelgemaakte fout om te checken:** komt onze noemer bij precision uit "alles wat het model afkeurt" (terecht + onterecht) of uit "alle echt-afgekeurde producten"? Het eerste is precision, het tweede is recall.

⃝ Onze noemers zijn dubbel-gecheckt en kloppen.

⃝ We hebben iets gevonden dat we niet zeker weten — vraag stellen aan trainer:
___________________________________________________________

---

## Vier getallen op een rij

*Schrijf de vier uitkomsten naast elkaar — dat is het patroon dat de trainer straks plenair vraagt.*

| Matrix | Precision | Recall |
|--------|:---------:|:------:|
| **A — strenge drempel**  |   ___ %   |  ___ % |
| **B — soepele drempel**  |   ___ %   |  ___ % |

---

## De trade-off in één eigen zin

*Strenger naar soepeler — wat zie je gebeuren met precision? Wat met recall? Schrijf de trade-off op in je eigen woorden.*

___________________________________________________________

___________________________________________________________

___________________________________________________________

*Voorbeeldformulering (gebruik je eigen woorden):* "Als je strenger instelt, vind je meer afkeur (recall stijgt) maar je gooit ook meer goede stuks weg (precision daalt). Soepeler is andersom. Beide tegelijk maximaal kan vrijwel nooit."

---

## Wat neem je mee naar fase 3?

*Eén zin: welke vraag is straks belangrijker — precision-hoog of recall-hoog? Het antwoord komt straks via twee scenario's. Voor nu: je eerste idee.*

___________________________________________________________

___________________________________________________________

---

*Bron: Precision en recall — narekenen op twee matrices | AIMM Module 2 — Train | lo-ai-fund-212 | v1.0*
