# Oltre l'RGB — Rappresentazioni iper-dimensionali per diagnostica e classificazione

Progetto accademico che propone di estendere la percezione artificiale **oltre lo spettro visibile umano** per abilitare diagnostica, classificazione e analisi multi-dominio.

## Anteprima della presentazione

**[Apri la presentazione interattiva](https://htmlpreview.github.io/?https://github.com/GiordanoMariaPipitone/Computer-Vision/blob/main/Oltre%20l%27RGB/Presentazione_Progetto.html)**

> La presentazione è un file HTML interattivo (slide navigabili da tastiera, mouse o touch). GitHub mostra solo il codice sorgente dei file `.html`: usa il link qui sopra per visualizzarla renderizzata, oppure scarica [`Presentazione_Progetto.html`](<./Presentazione_Progetto.html>) e aprila nel browser.

## Il progetto

### Il problema
Le reti neurali in computer vision — diagnostica vegetale, animale e umana — lavorano quasi esclusivamente su immagini **RGB**: tre matrici che codificano solo la porzione dello spettro elettromagnetico visibile all'occhio umano (~400–700 nm). Tre canali, tre prospettive sulla stessa scena, mentre la realtà fisica ne contiene molte di più.

### L'intuizione
Affiancare ai canali R, G, B altre matrici che descrivono la **stessa scena** da prospettive fisiche differenti: infrarosso vicino (NIR), infrarosso a onda corta (SWIR), ultravioletto (UV), termico e bande iperspettrali. Ogni piano è una matrice H × W impilata sulle altre, trasformando l'immagine in un tensore iper-dimensionale.

### Evidenze
La riflettanza fogliare nel NIR e SWIR permette di identificare patologie vegetali **prima della comparsa di sintomi visibili**: la malattia altera struttura cellulare e contenuto idrico, producendo differenze di riflettanza misurabili nell'infrarosso ma invisibili all'occhio. Lo stesso principio è estendibile alla diagnostica umana e veterinaria.

### Aspetti pratici
- **Strumentazione a basso costo** — sensori principali ed estensioni per acquisire le bande aggiuntive.
- **Preprocessing & feature enhancement** — tecniche come CLAHE e Canny per arricchire l'informazione.
- **Vincolo dimensionale** — tutte le matrici devono condividere la stessa risoluzione per essere impilate.
- **Costi e requisiti** — hardware di acquisizione e risorse di calcolo proporzionali al numero di canali × risoluzione × dimensione del dataset.

## File

| File | Contenuto |
|---|---|
| `Presentazione_Progetto.html` | Presentazione interattiva del progetto |
| `Report_Progetto.docx` | Report scritto del progetto |
