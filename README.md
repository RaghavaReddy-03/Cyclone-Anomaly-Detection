# Cyclone-Anomaly-Detection

## Overview
This project presents an **unsupervised cyclone trajectory anomaly detection framework**
that leverages **deep feature representations** extracted from satellite imagery and a
**PANDA-based scoring mechanism**.

The model is trained **exclusively on normal (non-curving) cyclone trajectories** and
identifies anomalous **curving cyclone patterns** based on deviations in the learned
feature space.

---

## Methodology 
- Single-frame deep feature extraction using a CNN backbone
- PANDA-based compact feature representation
- Elastic Weight Consolidation (EWC) for model stability
- k-NN distance-based anomaly scoring

---

## Why Unsupervised?
Cyclone trajectory anomalies are rare and highly diverse, making labeled anomaly data
scarce and unreliable.  
This motivates a **one-class, unsupervised learning setup**, where the model learns only
normal cyclone behavior and flags deviations as anomalies.

---

## Dataset
- **Training:** Non-curving cyclones (normal)
- **Testing (Normal):** Unseen non-curving cyclones
- **Testing (Anomalous):** Curving cyclones

---

## Results
The anomaly scores for curving cyclones are consistently higher than those for normal
cyclones, demonstrating effective separation in the learned feature space.


---

## Project Structure

```bash
Cyclone-Anomaly-Detection/
│
├── notebooks/
│   └── Cyclone_Anomaly_Detection.ipynb
│
├── src/
│   ├── feature_extraction.py
│   ├── model.py
│   ├── scoring.py
│   └── utils.py
│
├── Graphical_Results/
│   ├── anomaly_score_distribution.png
│   └── normal_vs_anomaly.png
│
├── data/
│   └── README.md
│
├── requirements.txt
└── README.md

