# Lab 4 – Epileptic Seizures (EEG Analysis)

## 📌 Objective
The goal of this lab is to analyze EEG signals in order to detect and understand epileptic seizures using both linear and nonlinear methods.

---

## 📊 Tasks Overview

### 1. Raw EEG, Spectrogram, and Spectral Entropy
- The raw EEG signal (17 minutes) is visualized.
- A spectrogram is computed to observe frequency changes over time.
- Spectral entropy is calculated to quantify signal complexity.

👉 Seizures appear as:
- High amplitude bursts in raw EEG
- Broadband activity in spectrogram
- Sudden drops in spectral entropy

---

### 2. Ictal vs Interictal Comparison
- Two 10-second segments are extracted:
  - **Ictal** (during seizure)
  - **Interictal** (normal activity)

These segments show clear differences in signal amplitude and behavior.

---

### 3. Nonlinear Analysis (2D Embedding)
- A segment containing preictal, ictal, and postictal states is extracted.
- Time-delay embedding is applied using Δ = 67.
- The system dynamics are visualized in 2D space.

👉 Different colors represent:
- **Cyan** → Ictal (seizure)
- **White/Black** → Pre/Post ictal
- **Red** → Interictal

This demonstrates that seizure activity produces a different attractor compared to normal EEG.

---

## 📷 Results

### Raw EEG Signal
![Raw EEG](results/RAW_EEG.png)

### Ictal vs Interictal Segments
![Ictal vs Interictal](results/Ictal_Interictal_EEG.png)

### EEG Segment and 2D Embedding
![2D Embedding](results/Segment_Embedding.png)

---

## 🧠 Key Observations
- Seizures are clearly identifiable in both time and frequency domains.
- Spectral entropy decreases during seizures, indicating more regular signal behavior.
- 2D embedding reveals a transition in system dynamics between normal and seizure states.

---

## ⚙️ Implementation
- MATLAB was used for signal processing and visualization.
- Key methods:
  - Spectrogram analysis
  - Spectral entropy calculation
  - Time-delay embedding (Δ = 67)

---

## ✅ Conclusion
This lab demonstrates how EEG signals can be analyzed to detect epileptic seizures using both linear and nonlinear approaches. The results show clear differences between normal and seizure activity, both visually and mathematically.
