# SpeechUnderstandingQ2
# Speech Processing Assignment

## Overview
This project focuses on analyzing urban sound datasets using various machine learning techniques. It involves data preprocessing, feature extraction, spectrogram generation, and classifier evaluation for audio classification tasks.

## Dataset
The dataset used is **UrbanSound8K**, which contains different classes of urban sound recordings. It is downloaded and extracted automatically within the script.

## Installation & Dependencies
Ensure you have the following dependencies installed before running the script:

```bash
pip install numpy pandas librosa matplotlib seaborn scikit-learn xgboost
```

Additionally, if using Google Colab, make sure to mount Google Drive and download the dataset correctly.

## Script Functionality
The script performs the following tasks:

### 1. Data Download and Preprocessing
- Downloads the **UrbanSound8K** dataset.
- Extracts and organizes the dataset.
- Loads audio files and converts them into structured data.

### 2. Spectrogram Generation
- Uses **Short-Time Fourier Transform (STFT)** with Hann, Hamming, and Rectangular window functions.
- Saves spectrograms as images for visualization.

### 3. Feature Extraction
- Extracts **MFCCs, Chroma, Mel Spectrogram, Spectral Contrast, and Tonnetz** features using `librosa`.
- Stores extracted features in a structured dataframe.

### 4. Classification using Machine Learning Models
- Uses classifiers like:
  - K-Nearest Neighbors (KNN)
  - Random Forest
  - AdaBoost
  - Gradient Boosting
  - XGBoost
  - Multi-Layer Perceptron (MLP)
- Evaluates models based on **accuracy, precision, and recall**.
- Displays a confusion matrix for performance comparison.

### 5. Spectrogram Analysis of Songs
- Generates spectrograms for additional audio files (if available in `.mp3` format).
- Uses **Librosa STFT** for visualization.

## Usage Instructions
Run the script using:
```bash
python speechassignment.py
```
Or, if using Google Colab, execute the notebook cells sequentially.

## Output
- **Waveform Plots**: Visual representation of time-domain signals.
- **Spectrograms**: Generated for each sound class with different window functions.
- **Feature Dataframe**: Contains extracted features for classification.
- **Model Evaluation Metrics**: Accuracy, precision, recall, and confusion matrix for classifiers.

## Author
- Your Name
- Contact: your.email@example.com

