# Location-vs-Structure_Hypothesis-Testing

# 🏠 HouseValueX: Do Size and Age Matter Most?

A data science project investigating whether **structural features** such as the **size** and **age** of a house are the most significant predictors of its market price—**regardless of location**.

---

## 📌 Project Objective

The aim of this study is to test the hypothesis:

> _"The size and age of a house are the most significant predictors of its market price, regardless of location."_

Using statistical testing and machine learning models, we analyze how much impact structural features (like square footage and construction year) have on home pricing, and whether they outweigh location-based attributes.

---

## 📊 Dataset

- **Source:** Cleaned dataset containing **13,515 residential properties** from **Northern California**
- **Features:**  
  - Structural: `bsqft`, `lsqft`, `br`, `year`  
  - Geographic: `city`, `county`, `lat`, `long`  
  - Target: `price`

---

## 🧪 Methods

### 1. 🧹 Data Preprocessing
- Dropped rows with missing values in critical columns
- Standardized feature formats and categorical encodings

### 2. 📈 Exploratory Data Analysis
- Price distributions, correlation heatmaps, and city-level visualizations

### 3. 🤖 Modeling
- Models used:
  - Linear Regression
  - Ridge Regression
  - Random Forest Regressor
- Evaluation metrics:
  - R² Score
  - Mean Absolute Error (MAE)
- Feature importance from Random Forest

### 4. 📉 Hypothesis Testing
- Independent **t-tests** comparing `bsqft`, `br`, and `year` between high- and low-priced homes

---

## 📌 Key Findings

- `bsqft` and `br` showed **strong correlation** and **statistically significant differences** (p < 0.0001)
- `year` also showed a significant but weaker effect
- Models yielded **moderate predictive power** (R² ~ 0.63)
- **Location-based variables** still held influence, suggesting:
  > **Structural features matter most, but location cannot be ignored.**

---

## 📁 Project Structure

├── Hypothesis1test.ipynb # Jupyter notebook with full analysis
├── housing.xlsx # Raw dataset (not included for privacy)
├── README.md # Project documentation
└── assets/ # Images for visualizations (optional)


---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/yourusername/HouseValueX.git
cd HouseValueX

# Install requirements
pip install -r requirements.txt

# Launch the notebook
jupyter notebook Hypothesis1test.ipynb

