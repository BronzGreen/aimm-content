---
id: lo-industry40-302-trainer
knowledge_object_id: ko-industry40-302
version: trainer
title: Data-pipeline ontwerpen voor een digital twin — vier knooppunten, drie keuzes
  (trainer-pakket)
target_audience: operator
content_level: MBO-4
language_level: B2
bloom_level: toepassen
knowledge_type: procedureel
competency_stage: bewust_onbekwaam
kolb_start_phase: ervaren
guidance_style: coachen
duration_minutes: 45
status: validated
updated_at: '2026-05-20'
correlation_id: ronde16-lo-industry40-302
---

# Data-pipeline ontwerpen — Trainer-samenvatting (één A4)

*Industry 4.0 — Module 2 (Train) | Duur 45 min | 8-16 deelnemers | B2-leeswerk ~5 min*

---

## Leerdoel

Deelnemers tekenen zelfstandig een eenvoudige data-pipeline (data-leiding) met de vier knooppunten (sensor, edge-buffer (tussenstation), opslag, consument) en onderbouwen drie ontwerp-keuzes — latentie (vertraging), volume (hoeveelheid data) en failover (terugval bij fout) — met één zin per keuze. Bloom-niveau: toepassen. Kirkpatrick-doel: gedrag (transfer naar werkvloer).

## Doelgroep en startpunt

MBO-4 operator. Stadium: bewust_bekwaam — kent sensor en dashboard apart, maar overziet het pad zelden in zijn geheel. Kolb-voorkeur: doener. Voorkennis: lo-industry40-021 (digital twin), ko-industry40-301 (sensor-keuze). Begeleidingsstijl (manier van begeleiden): **coachen** — stel vragen, laat zelf raden, geef pas in fase 3 de termen.

## Drie sturende principes

1. **Bloom toepassen — fysiek tekenen.** Deelnemers tekenen hun toegewezen knooppunt op A3. Vier subgroepen, vier A3's aan de muur. Daarna langslopen als groep.
2. **Kirkpatrick gedrag — vraag voorbereiden voor IT.** Vraagteken op werkblad is een geldige uitkomst — die gaat mee naar de werkvloer.
3. **Spuitgieterij als anker.** €2.500 → €120 per maand cloud-besparing door slimme edge-buffer. Factor twintig in kosten. Drie minuten waard.

## Kolb-overzicht (leerfasen)

| Fase | Activiteit | Duur | Werkblad |
|------|-----------|------|----------|
| 1. Ervaren | Drie storings-fragmenten — wat zou er mis zijn? | 12 min | wb-01-drie-storingen.md |
| 2. Reflecteren | Buurman-check — drie oorzaken naast elkaar | 10 min | wb-02-buurman-check.md |
| 3. Theoretiseren | Vier knooppunten + drie keuzes + A3-tekening | 13 min | wb-03-handout-pipeline.md |
| 4. Experimenteren | Eigen pipeline — teken jouw situatie | 10 min | wb-04-eigen-pipeline.md |

## Kerntermen (NL-haakjes-uitleg)

- **Pipeline** (data-leiding — pad van sensor naar dashboard)
- **Edge-buffer** (tussenstation — klein opslag-punt naast de machine)
- **Latentie** (vertraging — tijd tussen meting en zichtbaar zijn)
- **Volume** (hoeveelheid data per tijdseenheid)
- **Failover** (terugval bij fout — wat als de verbinding wegvalt)
- **Real-time** (onder 1 seconde — bij veiligheids-alarmen)
- **Near-realtime** (onder 60 seconden — bij drempel-bewaking)
- **Batch** (uren of dagen — bij rapportages)

## Top-3 valkuilen

1. **Te snel termen geven in fase 1.** Gevolg: vervreemding. Oplossing: laat groep met eigen woorden komen ('vertraging', 'data kwijt'). GEEN 'latentie' in fase 1.
2. **A3-tekening overslaan vanwege tijdgebrek.** Gevolg: Bloom toepassen wordt begrijpen. Oplossing: kort de uitleg in, niet de tekening. Vier knooppunten, vier minuten.
3. **Vraagtekens van deelnemers in de zaal oplossen.** Gevolg: Kirkpatrick gedrag faalt — deelnemer leert niet zelf met IT te praten. Oplossing: "Goede vraag — die gaat mee aan IT."

## CAR-check (competentie/autonomie/relatedness — drie psychologische basisbehoeften)

Fase 1 individueel (eerste eigen indruk), fase 2 duo (relatie expliciet), fase 3 subgroepen per knooppunt (samen tekenen), fase 4 individueel (eigen werkvloer-casus). Autonomie geborgd: vraagteken is geldige uitkomst.

## Materiaal-checklist

- [ ] Werkbladen wb-01 t/m wb-04 (geprint per deelnemer)
- [ ] A3-vellen (4-8 stuks) + dikke stiften (4 sets, zwart/blauw/rood)
- [ ] Bord of flipover + stiften
- [ ] Markeerstift per deelnemer
- [ ] Beamer voor drie storings-fragmenten (foto/video)
- [ ] Timer

## Transfer en follow-up

Deelnemers kiezen deze week één machine of lijn op de werkvloer. Tekenen op A4 de vier knooppunten. Beantwoorden de drie keuze-vragen (latentie, volume, failover) — of markeren met vraagteken. Vragen één vraag aan IT of teamleider. Volgende sessie: bespreking eigen pipeline + grootste risico.

---

*Volledig draaiboek: [`draaiboek.md`](./draaiboek.md) — workshop-presentatie: `lo-industry40-302-presentatie.slidev.md` — bron: Anaya et al. (2024); Bakopoulos et al. (2024), Ch. 5; EEMUA Publication 191 (failover-principes).*
