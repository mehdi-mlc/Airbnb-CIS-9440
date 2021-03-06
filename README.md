# Airbnb CitiBike Revenue Factor
- author(s): Mehdi Lahlou Charki, Ahmmed Hossain, Hojin Lee
- date created: 12/03/2021
- class: CIS 9440

Project Objective: Follow the Kimball Lifecycle to design and develop a public, cloud-based Data Warehouse with a functioning BI Applications

Project Tools:
The tools used to build this Data Warehouse were: (change this to make applicable to your project)
1. For data integration - python
2. For data warehousing - Google BigQuery
3. For Business Intelligence - Tableau

## Kimball Lifecycle Project Stages

### Project Planning

Motivation for project:

We are looking for Airbnb revenue factors generated by CitiBike traffic. Does
a neighborhood containing one or more CitiBike stations make a rental more attractive and
expensive? Where are the most served neighborhoods in terms of citi bike traffic, and do they contribute to higher
attractiveness for airbnb rentals in that area? Analyzing these questions will help Airbnb promote
certain locations more efficiently to generate higher income.

Description of the issues or opportunities the project will address:

We are trying to understand the correlation between revenue of Airbnb listings and the transit data
in regards to CitiBike pick up and drop offs. The opportunity that may arise based
on the findings of this project will allow Airbnb to understand where potentially lucrative short term
rentals are. In turn, Airbnb can promote or incentivize new and/or existing listings in those
respective hot zones.

Project Business or Organization Value:
What’s the Business Value?
Recover revenue lost from the global pandemic by improving customer satisfaction
and promoting listings in regions highly served, and where revenue potential is
heightened.

Data Sources:
1. http://insideairbnb.com/get-the-data.html

2. https://ride.citibikenyc.com/system-data


### Business Requirements Definition

List of Data Warehouse KPI's:
1. Number of citi bike trips per location
2. Total revenue per location
3. Average price a night per location
4. Number of rentals gemerated based on citibike trips per location
5. Average ratings per location

### Dimensional Model

This project's Dimensional Model consists of 1 Facts and 3 Dimensions

![Alt text](https://github.com/mehdi-mlc/Airbnb-CIS-9440/blob/main/Fact%20Table.png)

This project's Kimball Bus Matrix:

![Alt text](https://github.com/mehdi-mlc/Airbnb-CIS-9440/blob/main/bus.png)

### Business Intelligence Design and Development

List of Visualizations for each KPI:
Number of citi bike trips per location
- We will use a treemap to effectively show and compare the number of citi bike trips per location using size and color. We filtered it by using only the top 15 neighborhoods in terms of citi bikes traffic. The size and colors of the rectangles allow the readers to immediately make sense of what they’re seeing, and directly understand which neighborhoods are most visited.

Total Revenue per location
- We will use a scatter plot with two y-axis to easily describe the relationship between the total revenue per neighbourhood and the number of citi bike trips. We filtered it by using only the top 15 neighborhoods in terms of citi bikes traffic. The left y-axis would be the number of citi bike trips and the right y-axis would be the total revenue. This not only gives us the total revenue per most frequented neighborhood, but also explains the revenue’s relationship with the number of citi bike trips.

Average price a night per location
- We will use a scatter plot to show the relationship between two numerical values which are the average price of Airbnb per night and the average citi bike trips. This gives the reader an overview of the price for each zip code, and explains the relationship with the citi bike traffic.

Number of rentals generated based on citi bike trips
- We will also use a scatter plot to show the relationship between the number of rentals and the number of citi bike trips based on the location zip code and neighborhood name. Creating a scatter plot with a trend line makes it easier to understand how the greater the traffic in citi bike, the higher the number of listings will be rented.

Average ratings per location
- We will use a horizontal bar plot to show the average review scores of Airbnb per neighbourhoods in descending order. We filtered it by using only the top 15 neighborhoods in terms of citi bikes traffic. We chose to range the x-axis from 4 to 5 to show clearly the difference in ratings, as all neighborhoods have quite great and close average ratings.

BI Application Wireframe design:

![Alt text](https://github.com/mehdi-mlc/Airbnb-CIS-9440/blob/main/wire.png)

Picture of final Dashboard:

![Alt text](https://github.com/mehdi-mlc/Airbnb-CIS-9440/blob/main/dashboard.png)

### Deployment

The project was deployed on Tableau Public: https://public.tableau.com/app/profile/mehdi.lahlou.charki/viz/Tableaufinalproject_16383659899150/Dashboard1
