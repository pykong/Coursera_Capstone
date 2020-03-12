# Where do Western city dwellers like to eat out?

A survey into the restaurant landscape of Western metropolitan areas.

## Introduction

The restaurant business is one of the oldest business forms, dating back to ancient times. Its low barrier to entry results in a usually highly competitive business environment.

To gauge potential market opportunities for a big international restaurant chain, we like to quantify the restaurant landscape in five Western countries: US, Canada, Great Britain, France, and Germany.

We are interested in the question of what the most common restaurant types in major cities of those countries are. We also like to draw a relationship between GDP and restaurant type to gauge economic influences on food preferences.

### Identifying new business opportunities

This information might guide the decision of the customer to enter the market in any of those countries, by identifying a potentially unmet need for new food tastes.


## Data Section

-   Basic data on cities like geospatial or economic data is scraped from wikipidia.org.    
-   Geospatial data is supplemented by the use of the [Geocoder Python](https://geocoder.readthedocs.io/index.html) package where needed.
-   Restaurant data will be garnered from [Foursquare's API](https://developer.foursquare.com/).
    
    
## Methodology

A web scraper will retrieve geospatial or economic data for the five most populous cities of each country.
A sample of 500 restaurants for each city is retrieved from Foursquare and joined to the original data frame.

After normalization and cleanup, the ten most common restaurant types per city are garnered.

The findings are visualized in the form of:
-   Bar charts    
-   Word clouds    
-   Regplots for correlating GDP and restaurant preference    
-   Maps where suitable
