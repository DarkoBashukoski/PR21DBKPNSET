# PR21DBKPNSET

Seminar assignment for the subject Data Mining in the Faculty of Computer and Information Science - Ljubljana 2021/2022

## Authors

* Darko Bashukoski
* Kristijan Pucoski
* Nikola Simjanovski
* Edin Tufek

## Dataset Description

The topic we chose to analyze for this project is World Energy Consumption. The dataset we used can be found on Kaggle at the following link: https://www.kaggle.com/pralabhpoudel/world-energy-consumption

The dataset contains information on energy production and consumption for 242 different countries around the world, as well as what kind of fuel is used for the production of energy.
The data spans from the year 1900 until 2020 and contains 122 columns describing each countries energy consumptio and production for many different fuel types like Coal, Oil, Biofuel, Fossil Fuel, Nuclear, as well as renewable sources such as Solar, Wind and Water.
It also contains information about the population of a country for each year so its possible to compare the energy usage per person for each year.
Some of the more important attributes we are going to focus on will be:

`country` - Geographic location

`year` - Year of observation

`population` - Total population

`coal_consumption` - Primary energy consumption from coal, measured in terawatt-hours

`biofuel_consumption` - Primary energy consumption from biofuels, measured in terawatt-hours

`gas_consumption` - Primary energy consumption from gas, measured in terawatt-hours

`hydro_consumption` - Primary energy consumption from hydropower, measured in terawatt-hours

`nuclear_consumption` - Primary energy consumption from nuclear power, measured in terawatt-hours

`solar_consumption` - Primary energy consumption from solar, measured in terawatt-hours

`wind_consumption` - Primary energy consumption from wind, measured in terawatt-hours

`coal_production` - Coal production, measured in terawatt-hours

`gas_production` - Gas production, measured in terawatt-hours

`oil_production`  Oil production, measured in terawatt-hours

Also it is important to note that this data set is very messy and incomplete as not every country uses all forms of energy production, so there are a lot of null values in the data, meaning the data needs to be cleaned and filtered before use.

## Goals and question we would like to answer

With the current events of the world, energy consumption as well as fuel prices are increasing rapidly, so there is a greater need to transition into use of renewable energy sources. We would like to analyze energy consumtion around the world to find out if the trasnition has been started 

With our analysis we would like to answer the following questions:

* How much energy consumption has increased over the years
* Which countries consume the most energy and which ones produce the most
* How does a countries population affect energy consumption
* Which countries are too relient on consumable fuels
* Which countries use the most renewable energy sources and which ones do not
* Has the popularity of renewable energy sources increased over the past years

## Data Filtering

We started by filtering the data by year. The years before 1965 had little to no useful data, and contained large ammounts of empty fields, likely due to inability to accurately collect data at the time. After that from the 122 attributes we had available, we picked around 20 of them which seemed the most useful and separated them into different files for easier access.

## Initial Results

We started simply by inding how much of each energy type was used in the year 2019. From  the results we found that the most used fuel was `fossil fuel` at 130,000 kWh, with renewable fuels like Water, Wind and Solar yielding a total of 16,000 kWh. These results were not great but not far from the expected values. We later checked how much energy usage has increased over the past years and found that on average it increases by 2.5% each year. Both renewable fuel and consumable fuel usage grows at a simmilar rate, with the past 10 years being an acception and renewable fuels are starting to gain popularity. The final more interesting check we did was look  at the corre;ation between energy consumption and ppulation of a country. The results showed a 0.78 correlation between them, meaning they are closely related to each other.
