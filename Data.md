Below is the list of information that will be used

* Stratification data from Bogota: https://datosabiertos.bogota.gov.co/dataset/manzana-estratificacion-bogota-d-c
The previous link gives us a file in geoJSON format that contains all the city blocks and their respective stratum, each block is delimited by a polygon type figure.

* Top 1000 of valuable brands in the world: https://www.value.today/world/world-top-1000-companies


* Top 2000 of valuable brands in the world: https://www.forbes.com/global2000/#5197437e335d

The Project its divided in to parts

PART 1: COMPARE STRATIFICATION WITH POINTS WHERE INTERNATIONAL BRANDS ARE LOCATED

I hope to do this by following the following steps:
  1- Generate DF of places in Bogotá by request to FourSquare.
  2- In which stratum are the international places located? (The stratification JSON map of Bogotá will be used https://datosabierto.bogota.gov.co/dataset/manzana-estratificacion-bogota-d-c) A stratum column is added to the DF.
    3- List of international brands (scraping from https://www.value.today/world/world-top-1000-companies and / or https://www.forbes.com/global2000/#5197437e335d).
  4- From the list of places in Bogotá we only keep the international places.
  
  
PART 2: Clusterization to contrast with stratification

   1- Add to the DF of places in Bogotá a column about your score, number of evaluations for your score, number of comments and the opinion of prices given by the public. The above information will be obtained through requests to FourSquare.
  
  2- Clustering using 6 nodes of the types of places and add their label to the DF of places
  
  3- Classify the 6 clusters according to the grouping characteristics from 1 to 6, with 6 being the best and 1 the worst
  
  4- Obtain graphs in which the results obtained and their respective analysis are evidenced.
