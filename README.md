# Used-Clustering-to-Analyse-Business-Potential-Area-in-Pune City

# Problem Statement:

Pune, being a major metropolitan city in state of Maharashtra, India is a very fast developing city with plenty of opportunities for business. There are multiple potential business locations in this city. But its very difficult to decide upon the location and category or nature of the business. For someone with capital wanting to invest in or start a business, they must first know which are the areas which have good prospects for the business to run, which is the category of business with most competitors and which category is most probable to failure.
The target audience will be the someone who wants to start a new business of some category and needs to find a location with best prospects.
All this can be found by analyzing the venue data.

*Note:* The business categories will be limited to the Categories of the venues listed by the Foursquare API.

# Understanding the Case:

To start, first thing I need to know is which areas to analyze for this project. I will simply start by selecting few locations across Pune which are more bustling from what I 
know and heard from people. I will also include adjoining city, Pimpri-Chinchwad in my analysis. After selecting and getting coordinates of these areas(using geopy library), it 
will be possible to get the data on Venues from Foursquare.

The data of the venues depends on the search radius specified while requesting from Foursquare. It is very much possible that business venues location overlaps or is duplicate. 
So it needs to be clustered into different locations and named appropriately. Then these clusters can be analyzed separately for best choice of business category or for the 
possibility of success of preferred category.
To further dig and explore more about the area clustered I will use data about location connectivity, nearby banks and ATM's.


# Data Collection:

Data: `Area name/Neighborhood of potential locations` , `Public transport stops`, `ATM locations`,`Bank locations`

Specification: Address of the area, Area name/Neighborhood or stop name, Coordinates, Area name/Neighborhood, Coordinates, Area name/Neighborhood, Coordinates

source: Source: http://opendata.punecorporation.org/Citizen/CitizenDatasets/Indexcsv

other Source: Self decided, Asked people, I might use data for the routes of the bus to show it on map. It will be possible to check how many routes lead to or pass through the 
business locations.

Data format: CSV file

---
# Conclusion:

The analysis and the results are highly dependent on the venues data provided by Foursquare API. The results might not be accurate and be different from what the actual scenario 
is in the real world. The conclusion reached from the analysis although can be accurate if there is more information about venues.

## Analysis of clusters:
Looking at the locations covered by the clusters, it can be said that all the most popular areas for business are covered. The clusters formed are also satisfactory and are 
separated according to how the areas are perceived by people.
From the dataframes showing the top venues in each cluster, the popularity of different categories of business can be seen. The data shows a general trend that Restaurant is the 
category that is found to be popular in many of the areas. The restaurants in these areas either have a unique theme or are a franchisee of a renowned brand.
Other categories like gym, snack places and fast food shops are runner ups in popularity.

## Selecting category of new business:
If the question is - which category of business would be best? There is no category that can be said to be the one having the best prospects. As it was seen that restaurant was 
the category with highest hits, each one of those in the area they are popular in had unique themes or associated with a brand. So having a unique idea for a new restaurant is 
advisable in case you are looking for healthy competition. If one does not want competition, categories having the least number of businesses are a good option.

## Selecting the area and cluster region:
This step should be done after selecting the category. It can be seen that all the areas in each cluster have varying categories. So there is no case where only a particular 
category of business will flourish. Although there are many criteria like capital, nearby residential areas and other things to consider, there is a trend found in the data. 
For e.g. if one plans to open a restaurant, food place or similar categories, the areas under cluster_0 have the most of these categories making competition tough but also 
means good customer base. Similar conclusions can be drawn based on selected categories. Other criteria can be the availability of transport and connectivity. Based on the 
number of bus stops and their location the areas can be shortlisted. The availability of banks and ATMs can also be seen on the map.

