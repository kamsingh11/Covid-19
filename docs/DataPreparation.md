### Data Preparation
Missing Values Count:

    iso_code                              64
    continent                            276
    location                               0
    date                                   0
    total_cases                          355
    new_cases                            355
    total_deaths                         355
    new_deaths                           355
    total_cases_per_million              419
    new_cases_per_million                419
    total_deaths_per_million             419
    new_deaths_per_million               419
    new_tests                          23016
    total_tests                        22770
    total_tests_per_thousand           22770
    new_tests_per_thousand             23016
    new_tests_smoothed                 21897
    new_tests_smoothed_per_thousand    21897
    tests_units                        21129
    stringency_index                    6287
    population                            64
    population_density                  1507
    median_age                          3343
    aged_65_older                       3779
    aged_70_older                       3498
    gdp_per_capita                      3709
    extreme_poverty                    13552
    cardiovasc_death_rate               3334
    diabetes_prevalence                 2313
    female_smokers                      9540
    male_smokers                        9826
    handwashing_facilities             19653
    hospital_beds_per_thousand          6064
    life_expectancy                      466
    dtype: int64

* There are a total number of 33417 observations and the following variables have more than 60% of data as missing values. These variables were removed.

`new_tests, total_tests, total_tests_per_thousand, new_tests_per_thousand, new_tests_smoothed, new_tests_smoothed_per_thousand, tests_units`

* The variable `handwashing_facilities` has 19653 close to 60% of data as missing values. These variables were removed.

* The variable `extreme_poverty` is also having 40% of its values as missing values. However, we will try to consider this variable as it has less than 50% of its missing values.

* The below mentioned variables should also be removed as these are conversions per million. We would prefer to use per million numbers in general compared to just numbers, however, there are more missing values in variables using per million as conversions. Therefore, we stick to the original variables.

`total_cases_per_million, new_cases_per_million, total_deaths_per_million, and new_deaths_per_million`

* Total cases should include new cases and total deaths should include new deaths, Therefore, we can remove `new_cases` and `new_deaths` from our data to avoid redundancy.

* Because `population_density` is calculated using Population, we need to remove Population

* Looking at the categorical variables. Some of the rows for `iso_code` has no values and corresponding continent also doesn't have any values. Also, the corresponding location has only "International" as the values. This means there is no way to track which location in these rows belongs to which continent and such. Therefore, we should remove these rows. There are only 64 such rows with no values in iso_code variables. Therefore, removing such a small data will not affect our model.
