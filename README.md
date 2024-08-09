# Business Case Yulu Hypothesis Testing

### Insights:

- Analyzed Yulu's dataset using Python libraries and statistical methods to predict factors influencing demand for electric cycles.  
- Identified a 25% higher bike rental rate on weekdays than weekends, optimizing rental strategies.  
- Achieved a 30% rise in bike rentals on regular workdays over holidays, improving scheduling efficiency.  
- Revealed peak bike rental demand during season 3 (fall) and under clear weather conditions (weather 1), informing operational  planning.

### About Yulu

Yulu is India’s leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting.

Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and convenient!

Yulu has recently suffered considerable dips in its revenues. They have contracted a consulting company to understand the factors on which the demand for these shared electric cycles depends. Specifically, they want to understand the factors affecting the demand for these shared electric cycles in the Indian market.
### [Dataset:](https://github.com/AbhinavTalmale/Business-Case-Yulu-Hypothesis-Testing/tree/main/Dataset)

**Column Profiling:**

-   datetime: datetime
-   season: season (1: spring, 2: summer, 3: fall, 4: winter)
-   holiday: whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
-   workingday: if day is neither weekend nor holiday is 1, otherwise is 0.
-   weather:
    -   1: Clear, Few clouds, partly cloudy, partly cloudy
    -   2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
    -   3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
    -   4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
-   temp: temperature in Celsius
-   atemp: feeling temperature in Celsius
-   humidity: humidity
-   windspeed: wind speed
-   casual: count of casual users
-   registered: count of registered users
-   count: count of total rental bikes including both casual and registered

**Concept Used:**

-   Bi-Variate Analysis
-   2-sample t-test: testing for difference across populations
-   ANNOVA
-   Chi-square