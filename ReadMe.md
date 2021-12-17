
# Customer Pickup Location Recommender System for NYC Yellow Taxicab Drivers

## Analaysis of Predictability



## Solution

The solution provided here is a recommender system to recommend the best pickup location in a given hour.
The user has to input the hour. Then the program will produce the "best" __borough__ and the __zone__ . 
The best location is based on the __predictability__ of the __drivers' pay__. The higher the __predictability__
the __better__ the location.

The particular steps of finding the best location is as follows.

1. For each trip the __pay rate__ per unit time is calculated.
2. The data is grouped by and graphed by the location using the median __pay rate__.
3. The driver can input a __pay rate__ __threshold__ for which the system will garuntee that as a minimum __pay rate__.
4. From the locations which have higher __pay rates__ than the given __threshold__ a data structure is built for each hour having the *mean squared error* and the *r2 score* for each admissable location.
5. Then when the driver selects the *hour* the system will select the location where the *mse* is minimum in that hour.
6. Alternatively they can select the *hour* where the *r2 score* is at a minimum.




Data csv *yellow_tripdata_2019-01* is moved to project folder.