# Analysis of Covid-19 lockdown effects on pollutant concentration levels in Danmarks Plass measuring station in Bergen, Norway.

## Pulling data from their respective APIs
#### Vehicle volume data from https://www.vegvesen.no/trafikkdata/api/
#### Air quality data from https://api.nilu.no/
#### Meteorological data from https://frost.met.no/ (needs personal API key https://frost.met.no/auth/requestCredentials.html)

## Cleaning, tidying and then combining all the datasets by Date (hourly) column. 
#### Traffic data has a "Coverage" metric that gives a rating for data quality. Under 95% coverage hours will be omitted from research as it would undercount the number of vehicles. https://www.vegvesen.no/trafikkdata/start/om-trafikkdata
#### Adding seasonal variables and seasonal dummy variables 

## Creating comparable periods between Lockdown months in 2020 and same weeks/days from previous years of 2017, 2018 and 2019.
#### Omitting holidays as they would have unusually low traffic flow. Omitting weekends due to change in commuting patterns. 
#### Transforming negative values of pollutant concentrations to absolute value over 2.
#### Inspecting the distribution of NAs in pollutant concentrations.

## Summary statistics of hourly data on selected time periods
#### Comparison of Median, SD, IQR, Min, Max, and Coefficient of Variation on pollutant concentration levels and vehicle volume numbers. 

## Visualizations of the data
#### Average hourly pollutant concentration between periods.
#### Mean hourly distribution of vehicle length volumes and pollutant concentration levels.
#### Average daily pollutant concentration comparison between lockdown and pre-lockdown periods.
#### Average daily vehicle volume comparison between lockdown and pre-lockdown periods.

## Statistical tests
#### Linear models of the data with different variables as input.
#### Multicollinearity and autocorrelation present.
