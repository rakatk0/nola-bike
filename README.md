<!-- ### **Title** -->
# **New Orleans Bike Map**
<!-- ### **Description of data topic** -->
## ```Description:```

**What is this?:** 
This project is intended to be series of maps that will overview the bike network and allow for exploration of bike-related datasets of potential interest to the cycling community, public safety officials & policymakers, neighborhood associations and citizens.

#### Maps & Exploratory tools

- generate interactive maps of bicycle networks, past and present in the Greater New Orleans metro area.
- explore traffic safety data & generate meaningful insights and data visualizations
- explore police incident reports for bike-thefts
- exploratory toolset to peruse city-wide bike-share program datasets & generate meaningful insights, communicated through interactive data visualizations. 




## **map objectives**

<!-- ### ```I want to design exploratory and descriptive interactive maps that increase bicycle safety ... because I want others to have greater awareness of their environment when they travel by bike in order that everyone can be prepared.``` -->




<!-- ## **user needs scenario** -->


## **data sources**

#### **Existing bicycle infrastructure**: 
city maintained lanes - [City of New Orleans Open Data Portal](https://data.nola.gov/Transportation-and-Infrastructure/Bike-Lanes/8npz-j6vy)

[Regional Planning Commission]()
This map currently exists in a pdf format from the RPC's website and requires digitization. 

**regional connections** 
[Jefferson Parish Bike Network]()
[St. Bernard Parish Bike Network]()
[St. Tammany Parish Bike Network]()
[Louisiana Bootlace Trail]()

interactive layered map with custom base map

**complete streets map**:
interactive map exploring existing and proposed conditions. Complete Streets is an urban planning initiative that seeks to make streets safer and more friendly to pedestrians and cyclists through various adjustments and interventions in streetscapes.  


**Bike layers**: 

- amenities (points)
    - [parking racks/locations](https://data.nola.gov/Transportation-and-Infrastructure/Bicycle-Parking-Locations/atfa-cmev)
    - bike repair stations 
    - [bike share stations](https://data.nola.gov/Transportation-and-Infrastructure/Bike-Share-Stations/3het-ycdr)
    - bike shops/non-profits
- transit connections (lines)
    - transit stops
    - ferry landings
    - train station
- hazards & conditions (points, lines and polygons)
    - [streetlights](https://data.nola.gov/dataset/Streetlights/ut7r-kcda)
    - pavement conditions
    - railroad and streetcar tracks
    - hazardous bridges and crossings
    - construction alerts
        - [Department of Public Works](https://www.nola.gov/dpw/projects/all/)
        - [Sewer & Water Board]()
        - [LA DOT]()

<!-- *other connections:* integrate 3rd party crowdsource app api via Bike Easy?  -->

**Traffic Incident Data:** 

Source: 
[Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

This dataset is typical of what most states maintain, and can be used to isolate certain types of incidents, such as those involving pedestrians and/or cyclists. 

<!-- access to data is pending -->

where are most dangerous intersections at what times of day?
is there a streetlight correlation?
is there a bike network correlation? 


## **Bike-Share Program  Data**
### **Blue Bikes Usage Data**: 

_Points_: Bike Share Hubs

_Polygons_: Service Area, Other areas

_Lines_: Routes

As all bikes are gps-tracked, there is *alot* of route data being generated that could be analyzed for insights. 

<!-- ** *disclaimer:* This data may not be available.  Access is pending.  Freedom of Information requests may help gain access ** -->

**wrangling and analysis** 
<!-- use bluebike data to figure out *where* to look.. -->

- does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs?  
- What is the typical user of New Orleans bikeshare program?
- What sort of patterns of movement exist around certain neighborhoods and districts, at certain times?
- Bike share network users? tourist vs local? where do rides originate and end? can this be determined? 
- Bikeshare area - sufficient?  how many bikes leave the area?
- are there enough bikes/hubs, etc?
- What is average time/distance/speed of trip?
- What are the most trafficked roads? 
- What areas are most underserved by this program?
- Does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs?  
- What is the typical user of New Orleans bikeshare program?
- What sort of patterns of movement exist around certain neighborhoods and districts, at certain times?
- Ask the crowd: what's the the best way to get upriver/downriver,riverside/lakeside from user's location) 
- look at the beaucoup festivals/parades and impacts of weather and road construction impacts on routes taken could be interesting...



<!-- 
- bike network status? 
- physical infrastructure 
- accident history?
- streetlight coverage?
- correlation to proximity to traffic cameras? 
 -->



### **Anticipated queries and other data thoughts:**
#### how to explore new orleans bicycling with data analysis?

do these datasets characterize the typical new orleans bike network user?  


- flatness?...average grade change on ride vs other cities...bring in elevation data to visualize cross sections? 
- compact grids .... always a parallel alternative? A,B,C routes...look at similar trips with different routes...where does this breakout of bike network?
- weather - look at correlation between rainy days and bluebike usage? rainy days and avoidance of certain roadways/intersections? [historic weather data](wunderground.org)
 
- lotsa crowds, parades and festivals...how does Mardi Gras affect biking?


<!-- **mini-summary of recent New Orleans Bike History**: 
New Orleans is consistently updating their bicycle networks and entities such as Bike Easy have helped advocate for expanded awareness and infrastructure to support the Complete Streets movement. 

Maps could help to explain these efforts to residents, and expand awareness of a variety of safety factors.   -->




### content and requirements list

Variety of maps and dataset explorations:

1. bike network map
- relatively static
- smaller datasets

2. collision map
- will reference a static dataset
- perform analysis browser-side?
- large dataset (>30mb)

3. bike share usage maps 
- parse routes as tracings
- watch animation of routes
- highlight high traffic spots
- potentially very large dataset (>5gb)


### **Technology Stack:**


leaflet
mapbox gl js
mapbox studio

torque.js
turf.js

pySAL - spatial analysis 


hosting: 

**Basemap layers**:
<!-- probably will build this out in mapbox studio -->
- water edge
- curb
- building footprint
- streets w/ bike network

<!-- - identification of anticipated thematic representation (e.g., dot map, choropleth, prop symbols, etc.)
- description of the anticipated user interaction (UI) -->

### wireframes, paper prototypes, or mockups

### **Ethics/Critique**

**Maintaining Privacy** 

Are individuals able to be identified from their trip signature or within the dataset?

Do users know/care/expect that the bikes are tracked? 

The bike share usage dataset could potentially identify individuals or groups and would have to be effectively "scrubbed" prior to any sort of publishing.  Additionally, access to this dataset may require an agreement with data providers as to how the results of any analysis may be presented. 

<!-- review notes w/ dan @ name of 3rd party app developers  -->

**3rd party use of thesis deliverables:**
Access to some datasets will be achieved through leveraging partnerships with local advocacy and planning groups.

If insights inferred from spatial and temporal analysis of datasets can inform decision-making, or be used to determine effectiveness of policy-making (such as, impacts on public health, that would be an ideal outcome of this research and data presentation.

*prominent disclaimer:* use this data and related analysis at your own risk! 


## **literature review**
[Todd Schneider's R Analysis of Citibike Data]()




## Resources



- [bike lanes]()
- [bike share hubs]()
- [bike share service area]()
- [neighborhoods]()

- [City of New Orleans Data Portal]()
- [Bike Easy NOLA](http://bikeeasy.org/)
- [Regional Planning Commission](norpc.org)

- [NOLA traffic camera citations 2008-2019](https://data.nola.gov/Public-Safety-and-Preparedness/Traffic-Camera-Citations/va3u-jspg)


<!-- ## Connection to Traffic Camera Citations 2008-2019?

```
i want to explore a large dataset of citations
because I want to find patterns and correlations with other events
in order to understand the scale and estimate the of such implementations
```

  

Data is ready for a jupyter notebook. 

[NOLA traffic camera citations 2008-2019](https://data.nola.gov/Public-Safety-and-Preparedness/Traffic-Camera-Citations/va3u-jspg)

Crash Data: [Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

Points: Camera Locations, zip code centroids

Edges: neighborhoods

comparisons: to traffic history/crash data?

This has been a hot button topic in New Orleans since they were installed over a decade ago.  This dataset has location info for each camera, as well as offender zip code, and time of the offense making for an interesting look at where cars from wherever are speeding when!

4.5 million tickets were handed out in this time. Many have considered the actions of the city and its contractors to be illegal. -->

