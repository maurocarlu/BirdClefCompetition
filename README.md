# BirdClef2025 Competition

![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

*Notebook per la competizione BirdClef2025 su Kaggle - Identificazione di specie tramite bioacustica*

## Panoramica / Overview

Questa repository contiene i notebook e il codice utilizzato per la competizione Kaggle BirdClef2025, focalizzata sull'identificazione di specie animali (uccelli, anfibi, mammiferi, insetti) attraverso le loro impronte acustiche registrate nella Riserva Naturale El Silencio in Colombia.

*This repository contains notebooks and code used for the Kaggle BirdClef2025 competition, focused on identifying animal species (birds, amphibians, mammals, insects) through their acoustic signatures recorded in El Silencio Natural Reserve, Colombia.*

## Obiettivo della Competizione / Competition Goal

L'obiettivo è sviluppare algoritmi di machine learning in grado di:
1. Identificare specie di diversi gruppi tassonomici nella Valle del Magdalena in Colombia
2. Addestrare modelli con set di dati limitati per specie rare e in via di estinzione
3. Migliorare i modelli utilizzando dati non etichettati

*The goal is to develop machine learning algorithms capable of:*
*1. Identifying species from different taxonomic groups in the Magdalena Valley of Colombia*
*2. Training models with limited datasets for rare and endangered species*
*3. Enhancing models using unlabeled data*

## Contesto / Context

La Riserva Naturale El Silencio protegge 5.407 acri di foreste tropicali di pianura e zone umide. Ospita una fauna diversificata, tra cui 295 uccelli, 34 anfibi, 69 mammiferi, 50 rettili e quasi 500 specie vegetali. Una parte significativa della riserva, precedentemente utilizzata per l'allevamento estensivo di bestiame, è ora oggetto di un progetto di ripristino ecologico.

Attraverso questa competizione Kaggle, l'obiettivo è automatizzare il rilevamento e la classificazione di diversi gruppi tassonomici dai paesaggi sonori della Riserva Naturale El Silencio, con l'intento di fornire una migliore comprensione dei processi ecologici dei progetti di ripristino.

*El Silencio Natural Reserve protects 5,407 acres of tropical lowland forests and wetlands. It hosts diverse wildlife, including 295 birds, 34 amphibians, 69 mammals, 50 reptiles, and nearly 500 plant species. A significant part of the reserve, previously used for extensive livestock farming, is now under an ecological restoration project.*

*Through this Kaggle competition, the aim is to automate the detection and classification of different taxonomic groups from soundscapes of El Silencio Natural Reserve, with the intent to provide a better understanding of the ecological processes of restoration projects.*

## Dataset

Il dataset include:
- **train_audio/**: Registrazioni brevi di suoni individuali di uccelli, anfibi, mammiferi e insetti
- **test_soundscapes/**: Circa 700 registrazioni di 1 minuto utilizzate per la valutazione
- **train_soundscapes/**: Dati audio non etichettati dalle stesse località di registrazione dei test
- **train.csv**: Metadati per i dati di addestramento
- **taxonomy.csv**: Informazioni sulle diverse specie
- **recording_location.txt**: Informazioni sulla località di registrazione

*The dataset includes:*
*- **train_audio/**: Short recordings of individual sounds from birds, amphibians, mammals, and insects*
*- **test_soundscapes/**: About 700 one-minute recordings used for evaluation*
*- **train_soundscapes/**: Unlabeled audio data from the same recording locations as tests*
*- **train.csv**: Metadata for training data*
*- **taxonomy.csv**: Information about different species*
*- **recording_location.txt**: Information about the recording location*

## Struttura del Repository / Repository Structure

```
BirdClefCompetition/
├── notebooks/                     # Jupyter notebooks per l'analisi e il modello
│   ├── exploratory/               # Analisi esplorativa dei dati
│   ├── feature_extraction/        # Notebooks per l'estrazione delle feature audio
│   ├── model_development/         # Notebooks per lo sviluppo del modello
│   └── submission/                # Notebooks per la generazione di submission
├── src/                           # Codice sorgente riutilizzabile
│   ├── data/                      # Script di gestione dei dati
│   ├── features/                  # Codice per l'estrazione delle feature
│   ├── models/                    # Implementazione dei modelli
│   └── utils/                     # Funzioni di utilità
├── config/                        # File di configurazione
├── data/                          # Dati locali (può essere gitignored)
│   ├── raw/                       # Dati non elaborati
│   └── processed/                 # Dati elaborati
├── output/                        # Modelli allenati e output vari
└── README.md                      # Questo file
```

## Setup e Installazione / Setup and Installation

```bash
# Clona il repository
git clone https://github.com/maurocarlu/BirdClefCompetition.git
cd BirdClefCompetition

# Crea un ambiente virtuale
python -m venv venv
source venv/bin/activate  # Su Windows: venv\Scripts\activate

# Installa le dipendenze
pip install -r requirements.txt
```

## Esecuzione dei Notebook / Running Notebooks

```bash
jupyter notebook notebooks/
```

## Approccio alla Soluzione / Solution Approach

La soluzione prevede:
1. **Preprocessing audio**: conversione dei file audio in spettrogrammi mel 
2. **Feature extraction**: estrazione di caratteristiche rilevanti dai segnali audio
3. **Model architecture**: utilizzo di architetture CNN o transformer per la classificazione audio
4. **Ensemble techniques**: combinazione di diversi modelli per migliorare le performance
5. **Post-processing**: ottimizzazione delle previsioni finali

*The solution includes:*
*1. **Audio preprocessing**: converting audio files to mel spectrograms*
*2. **Feature extraction**: extracting relevant features from audio signals*
*3. **Model architecture**: using CNN or transformer architectures for audio classification*
*4. **Ensemble techniques**: combining different models to improve performance*
*5. **Post-processing**: optimizing final predictions*

## Risultati / Results

[In questa sezione verranno aggiunti i risultati e le performance dei modelli sviluppati]

*[Results and performance metrics of developed models will be added here]*

## Risorse Utili / Useful Resources

- [Kaggle BirdClef2025 Competition](https://www.kaggle.com/competitions/birdclef-2025)
- [Xeno-canto.org](https://www.xeno-canto.org/)
- [iNaturalist](https://www.inaturalist.org/)
- [Acoustic Species Identification Papers](https://scholar.google.com/scholar?q=acoustic+species+identification)

## Contributori / Contributors

- [maurocarlu](https://github.com/maurocarlu)

## Licenza / License

Questo progetto è sotto licenza MIT - vedi il file [LICENSE](LICENSE) per i dettagli.

*This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.*