# Exploring the Iris Dataset

This project performs an Exploratory Data Analysis (EDA) on the famous Iris dataset using Python libraries such as Pandas, Seaborn, and Matplotlib.

## Dataset Overview

The Iris dataset contains measurements of 150 iris flowers from three species: Setosa, Versicolor, and Virginica. Each sample includes four features:
- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)
- Species (categorical)

The dataset is stored in `dataset/Iris.csv`.

## Analysis Steps

### 1. Data Loading
- Load the dataset using Pandas' `read_csv` function.
- Display the first five rows with `df.head()`.

### 2. Data Structure
- Check the shape: 150 rows and 6 columns (including Id).
- Use `df.info()` to verify data types: Species is object (string), others are numeric.

### 3. Descriptive Statistics
- Use `df.describe()` to get summary statistics: count, mean, std, min, percentiles, max.

### 4. Missing Values
- Check for null values with `df.isnull().sum()`: No missing values found.

### 5. Duplicate Values
- Remove duplicates based on Species: Results in 3 unique species.
- Count occurrences: Each species has 50 samples.
- Visualize species distribution with a count plot.

### 6. Relationships and Scatter Plots
- Scatter plot of Sepal Length vs. Sepal Width, colored by Species.
- Scatter plot of Petal Length vs. Petal Width, colored by Species.

### 7. Pair Plot
- Use Seaborn's pairplot to visualize relationships between all numeric variables, hue by Species.

### 8. Histograms
- Plot histograms for Sepal Length, Sepal Width, Petal Length, and Petal Width to show distributions.

### 9. Correlation Analysis
- Compute Pearson correlation for numeric columns.
- Visualize with a heatmap.

### 10. Box Plots
- Box plots for each feature by Species to show distributions and outliers.

### 11. Outlier Handling
- Identify outliers in Sepal Width using IQR method.
- Remove outliers and verify with box plot.

## Key Findings
- The dataset is clean with no missing values.
- Species are evenly distributed (50 each).
- Petal measurements show clear separation between species, especially Virginica.
- Strong correlations between petal length/width and species.
- Some outliers in Sepal Width were removed.

## Requirements
- Python 3.x
- Pandas
- Seaborn
- Matplotlib
- NumPy

Install dependencies:
```
pip install pandas seaborn matplotlib numpy
```

## How to Run
1. Ensure the dataset is in `dataset/Iris.csv`.
2. Open `analysis_notebook.ipynb` in Jupyter Notebook or VS Code.
3. Run cells sequentially to reproduce the analysis.

## License
This project is for educational purposes.

## Solution 
https://roadmap.sh/projects/exploring-iris-dataset