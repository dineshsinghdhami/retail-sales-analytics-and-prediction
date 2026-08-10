# Retail Sales Analytics & Sales Prediction

## Project Overview

This project presents an end-to-end Retail Sales Analytics and Sales Prediction workflow using the Superstore Sales dataset.

The main objective of the project is to analyze historical retail sales data, identify useful business insights, perform SQL-based business analysis, create meaningful visualizations and dashboards, and build a basic Machine Learning model for Sales prediction.

The project demonstrates the complete data analytics workflow from raw data preparation to predictive modeling.

---

## Project Objectives

The main objectives of this project are to:

* Clean and preprocess retail sales data
* Understand the structure and quality of the dataset
* Perform Exploratory Data Analysis (EDA)
* Identify important business insights
* Create meaningful data visualizations
* Perform SQL-based business analysis
* Build a retail sales dashboard
* Develop a Linear Regression model for Sales prediction
* Evaluate the Machine Learning model
* Present the complete project in a structured GitHub repository

---

## Technologies Used

The following technologies and Python libraries were used:

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQLite
* SQL
* Scikit-learn
* Linear Regression
* Git
* GitHub

---

## Dataset

The project uses a Superstore Sales dataset containing historical retail transaction information.

The dataset includes information such as:

* Order ID
* Order Date
* Ship Date
* Ship Mode
* Customer ID
* Customer Name
* Customer Segment
* Country
* City
* State
* Region
* Product Category
* Product Sub-Category
* Product Name
* Sales

The original dataset is stored as:

`train.csv`

After data cleaning and preprocessing, the cleaned dataset is stored as:

`cleaned_superstore.csv`

---

## Project Structure

```text
Retail_Sales_Project/
│
├── 01_Setup.ipynb
├── 02_Data_Understanding.ipynb
├── 03_Data_Cleaning.ipynb
├── 04_EDA.ipynb
├── 05_SQL_Analysis.ipynb
├── 06_Sales_Prediction.ipynb
├── 07_Sales_Dashboard.ipynb
├── train.csv
├── cleaned_superstore.csv
├── retail_sales.db
├── requirements.txt
└── README.md
```

---

## Project Workflow

### 1. Environment Setup

The required Python libraries were installed and tested inside Jupyter Notebook.

Main libraries:

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

### 2. Data Understanding

The original Superstore Sales dataset was loaded using Pandas.

Initial analysis included:

* Dataset dimensions
* Column names
* Data types
* First records
* Missing values
* Statistical summary

This step helped identify data quality issues that needed to be handled before analysis.

---

### 3. Data Cleaning and Preprocessing

The dataset was cleaned before performing analysis.

The preprocessing process included:

* Handling missing Postal Code values
* Checking and removing duplicate records
* Converting Order Date to datetime format
* Converting Ship Date to datetime format
* Inspecting Sales values
* Creating Order Year
* Creating Order Month
* Creating Order Month Name
* Creating Order Quarter
* Calculating Shipping Days

The cleaned dataset was saved as:

`cleaned_superstore.csv`

---

## Exploratory Data Analysis

Exploratory Data Analysis was performed using Pandas, Matplotlib, and Seaborn.

The analysis included:

* Total Sales
* Total Orders
* Total Customers
* Average Order Value
* Sales by Category
* Sales by Sub-Category
* Sales by Region
* Sales by Customer Segment
* Top 10 Products
* Top 10 Customers
* Yearly Sales Trend
* Monthly Sales Trend
* Shipping Performance

---

## Key Performance Indicators

The project calculates important retail KPIs including:

* Total Sales
* Total Orders
* Total Customers
* Average Order Value

These indicators provide a high-level view of overall business performance.

---

## Key Business Insights

The exploratory analysis revealed several important findings:

