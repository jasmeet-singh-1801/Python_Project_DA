# ✈️ Flight Price Data Analysis

This project explores and analyzes flight pricing data to extract meaningful business insights using Python. It demonstrates a complete Data Analysis workflow—from data cleaning to exploratory data analysis (EDA), visualization, and actionable conclusions.

---

## 📌 Project Objectives

- Understand flight pricing trends across different airlines, sources, and routes.
- Clean and prepare real-world, unrefined data for analysis.
- Explore relationships between features (e.g., duration, stops, airline) and price.
- Identify key factors influencing flight prices.

---

## 🛠️ Tools & Libraries Used

- **Pandas** – Data manipulation and wrangling  
- **NumPy** – Numerical operations  
- **Matplotlib & Seaborn** – Data visualization  
- **Jupyter Notebook** – Interactive analysis  

---

## 📂 Project Structure

Flight_DA.ipynb ← Jupyter notebook with full analysis
png ← picture of graphs 
data-unrefined
|
   flight_price.xlsx ← Raw dataset


---

## 🔍 Workflow Overview

### 1. Data Loading
- The dataset is loaded using `pandas.read_excel()`.
- Initial exploration is done using `df.head()`, `df.shape`, and `df.info()`.

### 2. Data Cleaning & Preprocessing
- Missing values are identified and handled using `dropna()` or conditional imputing.
- Feature engineering is performed to:
  - Extract hours and minutes from `Duration`
  - Convert date/time columns to `datetime` format
  - Create derived features like `Total_Stops`, `Source`, `Destination`
- Irrelevant or high-cardinality columns are removed (`Route`, `Additional_Info`).

### 3. Exploratory Data Analysis (EDA)

#### 🧪 Univariate Analysis:
- Count plots for `Airline`, `Source`, `Destination`, and `Total_Stops` give distribution insights.
- Price distribution is visualized using histograms and boxplots.

#### 🔄 Bivariate Analysis:
- Boxplots and scatterplots analyze price variation with:
  - **Airline**
  - **Total Stops**
  - **Journey Date**
  - **Duration**
- Correlation heatmaps highlight key numerical relationships.

### 4. Insights Derived

- **Airline Pricing:** Premium airlines like Jet Airways have higher average prices.
- **Stops:** Flights with more stops tend to cost less.
- **Source/Destination:** Price varies by city pairs — e.g., flights from Delhi to Cochin are common and competitive.
- **Duration Impact:** Longer flights often cost more but may be correlated with stopovers.

---

## 📊 Sample Visualizations

- `sns.boxplot()` and `sns.countplot()` help showcase categorical distributions.
- Correlation matrix (`sns.heatmap()`) aids in identifying linear relationships.
- Trend lines and grouped mean visualizations assist in decision-making.

---

## 📚 Skills Demonstrated

✅ Data Cleaning & Transformation  
✅ Feature Engineering  
✅ EDA & Visualization  
✅ Business Insight Derivation  
✅ Effective Python Notebook Structuring  

---

## 📝 Future Improvements

- Add a predictive model (e.g., Linear Regression or Random Forest) for price forecasting.
- Optimize duration parsing using regex or vectorized functions.
- Automate missing value treatment dynamically.

---

## 📥 Dataset Source

📁 `flight_price.xlsx` — stored locally under:
Flight_Project/data-unrefined/


---

## 🚀 How to Run

1. Clone this repository
2. Open `Flight_DA.ipynb` in Jupyter Notebook or Google Colab
3. Ensure the Excel dataset path is correct
4. Run all cells sequentially to reproduce the full analysis

---

