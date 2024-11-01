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
# Running the Project

## Data Preprocessing
1. **Load and Clean Data**  
   - Import and clean the raw `gene_data.fasta` and `mutations.csv` files to prepare for segmentation.

2. **Generate Segment Files**  
   - Create `pathogenic_data.csv` and `normal_data.csv` by segmenting DNA sequences into 100-nucleotide segments around specified mutation points (positions 20, 50, 80).

## Feature Extraction
1. **FCGR Visualization**  
   - Run the FCGR script to generate visual representations for k-mers of lengths 3, 4, 5, and 6.

2. **DNA Sonification**  
   - Use the sonification script to convert DNA sequences into audio signals. Then, extract MFCC, chroma, and spectral descriptors as sonar features for further analysis.

## Classification Models
1. **Train on FCGR Data**  
   - Train CNN, CNN+LSTM, VGG16, and ResNet50 models on FCGR-generated images for classifying genetic mutation data.

2. **Train on Sonar Features**  
   - Train SVM and Random Forest models on the extracted sonar features.

3. **Evaluate Model Performance**  
   - The best accuracy achieved was **92.47% using CNN with k-mers 6 data**.

## Analysis and Visualization
- Access performance metrics, confusion matrices, and visual representations of model results in the results notebook.

## Results
- **CNN with k-mers 6 data** achieved a 92.47% accuracy rate, showcasing the potential of deep learning in genetic mutation analysis associated with Parkinson's Disease.

## Future Work
- **Explore Additional Genetic Markers**  
   - Investigate more genetic markers and environmental factors to develop a more comprehensive model.

- **Experiment with Advanced Architectures**  
   - Test alternative deep learning architectures and new feature extraction techniques for improved results.

## Contributing
- Contributions are welcome! Please open an issue or submit a pull request if you have suggestions for improvements, feature additions, or optimizations.

## License
This project is licensed under the AGPL-3.0 License.

---

**Developed by Badis Sdiri**
pip install tensorflow keras pandas numpy matplotlib librosa scikit-learn

This README provides a clear structure, installation steps, usage, and a brief of your findings. Let me know if there are any additional details you'd like included!
```bash
pip install tensorflow keras pandas numpy matplotlib librosa scikit-learn

This README provides a clear structure, installation steps, usage, and a brief of your findings. Let me know if there are any additional details you'd like included!
