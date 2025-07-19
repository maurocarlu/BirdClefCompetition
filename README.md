# BirdClef2025 Competition

![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

## Overview

*This repository contains notebooks and code used for the Kaggle BirdClef2025 competition, focused on identifying animal species (birds, amphibians, mammals, insects) through their acoustic signatures recorded in El Silencio Natural Reserve, Colombia.*

## Competition Goal

*The goal is to develop machine learning algorithms capable of:*
*1. Identifying species from different taxonomic groups in the Magdalena Valley of Colombia*
*2. Training models with limited datasets for rare and endangered species*
*3. Enhancing models using unlabeled data*

## Context

*El Silencio Natural Reserve protects 5,407 acres of tropical lowland forests and wetlands. It hosts diverse wildlife, including 295 birds, 34 amphibians, 69 mammals, 50 reptiles, and nearly 500 plant species. A significant part of the reserve, previously used for extensive livestock farming, is now under an ecological restoration project.*

*Through this Kaggle competition, the aim is to automate the detection and classification of different taxonomic groups from soundscapes of El Silencio Natural Reserve, with the intent to provide a better understanding of the ecological processes of restoration projects.*

## Dataset

*The dataset includes:*
*- **train_audio/**: Short recordings of individual sounds from birds, amphibians, mammals, and insects*
*- **test_soundscapes/**: About 700 one-minute recordings used for evaluation*
*- **train_soundscapes/**: Unlabeled audio data from the same recording locations as tests*
*- **train.csv**: Metadata for training data*
*- **taxonomy.csv**: Information about different species*
*- **recording_location.txt**: Information about the recording location*

## Repository Structure

The main folder contains the following files and notebooks:

- **notebook-birdclef MLP.ipynb**  
  Training notebook using the MLP head.
- **notebook-birdclef SED.ipynb**  
  Training notebook using the SED head (Sound Event Detection).
- **inference MLP.ipynb**  
  Inference notebook for the MLP model.
- **inference SED.ipynb**  
  Inference notebook for the SED model.
- **t-student.ipynb**  
  Notebook for statistical comparison between models using the t-student test on predictions.
- **Report Carlucci Mauro.pdf**  
  Technical documentation in pdf format.
- **README.md**  
  This description file.

## Solution Approach
*The solution includes:*
*1. **Audio preprocessing**: converting audio files to mel spectrograms*
*2. **Feature extraction**: extracting relevant features from audio signals*
*3. **Model architecture**: using CNN or transformer architectures for audio classification*
*5. **Post-processing**: optimizing final predictions*

## Useful Resources

- [Kaggle BirdClef2025 Competition](https://www.kaggle.com/competitions/birdclef-2025)
- [Xeno-canto.org](https://www.xeno-canto.org/)
- [iNaturalist](https://www.inaturalist.org/)

## Contributors

- [maurocarlu](https://github.com/maurocarlu)