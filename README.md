# PyBer_analysis
Perform a thorough exploratory analysis to gage an accurate summary of the relationship between city type, number of riders, and number of drivers as well as the total percentage of fares of riders and drivers for each city type.
## Project Overview
#### After accepting a job as a Data Analyst for PyBer, a Python based ride-sharing app company, CEO V. Isualize already has some work that must be done.  She has asked for a thorough statistical analysis to gage an accurate summary of the relationship between city type (urban, suburban adn rural), number of riders, and number of drivers as well as the total percentage of fares for riders and drivers in each city type. The purpose of this analysis was to offer PyBer the information to improve access and affordability of ride share services, especially in underserved neighborhoods.
## Results
#### After completing the exploratory analysis, ride-sharing data was collected on: total rides, total drivers, total fares, average fare per ride, average fare per driver, and total fare by city type.
#### - Total Rides: Total rides for each city type was found by using the 'groupby()' function on "type" and the 'count()' function on "ride ID."
#### <img width="258" alt="Screen Shot 2022-03-27 at 5 09 13 PM" src="https://user-images.githubusercontent.com/99656224/160301145-6ca24d7b-c7dd-4b67-8b7e-5ff6a06972f8.png">
#### - Total Drivers: Total drivers for each city type was found by using the 'groupby()' function on "type" and the 'sum()' function on "driver count."
#### <img width="298" alt="Screen Shot 2022-03-27 at 5 12 24 PM" src="https://user-images.githubusercontent.com/99656224/160301229-450d2a26-09d3-494f-a6cd-3b27232c319b.png">
#### - Total Fares: Total fares for each city type was found by using the 'groupby()' function on "type" and the 'sum()' function on "fare."
#### <img width="236" alt="Screen Shot 2022-03-27 at 5 16 06 PM" src="https://user-images.githubusercontent.com/99656224/160301370-f3c8a177-4b45-40f8-9efe-aa50f64b3bd1.png">
#### - Average Fare per Ride: Average fare per ride for each city type was found by defining "avg_ride_fare" by total fares divided by total rides.
#### <img width="220" alt="Screen Shot 2022-03-27 at 5 17 59 PM" src="https://user-images.githubusercontent.com/99656224/160301468-3cd1a62e-a61b-4f29-a725-82f02fe25afd.png">
#### - Average Fare per Driver: Average fare per driver for each city type was found by defining "avg_driver_fare" by total fares divided by total drivers.
#### <img width="200" alt="Screen Shot 2022-03-27 at 5 18 59 PM" src="https://user-images.githubusercontent.com/99656224/160301478-b365cdf4-11bc-412d-8aaf-44669dd15d47.png">
#### - Total Fare by City Type: Total fare by city type was found by creating a new dataframe with all the data collected above and using the 'groupby()' function on "type" and "date" and the 'sum()' function on "fare."  There was a specific date range that was requested for.  In order to get the sum of total fare by city type each week, the 'resample()' function was used to create a pivot table of the data collected.  A line chart was made from all the data collected for each month and each city type to display the total fare by each city type as seen below: 
#### <img width="600" alt="Screen Shot 2022-03-27 at 5 27 43 PM" src="https://user-images.githubusercontent.com/99656224/160301738-7b545e35-e988-4f40-83dd-90f6df6f198d.png">
