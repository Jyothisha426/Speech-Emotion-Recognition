# 🎙️ Speech Emotion Recognition (SER) using Deep Learning

This project focuses on recognizing human emotions from speech using advanced deep learning models and audio feature extraction techniques. It utilizes benchmark datasets like **RAVDESS** and **TESS**, and implements a **CNN-based architecture** trained on **log-Mel spectrograms**, **MFCCs**, and other features for effective emotion classification.

---

## 🧠 Motivation

Speech carries rich emotional content via tone, pitch, and rhythm. Accurate emotion recognition from speech can enhance:
- Human-computer interaction (e.g., intelligent assistants)
- Mental health diagnostics
- Emotion-aware applications like smart call centers, e-learning, and social robotics

---

## 📁 Datasets Used

### 1. [RAVDESS](https://zenodo.org/record/1188976)
- 1,440 audio files
- 24 actors (12 male, 12 female)
- 8 emotions

### 2. [TESS](https://doi.org/10.5683/SP2/E8H2MF)
- 2,800 audio files
- 2 actresses (ages 26 and 64)
- 7 emotions

---

## ⚙️ Methodology

### ✔️ Preprocessing
- Merged both datasets
- Removed the 'calm' label for uniform emotion categories
- Converted audio files to WAV format
- Applied noise addition, stretching, time shifting, and pitch shifting for **data augmentation**

### ✔️ Feature Extraction
- Zero Crossing Rate (ZCR)
- Chroma STFT
- MFCC (Mel-Frequency Cepstral Coefficients)
- Root Mean Square (RMS) Energy
- Mel Spectrograms

### ✔️ Model Architecture
- **Convolutional Neural Network (CNN)** trained on spectrogram-based features
- Early stopping, standard scaling
- Evaluation using accuracy, F1-score, confusion matrix

---

## 📊 Results

| Emotion  | Precision | Recall | F1-score |
|----------|-----------|--------|----------|
| Angry    | 0.92      | 0.91   | 0.92     |
| Disgust  | 0.83      | 0.85   | 0.84     |
| Fear     | 0.91      | 0.88   | 0.89     |
| Happy    | 0.79      | 0.86   | 0.82     |
| Neutral  | 0.84      | 0.96   | 0.90     |
| Sad      | 0.89      | 0.83   | 0.85     |
| Surprise | 0.92      | 0.84   | 0.88     |

✅ **Accuracy**: ~87%

---
