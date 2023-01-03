# fifa-2018-factor-analysis
This code performs factor analysis on a dataset containing soccer statistics from the 2018 FIFA World Cup.

Factor analysis is a statistical method used to identify the underlying structure in a dataset. It is commonly used to identify patterns and reduce the number of variables while still maintaining as much information as possible. Factor analysis can be used in a variety of fields such as psychology, marketing, and finance to understand relationships between variables and to extract meaningful factors from a large and complex dataset.

In this code, factor analysis is applied to a dataset containing soccer statistics from the 2018 FIFA World Cup. The first step in the process is to load and prepare the data by removing non-numeric columns and dropping rows with missing values. The next step is to calculate and visualize the correlation between the variables using a heatmap. It is important to check the correlation between variables because highly correlated variables may be redundant and provide little additional information.

After checking the correlation, an adequacy test called the Kaiser-Meyer-Olkin (KMO) Test is performed to check whether the data is suitable for factor analysis. The KMO test measures the proportion of variance among all the variables that can be traced back to the underlying factors. A KMO value of 0.5 or higher is considered adequate for factor analysis. If the KMO value is inadequate, it may be necessary to revise the list of variables or to consider using a different method.

The number of factors to be extracted is then determined by creating a scree plot and selecting the number of factors where the eigenvalues are greater than 1. Eigenvalues represent the amount of variance explained by each factor and are used to rank the importance of each factor. The larger the eigenvalue, the more important the corresponding factor. A scree plot is a graphical representation of the eigenvalues and helps to visualize the break point between the important and unimportant factors.

Finally, factor analysis is performed using the chosen number of factors and a rotation method called varimax rotation. Varimax rotation maximizes the variance of the loadings (correlations between the factors and the variables) and is often used to improve the interpretability of the factors. The loadings and the variance explained by each factor are then printed.

## Prerequisites
```
Python 3
pandas
seaborn
matplotlib
factor_analyzer
```
## Running the code
```
Download and extract the zip file.
Open a terminal and navigate to the directory where the code is located.
Run the code using the command python factor_analysis.py.
```
## Output
The code will output the loadings and variance explained by each factor.

## Understanding the code
Factor analysis is a statistical method used to identify the underlying structure in a dataset. It is commonly used to identify patterns in large datasets and to reduce the number of variables while still maintaining as much information as possible.

The code first loads and prepares the data by removing non-numeric columns and dropping rows with missing values. It then calculates and visualizes the correlation between the variables using a heatmap.

Next, the code performs an adequacy test called the Kaiser-Meyer-Olkin (KMO) Test to check whether the data is suitable for factor analysis. The KMO test measures the proportion of variance among all the variables that can be traced back to the underlying factors. A KMO value of 0.5 or higher is considered adequate for factor analysis.

The code then determines the number of factors to be extracted by creating a scree plot and selecting the number of factors where the eigenvalues are greater than 1. It then performs factor analysis using the chosen number of factors and a rotation method called varimax rotation, which maximizes the variance of the loadings (correlations between the factors and the variables). Finally, it prints the loadings and the variance explained by each factor.








