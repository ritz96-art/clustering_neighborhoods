# Clustering Neighborhoods  
This repository contains a machine learning project where neighborhoods of two major cities NEW YORK and TORONTO were grouped by comparing the most common venue categories in those locations using an unsupervised learning algorithm, **K means clustering.**  
Both cities are very diverse and are the financial capitals of their respective countries, so this clustering alogorithm can be very helpful for those who are searching for places to live in these cities according to their need of facilities in their neighborhoods or those who are shifting from NEW YORK to TORONTO or vice versa to get a similar neighborhood feeling as their current location.  
## Running locally  
1. install jupyterlab and then notebook  
2. Fork this repository  
3. clone your forked repo to your machine  
* git clone https://github.com/ritz96-art/clustering_neighborhoods.git  
4. install dependencies  
* lxml  
* html5lib  
* pandas  
* numpy  
* matplotlib  
* sklearn  
* folium  
* geopy   
## Data Acquisition
  * NEW YORK data set https://cocl.us/new_york_dataset    
  * TORONTO data set https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M  
  * Foursquare API was used to get the venue locations to explore neighbourhoods in New York City and Toronto  
## Data Preprosessing  
  Cities' dataframes were concatenated and the Foursquare API calls were made to get top most 100 important venues of each neighbourhood. The neighborhoods were grouped by their venue categories and the top most 10 common venue categories were selected for each neighbourhood.
  
  final data set  
  ![final data set](https://github.com/ritz96-art/clustering_neighborhoods/blob/master/out/project1.JPG)
## Modelling  
  * K means clustering algorithm was used with any arbitary value of K  
## Data Visualization  
  * clusters of neighbourhoods were marked in map using *folium* library   
  NEW YORK neighborhood cluster map  
  ![](https://github.com/ritz96-art/clustering_neighborhoods/blob/master/out/project2.jpg)  
  TORONTO neighborhood cluster map  
  ![](https://github.com/ritz96-art/clustering_neighborhoods/blob/master/out/project3.jpg)  
