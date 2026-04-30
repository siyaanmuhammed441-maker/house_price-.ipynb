# house_price-.ipynb
# 🏠 Bangalore House Price Analysis

This project focuses on **Exploratory Data Analysis (EDA)** and **Outlier Detection** on a Bangalore house price dataset, specifically analyzing the **price per square foot** feature.

---

## 📂 Dataset
- File: `house_price.csv`
- Description: Contains housing data such as price, area, and other features for properties in Bangalore.

---

## ⚙️ Libraries Used
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scipy  

---

## 🔍 Q1: Basic EDA
Performed initial analysis to understand:
- Dataset shape and structure  
- Column names and data types  
- Summary statistics  
- Missing values  

---

## 🚨 Q2: Outlier Detection & Removal

Applied multiple techniques to detect and remove outliers in `price_per_sqft`:

### 🅰️ Mean & Standard Deviation
- Used ±3 standard deviations from the mean  
- Removed extreme values  

### 🅱️ Percentile Method
- Considered 5th and 95th percentiles  
- Trimmed extreme lower and upper values  

### 🅲 IQR Method (Best)
- Used Interquartile Range (IQR)  
- Removed values outside:
  - Q1 − 1.5×IQR  
  - Q3 + 1.5×IQR  

### 🅳 Z-Score Method
- Removed values with Z-score > 3  

---

## 📦 Q3: Box Plot Analysis
- Visualized outliers before and after removal  
- Compared effectiveness of methods  
- **Conclusion:** IQR method performed best for this dataset  

---

## 📊 Q4: Normality Check
- Plotted histogram of `price_per_sqft`  
- Calculated skewness and kurtosis  

### 🔄 Transformation
- Applied **log transformation**  
- Reduced skewness  
- Improved normal distribution  

---

## 🔥 Q5: Correlation Analysis
- Computed correlation between numerical features  
- Visualized using a heatmap  
- Identified relationships between variables  

---

## 📈 Q6: Scatter Plot
- Plotted `total_sqft` vs `price`  
- Observed positive correlation between area and price  

---

## ✅ Final Conclusion
- IQR is the most effective method for outlier removal  
- Log transformation improves data normality  
- Strong relationship exists between area and price  
- Visualizations help better understand patterns in data  

---

## 🚀 How to Run

```bash
pip install pandas numpy matplotlib seaborn scipy