* Technology is one of the strongest product categories by total sales.
* The West region generates the highest total sales.
* The Consumer segment contributes the largest amount of sales.
* Sales performance varies significantly across product sub-categories.
* A small group of products generates a large amount of revenue.
* Some customers contribute significantly more revenue than others.
* Sales performance changes across years and months.
* Monthly Sales show noticeable fluctuations over time.
* Shipping duration differs depending on the selected Ship Mode.

These insights can support decisions related to marketing, inventory management, customer retention, regional strategy, and sales planning.

---

## SQL Business Analysis

SQLite was used to create a database directly from the cleaned Superstore dataset.

Database:

`retail_sales.db`

Table:

`sales`

SQL concepts used in this project include:

* SELECT
* FROM
* WHERE
* GROUP BY
* ORDER BY
* LIMIT
* DISTINCT
* SUM()
* COUNT()
* AVG()
* MAX()
* ROUND()

SQL queries were used to answer business questions such as:

* What is the total Sales revenue?
* How many unique Orders are present?
* How many unique Customers are present?
* Which Category generates the highest Sales?
* Which Region generates the highest Sales?
* Which Customer Segment contributes the most Sales?
* Which Sub-Categories generate the highest Sales?
* What are the Top 10 Products?
* Who are the Top 10 Customers?
* How do Sales change by Year?
* Which Months generate the most Sales?
* Which Region receives the highest number of Orders?
* What is the average Sales value by Category?
* How does Shipping Time differ between Ship Modes?

---

## Sales Dashboard

A dashboard-style analytics notebook was created using Python, Matplotlib, and Seaborn.

The dashboard includes:

* Total Sales
* Total Orders
* Total Customers
* Average Order Value
* Sales by Category
* Sales by Region
* Sales by Customer Segment
* Monthly Sales Trend
* Top 10 Products
* Top 10 Customers

The dashboard provides a summarized visual view of overall retail business performance.

---

## Machine Learning

A basic Machine Learning model was developed using Linear Regression.

### Target Variable

`Sales`

### Input Features

The model uses features including:

* Order Year
* Order Month
* Order Quarter
* Shipping Days
* Category
* Region
* Segment
* Ship Mode

Categorical variables were converted into numerical format using One-Hot Encoding.

---

## Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

The training dataset was used to train the Linear Regression model.

The testing dataset was used to evaluate the model on unseen records.

---

## Model Evaluation

The Linear Regression model was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score
* Actual vs Predicted Sales visualization
* Prediction Error analysis

The model serves as a basic baseline Sales prediction model.

Retail Sales can depend on additional factors that are not available in this dataset, such as:

* Product Price
* Quantity
* Discount
* Promotions
* Holidays
* Economic Conditions
* Customer Purchasing Behavior

Therefore, additional features and more advanced Machine Learning models could potentially improve prediction performance.

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Open the project folder

```bash
cd Retail_Sales_Project
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the notebooks in order

```text
01_Setup.ipynb
02_Data_Understanding.ipynb
03_Data_Cleaning.ipynb
04_EDA.ipynb
05_SQL_Analysis.ipynb
06_Sales_Prediction.ipynb
07_Sales_Dashboard.ipynb
```

---

## Future Improvements

The project can be improved further by:

* Adding Power BI visualizations
* Adding more interactive dashboard filters
* Performing advanced feature engineering
* Testing additional Machine Learning algorithms
* Comparing multiple prediction models
* Adding Profit, Quantity, and Discount features if available
* Performing time-series forecasting
* Deploying the dashboard as a web application

---

## Conclusion

This project demonstrates a complete beginner-level Data Analytics and Machine Learning workflow using a real-world retail dataset.

The project covers:

* Data preparation
* Data cleaning
* Exploratory Data Analysis
* Data visualization
* Business insight generation
* SQL analysis
* Dashboard development
* Machine Learning
* Sales prediction
* Model evaluation

The project shows how Python, SQL, visualization tools, and basic Machine Learning can be combined to solve practical retail business problems.
