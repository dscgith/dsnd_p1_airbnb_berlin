--- 
# Airbnb Berlin: a short analysis on pricing and superhosts

This short data analysis on Airbnb data from Berlin was done as part of the Data Scientist Nanodegree from Udacity

---

### Libraries used
+ Pandas
+ Numpy
+ Matplotlib
+ Seaborn
+ sklearns

Python Version 3.7.9 was used for this project

---

### Motivation
The goal of this project is to get some insight on Airbnb listings in Berlin with a focus on what factors are influencing the price and what makes superhosts and normal hosts different.

---

### Data
The collection of datasets was downloaded from http://insideairbnb.com/get-the-data.html on 20th of march 2021 (data compile date 20th of February 2021):

| filename | file description |
| :-- | :-- |
| listings.csv | Detailed Review Data for listings in Berlin |
| listings_short.csv | Summary information and metrics for listings in Berlin (good for visualisations) |
| calendar.csv | Detailed Calendar Data for listings in Berlin |
| reviews.csv | Detailed Review Data for listings in Berlin |
| reviews_short.csv | Summary Review data and Listing ID (to facilitate time based analytics and visualisations linked to a listing) |
| neighbourhoods.csv | Neighbourhood list for geo filter. Sourced from city or open source GIS files |
| neighbourhoods.geojson | GeoJSON file of neighbourhoods of the city |

Of those files only the listings dataset was analyzed in this notebook.

---

### Results
A short summary of the results from the analysis:
1. How do superhosts compare to standard hosts?
    * Both superhosts and normal hosts come mainly from Germany, while only a small percentage is from other countries like the United States.
    * There is no clear difference visible from the data, that would indicate current superhosts being longer Airbnb users.
    * There is also not a very clear distinction between the locations of superhost listings vs. the locations of listings from normal hosts.
    * Superhosts get slightly better reviews from their guests which is visible in the mean overall rating of 97.2 vs. 93.8.
    * Contrary to what one could expect, the hosts with the most listings are no superhosts. While superhosts have at maximum 44 listings, there are some non superhosts with up to 73 listings.
2. How does the listing location influence the price?
    * The plots show a rather uniform distribution on the 10-300\$ range across the city. For prices over 300\$ however, those listings are more or less focused in the city center region.
3. What other factors influence the price?
    * The most important factors are related to the size of the accomodation. Strong negative correlation can be seen when it comes to sharing space.

---
