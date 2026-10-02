[README.md](https://github.com/user-attachments/files/32712973/README.md)
# Weather Data Project

> The purpose of this project is to compare whether Seattle, WA or Portland, OR is the rainier city.

\---

## Project Overview

* **Objective:** To analyze different measures of 'rain' to determine which city might be 'rainier.'
* **Domain:** Weather
* **Key Techniques:** t-test; z-test

\---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

\---

## Data

* **Source:**

  * https://github.com/brian-fischer/DATA-5100/blob/main/weather/seattle\_rain.csv
  * https://www.ncei.noaa.gov/orders/cdo/4399932.csv
* **Description:** Each dataset contains precipitation values from a single weather station for Seattle and Portland, respectively, between January 1st, 2018 and December 31st, 2022.

\---

## Analysis

Analysis was done through the weather\_data.ipynb notebook. Analysis was all run in order.

The two city data frames were cleaned by selecting only the relevant variables, imputing missing values by using the mean values of similar entries, and combining them into a new data frame: clean\_sea\_pdx\_weather.csv

Using this new data frame, mean precipitation in inches per month and proportion of days per month with measured precipitation were calculated for each city.

A t-test and z-test were done between these new values, respectively, to find any statistically significant differences.

\---

## Results

Mean precipitation per month was comparable between both cities, except for July and August where Portland had significantly less rainfall.

The proportion of rainy days per month had statistically significant differences for eight months, all of which showed that Portland had fewer rainy days per month in those months.

These findings suggest that while Portland has significantly fewer rainy days, those days saw more rainfall on average.

\---

## Authors

* Jacqueline Muse

\---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

\---

## Acknowledgements

* pandas
* numpy
* matplotlib.pyplot
* seaborn

