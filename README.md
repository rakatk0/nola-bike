
There are three directions this thesis might take. 

## 1. "Site-suitability matrix builder"

```
i want to design a map that explores the changes that have occured in a community

because i think it would be interesting to compare what exists to what existed, and how locals have perceived this change

in order to continue a conversation begun 20 years ago. 
```
```
I want to design a map that allows a commmunity to take an active role in planning their environment 

because I want to find out how communities can be better involved in planning processes

in order to make better places for everyone.
```
```
i want to design a map that allows anyone to design complex site suitability matrices using physical and cultural features 

because I want to empower users to better understand their environment and landscapes 

in order to be a more informed, more involved citizen.   
```

```
i want to design a map that captures and visualizes user input
because I want others to look at data created that represents all voices
so that collaborations are captured
```

```
i want to design an interactive map that visualizes aggregated user input from the above map 
because I want others to share their ideas
in order that everyone has a say.
```

That's 5 maps, and all are significant undertakings, each with their own issues and sensitivities that must be addressed. Isolating one concept or experience

A little background: Many of the ideas for the above maps are rooted in a capstone project completed in Fall 2005 for the UK Department of Landscape Architecture Final capstone.  Utilizing community-generated data, the class developed a preliminary master land use for the county to implement. ![preliminary master plan](/images/gbd3.png "prelim plan")  

Were any of these considerations adopted?  What happened to the plan?  How could the tools utilized in 2005 been enhanced with modern-day webmapping and social media technology?

The above map(s) would tell the story of the community and the 2005 planning process.  Included could be an interactive map of the 2005 proposed plan, as well as interactive analysis of how the community has changed in 15 years. 

Finally, participants could modify their own site suitability maps and explore how different land use planning decisions would affect them at various scales.

In 2005, the site-suitability scenarios were initially generated using raster calculator in ArcGIS.![alt text](/images/gbd2.png "suitability scenario builder") At the community planning meeting, these were presented via posterboard and powerpoint, and participants were handed radio-linked handheld computers within which they would input their preferences to a variety of planning-related questions.  

Recreating this data exporation and collection process via interactive webmap is an exciting concept because of its applicability as a platform at many scales.   

# or

## 2. New Orleans Bicycle Map
```
i want to design exploratory and descriptive interactive maps that increase bicycle safety
because I want others to have greater awareness of their environment when they travel by bike
in order that everyone can be prepared
```

This project would have multiple facets: 
- generate interactive maps of bicycle networks
- explore traffic safety data
- explore city-wide bicycle rental program datasets & generate meaningful insights and data visualizations

Working with Bike Easy, an established non-profit in New Orleans, I would have access to a significant amount of data.  The city-wide bicycle data would be a trove of location data over the past few years of the city-approved bicycle rental network. 

<!-- Bike Easy has mapping assets and other needs for maps. -->

## DATA
Acquired: 


Data would come primarily from a few sources: 
**Existing bicycle infrastructure**: [City of New Orleans Open Data Portal](https://data.nola.gov/Transportation-and-Infrastructure/Bike-Lanes/8npz-j6vy)
regional bicycle layers 

An interactive layered map with custom base map and 


**Bicycling-centric layers**: [Bike Easy NOLA](http://bikeeasy.org/)
- amenities
    - [parking racks/locations](https://data.nola.gov/Transportation-and-Infrastructure/Bicycle-Parking-Locations/atfa-cmev)
    - bike repair stations
    - [bike share stations](https://data.nola.gov/Transportation-and-Infrastructure/Bike-Share-Stations/3het-ycdr)
- transit connections
    - transit stops
    - ferry landings
    - train station
- hazards & conditions
    - [streetlights](https://data.nola.gov/dataset/Streetlights/ut7r-kcda)
    - pavement conditions
    - railroad and streetcar tracks
    - bridges and crossings
    - construction (requires )
        - [DPW](https://www.nola.gov/dpw/projects/all/)
        - [LA DOT]()
- bike shops/resources
- user-added content (requires moderation?)

**Crash Data access?**: [Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

**Blue Bikes Rental Data**: via their partnership with Bike Easy. 

*privacy?* are individuals able to be identified from their trip signature or within the dataset?  
*only subset of total users?* does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs.  What is the typical user of New Orleans bikeshare program? What is the typical New Orleans bicyclist? 
*data rights?



<!-- connection to uber datasets -->

**Post-Katrina mini-summary of New Orleans Bike History**: 

New Orleans is consistently updating their bicycle networks and entities such as Bike Easy have helped advocate for expanded awareness and infrastructure to support the Complete Streets movement. 

Maps could help to explain these efforts to residents, and expand awareness of a variety of factors.  



*data wrangling & analysis methods*: 
R analysis via Todd Schneider? 
data wrangling & analysis

spatial analysis to support decision-making

use bluebike data to figure out *where* to look..
bike network status?
accident history?
streetlight coverage?
correlation to proximity to traffic cameras?

ground-truthing


#### how to explore new orleans bicycling with data analysis?
- flatness?...average grade change on ride vs other cities
- grids .... always a parallel alternative? look at similar trips with different routes...where does this breakout of bike network? 
- rainy, but not cold - look at correlation between rainy days and bluebike usage? rainy days and avoidance of certain roadways/intersections?
- tourist vs local? 
- lotsa parades and festivals...how does that affect biking?




# OR

## Traffic Camera Citations 2008-2019 vs Louisiana Crash Data...maybe?

```
i want to explore a large dataset of citations
because I want to find patterns and correlations with other events
in order to understand the scale and estimate the of such implementations
```

4.5 million tickets were handed out in this time. Many have considered the actions of the city and its contractors to be illegal.  

[NOLA traffic camera citations 2008-2019](https://data.nola.gov/Public-Safety-and-Preparedness/Traffic-Camera-Citations/va3u-jspg)
Crash Data: [Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

Points: 
Camera Locations, zip code centroids
Edges:
neighborhoods

comparisons: 
to traffic history/crash data?


This has been a hot button topic in New Orleans since they were installed over a decade ago.  This dataset has location info for each camera, as well as offender zip code, and time of the offense making for an interesting look at where cars from wherever are speeding when!

This could have an awesome animation and exploration interface, but would get a little boring without a timeline with historical events included, like when speed limits were changed or after notable newsworthy disabling.    













