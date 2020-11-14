# How Weather Affects The Health of The Saguaro Population at Desert Botanical Garden

## Tip: After reading this introduction, it is recommended that you read the Analysis notebook located in Final/Jupyter Notebooks. If you are interested in seeing the full data clean-up and preparation, check out the data prep notebooks in the same file.

## Thank you
* To the research team at Desert Botanical Garden - staff and volunteers - for the time and energy you have invested in creating this invaluable dataset and for supporting our class project.

## Data analysis team
* Steve Ovsak researched historical weather data sources, obtained and formatted the weather data for analysis, and carried out weather data exploration.
* Steven Rohano's background is in the agricultural industry. He cleaned up and structured the historical saguaro inventory dataset for analysis and debugged the analysis notebook.
* Michael Fahey debugged jupyter notebooks and hosted the GitHub repo.
* Veronica Nixon was responsible for organizing the Saguaro Inventory from 2012 to 2020 as the Garden's GIS Manager. She continues to support the Garden as a volunteer. Her background is in geographic information systems and science and she contributed botanical information to this analysis as well as data prep, analysis, and general project management.

## Introduction
* Desert Botanical Garden (DBG) has conducted an annual Saguaro Inventory since 2012. Every year 20+ volunteers and staff visit each saguaro on the property to assess its condition. Height measurements are taken every 5 years. We obtained the full historical saguaro inventory dataset from DBG and performed basic statistical analyses to look for any patterns or trends in the data. We obtained a daily historical weather dataset and focused this analysis on the affect on weather on the health of the DBG saguaro population.

## Research questions
* Is there a relationship between saguaro mortality and the number of nights above 90 degrees in a year? Cacti cannot "breathe" when the night-time temperature stays above 90, so we would expect to see higher mortality in years with more nights above 90.
* Is there a relationship between saguaro growth rate and precipitation? We would expect to see higher growth rates in the year(s) following a high precipitation year.

## Data
* Historical Saguaro Inventory records were provided by Desert Botanical Garden from https://www.livingcollections.org.
* Weather data was purchased from Visual Crossing: https://www.visualcrossing.com/weather/weather-data-services#/login
* Saguaro and weather datasets were cleaned up and reformated using pandas.
* Mortality_per_year_ready_for_analysis.csv contains the count of how many saguaros were lost in each year of interest.
* GrowthRates_ready_for_analysis.csv contains average annual growth rates for each timespan of interest.
* Nights_above_90_ready_for_analysis.csv contains the count of how many days had a low >= 90 F for each year.
* precip_ready_for_analysis.csv contains average precipitation for each timespan of interest.

## Analysis of saguaro mortality patterns
* Bar plot of saguaro losses each year
* Bar plot of nights above 90 earch year
* Scatter plot of saguaro losses versus nights above 90

## Analysis of saguaro growth rate patterns
* Bar plot of saguaro growth rate per timespan
* Bar plot of average annual precipitation per timespan
* Scatter plot of saguaro growth rate versus average annual precipitation

## Conclusions and Future Work
* The scatterplot backed up the trend we were expecting to find between saguaro mortality and nights above 90. However, the scatterplot of growth rate versus precipitation revealed the opposite of what we were expecting. However, given that the growth rate versus precipitation trend is only based on 2 timespans, we need to wait for more years of data to be collected before the trend can be analyzed statistically. It is also very surprising to see that the growth rate doubled between timespans 1 and 2, particularly given the decrease in mean annual rainfall.

* Due to the difficulty of measuring saguaro heights, they can only be measured every 5 years. Therefore we only had access to two growth rate datapoints. As time passes and more data is collected, it will be interesting to run regression analyses on growth rate-related trends.

* Future work will (hopefully) include Saguaro Inventory 2021 in February!
