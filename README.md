# Honda Car Sales Analysis

## Overview

This repository contains the final project for IST 652 - Scripting for Data Analysis. The project involves analyzing Honda car sales data from Cars.com, focusing on various aspects such as pricing, fuel efficiency, and model ratings. The goal is to understand the factors driving car prices, evaluate the changes in fuel efficiency over time, and identify the best deals across different budgets.

## Report Contents

### 1. Introduction

- **Dataset**:
  - The dataset is sourced from Kaggle, featuring Honda car listings from Cars.com. It includes 4,999 rows and 25 columns detailing various attributes like model, year, price, and specifications.
  - Key Variables: Model, Year, Price, Mileage, Transmission, Engine Specifications, Fuel Type, and Ratings.

- **Project Goals**:
  - Identify key components driving car prices.
  - Analyze price differences across states.
  - Evaluate how miles per gallon (MPG) has changed over the years for different models.
  - Determine which models have the best ratings.
  - Find the best deals for various budget ranges.
  - Assess which models have been sold for the most years.

### 2. Data Preparation and Cleaning

- **Data Issues Addressed**:
  - Misaligned columns were shifted to correct positions.
  - Missing transmission data was manually filled using similar configurations.
  - Text and symbols were removed from the price and mileage columns, converting them to integers.
  - Misnamed states were corrected or set to null.
  - Drivetrain options were aligned, and transmission values were standardized.

- **New Variables Created**:
  - **Model Category**: Grouped cars by model, ignoring specific trims and body styles.
  - **Average MPG**: Calculated by averaging the range of MPG values.
  - **Exterior Color Category**: Simplified the dazzling array of color names into basic categories.
  - **Transmission Category**: Streamlined the various transmission descriptions.
  - **Engine Details**: Extracted cylinder size, count, valve count, cams, injection type, hybrid status, and turbo presence using regex.

### 3. Exploratory Data Analysis

- **Initial Insights**:
  - Correlation analysis revealed relationships between price, mileage, year, and various engine features.
  - Price distribution showed a mean near $35,000, ranging from single thousands to over $60,000.
  - Specific engine features like cylinder size and valve count significantly impacted the price.

- **Visualizations**:
  - Plotted distributions and relationships of key variables like price, MPG, and ratings.
  - Examined the impact of drivetrain, fuel type, and engine configuration on car prices.

### 4. Statistical Modeling and Analysis

- **Key Drivers of Price**:
  - Explored how engine components and features drive price points, highlighting the importance of engine size, cylinder count, and fuel injection type.

- **State-wise Price Analysis**:
  - Identified states with the highest and lowest average car prices, with Delaware being the most expensive and Rhode Island the least.

- **Fuel Efficiency Trends**:
  - Analyzed how MPG has evolved over time for different models, noting significant improvements in models like the Accord and Insight.

- **Model Ratings**:
  - Assessed which models have the best overall ratings, with the Pilot and Passport emerging as top performers.

- **Best Deals by Budget**:
  - Identified the best deals for different budget ranges, from under $10,000 to $60,000, with the Civic often being a standout choice.

- **Model Longevity**:
  - Evaluated the duration of models' availability, with the Civic having the longest span and the Clarity the shortest within the dataset.

### 5. Tools and Libraries

- **R Programming**:
  - The analysis and modeling were performed using R, leveraging libraries such as dplyr for data manipulation, ggplot2 for visualizations, and caret for modeling.

## Authors

- Kelsey Kirby
- Sean Deery
- Mark Stiles



## How to Use This Repository

1. **Data Cleaning and Preparation**:
   - Open and run the `honda-car-analysis.ipynb` notebook in Google Colab to load and clean the data. The notebook includes steps for correcting column alignments, filling missing values, and creating new variables for analysis.

2. **Data Exploration and Visualization**:
   - The notebook also contains sections for exploring the dataset and visualizing key relationships between variables. You can generate plots and summary statistics to gain deeper insights into the data.

3. **Model Building and Analysis**:
   - Continue through the notebook to perform statistical modeling and address the key questions posed in the analysis. The notebook includes code for evaluating price drivers, analyzing state-wise trends, assessing fuel efficiency changes, and more.

4. **Review the Full Report**:
   - Access the `homda-cars-report.docx` folder to read the detailed report, which provides comprehensive insights and conclusions based on the analysis.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.





