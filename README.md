# R Case-Shiller Housing Data Project

Harvard Math23A: Linear Algebra and Real Analysis I

Final Data Project

Fall 2020

Authors: Rudra Barua, Hope Ha, Matti Tan

## Case-Shiller Price Index
Our first data set contains information about how US residential house prices have changed throughout 1987 to 2015. The prices for housing were collected each month of the year from 20 metropolitan regions in the US and were normalised using the Case-Shiller Index. Although this was not done by the group, it might be interesting to know that the Case-Shiller Index is considered to be one of the most reliable measures of the trends for housing prices as it can almost accurately predict the “true appreciated value” of a single quantity of housing.

The link for the data set can be found [here](https://datahub.io/core/house-prices-us).

We performed a Fourier Analysis for 5 cities in this data set using our [Fourier App](https://mattitan.shinyapps.io/FourierRDataProject/).

In this application, we concentrated on 5 cities (New York, Boston, San Francisco, Los Angeles, and Chicago), and, for each city, we graphed the housing price trends in terms of the Case-Shiller Index from the years 2000 to 2015. Using the application, we approximated/reconstructed the graphs which appear to be quasi-periodical functions of time using basis functions of the form cosmx and sinmx.

We also developed a Linear Regression App to model the relationship between individual cities' housing price indices and the national housing price index which can be found [here](https://hopeha.shinyapps.io/RProjectLinReg/).


## Housing Information: California 1990 Census
Our second dataset contained information from the 1990 California Census. The data focused on houses found in a given California district, in relation to its proximity to the ocean, and listed longitude, latitude, the median age of the house, total number of rooms within a block, total number of bedrooms within a block, population residing within a block, the number of households residing within a block, the median income for households within a block, and the median house value for households within a block.

The link for the data set can be found [here](https://www.kaggle.com/camnugent/california-housing-prices).

For this data set, we used the statistical concept of Permutation Tests to test whether the median household income or the median house value was statistically significant in relation with the houses’ location using our [app](https://hopeha.shinyapps.io/RProjectPermTest/).

Also, we used the same dataset concerning California Housing to generate an app which displayed the data in forms of histograms, barplots, box plots, scatterplots, and regression lines: [Displaying Numeric Data](https://hopeha.shinyapps.io/RProjectNumericDisplay/).


## Google Search Trends on Housing Sales
For our final data set, we wanted to analyse large scale data regarding consumer interest in housing. Without a readily available data set, we sought out to scrape our own data, and we used RSelenium, a library to automate web browser actions, to create a tool to scrape data from Google search data from every state in the U.S. (including the District of Columbia) into CSVs. Then, we performed a principal component analysis on interest regarding housing in each state over the past two decades with this [application](https://rudrabarua.shinyapps.io/HousingPCAnalysis/?fbclid=IwAR1tnPnAIaUkQHPLMurhEnCzB3rUl6Q6W_JXZeWwe4SpaaDayF56-o9TgHs).

The [data](https://trends.google.com/) was scraped from Google Trends using RSelenium and cleaned by us in R.
