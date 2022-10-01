# python-Tableau_Airbnb_share_-economy_or_business_model

# **Project Overview**

## **Business Case**

#### Surrounded by controversy because of the effect of its operations on the housing affodrability, unfair regulations and disputes, Airbnb is a company that since 2008 has positioned itself as one of the strongest leaders in the shared-economy model, especifically in the short-term homestay sector.

#### Even though its precepts can be found in  economical, historical and philosophcal theories from the past, the concept of "shared-economy" has been around for just a few years, but securing terrain by the hand of the communications and technologies development.


#### **Analysis Goal**

#### The interest of this analysis is to know **how is the Airbnb market in the biggest city in the northern hemisphere of the globe**, and in parallel, to unveil if there is a trend that can **show if Airbnb has deviated from the shared-economy model and became another type of business model**.


#### **What better sample for the analysis than the biggest city in the northern hemisphere?**

#### Mexico City is one of the most popular destinations in terms of tourism not only because of it's historical heritage, but also because it has a population of around 9.2 million people in the city, and 9 million more in it's metropolitan area, setting an important base for privates to fulfill a considerable demand, and more than enough information for the analysis.


#### **Data Sourcing, Descritpion & Limitations**

#### The information used for the analysis has been directly scrapped from Airbnb's website by the InsideAibnb initiative (which looks to provide clarity on how Airbnb is negatively disrupting the hotel industry and pushing up the housing prices), and downloaded form their web page ( https://insideairbnb.com).

#### Three data sets containing information on listings, bookings and reviews were cleaned, some variables derived and  merged into a single one with the help of Python. The main dataset  contains variables such as: 

#### - Listings IDs
####- Hosts IDs
#### - Prices
#### - Scores on reviews, cleanliness, communication, value, and location
#### - Number of reviews
#### - Listings count per host
#### - Locations, etc.

#### Though the data is quite complete, it's timeframe is limited to one year, from February 2021 to February 2022; but given the amoun of records, we can still extract important insights from it. 


#### **Understanding the Airbnb market in Mexico City**

#### A good way to understand Airbnb's market in Mexico City is by studying the evolution of the hosts base and average prices thoughout time, and the listings prices distribution.

#### 1. Understanding the evolution of the host base and average prices throughout time 
#### - New Hosts Timeline 2009 - 2022 https://public.tableau.com/app/profile/david.aroche/viz/NewAirbnbHostsinMexicoCityTimeline/NewHostsTimeline2009-2022?publish=yes)
#### In the left timeline it's clear how from 2009 to 2016 the host base exponentially grew, then stabilized  in the following three years, and finally dropped in 2020  as consequence of the COVID-19 pandemic.

#### - Average USD Price Timeline 2009 - 2022 (https://public.tableau.com/app/profile/david.aroche/viz/AverageAirbnbPricesinMexicoCItyTimeline2009-2022/AverageUSDPriceTimeline2009-2022?publish=yes)
#### In the timeline below, we can observe how the exponential grow of the host base regulated the prices from 2009 to 2012, 
and then again when the host base reached its peak in 2016, the prices dropped as consequence of the high competition; also, the jump from 2021 to 2022 may talk about the recovering of the market due to ease of the restrictions on COVID-19.


#### 2. Understanding the prices distribution (https://public.tableau.com/app/profile/david.aroche/viz/PricesHistogramRoomTypeCounts/PricesHistogram?publish=yes)
#### - Average Prices Histogram
#### Another way to evaluate the competition is by studying the prices distribution, which can be seen in the histogram at the bottom-left. You'll notice that the mojority of the listings range in between $10 and $250 USD, which is a symptom of high competition.

#### 3. A linear regression was made to understand how the demand is and predict it (the number of reviews is a way to measure the demand as they are given when a listings are occupied) in terms of listings prices and room types (https://public.tableau.com/app/profile/david.aroche/viz/OccupatinLinearRegression-RoomType/OccupationRelationship?publish=yes).

#### The listings are grouped by room type--the linear regression of the total listings is pretty similar to the entire home regression (the majority of the listings are entire homes). The more competitive the price  the more number of reviews a listings will receive(negative slope), nonetheless, this is not determinant for the regression model as most of the data points are far from the line (low r-squred). A cluster analysis was made for further exploration.

#### 4. Then, a cluster analysis was made to understand the relationships between all of the implicit and emanated varaibles realted to all of the listings in terms of number of reviews (fulfilled demand) and rating scores (offer quality). By looking at the clusters and their distribution along the plot, we corroborated that the competitiveness is high (https://public.tableau.com/app/profile/david.aroche/viz/ListingsClusters-Revs_Num_RatingScore/ListingIDClusters?publish=yes).

#### 5. An important question that drove this analysis is to know if Airbnb has deviated from its original purpose of cooperation based on the  "shared-economy" concept, or if it has evolved(?) into another type of business model swayed by the prevailing economic model.

#### In the bar chart, table and maps contained in the oarenthesis lings at the end, you'll be able to visualize the market share each host has based on the amount the amount of listings and the total number of reviews they have received since they enrolled as Airbnb hosts. At the top-left, there's a table in which you can further explore the same information. Finally, you can explore the  spatial distribution of the listings amount per host in the map below the charts (https://public.tableau.com/app/profile/david.aroche/viz/AirbnbShared-EconomyorBusinessModelTheMexicoCityCase/AirbnbShared-economyorbusinessmodel?publish=yes).


#### ** Additional visualizations**

#### Average Airbnb Prices in Mexico City by Borough 2022 - https://public.tableau.com/app/profile/david.aroche/viz/AverageAirbnbPricesinMexicoCitybyBorough2022/BoroughsAvgPrice2022?publish=yes

#### Room Tye Proportions in Mexico City by Borough - https://public.tableau.com/app/profile/david.aroche/viz/RoomTyeProportionsinMexicoCitybyBorough/ProportionsofRoomTypesbyBorough2022?publish=yes

#### (Top) Hosts in Mexico City by Reviews and Listings Count - https://public.tableau.com/app/profile/david.aroche/viz/TopHostsinMexicoCitybyReviewsandListingsCount/TopHosts?publish=yes

#### Story dashboards:
#### https://public.tableau.com/app/profile/david.aroche/viz/Dash-Intro/Dash-Intro?publish=yes
#### https://public.tableau.com/app/profile/david.aroche/viz/Dash-MotiveData/Dash-MotiveandData?publish=yes
#### https://public.tableau.com/app/profile/david.aroche/viz/Dash-OfferDemand/OfferDemand?publish=yes
#### https://public.tableau.com/app/profile/david.aroche/viz/HostsMarketShare/TopHosts?publish=yes
#### https://public.tableau.com/app/profile/david.aroche/viz/AirbnbShared-EconomyorBusinessModelTheMexicoCityCase/AirbnbShared-economyorbusinessmodel?publish=yes



#### **Fianllym you will be able to find the scripts qith all the required steps and notes for the Wrangling, Cleaning, Analysis and Exports of the Data.**
