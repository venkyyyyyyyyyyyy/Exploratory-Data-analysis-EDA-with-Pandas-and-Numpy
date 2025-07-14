# Exploratory-Data-analysis-EDA-with-Pandas-and-Numpy
# Import necessary libraries
# import pandas as pd
# import numpy as np
# import matplotlib.pyplot as plt

# Load the dataset
df = pd.read_csv('iris.csv')

# View the first few rows of the dataset
print(df.head())

# Calculate summary statistics
print(df.describe())

# Plot histograms for each variable
for col in df.columns:
plt.hist(df[col])
plt.title(col)
plt.show()

# Calculate correlations between variables
corr_matrix = df.corr()
print(corr_matrix)

# Plot a scatter plot to visualize relationships between variables
plt.scatter(df['sepal_length'], df['sepal_width'])
plt.xlabel('sepal length')
plt.ylabel('sepal Width')
plt.show()
