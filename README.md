!(https://github.com/hijirdella/House-Price-Analysis-EDA-and-Correlation-Insights/blob/d8fe50341ccb3ec7c76d2fc7a380a5eac3c971f9/EDA%20House%20Prices.jpg)


---

# Exploratory Data Analysis (EDA) for House Prices

This repository contains a comprehensive exploratory data analysis (EDA) of house price data. The project focuses on uncovering trends, correlations, and statistical insights that provide valuable business and data-driven insights for the housing market.

---

## **Table of Contents**
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features and Variables](#features-and-variables)
- [Analysis Performed](#analysis-performed)
- [Key Insights](#key-insights)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Contact](#contact)

---

## **Project Overview**
This project explores the factors affecting house prices using Python. The analysis includes:
- Data Profiling
- Data Preprocessing
- Univariate and Multivariate Analysis
- Statistical Analysis:
  - Pearson Correlation
  - Chi-Square Test
  - Linear Regression
  - T-Test
  - ANOVA

By analyzing these, the project uncovers patterns and trends in the housing market between 2006 and 2010, helping stakeholders understand market behavior.

---

## **Dataset**
The dataset is sourced from Kaggle's **House Prices - Advanced Regression Techniques** competition:
- [House Prices Dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

---

## **Features and Variables**
The dataset contains 81 columns, including:
- **Numerical Features:** SalePrice, LotArea, GrLivArea, GarageArea, etc.
- **Categorical Features:** MSZoning, Neighborhood, SaleCondition, etc.
- **Target Variable:** `SalePrice` (House Price)

Key variables like `OverallQual`, `GrLivArea`, and `Neighborhood` show strong relationships with house prices.

---

## **Analysis Performed**
### 1. **Data Profiling**
   - Handling missing values.
   - Identifying and removing duplicates.
   - Statistical summaries of the dataset.

### 2. **Univariate Analysis**
   - Histogram and boxplot visualizations for numerical columns.
   - Countplots for categorical columns.

### 3. **Multivariate Analysis**
   - Heatmap for correlation among numerical variables.
   - Boxplots for relationships between categorical features and `SalePrice`.

### 4. **Statistical Tests**
   - **Pearson Correlation:** Relationship between `YrSold` and `SalePrice`.
   - **Chi-Square Test:** Distribution differences in `SalePrice` categories over the years.
   - **Linear Regression:** Trend analysis for `YrSold` and `SalePrice`.
   - **T-Test:** Comparing mean house prices between different years.
   - **ANOVA:** Testing variance in house prices across years.

## Hasil Pengujian Statistik

| **Pengujian yang Digunakan**   | **Uji Pearson**                                                                                       |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
| **Tujuan**                     | Menguji hubungan signifikan antara tahun penjualan dan harga rumah                                     |
| **Statistik Uji**              | Pearson Correlation: -0.0289                                                                          |
| **P-Value**                    | 0.2694                                                                                               |
| **Kesimpulan**                 | Gagal menolak Hipotesis Nol (H0)                                                                      |
| **Interpretasi**               | Tidak ada hubungan signifikan antara tahun penjualan dan harga rumah                                  |

---

| **Pengujian yang Digunakan**   | **Uji Chi-Square**                                                                                    |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
| **Tujuan**                     | Menguji perbedaan signifikan dalam distribusi harga rumah                                              |
| **Statistik Uji**              | Chi2 Statistic: 8.6713                                                                                |
| **P-Value**                    | 0.7307                                                                                               |
| **Kesimpulan**                 | Gagal menolak Hipotesis Nol (H0)                                                                      |
| **Interpretasi**               | Tidak ada perbedaan signifikan dalam distribusi harga rumah dari tahun 2006-2010                      |

---

| **Pengujian yang Digunakan**   | **Uji T-Test**                                                                                        |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
| **Tujuan**                     | Menguji perbedaan signifikan dalam rata-rata harga rumah                                               |
| **Statistik Uji**              | T-Statistic: 0.4950                                                                                  |
| **P-Value**                    | 0.5344                                                                                               |
| **Kesimpulan**                 | Gagal menolak Hipotesis Nol (H0)                                                                      |
| **Interpretasi**               | Tidak ada perbedaan signifikan dalam rata-rata harga rumah dari tahun 2006-2010                      |

---

| **Pengujian yang Digunakan**   | **Uji ANOVA**                                                                                         |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
| **Tujuan**                     | Menguji perbedaan signifikan dalam rata-rata harga rumah                                               |
| **Statistik Uji**              | F-Statistic: 0.6455                                                                                  |
| **P-Value**                    | 0.6301                                                                                               |
| **Kesimpulan**                 | Gagal menolak Hipotesis Nol (H0)                                                                      |
| **Interpretasi**               | Tidak ada perbedaan signifikan dalam rata-rata harga rumah dari tahun 2006-2010                      |

---

| **Pengujian yang Digunakan**   | **Regresi Linear**                                                                                   |
|--------------------------------|--------------------------------------------------------------------------------------------------------|
| **Tujuan**                     | Menguji hubungan linear antara tahun penjualan (YrSold) dan harga rumah (SalePrice)                   |
| **Statistik Uji**              | R-squared: 0.001, F-statistic: 1.221                                                                 |
| **P-Value**                    | 0.2690                                                                                               |
| **Kesimpulan**                 | Gagal menolak Hipotesis Nol (H0)                                                                      |
| **Interpretasi**               | Tidak ada perbedaan signifikan antara harga rumah pada tahun 2006-2010. Kenaikan harga rumah tidak signifikan. |


---

## **Key Insights**
1. **Features Affecting House Prices:**
   - `OverallQual`, `GrLivArea`, and `GarageCars` have the strongest correlations with `SalePrice`.
   - Neighborhood significantly influences house prices.

2. **Trends Over Time:**
   - House prices between 2006 and 2010 show minimal significant variation, indicating a stable market.

3. **Outliers:**
   - Features like `LotArea` and `GrLivArea` have significant outliers that correspond to premium properties.

4. **Seasonality:**
   - Sales peak during summer months (May–July), while winter months (November–February) have lower activity.

---

## **Technologies Used**
- **Python Libraries:**
  - `pandas` - Data manipulation and cleaning.
  - `numpy` - Numerical analysis.
  - `matplotlib` & `seaborn` - Data visualization.
  - `statsmodels` & `scipy` - Statistical tests and modeling.

---

## **How to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/hijirdella/House-Price-Analysis-EDA-and-Correlation-Insights.git
  
   ```
2. Run the Jupyter Notebook:
   ```bash
   jupyter notebook EDA_House_Prices.ipynb
   ```

---

For further inquiries, please contact **Hijir Della Wirasti** via:
- **Email**: [hijirdw@gmail.com](hijirdw@gmail.com)
- **GitHub**: [https://github.com/hijirdella](https://github.com/hijirdella)
- **LinkedIn**: [https://www.linkedin.com/in/hijirdella/](https://www.linkedin.com/in/hijirdella/)


Let me know if you'd like to refine this further or add more details!
