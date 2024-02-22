# Exploring the Relationship Between Weather Conditions and COVID-19 Rates

## Introduction
In response to the global significance of the COVID-19 pandemic, our research aimed to uncover potential correlations between weather conditions and transmission rates of the virus. Focusing on temperature and geographical location as key variables, we gathered data from major cities across the US, including Los Angeles (CA), Jacksonville (FL), Detroit (MI), New York City (NY), and Houston (TX). The goal was to contribute insights into factors influencing transmission rates and inform strategies for prevention.

## Data Collection and Variables
Our dataset included COVID-19 cases and deaths per date, along with various weather variables such as precipitation, wind speed, dew, and pressure. Additional variables like `new_cases` and `cases_growth` were introduced to account for daily fluctuations and compare transmission rates across different population sizes.

## Accounting for Incubation Period
To address the incubation period, we adjusted the COVID-19 dataset by shifting dates back an average of 5 days, considering the varying incubation periods reported by the CDC.

## Data Splitting for Analysis
To facilitate analysis and model development, we divided the dataset into a 60% training set, 20% validation set, and 20% testing set. This division allowed for effective exploration, model tuning, and final validation.

## Related Works and Literature Review
We drew inspiration from previous studies, including research from the National Library of Medicine and Tomasz Zuk and colleagues, who explored correlations between weather variables and COVID-19 rates.

## Exploratory Data Analysis (EDA)
We conducted extensive exploratory data analysis, including ANOVA tests and TukeyHSD tests, to understand the impact of weather variables on COVID-19 transmission. Outliers were filtered to ensure consistency in our analyses.

## Models and Methods
### ANOVA & TukeyHSD
We applied ANOVA tests to examine the influence of seasons and city locations on temperature variations. TukeyHSD tests were used to identify significant differences, revealing the impact of temperature variations between seasons and locations.

### Logistic Regression
Logistic regression was employed to assess binary variables such as state political affiliation, temperature, and rainfall on COVID-19 growth rates. Graphical analysis was conducted to evaluate the suitability of the logistic regression model.

### Linear Regression
Linear regression was employed to explore potential linear relationships between weather variables and COVID-19 growth rates. However, the analysis did not reveal significant correlations.

### Logarithmic Regression
In an attempt to capture potential logarithmic relationships, we applied logarithmic regression. Despite adjustments, the model failed to identify a significant correlation between weather conditions and COVID-19 transmission.

## Conclusion
While our extensive exploration did not yield significant correlations between weather conditions and COVID-19 transmission using the chosen models and methods, we acknowledge the complexity of the research domain. Further investigations, alternative models, and adjustments, such as averaging data on a weekly basis, may unveil potential correlations. Our research underscores the importance of ongoing studies in understanding the multifaceted dynamics of COVID-19 transmission.

## Sources
- [National Library of Medicine Article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9387066/)
- [US Department of Commerce - Climate](https://www.weather.gov/wrh/Climate?wfo=lox)
- [Literature Review on Temperature and Humidity](https://orf.od.nih.gov/TechnicalResources/Bioenvironmental/Documents/FINALPUBLISHEDPaperonHUMIDITYandViruses509.pdf)
- [University of Manchester Study](https://www.manchester.ac.uk/discover/news/new-study-shows-link-between-weather-and-spread-of-covid-19/)
- [Malki et al., Chaos, solitons, and fractals](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7367008/)
- [Kaggle - Open Datasets and Machine Learning Projects](https://www.kaggle.com/datasets)
- [National Weather Service](https://www.weather.gov/mfl/)
