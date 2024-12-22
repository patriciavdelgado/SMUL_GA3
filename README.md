# Environmental Sound Classification Project

## Overview
This project implements a system for classifying environmental sounds using the UrbanSound8K dataset. The methodology combines feature extraction techniques (log mel spectrograms and MFCCs) with a Support Vector Machine (SVM) classifier. This repository contains all the necessary files and scripts to reproduce the results and train the model.

## Features
- **Dataset**: UrbanSound8K, a collection of 8,732 labeled sound excerpts across 10 classes.
- **Features Extracted**:
  - Log mel spectrograms: Capturing frequency distribution as image representations.
  - Mel-Frequency Cepstral Coefficients (MFCCs): Compact audio representations for spectral properties.
- **Model**: SVM with an RBF kernel optimized using GridSearchCV.
- **Performance**: Achieved best cross-validation accuracy of 88.23% with optimal parameters (C = 100, gamma = 0.01).

## Repository Structure
- `svm_model`: Directory containing Features Extraction, SVM model with linear kernel (with classification report) , Grid Search for RBF parameters, SVM model with RBF kernel(with classification report).

## Requirements
-FMP Jupyter Notebooks (Python). https://www.audiolabs-erlangen.de/resources/MIR/FMP/FMP_1.2.6.zip
- Python 3.8.20
- librosa  0.8.0
-pandas   2.0.3 
-numpy    1.23.5
-tqdm     4.67.1 
-pickleshare   0.7.5 
- Extracted Dataset.
- A GPU is optional but can improve the feature extraction process.

## Instructions
You need to have the UrbanSound8K dataset extrated and change the part of the code related to the datapath.


## Acknowledgments
- UrbanSound8K dataset:
  - J. Salamon, C. Jacoby, and J. P. Bello, “A dataset and taxonomy for urban sound research,” in *Proceedings of the 22nd ACM international conference on Multimedia*. ACM, November 2014, pp. 1041–1044.
- References to relevant methodologies:
  - Y. Su et al., “Performance analysis of multiple aggregated acoustic features for environment sound classification,” *Applied Acoustics*, vol. 158, p. 107050, 2020.
  - Z. Mushtaq et al., “Spectral images based environmental sound classification using CNN with meaningful data augmentation,” *Applied Acoustics*, vol. 172, p. 107581, 2021.
  - K. J. Piczak, “ESC: Dataset for Environmental Sound Classification,” in *Proceedings of the 23rd ACM International Conference on Multimedia*. ACM, October 2015, pp. 1015–1018.

