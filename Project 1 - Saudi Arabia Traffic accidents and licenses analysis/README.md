# Project 1

Driving Licenses, Traffic Accidents and Casualties Analysis

## Blog post link

[Click me](https://medium.com/@baghlafturki/analyzing-saudi-arabias-driving-licenses-traffic-accidents-and-casualties-2780d226ff6a)

## Prerequisites

This project depends on the libraries below 
- numpy
- pandas
- seaborn
- pyplot
- sklearn
- scipy

## Problem Statment

In 2017, it was estimated that a car accident happens every minute on average in Saudi Arabia. Furthermore, the estimation was considered an improvement when compared to 2016 [Reference](https://stepfeed.com/a-car-crash-happens-every-minute-in-saudi-arabia-3428). As we have access to car traffic accidents data, the primary objective of this project is to link recent incidents or developments to changes of trends in our dataset.


## Executive Summary

In Conclusion, the reduction in annual traffic accidents and casualties could be linked to recent developments in the infrastructure of Saudi Arabia. However, more data is needed to interpret deviant regions.

## Data Dictionary

[Driving Licenses](https://datasource.kapsarc.org/explore/dataset/saudi-arabia-driving-licenses-issued-in-the-kingdom-2004-2008/information/?disjunctive.administritive_area&sort=time_period&location=5,24.37495,45.08024&basemap=jawg.streets)
This dataset contains Saudi Arabia Driving Licenses Issued By Administrative Area for 1993 - 2016. Data from General Authority for Statistics . Follow datasource.kapsarc.org for timely data to advance energy economics research.

[Traffic Accidents and Casualties](https://datasource.kapsarc.org/explore/dataset/saudi-arabia-traffic-accidents-and-casualties-injured-dead-2008/export/?disjunctive.region&disjunctive.indicator&sort=time_period)
This dataset contains Saudi Arabia Traffic Accidents and Casualties by Region for 2016 - 2018. Data from General Authority for Statistics. Follow datasource.kapsarc.org for timely data to advance energy economics research.


|Feature|Type|Dataset|Description|
|---|---|---|---|
|**traffic_year**| int| Traffic_Accidents| The year of the recorded accidents|
|**traffic_region**|object|Traffic_Accidents|The region in which the accedents occured|
|**traffic_indicator**|object|Traffic_Accidents|An extra description regarding the accidents' record|
|**traffic_value**|int|Traffic_Accidents|A number corresponds to the traffic_indicator|
|**traffic_geo_point_2d**|object|Traffic_Accidents|A tuple of latitude and longitude coordinates of the center of the region|
|**traffic_x**|float|Traffic_Accidents|The latitude coordinate of the center of the region|
|**traffic_y**|float|Traffic_Accidents|The longitude coordinate of the center of the region|
|**license_year**|int|Driving_Licenses|The year of the licenses record|
|**license_administritive_area**|object|Driving_Licenses|The admistrative region that issued the licenses|
|**license_amount_issued**|int|Driving_Licenses|The number of driving licenses issued|
|**license_geo_point_2d**|object|Driving_Licenses|A tuple of latitude and longitude coordinates of the center of the region|
|**license_x**|float|Driving_Licenses|The latitude coordinate of the center of the region|
|**license_y**|float|Driving_Licenses|The longitude coordinate of the center of the region|

