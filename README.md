# Data Mining: Iris Data Exploration

This repository contains the solution for Project 1 of a Data Mining course. The primary objective of this project is to perform comprehensive Exploratory Data Analysis (EDA) on the classic Iris Dataset. The project covers univariate and bivariate statistical analysis, correlation analysis, and extensive data visualization to understand the characteristics and relationships within the data.

## Dataset
The analysis is performed on the Iris Dataset, originally introduced by Ronald Fisher in 1936.
+ Source: UCI Machine Learning Repository
+ Instances: 150
+ Features: 4 (Sepal Length, Sepal Width, Petal Length, Petal Width)
+ Classes: 3 (Iris Setosa, Iris Versicolor, Iris Virginica)

## Features

This project implements the following data mining tasks:
1. Univariate Summary Statistics(dist/statistics.csv): Calculates detailed statistics for sepal width grouped by species:
	+ Missing values, Min, Max, Mean
	+ Quartiles (Q1, Median, Q3), 95th Percentile
	+ Range, IQR, Standard Deviation (Sample & Population), MAD
2. Correlation Analysis(dist/correlation.csv): Computes Pearson's correlation matrix for all numerical features and identifies minimum/maximum correlations.
	+ A 4x4 matrix showing Pearson correlation coefficients between:Sepal Length, Sepal Width, Petal Length, Petal Width
3. Data Visualization:
	+ Histograms: Distribution of Petal Length and Sepal Width.
	+ 3D Histogram: Joint distribution of Petal Length and Sepal Width.
	+ Box Plots: Distribution of features per species to identify outliers.
	+ Scatter Plots: Pairwise relationships between all features, colored by species.
	+ 3D Scatter Plot: Separability analysis using Sepal Length, Sepal Width, and Petal Length.
	+ PDF Curves: Probability Density Function estimation for Petal Length per species.

## Project Structure
```
.
├── src/
│   └── run.ipynb          # Main Jupyter Notebook containing the analysis code
├── dist/
│   ├── statistics.csv     # Generated univariate statistics
│   └── correlation.csv    # Generated correlation matrix
├── data/                  # Directory for dataset storage 
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
```

## References
1. Fisher, R. A. (1936). "The use of multiple measurements in taxonomic problems". Annals of Eugenics.
2. Stevens, S. S. (1946). "On the theory of scales of measurement". Science.
3. UCI Machine Learning Repository: Iris Dataset