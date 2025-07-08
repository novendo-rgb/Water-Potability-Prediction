# Water-Potability-Prediction
Analyzing and predicting the drinking water potability based on the water quality metrics

## Project Overview
- Performed data cleaning and preprocessing by handling missing values and removing non-feature columns.
- Conducted exploratory data analysis (EDA) to understand the distribution and relationships of both numerical and categorical features in univariate, bivariate, and multivariate analysis.
- The data was prepared for modeling by performing a train-test split and applying feature scaling to normalize the numerical features.
- Built three classification models — SVM (Support Vector Machine), K-NN (K-Nearest Neighbors), and Random Forest — and optimized their parameters using GridSearchCV.
- The best model was selected by evaluating and comparing performance metrics such as the confusion matrix, classification report, and accuracy scores on both training and testing data.

## Dataset
1. The primary dataset used in this project was [water_potability.csv](https://github.com/novendo-rgb/Water-Potability-Prediction/blob/main/Dataset/water_potability.csv), which contains water quality metrics from 3.276 different water bodies. Each entry contains water quality parameters such as pH, Hardness, Solids, Chloramines, Sulfate, Conductivity, Organic Carbon, Trihalomethanes, Turbidity, and a Potability label (1 = safe to drink, 0 = not safe).
2. The dataset is based on a [kaggle_dataset](https://www.kaggle.com/datasets/adityakadiwal/water-potability) by Aditya Kadiwal.

## Data Cleaning
- Data Cleaning is a crucial step to to prepare clean and consistent data before proceeding to the exploratory data analysis (EDA) and model building stages.
- Null values were checked in the dataset. Since there were many missing values, simply removing them could affect the data distribution. Therefore, the distribution of all columns was first examined for skewness, and appropriate imputation methods were chosen accordingly.
- Create the feature list by excluding the non-feature columns.

## EDA
1. Univariate Analysis
   - Performed descriptive statistics using 'df.describe()' separately on features and target to understand their distributions.
   - Distribution plots and boxplots were created to analyze the distribution of each feature and to detect outliers.
   - The categorical target variable was analyzed using a countplot.
2. Bivariate Analysis
   - Created boxplots, violin plots, barplots, and hisplots  to analyze the distribution of the features grouped by the popularity label, as well as to detect outliers.
   - Mutual information was used to quantify the relationship between each feature and the target variable.
3. Multivariate Analysis
   - Created pairplot to explore the relationship between individual features and the water potability.
   - Generated a correlation matrix to examine linear relationships between features and to identify potential multicollinearity.
  
## Model Preparation
   
