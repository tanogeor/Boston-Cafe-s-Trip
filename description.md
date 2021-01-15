## Boston-Cafe-s-Trip
Boston Coffee Shops and the Travelling Salesman

# Introduction
The travelling salesman problem has worried logistics managers and route planners for quite a long time now.
To cite Wikipedia and its respective site: "Given a list of cities and the distances between each pair of cities,
what is the shortest possible route that visits each city exactly once and returns to the origin city?".
In fact, it is a problem of operational research and its solution lies not too far from the traditional method of 
Simplex.

Moreover, the optimization of FTL (Full-Truck-Load) mileage is the key questions to be answered. A set of questions
derive from this. How can the FTL mileage be maximised? Assuming a fleet of two or more trucks is available, what 
is the optimised route for each truck?

But, for reasons of simplicicty, though, this study will focus on minimizing the miles of a truck's full circle
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
A thorough observation of data is necessary to identify possiblie anomalies in it. Neighbourhoods whose coordinates we 
could not get, were dropped.

3. Get Venues
It is needed to get the venues around every Boston neighbourhood, using the Foursquare API again.

4. Clean Venues
All the different venues may address all the different stores and shops of Boston. We need to throw away the ones that 
don't cater to our needs and only keep the ones that refer to Coffee Shops.

5. Route Optimization
Gurobi Optimization offers a great library of Optimization tools for the solution of the Travelling Salesman Problem.
Not only that, but a similar example is readily available at their website.

# Discussion
The Travelling Salesman Problem, as already mentioned, in its simplest form is not one of rather troublesome nature, when
the tools are readily available to a professional. The most difficult parts of this research were the engineering of the problem,
in terms of parameter tuning, data exploration, data cleaning. Further studies can focus on the addition of extra parameters to 
the problem. Fox example, that of a fleet of more than one trucks, or the maximization of mileage of FTL.

# Conclusion
To conclude, the derived resulting map connects all the venues derived for the answering of the question and it is shown in the following 
parts of code and presentation. 
Lastly, combining the abilities of fetching venues and data through the use of a Foursquare API and bringing them to a form of analytical 
understanding through the use of the Gurobi Optimization library is a methodology of great and insightful results. 


