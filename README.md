FIFA Player Stats Analysis Project
Overview
This project analyzes a FIFA Player Stats dataset to uncover key insights into player attributes and career data. By performing data cleaning, transformations, and exploratory data analysis (EDA), the project provides valuable insights into players' physical and technical attributes, trends, and correlations that can help in understanding player performance and career progression.

Objectives
Understand the Dataset:

Explore the structure, size, and key features of the dataset.
Identify and handle missing values and duplicates.
Data Cleaning and Transformation:

Perform necessary data preprocessing to ensure consistency and accuracy.
Transform specific columns for better usability, such as converting height and weight units.
Exploratory Data Analysis (EDA):

Conduct univariate, bivariate, and multivariate analyses to uncover patterns and relationships among variables.
Use visualizations to highlight player performance trends and distributions.
Dataset
Summary:
Key Features:
Name: Player's name.
Height: Player height (transformed for consistency).
Weight: Player weight (cleaned of extra symbols).
Joined: Date when the player joined a club (converted to datetime).
Various numerical and categorical features representing player skills, attributes, and performance metrics.
Issues Identified:
Missing values in some columns.
Duplicate rows.
Inconsistent data formats (e.g., height in ft, symbols in weight).
Methodology
1. Data Understanding
Explored the dataset using:
shape to determine rows and columns.
columns, head(), and tail() to understand the structure and data.
info() and describe() for data types and statistical summaries.
2. Data Cleaning and Transformation
Missing Values:
Checked missing values using isnull().sum() and addressed them appropriately.
Duplicates:
Detected and removed duplicates using drop_duplicates().
Height Conversion:
Converted height from ft to inches using a calculation for uniformity.
Weight Cleaning:
Removed unwanted symbols from the weight column using str.replace().
Date Column Transformation:
Converted the Joined column to a datetime format using pd.to_datetime() and extracted the year with .dt.year.
3. Exploratory Data Analysis (EDA)
a. Univariate Analysis:
Examined distributions of individual columns like player age, overall rating, height, and weight.
Used histograms, box plots, and bar charts.
b. Bivariate Analysis:
Explored relationships between two variables, such as:
Correlation between age and overall rating.
Relationship between player position and height/weight.
Visualized using scatter plots, heatmaps, and grouped bar charts.
c. Multivariate Analysis:
Explored complex relationships among multiple variables:
Analyzed overall player ratings across positions and years.
Investigated the interplay of player skills (e.g., passing, shooting, dribbling).
Used pair plots and advanced Seaborn visualizations for insights.
