# ⚽ Football Intelligence Platform – Market Value & Replacement Insights

This project delivers a powerful football analytics solution using machine learning and visual dashboards to support clubs, analysts, and managers in decision-making. From predicting player market values to recommending performance-based replacements, the platform leverages data science to modernize scouting and transfer strategies.

---

## 📌 Overview

The platform offers two core capabilities:

1. **Player Market Value Estimation**
   - Predicts transfer market values using features like age, goals, assists, pass accuracy, and contract length.
2. **Player Replacement Finder**
   - Suggests alternative players based on performance similarity and team-fit predictions.

Visual dashboards in **Power BI** and **Tableau** allow users to interactively explore trends in player stats and valuations across leagues.

---

## 🚀 Core Features

### 💰 Market Value Prediction
- Model: **Gradient Boosting Regressor**  
- Achieved ~90% R² score  
- Key inputs: Age, goals, assists, passing metrics, contract years

### 🔁 Player Replacement Suggestions
- Cosine similarity identifies comparable players
- Classifiers (Random Forest + Gradient Boosting) determine team fit
- Handled class imbalance using **SMOTE**

### 📊 Visual Dashboards
- **Power BI**: Highlights performance trends, comparisons, and market insights  
- **Tableau**: Visualizes stats by age, height, position, and value range

---

## 🧱 Project Directory Structure

```plaintext
.
├── code/
│   ├── main.py                     # Streamlit application launcher
│   ├── market_value_model.py       # ML pipeline for market value
│   └── player_replacement_model.py # Replacement logic and classifiers
├── data/
│   ├── player_stats.csv            # Raw player performance data
│   └── market_values.csv           # Market valuation dataset
├── model/
│   ├── gbr_model.pkl               # Serialized Gradient Boosting model
│   └── similarity_model.pkl        # Cosine similarity object
├── dashboards/
│   ├── power_bi_dashboard.pbix     # Power BI dashboard file
│   └── tableau_dashboard.twbx      # Tableau dashboard file
├── requirements.txt                # Project dependencies
└── README.md                       # Project documentation
```

---

## ⚙️ Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-repo/football-analytics.git
cd football-analytics
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the Streamlit app
```bash
streamlit run code/main.py
```

### 4. View Dashboards
- **Power BI**:  
  [Launch Power BI Dashboard](https://app.powerbi.com/groups/me/reports/018b1e0d-080e-481e-9f8e-1fc94f0b468b/192daea5bdfd502dc7b8?experience=power-bi)

- **Tableau**:  
  [Open Tableau Dashboard](https://public.tableau.com/app/profile/vineeth.rayadurgam/viz/FootballAnalyticsDashboard-DATA230/Dashboard1)

---

## 📊 Data & Models

### 🧾 Data Sources
- Scraped and cleaned data from **Transfermarkt**
- Includes performance metrics, age, height, playing position, and contract status

### 🤖 Machine Learning Models
- **Market Value Estimator**: Gradient Boosting Regressor (`gbr_model.pkl`)
- **Replacement System**:
  - Cosine Similarity for match scoring
  - Classification via Random Forest & Gradient Boosting (team-fit predictions)

### 📈 Metrics
- R²: ~90% for regression accuracy
- Classification Accuracy: ~85%  
- Balanced precision/recall with SMOTE handling

---

## 💡 Key Findings

- Players aged 21–27 and height range of 180–190 cm often have higher market value
- Goal contributions and progressive passing are major indicators
- Top replacements ranked using similarity and classifier predictions

---

## 🔮 Future Enhancements

- Add **historical performance timelines**
- Integrate **live API feeds** for up-to-date stats
- Support advanced metrics like **Expected Goals (xG)** and injury records

---

## 👨‍💻 Contributors

- **Sai Kiran Reddy Pothuganti**
- **Vivek Varma Rudraraju**
 
