# House Rocket Insights
## Welcome to the House Rocket Data Analysis
![alt text](https://github.com/lfreitas16/Insights-House-Rocket/blob/main/real_estate.jpg?raw=true)
# House Rocket Insights 

## Welcome to the House Rocket Data Analysis

## 1 - Business Problem

### 1.1 - Description

House Rocket is a real estate technology company (fictional) interested in digital innovations to help them buy and sell homes.

The purpose of this project is to create insights through data analysis to help the decision-makers find the best business opportunities in the real estate market of King County. In other words, finding homes below market value in good locations and with good potential for future resale at a higher price.

### 1.2 - Data Overview

The data for our portfolio comes from the official public records of home sales in the King County area, Washington State. The dataset contains 21613 rows. Each represents a home sold from May 2014 through May 2015. Below is a breakdown of the attributes:

id - Unique ID for each home sold
date - Date of the home sale
price - Price of each home sold
bedrooms - Number of bedrooms
bathrooms - Number of bathrooms, where .5 accounts for a room with a toilet but no shower
sqft_living - Square footage of the home interior living space
sqft_lot - Square footage of the land space
floors - Number of floors
waterfront - A dummy variable for whether the home was overlooking the waterfront or not
view - An index from 0 to 4 of how good the view of the property was
condition - An index from 1 to 5 on the condition of the home
grade - An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high quality level of construction and design
sqft_above - The square footage of the interior housing space that is above ground level
sqft_basement - The square footage of the interior housing space that is below ground level
yr_built - The year the home was initially built
yr_renovated - The year of the home’s last renovation
zipcode - What zip code area the home is in
lat - Latitude
long - Longitude
sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors

COLOCAR REFERÊNCIA

## 2 - Business Assumptions

All homes in the dataset considered available for purchase regarding the purchase recommendation report.

To be included in the purchase recommendation report, the home had to be at least as condition 3.

All homes in the dataset considered as owned by the company regarding the sale price calculation.

Seasons of the year considered to affect house prices.

## 3 - Solution Strategy


Step 01. Descriptive Analysis: Analyze each of the columns providing descriptive metrics for each attribute, obtaining a table with a statistical summary of the dataframe.

Step 02. Reverse Geocoding: Get the address using a Geopy tool called Nominatim, which can find the nearest address given the latitude and longitude. Add the following information to each home: road, house number, neighborhood, city, county, and state.

Step 03. Data Visualization: Create different graphs to explore and better understand our data.
Commercial Attributes: Examine the average prices by year of construction, number of bedrooms, and residence type.
Houses Attributes: Examine the concentration of homes by the number of bedrooms, number of bathrooms, number of floors, and waterfront.

Create a map that shows the geographic location of the homes and a visual representation regarding the price and condition.

Step 04. Cloud Application: Build, deploy and run a cloud application where the House Rocket CEO can do the analyses by himself reviewing the company's portfolio. The app will have graphs and a map with an interactive user interface. With the available filters, one can select the data to be shown in tables and graphs. Selection can be made by one or more attributes, by zip code, by maximum price, and so on. A map will show the portfolio density (number of homes) by zip code area.

You can launch the app here:
COLOCAR UM LINK PARA O HEROKU

Step 05. Hypotheses Testing: Discover insights and trends and communicate the findings to the business team. Insights are unexpected discoveries through data.

Step 06. Purchase Recommendation Report:  Group the homes by area (zip code). Calculate the median price within each area. Include in the report homes that are below the median price for each area and that are in good condition (at least 3).

Step 07. Sale Price Report: Create a report listing all homes with a recommended sale price for each one. Group the homes by area (zip code) and by seasons (summer, winter, and so on). Calculate the median price within each area and season.

You can find more information here:
COLOCAR LINK PARA O NOTEBOOK

## 4 - Top 3 Data Insights
Hypothesis 01: Waterfront houses are 30% more expensive, on average.
TRUE: Waterfront houses are 213% more expensive, on average.

Hypothesis 02: Houses built before 1955 are 50% cheaper, on average.
FALSE: Houses built before 1955 are only 1% cheaper, on average.

Hypothesis 03: Houses without a basement are 50% bigger, on average.
FALSE: Houses without a basement are only 23% bigger, on average.

## 5 - Business Results
The sale price was calculated for two situations:
1) If the purchase price is greater than the area median price plus the effect of the season, then the sale price will be equal to the purchase price plus 10%.
2) If the purchase price is lower than the area median price plus the effect of the season, then the sale price will be equal to the purchase price plus 30%.

Sale Conditions
No of Homes
Total Cost (US$)
Sales Revenue (US$)
Profit (US$)
1
10682
4,119,644,414.00
5,355,537,738.20
1,235,893,324.20
2
10931
7,553,280,594.00
8,333,846,174.20
780,565,580.20
Grand Total
21613
11,672,925,008.00
13,689,383,912.40
2,016,458,904.40



You can download the reports here:
ANEXAR AS PLANILHAS

## 6 - Conclusions
The plan was to use data visualization and calculation tools to solve business problems, improving our understanding of the available dataset, for example, which characteristics had the biggest impact on the results.
The findings (insights) will help the business team on closing the best deals in the real estate market.

## 7 - Next Steps to Improve
=> o que deixou de fazer para melhorar

## 8 - Technologies

* Jupyter Notebook
* Heroku
* PyCharm
* Python
* Streamlit


## 9 - Author

Leonardo de Freitas
Aspiring Data Scientist
