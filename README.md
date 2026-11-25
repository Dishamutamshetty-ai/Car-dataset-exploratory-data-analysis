# 🚗 Exploratory Data Analysis on a Cars Dataset

## 📌 Project Overview

This project focuses on Exploratory Data Analysis (EDA) of a cars dataset using Python. The goal is to understand the dataset, identify missing and duplicate values, explore data distributions, analyze relationships between variables, and visualize important patterns.

This is my first Data Science project, completed as part of my AIML Minor Project 1.

## 🎯 Project Objectives

- Understand the structure and characteristics of the cars dataset.
- Identify and handle missing values and duplicate records.
- Perform data cleaning and preprocessing.
- Analyze the distribution of car selling prices.
- Explore relationships between kilometres driven and selling price.
- Visualize correlations and inspect outliers.
- Extract meaningful observations from the dataset.

## 📂 Dataset Information

**Dataset:** `Car_details.csv`

- Original dataset size: 8,128 rows and 13 columns.
- Contains information about car prices, manufacturing year, fuel type, transmission, mileage, engine, power, and other features.
- The original dataset publisher and public source URL were not identified in the supplied project materials.

## 🛠️ Technologies Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Label encoding
- Jupyter Notebook – Development environment

## 🔍 Project Workflow

### 1. Data Understanding
- Imported the dataset using Pandas.
- Explored the first and last records.
- Examined dataset information, shape, and columns.
- Checked missing values and duplicate records.

### 2. Data Cleaning
- Identified missing values.
- Filled missing categorical values using the mode.
- Filled missing numerical values using the median.
- Removed duplicate records.
- Dropped the `name` and `owner` columns.
- Applied Label Encoding to remaining categorical columns.

After removing 1,202 duplicate rows, the dataset contained 6,926 records.

### 3. Exploratory Data Analysis

Performed:
- Univariate analysis
- Bivariate analysis
- Multivariate analysis
- Correlation analysis
- Outlier inspection and treatment

### 4. Data Visualization

The project includes visualizations such as:

- Distribution of Selling Price – Histogram
- Kilometres Driven vs Selling Price – Scatter Plot
- Correlation Heatmap
- Outlier Inspection – Box Plot
- Outlier Inspection After Treatment – Box Plot
- Number of Cars by Fuel Type – Bar Chart

### 5. Outlier Treatment

Used the Interquartile Range (IQR) method to identify outliers. Values outside the calculated IQR boundaries were replaced with the median of their respective columns.

## 📊 Key Findings

- The dataset originally contained 8,128 records.
- A total of 1,202 duplicate records were identified and removed.
- Diesel cars accounted for 54.2% of the records.
- Petrol cars accounted for 44.7% of the records.
- Manual transmission cars represented 87.1% of the dataset.
- Individual sellers formed the largest seller category, with 6,766 records.
- The mean selling price was approximately 638,272, while the median was 450,000.
- The selling price distribution showed a long upper tail.

## ⚠️ Limitations

- The original dataset publisher was not specified.
- Some measurement columns, including mileage, engine, max_power, and torque, were stored as text.
- Label encoding these fields can produce misleading correlations.
- Outlier treatment was applied to encoded categorical columns as well as numerical columns.
- The `name` and `owner` columns were removed, limiting further analysis of car models and ownership.

These limitations are important when interpreting the results.

## ▶️ How to Run This Project

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. Open the Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `EDA_Minor_Project1.ipynb`.
6. Make sure `Car_details.csv` is in the same folder as the notebook.
7. Update the dataset loading path in the notebook to:

```python
df = pd.read_csv("Car_details.csv")
```

8. Run the notebook cells sequentially.

## 📁 Project Structure

```text
Car-dataset-exploratory-data-analysis/
│
├── Car_details.csv
├── EDA_Minor_Project1.ipynb
├── EDA_Minor_ProjectReport1.pdf
└── README.md
```

## 📄 Project Report

The detailed project report is available in:

`EDA_Minor_ProjectReport1.pdf`

## 🌱 Learning Outcomes

Through this project, I gained practical experience in:

- Working with datasets using Pandas and NumPy.
- Handling missing and duplicate values.
- Performing exploratory data analysis.
- Creating data visualizations.
- Understanding distributions, correlations, and outliers.
- Communicating data insights and recognizing analytical limitations.

## 🚀 Future Improvements

- Extract numerical values from measurement columns.
- Improve categorical data preprocessing.
- Perform deeper analysis of car prices based on year, fuel type, and transmission.
- Investigate outliers more carefully.
- Explore additional patterns in the dataset.

---

**This is my first Data Science project, and I'm excited to continue learning and building more projects in Python, Data Analytics, and Machine Learning.** 🌱
