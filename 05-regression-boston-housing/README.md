# 🏠 House Price Prediction & Analysis (Excel-based)

Welcome!  
In this project, I explored what really drives house prices per unit area — all done **entirely in Excel** using regression analysis and correlation techniques.  
This project shows that powerful data insights don’t always need code: Excel can do it too! 📊✨

---

## 📌 **Project Goal**

To identify which factors significantly impact house prices per unit area, using:

- ✅ Multiple Linear Regression
- ✅ Correlation Matrix Analysis
- ✅ Data interpretation, all built with Excel

---

## 🧩 **Dataset Overview**

| Feature                            | Description                 |
| ---------------------------------- | --------------------------- |
| X1 transaction date                | Numeric date of transaction |
| X2 house age                       | Age of the house in years   |
| X3 distance to nearest MRT station | Distance in meters          |
| X4 number of convenience stores    | Number of shops nearby      |
| X5 latitude                        | Geographic coordinate       |
| X6 longitude                       | Geographic coordinate       |
| Y house price of unit area         | Target variable             |

---

## 📈 **Regression Analysis (Excel Output)**

| Feature             | Coefficient | P-value | Interpretation                     |
| ------------------- | ----------: | ------: | ---------------------------------- |
| Intercept           |   -14441.98 |    0.03 | Baseline price level               |
| X1 transaction date |       +5.15 |   0.001 | Recent transactions → higher price |
| X2 house age        |       -0.27 |      ≈0 | Older houses → cheaper             |
| X3 distance to MRT  |     -0.0045 |      ≈0 | Closer to MRT → higher price       |
| X4 number of stores |       +1.13 |      ≈0 | More stores → higher price         |
| X5 latitude         |     +225.47 |      ≈0 | Further north → higher price       |
| X6 longitude        |      -12.42 |    0.79 | Not significant                    |

✅ **Key takeaway:** MRT distance, house age, number of nearby shops, and latitude matter most. Longitude is not significant.

---

## 📊 **Correlation Matrix Highlights**

| Feature vs. Price   | Correlation |
| ------------------- | ----------: | --------------------------- |
| X3 distance to MRT  |       -0.67 | Strong negative correlation |
| X4 number of stores |       +0.57 | Moderate positive           |
| X5 latitude         |       +0.55 | Moderate positive           |
| X6 longitude        |       +0.52 | Moderate positive           |
| X2 house age        |       -0.21 | Mild negative               |
| X1 transaction date |       +0.09 | Slight positive             |

⚠ **Multicollinearity alert:**

- Strong negative correlation between distance to MRT & longitude (-0.80)
- Moderate correlations among other location features and store counts

---

## ✅ **Summary**

- Houses closer to MRT stations and with more shops cost more.
- Newer houses are more expensive.
- Latitude affects price; longitude doesn’t significantly.
- Some predictors are correlated — important to consider when modeling.

---

## ⚙ **Tools Used**

- Microsoft Excel (Data Analysis ToolPak)
- Excel functions: `CORREL`, `LINEST`
- Built-in regression & descriptive statistics tools

---

## 🚀 **Next Steps**

- Build more visuals
- Try the same analysis in Python / Power BI
- Explore advanced regression (e.g., regularization)

---

## ⭐ **Why this matters**

Data analysis isn't always about complex code.  
Even Excel can reveal actionable insights — making data accessible to everyone.

Feel free to fork this project, give it a ⭐, or share your thoughts!  
Thanks for visiting! 🙌📊
