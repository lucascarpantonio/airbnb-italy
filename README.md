#  Airbnb Market Analysis in Venice, Italy
### by Luca Scarpantonio

---

##  Project Overview

This project explores how the **Airbnb market in Venice** has evolved over the past decade, focusing on changes in **supply, pricing, and host behavior**.  
The analysis follows the **CRISP-DM process** — from data gathering and cleaning to modeling and visualization — and aims to answer a set of real-world business questions relevant to the tourism economy of Venice.

The notebook was developed as part of the **Udacity Introduction to Data Science Nanodegree**.

---

## Project Objectives

The analysis investigates key questions about Airbnb’s role in Venice:

1. **How has the number of Airbnb listings evolved in recent years?**  
   → Understanding the growth trend of Airbnb activity in Venice.

2. **How have supply and demand affected listing prices over time?**  
   → Exploring the relationship between market expansion and average nightly rates.

3. **How has the number of active hosts evolved compared to listings?**  
   → Identifying whether growth comes from new hosts or increased host activity.

4. **Do price patterns vary across Venice’s geographical areas?**  
   → Analyzing spatial segmentation (mainland vs. central Venice vs. islands).

5. **Can we predict listing prices based on room type and location?**  
   → Building a simple regression model to identify the most relevant price factors.

---

## Dataset

- **Source:** [Inside Airbnb](http://insideairbnb.com/get-the-data.html)  
- **City:** Venice, Italy  
- **Files Used:** `listings.csv`, `neighbourhoods.csv`  
- **Temporal coverage:** 2015–2025  
- **Observation:**  
  Dates are based on *review timestamps*, assuming that review activity correlates with the period when the property was actively listed.

### Data Wrangling Steps
1. Removed duplicate and inconsistent records.  
2. Converted prices from string (`€/$`) to numeric format.  
3. Filtered unrealistic prices (`price < 1000`).  
4. Removed missing or non-informative values (`Not Available`, `NaN`).  
5. Extracted temporal features from `last_review` (year, month).  
6. Aggregated average price and listings per month/year.

---

## 🔍 Methodology — CRISP-DM Process

| Phase | Description |
|-------|--------------|
| **1. Business Understanding** | Framed analytical questions around market growth, price evolution, and host behavior. |
| **2. Data Understanding** | Loaded and inspected Airbnb Venice listings; assessed missing data and outliers. |
| **3. Data Preparation** | Cleaned and transformed data, derived temporal and spatial features. |
| **4. Modeling** | Built a linear regression model to predict prices based on location and room type. |
| **5. Evaluation** | Interpreted model coefficients and evaluated fit (R²). |
| **6. Deployment** | Communicated insights via visualizations and this notebook. |

---

##  Key Findings

###🏙️ 1. Rapid Market Expansion
- The number of active listings grew exponentially after 2016.  
- Despite the pandemic slowdown in 2020, Airbnb’s presence recovered quickly, reaching record highs by 2025.

### 2. Price Stability Despite Supply Growth
- Average nightly prices remained stable between €160–€200 even as listings increased.  
- This indicates a **mature and competitive market**, suggesting accessibility for travelers.

### 3. Persistent Spatial Segmentation
- Central Venice (San Marco, Dorsoduro, Cannaregio) maintains premium prices.  
- Mainland and island areas (Marghera, Lido, Giudecca) are significantly cheaper.

### 👥 4. Host Dynamics
- The number of active hosts also increased, but **the average number of listings per host rose faster**, suggesting professionalization among hosts.

###  5. Predictive Insights
- Linear regression identified **room type** and **location** as the strongest predictors of price.  
- The model confirmed the price gap between central and peripheral areas.

---

##  Visual Highlights

| Visualization | Insight |
|----------------|----------|
| Line plot of listings per year | Airbnb expansion over time |
| Scatter plot (Listings vs. Price) | Relationship between market growth and affordability |
| FacetGrid by area | Spatial variation of prices |
| Regression model output | Price prediction by room type and neighbourhood |

---

##  Conclusion

The Airbnb market in Venice evolved from an emerging platform to a mature, balanced ecosystem.  
While central districts remain premium, the rise of listings in peripheral areas has **democratized access to the city**, making Venice more affordable for short-term visitors.

> **In essence:**  
> Airbnb reshaped tourism in Venice, balancing exclusivity and accessibility — preserving the charm of the lagoon city while opening it to a wider audience.

---

##  Tools and Libraries

- **Python 3.11**
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `jupyter`, `nbconvert`

---

---

##  Author & Acknowledgments

**Author:** Luca Scarpantonio  
**Nanodegree:** Udacity — Introduction to Data Science  
**Dataset source:** [Inside Airbnb](http://insideairbnb.com)  
**Inspiration:** Airbnb market studies in European cities

---

## 📰 For Further Reading

This analysis is also available as a Medium-style article:  
> *“How Airbnb Transformed Venice: A Data-Driven View on Tourism and Accessibility”*

---

##  Key Takeaway for Portfolio Reviewers

> This project demonstrates a complete **end-to-end data science process**: from data cleaning and visualization to modeling and business storytelling — all focused on a real-world dataset that reflects both technical and analytical expertise.