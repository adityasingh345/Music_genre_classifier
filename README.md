# Music_genre_classifier

# 🎵 Music Genre Classifier (GTZAN Dataset)

This project is a machine learning-based music genre classification system built using the [GTZAN dataset]. It extracts relevant audio features from `.wav` files using Librosa, applies feature scaling, and trains multiple models to accurately predict the genre of music.

> ✅ Achieved **70% accuracy** using SVM on handcrafted audio features.

---

## 📁 Dataset

- Dataset Used: [GTZAN Genre Collection](http://marsyas.info/downloads/datasets.html)
- Format: `.wav`
- Size: ~1.2 GB
- 10 Genres: blues, classical, country, disco, hiphop, jazz, metal, pop, reggae, rock
- 100 audio files per genre (each ~30 seconds)

---

## 🧠 Features Extracted

Extracted using `librosa`:

- **MFCC (13 coefficients)**
- **Chroma frequencies (12 bins)**
- **Zero Crossing Rate (mean + std)**
- **Spectral Contrast (7 bands)**
- **Tempo (beats per minute)**

---

## ⚙️ Tech Stack

| Tool/Library       | Purpose                       |
|--------------------|-------------------------------|
| `Python`           | Core programming language     |
| `Librosa`          | Audio feature extraction      |
| `NumPy / Pandas`   | Data handling                 |
| `Scikit-learn`     | ML models + preprocessing     |
| `Matplotlib`       | Optional for visualization    |

---

## 🚀 ML Models Used

| Model              | Accuracy (Test Set) |
|--------------------|---------------------|
| Random Forest      | ~65%                |
| **SVM (RBF Kernel)**| **~70% ✅**         |

---

## 📊 Workflow

1. **Load Dataset & Clean Files**
2. **Extract Features from Each `.wav` File**
3. **Flatten and Combine into Feature Vectors**
4. **Scale Features using StandardScaler**
5. **Split into Train/Test using Stratified Split**
6. **Train & Evaluate Models**

---

## 📝 Results

- **Best Accuracy:** 70% using **SVM** with RBF kernel
- **Balanced performance** across most genres

---


