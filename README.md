# ANALYSIS AND CLASSIFICATION OF GENETIC MUTATIONS ASSOCIATED WITH PARKINSON'S DISEASE

## Project Overview
This project focuses on analyzing and detecting Parkinson's disease through genetic mutations using DNA signal processing and deep learning. Key methodologies include:

- **Frequency Chaos Game Representation (FCGR):** Visualizes DNA sequences, generating data for k-mers of lengths 3, 4, 5, and 6.
- **Convolutional Neural Networks (CNN) and Deep Learning Models:** Includes VGG16, ResNet50, and a combined CNN+LSTM model to classify spatial and sequential features.
- **DNA Sonification:** Transforms DNA sequences into audio, extracting sonar features (MFCC, chroma, spectral descriptors) and using these features in SVM and Random Forest classifiers.

This repository provides all necessary scripts, preprocessing steps, and visual aids, allowing for replication and further exploration in genetic mutation analysis.

## Project Structure
- `data/`: Contains raw and processed data files.
  - `gene_data.fasta`: Fasta file containing sequences of 11 genes related to Parkinson's Disease.
  - `mutations.csv`: CSV file with descriptions of mutations.
  - `pathogenic_data.csv` & `normal_data.csv`: Data files containing pathogenic and normal gene segments, each 100 nucleotides in length and targeted around mutation positions (20, 50, 80).
- `notebooks/`: Jupyter notebooks for data preprocessing, FCGR generation, sonification, and model training.
- `results/`: Output files, model accuracies, and visual representations of the models.

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required libraries: `tensorflow`, `keras`, `pandas`, `numpy`, `matplotlib`, `librosa`, `scikit-learn`

Install the required libraries:
```bash
pip install tensorflow keras pandas numpy matplotlib librosa scikit-learn
