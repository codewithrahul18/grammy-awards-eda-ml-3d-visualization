# 🎵 Grammy Awards Analysis (1959–2026)

> A professional data science project analyzing six decades of Grammy Award history through exploratory data analysis, interactive visualizations, 3D charts, and machine learning.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Plotly-3D%20Viz-3F4F75?style=for-the-badge&logo=plotly&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge"/>
</p>

---

## 👤 Author

**RAHUL CHAUHAN**

[![GitHub](https://img.shields.io/badge/GitHub-codewithrahul18-181717?style=flat-square&logo=github)](https://github.com/codewithrahul18)
[![Kaggle](https://img.shields.io/badge/Kaggle-codewithrahul18-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/rahulchauhan016)

---

## 📌 About This Project

The Grammy Awards are the most prestigious recognition in the music industry. This project dives deep into the full winner history from **1959 to 2026**, covering all 68 ceremonies, to answer questions like:

- Which artists have won the most Grammys of all time?
- How has the Big Four category dominated over the decades?
- Can we predict what award group a winner belongs to using machine learning?
- Which artists have the highest career success based on wins, longevity, and category diversity?

---

## 📊 Advanced Visualization Preview

![Sunburst Chart](assets/screenshot_sunburst.png)
*Interactive Sunburst — Full Grammy taxonomy from Era → Award Group → Category*

---

## 🔍 Project Workflow

The notebook is structured as a clean end-to-end data science pipeline:

| Step | Description |
|------|-------------|
| 📥 Data Loading | Load raw CSV dataset from Kaggle |
| 🧹 Data Cleaning | Remove duplicates, fix data types, engineer new features |
| 📊 EDA | Explore trends by year, artist, decade, and award group |
| 🌐 Interactive Charts | Sunburst, Treemap, and Animated Bar using Plotly |
| 🌌 3D Visualizations | 3D Scatter, 3D Surface, and 3D Line charts |
| 🤖 Machine Learning | Random Forest model to predict award group |
| ⭐ Scoring | Weighted artist success score based on multiple career factors |
| 💾 Export | Save cleaned data and artist scores as CSV files |

---

## 🌌 Visualizations Included

**Static Charts (Matplotlib & Seaborn)**
- Grammy winners timeline across all years
- Top 15 artists by total wins
- Award group distribution — pie and bar
- Wins by decade grouped by award type
- Feature correlation heatmap
- Confusion matrix and feature importance

**Interactive Charts (Plotly)**
- Sunburst chart — Era → Award Group → Category
- Treemap — artists with 2+ wins by award type
- Animated bar chart — wins per year from 1959 to 2026
- Bubble chart — career span vs wins vs success score

**3D Charts (Plotly)**
- 3D Scatter — Year × Career Wins × Annual Wins
- 3D Surface — win density across decades and award groups
- 3D Line — Big Four category trends over time

---

## 🤖 Machine Learning Model

A **Random Forest Classifier** is trained to predict whether a Grammy winner belongs to the **Big Four** or **Genre** award group.

- **Features used:** Year, Artist, Category, Era, Decade
- **Evaluation:** Test accuracy, 5-fold cross validation, confusion matrix
- **Insight:** Category encoding is the strongest predictor at 65.8% importance

---

## ⭐ Artist Success Score

Each artist is scored using a weighted formula that goes beyond just counting wins:

```
Success Score =
    Total Wins       × 2.0   (base win count)
  + Big Four Wins    × 3.5   (prestige multiplier)
  + Career Span      × 0.3   (longevity bonus)
  + Unique Categories× 1.0   (diversity bonus)
  + Recency Bonus    × 2.0   (active in recent years)
```

---

## 🛠️ Tech Stack

| Library | Version | Purpose |
|---------|---------|---------|
| Python | 3.12 | Core language |
| Pandas | Latest | Data manipulation |
| NumPy | Latest | Numerical operations |
| Matplotlib | 3.x | Static visualizations |
| Seaborn | 0.13 | Statistical plots |
| Plotly | Latest | Interactive & 3D charts |
| Scikit-learn | Latest | Machine learning |

---

## 🚀 Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/codewithrahul18/grammy-awards-eda-ml-3d-visualization.git
cd grammy-awards-eda-ml-3d-visualization
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn jupyter
```

**3. Download the dataset**

Get the dataset from [Kaggle](https://www.kaggle.com) and place the CSV at:
```
/kaggle/input/grammy-award-winners-1959-2026/Grammy_Awards_Winners_20260208_055452.csv
```

**4. Launch the notebook**
```bash
jupyter notebook grammy_improved.ipynb
```

---

## 📁 Repository Structure

```
grammy-awards-eda-ml-3d-visualization/
│
├── grammy_improved.ipynb        ← Main analysis notebook
├── README.md                    ← Project documentation
├── cleaned_grammy_data.csv      ← Cleaned dataset output
├── artist_success_scores.csv    ← Artist scoring output
├── LICENSE                      ← MIT License
└── assets/
    └── screenshot_sunburst.png  ← Visualization preview
```

---

## 📄 MIT License

```


```

---

## 🙌 Acknowledgements

- Dataset collected from **Wikipedia** and published on **Kaggle**
- Grammy Award data © The Recording Academy
- Built entirely with open-source Python libraries

---

<p align="center">⭐ If you found this useful, please star the repository!</p>
