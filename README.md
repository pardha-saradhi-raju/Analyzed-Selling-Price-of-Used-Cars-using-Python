# Analyzing Selling Price of Used Cars using Python

## Overview
This project focuses on analyzing and predicting the selling price of used cars based on various features using Python. The dataset consists of multiple variables such as car make, fuel type, engine size, drive wheels, and more. The project involves data cleaning, preprocessing, visualization, and the application of several analytical techniques to explore key factors influencing car prices.

## Dataset
The dataset used in this project contains information about various car features such as:
- Symboling
- Normalized losses
- Make
- Fuel type
- Body style
- Engine size
- Horsepower
- Price (target variable)

The dataset is publicly available and consists of 200 rows and 26 columns.

## Key Features of the Project

### 1. **Data Preprocessing**
   - **Handling Missing Values**: Replaced missing values and dropped rows with non-numeric entries.
   - **Renaming Columns**: Assigned descriptive names to the dataset columns for better understanding.
   - **Unit Conversion**: Converted fuel consumption from miles per gallon (mpg) to liters per 100 kilometers (L/100km) for a more intuitive representation.

### 2. **Data Visualization**
   - **Histograms**: Used to visualize the distribution of car prices and categorized price ranges (Low, Medium, High).
   - **Box Plots**: Displayed the relationship between car features (like drive wheels and body style) and price.
   - **Scatter Plots**: Visualized the correlation between engine size and price, showing the positive relationship between these two variables.
   - **Heatmaps**: Applied to show the relationship between drive wheels, body style, and price, providing insights into how different combinations affect the average car price.

### 3. **Data Transformation**
   - **Binning**: Grouped continuous price values into three categories — Low, Medium, and High.
   - **Dummy Variables**: Converted categorical variables (like fuel type) into numerical values using pandas’ `get_dummies()` function to facilitate machine learning and analysis.

### 4. **Descriptive Analysis**
   - Used the `describe()` function to calculate summary statistics (mean, standard deviation, etc.) for each feature. It provided an overview of the dataset's structure and helped to identify outliers and trends.

### 5. **Predictive Analysis**
   - **Correlation and Regression**: Applied regression analysis to predict car prices based on engine size and other factors. Scatter plots were used to visualize this relationship.
   - **ANOVA (Analysis of Variance)**: Conducted an ANOVA test to compare the average prices of different car makes (e.g., Honda vs. Subaru) and determine if there are statistically significant differences between them.

## Project Structure
- **data/**: Contains the dataset used for the analysis (`imports-85.data.csv`).
- **notebooks/**: Jupyter notebooks containing the code and step-by-step analysis.
- **src/**: Source code including functions for data preprocessing, visualization, and analysis.
- **README.md**: Project documentation.

## Installation and Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/pardha-saradhi-raju/used-car-price-analysis.git
   ```

2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib seaborn scipy
   ```

3. Run the Jupyter notebook or Python script to execute the project.

## Dependencies
- Python 3.x
- Numpy
- Pandas
- Matplotlib
- Seaborn
- Scipy

## How to Use

1. Load the dataset by running the provided Python script or Jupyter notebook.
2. Preprocess the data to handle missing values, convert units, and create dummy variables.
3. Run the analysis and visualizations to explore trends and predict prices.
4. Interpret the visualizations and statistical results to gain insights about the dataset.

## Key Visualizations
- **Histograms**: Show the distribution of car prices across the dataset.
- **Box Plots**: Illustrate the spread and outliers for car prices based on categorical features.
- **Heatmaps**: Provide a color-coded matrix showing the relationship between different categorical variables and price.

## Results
- Engine size is positively correlated with price, meaning larger engines tend to have higher prices.
- Rear-wheel drive (RWD) cars, especially convertibles, tend to have the highest average prices.
- ANOVA results show that there is no statistically significant difference between prices of Honda and Subaru cars (p > 0.05).

## Conclusion
This project provides an in-depth exploration of the factors affecting used car prices and demonstrates how various Python libraries (such as Pandas, Matplotlib, Seaborn) can be used for data analysis and visualization. It highlights the relationship between price and other features like engine size and drive wheels, helping to predict used car prices more accurately.

## Future Work
- Implement advanced machine learning algorithms like Linear Regression and Random Forest to improve price predictions.
- Expand the dataset to include more car makes and features.
- Explore time-series data to predict price changes over time.

