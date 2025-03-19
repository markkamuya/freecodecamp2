# Demographic Data Analysis

## Overview

This project performs a demographic analysis on the `adult.data.csv` dataset, containing information about individuals in terms of their age, race, sex, education, occupation, working hours, and salary. The primary goal is to generate key insights into various demographic factors, including the distribution of races, educational background, income levels, and working conditions, with a focus on identifying trends among individuals earning more than 50K annually.

The analysis leverages the `pandas` library for data manipulation and calculation, providing insights such as:

1. **Race distribution** in the dataset.
2. **Average age** of men.
3. **Percentage of individuals** with a Bachelor's degree.
4. **Income distribution** among individuals with higher education versus those without.
5. **Minimum work hours** per week and income trends for individuals working these hours.
6. **Country with the highest percentage of individuals earning more than 50K**.
7. **Top occupations in India** for individuals earning more than 50K.

## Functionality

The script provides a function, `calculate_demographic_data`, which performs the following tasks:

- Reads and loads the data from `adult.data.csv`.
- Calculates the count of individuals for each race.
- Computes the average age of men in the dataset.
- Calculates the percentage of individuals holding a Bachelor's degree.
- Compares the income of individuals with higher education (Bachelor's, Master's, Doctorate) to those without.
- Determines the minimum number of hours worked per week and analyzes income patterns for those working the least hours.
- Identifies the country with the highest percentage of individuals earning more than 50K annually.
- Finds the most popular occupation among individuals earning more than 50K in India.

## Results

Once the function is executed, the following insights are printed:

1. **Race distribution**: A breakdown of the number of individuals belonging to different racial groups.
2. **Average age of men**: The mean age of male participants in the dataset.
3. **Percentage with Bachelor's degrees**: The proportion of individuals holding a Bachelor's degree.
4. **Higher education income**: The percentage of people with higher education earning more than 50K annually.
5. **Lower education income**: The percentage of individuals without higher education earning more than 50K annually.
6. **Minimum work hours**: The least number of hours worked by individuals, along with the percentage of those earning more than 50K.
7. **Top countries with high earners**: The country with the highest percentage of high earners.
8. **Top occupation in India for high earners**: The most common occupation for individuals in India earning more than 50K annually.

## Data Requirements

To run this analysis, the following file is required:

- `adult.data.csv`: This dataset should be present in the working directory. It contains information such as age, sex, race, education, occupation, hours worked per week, and salary.

## How to Use

1. Ensure that you have the required dataset (`adult.data.csv`) in the same directory as the script.
2. Run the script using Python 3.x. The `pandas` library is required, so you will need to install it if you haven't already:

    ```bash
    pip install pandas
    ```

3. After running the script, the function `calculate_demographic_data()` will output the results to the console.

## Sample Output

Here is an example of the output when the function is executed:

```
Number of each race:
 {'White': 27816, 'Black': 3124, 'Asian-Pac-Islander': 1039, 'Amer-Indian-Eskimo': 311, 'Other': 271}
Average age of men: 39.43
Percentage with Bachelors degrees: 16.45%
Percentage with higher education that earn >50K: 46.54%
Percentage without higher education that earn >50K: 17.37%
Min work time: 1 hours/week
Percentage of rich among those who work fewest hours: 0.1%
Country with highest percentage of rich: United-States
Highest percentage of rich people in country: 91.46%
Top occupations in India: Prof-specialty
```
