# Railways-Exploratory-Analysis-and-Dashboard
Expoloratry Analysis of Railway Company Using Python and Tableau

Link to the dashboard in Tableau

https://public.tableau.com/app/profile/maria5911/viz/Railways_Dashboard/PerformanceAnalysisDashboard2

## Project Overview

This project aims to analyze the dataset of National Rail, a company providing services to passengers in the UK. The dataset contains data for January-April 2024. The exploration focuses on the most popular routes, peak travel times, revenue from operations, and on-time performance. 

## Data Source

The dataset is provided by Maven Analytics, the link is as follows: https://maven-datasets.s3.amazonaws.com/UK+Train+Rides/UK+Train+Rides.zip

## Approach

To be able to give a more detailed picture of the company’s operations I decided to present the data on three different dashboards:
-	Routes Analysis
-	Revenue Analysis
-	On-time Performance Analysis

## Data Cleaning and Preparation

The data was well-organized and clean, so only minor tweaks were required. I used Python to prepare the data for future analysis. 
The preparation in Python included changing the type of data for selected columns and creating new columns. The updated dataset was then saved into a CSV file for further work in Tableau. 
The dataset did not include latitude and longitude coordinates for stations, which were required to show the routes on the map in Tableau. Using Tableau instruments the latitude and longitude coordinates were saved into separate text files ‘Origin Stations’ and ‘Destination Stations’, these files were then joined to the main file with data in Tableau.


## Visualization

Tableau was selected as the tool for the main analysis and visualization. I created several calculated fields and added filters and filter actions on the dashboard so the user can manipulate data by selecting required departure or destination points, and periods of operations. 

![] (https://github.com/MariaSozinova/Railways-Exploratory-Analysis-and-Dashboard/blob/main/assets/Route%20Analysis.jpg)

![] (https://github.com/MariaSozinova/Railways-Exploratory-Analysis-and-Dashboard/blob/main/assets/Revenue%20Analysis.jpg)

![] (https://github.com/MariaSozinova/Railways-Exploratory-Analysis-and-Dashboard/blob/main/assets/Performance%20Analysis.jpg)

## Key Findings

1.	The company operated on 64 routes. The most popular route by number of passengers is Manchester-Liverpool and the least popular is Liverpool-Birmingham. The most popular routes suggest potential opportunities for expanding services provided to passengers.
2.	While Manchester-Liverpool route is the most popular in terms of tickets sold, the route from London Kings Cross to York generates the highest revenue. This emphasizes the importance of considering not only passenger volume but also revenue generation when planning the routes and allocating resources. 
3.	For the whole period (January-April 2024) the National Rail transported 29,773 passengers during 19,891 trips.
4.	The peak hours are from 6 am to 7 am, and from 5 pm to 6 pm. The number of passengers is relatively evenly distributed among the days of the week, showing a slightly smaller number on Mondays and Thursdays. Understanding the patterns of peak travel time will allow for better resource allocation. 
5.	There was a decline in revenue in February, but in March and April, the revenue was nearly back to the level of January. 
6.	There are three ticket types: advance, any-time, off-peak. The sales of tickets are nearly the same for all ticket types. 
7.	The revenue from cardholders is only around 23% of total revenue. One of the possible recommendations to the marketing team is to work on promoting various cards and developing reward programs. 
8.	Of all trips, 5.34% were delayed and 3.98% were cancelled. 
9.	The most frequent reason for both delays and cancellations is technical issues. Since they are mainly under the company’s control, it can be recommended to strengthen technical maintenance to avoid further increases in delayed/cancelled trips, which often results in the refunds decreasing revenue.
