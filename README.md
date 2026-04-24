# 🧠 Mind-Wander: EEG-Based Attention State Detection using Dual-Stream Deep Learning

## 📌 Overview
**Mind-Wander** is a deep learning framework designed to detect **mind-wandering (MW)** vs **on-task (OT)** cognitive states using EEG signals.

The system combines:
- 🧩 Temporal modeling (raw EEG)
- 📊 Spectral feature learning (frequency bands)
- 🔗 Cross-attention fusion

---

## 🚀 Key Contributions
- Novel **Dual-Stream EEG Architecture**
- Integration of **temporal + spectral features**
- **Cross-attention mechanism** for feature fusion
- Evaluated using **Leave-One-Subject-Out (LOSO)**
- Achieved **96.9% accuracy**

---

## 🧠 Architecture

### Dual-Stream Model
| Stream | Input | Purpose |
|-------|------|--------|
| Temporal | Raw EEG | Capture waveform patterns |
| Spectral | Bandpower | Capture oscillatory activity |

### Fusion
- Cross-attention aligns temporal and spectral features
- Produces unified embedding for classification

---

## 📂 Dataset
- Dataset: BCIT Mind-Wandering Dataset  
- Subjects: 12  
- Channels: 74  
- Sampling Rate: 1024 Hz → 128 Hz  
- Total Samples: 22,271  

---

## ⚙️ Preprocessing
- Bandpass filtering  
- Artifact removal  
- ICA denoising  
- Segmentation  

---

## 📊 Results

| Model | Accuracy |
|------|--------|
| EEGNet | 53.7% |
| CNN | 75.2% |
| CNN-TCN | 81.1% |
| **Dual-Stream** | **96.9%** |

---

## 🧾 Project Structure
Mind-Wander/
│
├── data/
├── models/
├── training/
├── evaluation/
└── README.md

---

## ▶️ Usage

Train:
python train.py

Evaluate:
python evaluate.py

---

## 👩‍💻 Authors
- Sonali Gupta  
- Disha Rani  
- Sparsh Agarwal  
- Ashish Bajaj  

---

## ⭐ Support
Give a ⭐ if you like this project!
