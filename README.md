# Cyclone-Anomaly-Detection
Unsupervised cyclone trajectory anomaly detection using deep feature learning and PANDA-based scoring
This project presents an **unsupervised cyclone trajectory anomaly detection framework**
that leverages deep feature representations extracted from satellite imagery and a
PANDA-based scoring mechanism. The model is trained exclusively on normal (non-curving)
cyclone trajectories and identifies anomalous curving patterns based on deviation
in learned feature space.


Cyclone-Anomaly-Detection/
│
├── data/
│   ├── README.md
│
├── notebooks/
│   └── Method_B_Cyclone_Anomaly_Detection.ipynb
│
├── src/
│   ├── feature_extraction.py
│   ├── model.py
│   ├── scoring.py
│   └── utils.py
│
├── Graphical_Results/
│   ├── anomaly_score_distribution.png
│   ├── normal_vs_anomaly.png
│
├── requirements.txt
└── README.md
