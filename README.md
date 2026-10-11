# Diabetes Data Cleaning and Exploratory Data Analysis

## Project Overview

This project focuses on cleaning, analysing and visualising a diabetes dataset using Python. It demonstrates data preprocessing, handling invalid values, outlier treatment, feature engineering and exploratory data analysis.

The project also includes visualisations to explore patterns in the data and a dataset prepared for use in Tableau.

## Project Objectives

- Explore the structure and statistical summary of the dataset.
- Identify missing values, invalid zero values and duplicate records.
- Clean the data using appropriate preprocessing techniques.
- Detect and treat outliers using the Interquartile Range (IQR) method.
- Create a new feature called `DiabetesRiskScore`.
- Visualise data distributions, relationships and correlations.
- Prepare data for further exploration through Tableau.

## Data Cleaning and Analysis

The following steps were carried out in the Jupyter Notebook:

**1. Data Exploration**

Inspected the dataset using methods such as `head()`, `info()` and `describe()` to understand its structure, data types and statistical summaries.

**2. Data Cleaning**

Checked for missing values and duplicate records. Identified zero values in Glucose, BloodPressure, SkinThickness, Insulin and BMI that could represent missing measurements, then replaced them with the median of the corresponding column.

**3. Outlier Treatment**

Used the Interquartile Range (IQR) method to identify and handle outliers by applying lower and upper limits to numerical columns.

**4. Feature Engineering**

Created a new feature called `DiabetesRiskScore` using the following formula:

`DiabetesRiskScore = (0.5 × Glucose) + (0.3 × BMI) + (0.2 × Age)`

This is a simple, project-defined score used for exploratory analysis.

**5. Data Visualisation**

Created visualisations to understand the dataset, including:

- Histograms showing the distributions of Glucose, BMI and DiabetesRiskScore.
- A bar chart showing the distribution of diabetes outcomes.
- A correlation heatmap to examine relationships between numerical variables.
- Boxplots comparing Glucose and BMI across diabetes outcome groups.

## Tools and Technologies

- **Python** – Data processing and analysis
- **pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualisation
- **Seaborn** – Statistical visualisation
- **Jupyter Notebook** – Writing and running Python code
- **Tableau** – Dashboard visualisation

## Repository Contents

- `Diabetes Dataset.csv` – Original dataset used for the analysis.
- `Practical 1.ipynb` – Jupyter Notebook containing the Python code for data cleaning, analysis and visualisation.
- `Diabetes_Tableau_Final.csv` – Dataset prepared for use in Tableau.

## How to Run the Project

1. Download or clone this repository.
2. Ensure Python and Jupyter Notebook are installed.
3. Install the required libraries:

   `pip install pandas numpy matplotlib seaborn`

4. Open `Practical 1.ipynb` in Jupyter Notebook, JupyterLab or a compatible notebook environment.
5. Ensure the required CSV files are available in the working directory.
6. Run the notebook cells in order to follow the data cleaning and analysis process.

## Important Note

The `DiabetesRiskScore` is a simple feature created for this academic project. It is not a validated clinical score and should not be used to diagnose diabetes or make medical decisions.
