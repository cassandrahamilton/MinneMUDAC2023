# MinneMUDAC2023
Data competition hosted by MinneAnalytics in coordination with the MN Twins

## Goal
To forecast game attendance at all regular season MLB games in 2023

## Methods
1. Gather historical data from 2012-2022 (around 25K observations)
2. Create several predictive models using training data from 2012-2021 (2020 excluded due to COVID) and with training data from 2022

## Data Gathering
### Sources
- Retrosheet
	- Game by game records (score, roster, day of the week, day/night game)
	- Hall of Fame players
- Ballparks of baseball
	- Ballpark capacities
	- Cost of construction
- Global sports salaries survey 2019
	- Social media followers (instagram, twitter, facebook, other)
- Swish Analytics
	- Hourly weather reports at the stadium (temperature, percipitation, wind speed)
- Baseball Reference
	- World Series winners and runner ups
- Spotrac
	- Yearly salary averages
- Wikipedia
	- Missing stadium statistics

### Variables
There were 40 total variables. The most relevent were the following:
avg payroll, season record, number of players on the field who are now in the Hall of Fame, number of total social media followers, region/league, day of the week, year, day/night game

### Data gathering methods
**Python Webscraper**- used for the weather data. The associated Jupyter notebook is in this repo \
**IA Wayback Machine**- used to find salary information that is no longer publicaly accessible \
**Excel Data from Picture**- used to take a picture of a table and quickly transcribe to numbers 

## Models
The following models were used: XG Boost, PCA Multiple Linear Regression, Regression Tree (JMP), Random Forest

