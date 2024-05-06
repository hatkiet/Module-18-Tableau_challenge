_(Note)_ To calculate distances between latitude and longitude coordinates using the Haversine formula, which is commonly used to calculate distances between two points on a sphere. I have used assistant from ChatGPT for algorithm to build my code. 

URL to your Tableau Public workbook: https://public.tableau.com/app/profile/kiet.hoang3280/viz/Module_18_challenge_final/Story1?publish=yes 

# Tableau_challenge

![citi-bike-station-bikes](https://github.com/hatkiet/Tableau_challenge/assets/154276115/5e802b4a-9e4d-4038-ba2f-c8819e4992ae)


Congratulations on your new job! As the new lead analyst for the New York Citi BikeLinks to an external site. program, you are now responsible for overseeing the largest bike-sharing program in the United States. In your new role, you will be expected to generate regular reports for city officials looking to publicize and improve the city program.

Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the Citi Bike Data https://www.citibikenyc.com/system-data 

However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have questions about the program, so your first task on the job is to build a set of data reports to provide the answers.

# Instructions

- Your task in this assignment is to aggregate the data found in the Citi Bike Trip History Logs and find two unexpected phenomena.

- Design 2–5 visualizations for each discovered phenomenon (4–10 total). You may work with a timespan of your choosing. Optionally, you can also merge multiple datasets from different periods.

- Use your visualizations (not necessarily all of them) to design a dashboard for each phenomenon. The dashboards should be accompanied by an analysis explaining why the phenomenon may be occurring.

- Create one of the following visualizations for city officials:

**Basic**: A static map that plots all bike stations with a visual indication of the most popular locations to start and end a journey, with zip code data overlaid on top.

**Advanced**: A dynamic map that shows how each station's popularity changes over time (by month and year). Again, with zip code data overlaid on the map.

- The map you choose should also be accompanied by a write-up describing any trends that were noticed during your analysis.

- Create your final presentation: Create a Tableau story that brings together the visualizations, requested maps, and dashboards.

Ensure your presentation is professional, logical, and visually appealing.

# Data Source 

We used CSV files covering June, July, and August 2023. As they contained similar information, they were merged using 'Union' in Tableau or using Pandas to merge. The CSV used in Tableau was combined by Python from the three CSV files, named “JC-202306_08-citibike-tripdata.csv.”

# Dashboards

Four dashboards were designed to visualize and analyze Station, Trip, User, and Map data on a Welcome homepage.

## Homepage 

* This page offers an overview of the project and provides navigation options to access specific pages.

<img width="1020" alt="Screenshot 2024-05-06 at 3 55 09 PM" src="https://github.com/hatkiet/Tableau_challenge/assets/154276115/2ffcfc94-363f-42f9-9a71-07cc21879b71">

## Station Information 

* This report includes data on the total number of bikes used, the total trip duration, and the cumulative number of start and end stations for bike rides. It also provides an analysis of the most popular stations to start and end a journey. Additionally, you can view the distance traveled by different bikes at each station.

* After analyzing the data, it appears that there are more end stations than start stations.
* The bubble chart displays the top ten start and end stations. It is evident that the most commonly used stations for starting and ending trips are South Waterfront Walkway - Sinatra Dr & 1 St to South Waterfront Walkway - Sinatra Dr & 1 St 0, with a total of 1,626 trips.
* The chart shows that 'Average Distance Traveled' steadily rose in June-August. This could be due to hot weather and no snow limiting bike trips.
* According to the data, classic bikes have traveled a greater total distance than the other two types of bikes.

<img width="1000" alt="Screenshot 2024-05-06 at 3 55 22 PM" src="https://github.com/hatkiet/Tableau_challenge/assets/154276115/f0bce1f0-8b23-4e47-8979-0ed37966b930">

## Trip Information 

* This display shows the bike usage by day of the week and bike type over a three-month period.
  
* Bike usage increased every month and is more frequent on weekdays than weekends. Wednesdays and Thursdays are the most frequently used days, and Saturdays are the least, except in July. Stations are conveniently located near homes and offices. Bike usage increased by 35.49% in August.

* Classic bikes were used more frequently than other types. Electric bikes may need charging, and docked bikes may have usage time limitations.

<img width="1028" alt="Screenshot 2024-05-06 at 3 55 33 PM" src="https://github.com/hatkiet/Tableau_challenge/assets/154276115/20967338-c75d-4988-bdb0-0cadfd174f2b">

## User Information 

* Presents a heatmap indicating bike usage by weekday and time of day, as well as member status information. 

* The data for three months shows that bike stations are busiest on Thursdays at 6 pm with a total of 5,311 trips. Generally, weekdays between 5 pm and 6 pm are the most popular times for bike usage. This is likely because people finish work and school around this time and use bikes to get to other destinations. Additionally, it is also quite busy at 8 am on weekdays, which further supports the hypothesis that bikes may be used for commuting to work or school.

* It appears that there are more Citi Bike program members who use the service compared to casual riders, and the number of members has increased from June to August. This trend may indicate that more people are relying on Citi Bike for their daily commutes. Although casual riders tend to take longer trips measured in minutes, this may simply imply that members are faster riders who require less time to reach their destinations.

<img width="1003" alt="Screenshot 2024-05-06 at 3 55 43 PM" src="https://github.com/hatkiet/Tableau_challenge/assets/154276115/60af93d4-e8e1-442c-9a8f-3f3099f22524">

## Map 

* Includes the geographical locations of start and end stations. 

* These maps present the collection of start and end stations for June, July, and August 2023. The most frequently used stations are concentrated in the zip codes 07302 and 07030. This shows that residents of Jersey City rely on the bike-sharing service based on its cost-effectiveness compared to other modes of transportation. 

<img width="998" alt="Screenshot 2024-05-06 at 3 55 53 PM" src="https://github.com/hatkiet/Tableau_challenge/assets/154276115/f937160d-bf4d-473e-99a0-eee937dea1e6">

## Conclusion 

This Tableau analysis gives a brief overview of the trends and patterns in Citi Bike usage over the recent three months. One insightful phenomenon observed is the high reliance on bikes by residents of Jersey City, New Jersey, especially during weekdays during rush hours. This gathered information serves as a valuable resource for further research on Citi Bike. 

