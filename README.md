# 🏡 Airbnb Market Analysis — Italy
### by Luca Scarpantonio

---

## 📘 Project Overview

This project explores **Airbnb listings data** for an Italian city using the **CRISP-DM** framework.  
The goal is to understand **what drives listing prices** and how host attributes, location, and reputation influence market trends.

The analysis follows a typical **data science workflow**:
1. **Data Collection** — from [Inside Airbnb](http://insideairbnb.com/get-the-data.html)
2. **Data Assessment** — identifying missing values, inconsistencies, and outliers
3. **Data Cleaning** — removing duplicates, converting data types, and filtering out unrealistic prices
4. **Exploratory Data Analysis (EDA)** — discovering relationships through statistical summaries and visualization
5. **(Optional) Predictive Modeling** — using linear regression to explore relationships between features and price
6. **Visualization and Insights** — summarizing key takeaways with clean, insightful plots

---

## 🎯 Business Questions

1. What is the **distribution of prices** across different room types?  
2. How do **prices vary by neighbourhood**?  
3. Is there a **relationship between price and number of reviews**?  
4. Do **ratings impact listing prices**?  
5. Which **factors best predict listing price**?

---

## 📊 Key Insights

- **Entire apartments** are priced higher than private or shared rooms.  
- There is **considerable variation** in prices across neighbourhoods.  
- Listings with **higher review scores** tend to command higher prices.  
- Some records contain **inconsistent data** (e.g., missing values, unrealistic prices) — these were filtered for clarity.  
- The correlation between number of reviews and price is **weak**, suggesting reviews influence reputation more than pricing.

---

## 💻 Tech Stack

- **Python** — Data Analysis and Visualization  
- **Pandas / NumPy** — Data Wrangling and Aggregation  
- **Seaborn / Matplotlib** — Data Visualization  
- **Scikit-learn** — Linear Regression (Optional)  
- **Jupyter Notebook** — Interactive Analysis Environment

---

## 🧠 CRISP-DM Framework Applied

| Phase | Description |
|-------|--------------|
| **Business Understanding** | Define the main objectives: understanding Airbnb pricing dynamics |
| **Data Understanding** | Load and explore the dataset (structure, types, missing values) |
| **Data Preparation** | Clean and preprocess the data for reliable analysis |
| **Modeling** | Apply regression to estimate relationships between features and price |
| **Evaluation** | Interpret metrics and validate insights |
| **Deployment** | Present results through notebook visualizations and GitHub documentation |

---

## 📂 Repository Structure

```
Airbnb-Market-Analysis/
│
├── Airbnb_Analysis_Italy.ipynb     # Main Jupyter Notebook
├── README.md                       # Project documentation
├── /data                           # (Optional) raw Airbnb dataset
├── /images                         # Exported plots for presentation
└── requirements.txt                # Python dependencies
```

---

## 🔗 Data Source

- **Inside Airbnb**: [http://insideairbnb.com/get-the-data.html](http://insideairbnb.com/get-the-data.html)  
- Public dataset for educational and non-commercial analysis.  

---

## 📈 Example Visualizations

| Plot Type | Description |
|------------|--------------|
| **Boxplot** | Distribution of price by room type |
| **Heatmap** | Correlation between price, reviews, and ratings |
| **Bar Chart** | Price variation across neighbourhoods |
| **Scatter Plot** | Price vs. number of reviews |
| **Linear Regression Line** | Model relationship between rating and price |

---

## 🧩 Author

**Luca Scarpantonio**  
*Data Analyst | Quality Assurance Specialist | Data Science Enthusiast*  
📧 [Contact on GitHub](https://github.com/scarpl)

---

## 🏁 Acknowledgements

This project was developed as part of the **Introduction to Data Science Nanodegree** (Udacity).  
All datasets are property of [Inside Airbnb](http://insideairbnb.com/get-the-data.html).
