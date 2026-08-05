# 🚀 SpaceX Falcon 9 First Stage Landing Prediction

[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Dash-Plotly-orange.svg)](https://dash.plotly.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **IBM Data Science Professional Certificate - Capstone Project**  
> Repository Link: [https://github.com/marcelocards/capstone_spacex](https://github.com/marcelocards/capstone_spacex)

---

## 📌 Executive Summary

Commercial space launch providers like SpaceX have revolutionized the space industry by drastically reducing launch costs. A primary factor behind this cost reduction is the successful recovery and reuse of the **Falcon 9 first-stage booster**. While traditional launches cost upwards of **$165 million**, a Falcon 9 launch is priced around **$62 million**—largely due to booster reuse.

### Key Insights & Findings
* **Optimal Payload Range:** The landing success rate is highest for payloads between **2,000 kg and 4,000 kg**.
* **Launch Site Performance:** **KSC LC-39A** achieved the highest overall success rate (~76.9%), while **CCAFS LC-40** handled the highest volume of total successful launches.
* **Booster Evolution:** Newer booster iterations (**FT** and **Block 5**) achieved a near 100% successful landing rate compared to earlier variants (v1.0 and v1.1).
* **Best Predictive Model:** The **Decision Tree Classifier** (alongside SVM/KNN depending on hyperparameter tuning) achieved the top accuracy score (~83.3%) on test data.

---

## 📂 Repository Structure

```text
capstone_spacex/
│
├── data/
│   ├── dataset_part_1.csv         # Raw API collected data
│   ├── dataset_part_2.csv         # Processed dataset after wrangling
│   └── dataset_part_3.csv         # One-hot encoded features for ML
│
├── notebooks/
│   ├── 01_SpaceX_Data_Collection_API.ipynb
│   ├── 02_SpaceX_Data_Collection_WebScraping.ipynb
│   ├── 03_SpaceX_Data_Wrangling.ipynb
│   ├── 04_SpaceX_EDA_SQL.ipynb
│   ├── 05_SpaceX_EDA_Visualization.ipynb
│   ├── 06_SpaceX_Interactive_Visual_Analytics_Folium.ipynb
│   └── 07_SpaceX_Machine_Learning_Prediction.ipynb
│
├── dash_app/
│   └── dash_capstone.py           # Plotly Dash Interactive Dashboard
│
├── presentation/
│   └── SpaceX_Capstone_Final_Presentation.pdf
│
└── README.md
