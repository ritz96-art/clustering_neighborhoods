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
## Steps followed in this project  
1. **data acquisition** :
  * source of NEW YORK data https://cocl.us/new_york_dataset    
  * source of TORONTO data https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M  
  * Foursquare API was used to get the venue locations to explore neighbourhoods in New York City and Toronto  
2. **data preprosessing** :  
  * missing data points were handled carefully  
  * these two city’s dataframes were concatenated and the Foursquare API calls were made to get top 100 most important venues of each neighbourhood. The venues were grouped by their categories and finally for each neighbourhood top 10 most common venue categories were selected and the final refined cleaned and ready for future analysis dataset is formed.  
  ![screenshot](project1.jpg)
3. **modelling** :  
  * K means clustering algorithm was used with an assumed K value  
4. **data visualization**  
  * clusters of neighborhoods were marked in map using *folium* library  
5. **result and conclusion**
