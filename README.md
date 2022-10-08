# Tom_Portfolio

Data Analysis


## [Project 1: June 2022 Oil Price Analysis](https://github.com/jaffacakes2323/oil_price_scraping)

### Collecting Data
- [Downloaded data from Kaggle for analysis](https://www.kaggle.com/datasets/zusmani/petrolgas-prices-worldwide)
- [Scraped extra data for further anaylsis on Oil production and country populations](https://www.worldometers.info/oil/oil-production-by-country/)
- Program built in PyCharm for scraping data
  - BeautifulSoup & Pandas used
- New data combined with old, then saved as a new CSV [New_Oil_Dataset(20.06.2022).csv](https://github.com/jaffacakes2323/oil_price_scraping/blob/main/New_Oil_Dataset(20.06.2022).csv)

### Data wrangling
- CSV opened in Excel
- Most data had already been cleaned
- New rows with formulas & Flash Fill added for GBP
- Altered some spelling (e.g Liter > Litre) and udpated headers with PROPER function
- TRIM function for unwanted spaces
- Format column types (Currency, numeric commas etc.)
- Replace null values
- Added normalised row (simple feature scaling) for population and yearly oil consumption
- Insert Table & PivotTable (new sheet)
- Added specific columnns for PivotTable, and applied some conditional formatting to highlight areas of interest
![](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/oil_pivot.png)

### Analysis and Visualisation
- First thing to notice when looking at the PivotTable, is out of the top 30 of highest oil producing countries, 15 of these are part of the lowest 20% regarding price per litre. Which you would except from the top producing countries. However, 3 of the top 5 would appear to have a relatively high price in comparison (US, China and Russia). This is likely down to the high consumption per capita and other political influences. 

![Screenshot 1](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/oil_consumption_2.png)
![Screenshot 2](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/oil_production.png)

- The below pie chart shows that, out of the top 10 oil producing countries, the US, Saudia Arabia and Russia are the biggest contirbutors by a considerable amount (58% of total top 10 production).
![Screenshot 3](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/oil_production_pie.png)
![Screenshot 4](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/population_oilconsumption.png)

- Created a column chart to show the top 25 populated countries alongside oil consumption. Again the US stands out here with a much higher consumption rate in compared with population. Created a similar column chart whilst fitering by consmption instead, provides another angle. There are further coutries here that show a higher consumption raite in proportion to their population (Japan, Russia, Saudi Arabia, South Korea...). 

![Screenshot 5](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/population_oilconsumption.png)

The below combo chart helps explore usage per capita further. I was suprised to see the US outside of the top 10, considering their overal usage. Singapore is definitely an outlier here, at least doubling all other yearly litres per capita. 7 of these top 10 countries have a much smaller land mass, which is a major point of interest and inspires further invesitagation. What causes these smaller countries to be consuming more per capita? Is this politically, ecenomically or cultrally influenced? This also poses the question of whether the data source is trustworthy, and if the information is accurate.

![Screenshot 6](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/litres_per_capita_by_price.png)

The final 2 graphs help visualise the countries with the highest and lowest prices per litre. North Korea having a 10 times higher price than the average (£1.25 per litre). Clearly a result of heavy sanctions and limited sources.

![Screenshot 7](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/highest_price.png)

Below shows a combo graph for the coutries with the lowest price per litre (line), and their production rates, to see if there is a strong correlation with price and production. However, whilst there are some high producing countries here with low prices (Saudi Arabia in particular), there is no clear relationship, as some of the coutnries with the lowest pricest, also have a low contribution in terms of production.

![Screenshot 8](https://github.com/jaffacakes2323/Tom_Portfolio/blob/main/images/lowest_price_production.png)
