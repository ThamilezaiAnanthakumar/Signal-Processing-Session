# Signal Processing Session

This repository contains implementations and experiments focused on **PPG (Photoplethysmography) signal processing**, including preprocessing pipelines, peak detection–based heart rate estimation, and integration with foundation models such as Papagei.

---

## 📌 Overview

This project is designed to help understand and build  pipelines for physiological signal processing. It includes:

- 📊 Signal preprocessing (filtering, normalization, resampling)
- ❤️ Heart rate (HR) estimation using peak detection
- 🤖 Integration with Papagei foundation model
- 🧠 Usage of NeuroKit2 for physiological signal analysis
- 📈 Visualization in time and frequency domains

---

## 🚀 Features

### 1. PPG Preprocessing
- Bandpass filtering (removes noise and motion artifacts)
- Resampling to a target frequency
- Signal normalization
- Segmentation with overlapping windows

### 2. Peak Detection-Based HR Estimation
- Uses `scipy.signal.find_peaks`
- Configurable parameters:
  - `distance` (minimum gap between peaks)
  - `prominence` (peak strength threshold)
- Converts peak intervals into heart rate (BPM)

### 3. Papagei Foundation Model
- Preprocessed signals are compatible with Papagei-based pipelines
- Enables representation learning from physiological signals
- Useful for:
  - HR prediction
  - Signal quality assessment
  - Health monitoring

### 4. NeuroKit2 Integration
We use [NeuroKit2](https://neuropsychology.github.io/NeuroKit/), a widely used Python package for biosignal processing.

Capabilities:
- PPG/ECG cleaning
- Peak detection
- HRV analysis
- Signal simulation

---

## 📚 References

Papagei Foundation Model [Paper](https://arxiv.org/pdf/2410.20542)
Papagei Foundation Model [Github](https://github.com/Nokia-Bell-Labs/papagei-foundation-model)
