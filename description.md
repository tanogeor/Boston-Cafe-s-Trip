## Boston-Cafe-s-Trip
Boston Coffee Shops and the Travelling Salesman

# Introduction
The travelling salesman problem has worried logistics managers and route planners for quite a long time now.
The optimization of FTL (Full-Truck-Load) mileage is the key questions to be answered.
For reasons of simplicicty, though, this study will focus on minimizing the miles of a truck's full circle
of their delivery points without taking the full truck load aspect into consideration.

Boston is a very vivid metropolis of the state of Massachusetts. Coffee, as in many other cities of the USA, is
loved and worshipped there.

The question derived from the above is: how can a route planner, optimally plan the delivery points of a driver 
so that the distance covered, to pass through its designated coffee shops, is the best possible.

# Data Used
The data used for the answering of the above question is derived from the official site of the data hub of the city of Boston
and is available here: https://data.boston.gov/dataset/boston-neighborhoods/resource/07caa2dd-1499-491e-a1d2-7bcba414cdd7 .
The csv includes all 26 of the Boston neighbourhoods.

# Methodology
To begin, we have the csv with the names of the Boston neighbourhoods and some other features concerning their spatial area 
they cover. A strategic plan of how to proceed is deemed necessary for the project to be complete in time. Below, the steps 
followed and their brief explanation are listed. 

1. Get Coordinates
The first step is to take advantage of the Foursquare API and get the latitude and longtitude coordinates of each
neighbouhood. 

2. Data exploration
A thorough observation of data is necessary to identify possiblie anomalies in it. Neighbourhoods whose coordinates could not we 
could not get, were dropped.

3.




