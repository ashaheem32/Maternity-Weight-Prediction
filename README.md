# Maternity Weight Prediction

Predicting newborn weight using maternal and pregnancy features through data analysis and machine learning.

---

## 🧭 Overview

This project demonstrates a complete end-to-end data science workflow for predicting newborn weight from prenatal and maternal characteristics. Using regression models and exploratory data analysis, we identify key factors influencing birth weight and develop predictive tools for healthcare applications.

**Key Components:**
- Comprehensive data cleaning and preprocessing
- In-depth exploratory data analysis with visualizations
- Feature engineering for optimal model performance
- Baseline and advanced regression models
- Performance comparison and insights

---

## 📂 Repository Structure

```
Maternity-Weight-Prediction/
├── Weight_Prediction.ipynb          # Complete analysis & modeling workflow
├── baby-weights-dataset.csv         # Training dataset
├── data-description.txt             # Feature metadata and descriptions
├── requirements.txt                 # Python dependencies
└── README.md                        # Project documentation
```

---

## 📊 Dataset

**File:** `baby-weights-dataset.csv`

Contains maternal and pregnancy-related variables including age, BMI, gestation period, blood pressure, and lifestyle factors used to predict newborn weight.

**Features:** Detailed in `data-description.txt`

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handling missing values and outliers
- Categorical variable encoding
- Feature scaling and normalization

### 2. Exploratory Data Analysis
- Univariate and bivariate analysis
- Correlation analysis with heatmaps
- Target variable distribution analysis

### 3. Model Development
- **Linear Regression** — Baseline linear model
- **Decision Tree Regressor** — Capture non-linear patterns
- **Random Forest Regressor** — Ensemble approach for improved performance

### 4. Model Evaluation
Metrics used: MAE, RMSE, and R² score

| Model | R² Score | RMSE | MAE |
|-------|----------|------|-----|
| Random Forest | 0.586 | 0.658 | 0.487 |
| XGBoost | 0.593 | 0.652 | 0.485 |
| LightGBM | 0.594 | 0.652 | 0.483 |

**Insights:** LightGBM achieved the best overall performance with the highest R² score (0.594) and lowest MAE (0.483), demonstrating superior predictive capability for newborn weight estimation.

---

## 🚀 Getting Started

### Option 1: Run Locally

**1. Clone the repository**
```bash
git clone https://github.com/ashaheem32/Maternity-Weight-Prediction.git
cd Maternity-Weight-Prediction
```

**2. Create and activate a virtual environment**
```bash
# macOS/Linux
python -m venv venv
source venv/bin/activate

# Windows (PowerShell)
python -m venv venv
venv\Scripts\Activate.ps1
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

If `requirements.txt` is unavailable, install manually:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter ipykernel
```

**4. Launch the notebook**
```bash
jupyter notebook Weight_Prediction.ipynb
```

---

### Option 2: Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload `Weight_Prediction.ipynb`
3. Upload `baby-weights-dataset.csv` or mount Google Drive
4. Adjust file paths if needed and run all cells

---

## 🔧 Technical Stack

- **Python 3.8+**
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **scikit-learn** — Machine learning models and evaluation
- **Matplotlib & Seaborn** — Data visualization
- **Jupyter** — Interactive notebook environment

---

## 🎯 Future Enhancements

- Implement advanced ensemble models (XGBoost, LightGBoost, Gradient Boosting)
- Hyperparameter optimization (GridSearchCV, RandomizedSearchCV)
- K-fold cross-validation for robust evaluation
- Flask/FastAPI web application for real-time predictions
- Model explainability with SHAP or LIME visualizations
- Automated model deployment pipeline

---

## ♻️ Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes
   ```bash
   git commit -m "Add descriptive commit message"
   ```
4. Push and open a Pull Request

---

## 📜 License

This project is currently unlicensed. Consider adding a [MIT License](https://opensource.org/licenses/MIT) for open-source distribution.

---

## 👩‍💻 Author

**Ashaheem**
- GitHub: [@ashaheem32](https://github.com/ashaheem32)

---

## ⚠️ Disclaimer

This project is for educational and research purposes only. Predictions should not be used for clinical or diagnostic decisions without professional medical validation and expert review.

---

**Questions or feedback?** Feel free to open an issue or reach out!
