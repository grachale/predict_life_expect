# Regression

## Data Source
We will focus on predicting life expectancy in different countries and years. We have training data in the file `data.csv` and evaluation data in the file `evaluation.csv`.

## Feature List
- `Year`: Year
- `Status`: Developed or developing country
- `Life expectancy`: Life expectancy in years (target variable to predict)
- `Adult Mortality`: Adult mortality rate (probability that individuals who have reached the age of 15 will die before reaching the age of 60, per 1,000 individuals)
- `Infant Deaths`: Number of infant deaths per 1,000 population
- `Alcohol`: Alcohol consumption per capita (15+ years) in liters of pure alcohol
- `Percentage Expenditure`: Health expenditure as a percentage of gross domestic product (GDP) per capita (%)
- `Hepatitis B`: Hepatitis B vaccination coverage among 1-year-olds (%)
- `Measles`: Reported cases of measles per 1,000 population
- `BMI`: Average Body Mass Index (BMI) of the entire population
- `Under-Five Deaths`: Number of deaths under five years old per 1,000 population
- `Polio`: Polio immunization coverage among 1-year-olds (%)
- `Total Expenditure`: Government expenditure on health as a percentage of total government expenditure (%)
- `Diphtheria`: DTP3 vaccination coverage among 1-year-olds (%)
- `HIV/AIDS`: Number of deaths due to HIV/AIDS per 1,000 live births (0-4 years)
- `GDP`: Gross Domestic Product per capita (in USD)
- `Population`: Population of the country
- `Thinness 1-19 Years`: Percentage of children aged 10-19 with BMI less than 2 standard deviations below the median
- `Thinness 5-9 Years`: Percentage of children aged 5-9 with BMI less than 2 standard deviations below the median
- `Income Composition of Resources`: Human Development Index based on income composition of resources (index ranging from 0 to 1)
- `Schooling`: Number of years of schooling


## Given Task

1. Load the data from the `data.csv` file into a notebook. Divide it into subsets for training, validation, and testing.
2. Conduct basic data preprocessing:
   - Transform individual features for use in the chosen regression model.
   - Handle missing values appropriately, avoiding methodological errors.
   - Utilize visualizations, providing concise but proper commentary.
3. Create your implementation of a random forest. Use the provided template below.
4. Apply your random forest model to the prepared data, along with one linear regression or ridge regression model and at least one additional model of your choice. For each of these models:
   - Comment on the suitability of the model for the given task.
   - Experiment with normalization (standardization/min-max) if you expect a favorable impact on the model.
   - Select key hyperparameters for tuning and find their optimal values (considering RMSE).
   - Determine the model's error using RMSE and MAE. Beware of methodological errors.
   - Provide thorough commentary on the obtained results.
5. Choose the final model from the tested options in the previous step. Estimate the expected error (RMSE) on new data not previously available. Beware of methodological errors.
6. Load the evaluation data from the `evaluation.csv` file. Use the final model to make predictions for these data. Create a `results.csv` file with three columns: Country, Year, Life expectancy. Submit this file alongside the notebook.

Example of the first rows in the `results.csv` file:
```
Country,Year,Life expectancy
Peru,2012,71.4
Peru,2013,72.6
...
```