<!-- ### **Title** -->
### **New Orleans Bike Map**
<!-- ### **Description of data topic** -->
### ```Description of data topic```

This project would have multiple facets:

- generate interactive maps of bicycle networks, past and present
- explore traffic safety data & generate meaningful insights and data visualizations
- explore city-wide bicycle rental program datasets & generate meaningful insights and data visualizations

Working with Bike Easy, an established non-profit in New Orleans, I would have access to a significant amount of data. The city-wide bicycle data would be a trove of location data over the past few years of the city-approved bicycle rental network.

### *map objectives*

### ```I want to design exploratory and descriptive interactive maps that increase bicycle safety ... because I want others to have greater awareness of their environment when they travel by bike in order that everyone can be prepared.```

### *literature review*
### user needs, articulated through a persona/scenario
### data sources



## DATA STATUS
### **Existing bicycle infrastructure**: 
city maintained lanes - [City of New Orleans Open Data Portal](https://data.nola.gov/Transportation-and-Infrastructure/Bike-Lanes/8npz-j6vy)

[Regional Planning Commission]()
This map currently exists in a pdf format from the RPC's website.  

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



**Collision Data?**: [Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

### spatial analysis
where are most dangerous intersections at what times of day?
is there a streetlight correlation?
is there a bike network correlation? 



## **Bike-Share Program  Data**
### **Blue Bikes Usage Data**: 

Points: Bike Share Hubs

Polygons: Service Area, Other areas

Lines: Routes

As all bikes are gps-tracked, there is alot of route data being generated that could be analyzed for insights. 

- What is average time/distance/speed of trip?
- What are the most trafficked roads? 
- What areas are most underserved by this program?
are there enough bikes/hubs, etc?
- Does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs?  
- What is the typical user of New Orleans bikeshare program?
- What sort of patterns of movement exist around certain neighborhoods and districts, at certain times?

<!-- ** *disclaimer:* This data may not be available.  Access is pending.  Freedom of Information requests may help gain access ** -->
**wrangling and analysis** 
geopandas or d3 version of [Todd Schneider's R analysis]() 


does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs?  
What is the typical user of New Orleans bikeshare program?
What is the typical New Orleans bicyclist?
What sort of patterns of movement exist around certain neighborhoods and districts, at certain times?


use bluebike data to figure out *where* to look..
- bike network status? 
- physical infrastructure 
- accident history?
- streetlight coverage?
- correlation to proximity to traffic cameras?

other connections: integrate 3rd party crowdsource app api via Bike Easy? 


### **Anticipated queries and other data thoughts:**
#### how to explore new orleans bicycling with data analysis?
New Orleans is a mostly flat experience for bicyclists, without much grade change.  
- flatness?...average grade change on ride vs other cities...bring in elevation data to visualize cross sections? 
- compact grids .... always a parallel alternative? A,B,C routes...look at similar trips with different routes...where does this breakout of bike network?
- weather - look at correlation between rainy days and bluebike usage? rainy days and avoidance of certain roadways/intersections? [historic weather data](wunderground.org)
- Bike Betwork users? tourist vs local? where do rides originate and end? can this be determined? 
- Bikeshare area - sufficient?  how many bikes leave the area?  
- lotsa crowds, parades and festivals...how does Mardi Gras affect biking?


<!-- **mini-summary of recent New Orleans Bike History**: 
New Orleans is consistently updating their bicycle networks and entities such as Bike Easy have helped advocate for expanded awareness and infrastructure to support the Complete Streets movement. 

Maps could help to explain these efforts to residents, and expand awareness of a variety of safety factors.   -->




### content and requirements list

Variety of maps and dataset explorations:

bike network map

collision map

bike share routes map 
- could be constrained to just the animation or could show 

**Basemap layers**:
<!-- probably will build this out in mapbox studio -->
- water edge
- curb
- building footprint
- streets w/ bike network

<!-- - identification of anticipated thematic representation (e.g., dot map, choropleth, prop symbols, etc.)
- description of the anticipated user interaction (UI) -->



### wireframes, paper prototypes, or mockups

### Ethics/Critique
**privacy?** 
are individuals able to be identified from their trip signature or within the dataset?
Do users know/care/expect that the bikes are tracked? 






## resources
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

