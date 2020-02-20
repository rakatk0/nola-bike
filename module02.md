```
    The topic and a draft description of your mapping project . This can still be broadly defined, but narrow as much as you can at this point. Include a  potential title for the map or project. This can be changed later but helps your thinking to articulate it in terms of the what, where, when. E.g., "Pedestrian fatalities in London 2016 - 2018. This will likely be the main heading (#) and first subheading (##) within the README.md file.
    Did someone say data? This is the most important part. Provide a description of the state of the data and link to sources. Add data (or examples) within a data/ directory (be careful when committing large (100MB+) files to Git ... use Git LFS (Links to an external site.)). Is it vector or raster data? Think about what the final format for loading into the web map will be: GeoJSON, CSV, a (JSON) request from a PostGreSQL database, a Mapbox Studio tileset, etc.
        Create Jupyter Notebooks and begin loading your data into them for exploration, visualization, and wrangling. Document your data process within them using comments and Markdown cells. Note: the Jupyter Notebooks serve an important role in the MS project defense as they help organize your presentation and provide visual explanation of the data process for your committee.
    An edited and cleaned up README.md file. Either delete or, better yet, move older thoughts and writing to another file in the repo (name it scraps.md or brainstorming.md or something). The README.md file is the landing page for your repo, so keep it clean and readable.

Also, feel free to (optional):

    Rename the repo (something related to your topic ... for instance "lex-foodscape" or "water-politics" ...).
    Begin drafting map objectives and requirements, etc., although I'd prefer for us to spend more time in the coming weeks getting the data solid. 
    Include a basic mockup idea or pencil sketch (these are helpful for thinking!) or links to similar maps/inspiration.
    Invite your fellow classmates to your repo (perhaps just with the "Read" permissions) if you're keeping your repo private for now. I've included your GitHub handles below.
```
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

**Basemap layers**:
<!-- probably will build this out in mapbox studio -->
- water edge
- curb
- building footprint
- streets
- bike network?

**Collision Data?**: [Louisiana Department of Transportation](ladot.gov)
or
[regional planning commission](norpc.org)

hexbin crash analysis
where are most dangerous intersections at what times of day?
is there a streetlight correlation?
is there a bike network correlation? 



## Bike Share Data
### ** Blue Bikes Rental Data**: 

<!-- ** *disclaimer:* This data may not be available.  Access is pending.  Freedom of Information requests may help gain access ** -->
**wrangling and analysis** 
geopandas or d3 version of [Todd Schneider's R analysis]() 

only subset of total users?
does this dataset represent the behavior of all cyclists in new orleans, or just a subset of those using bike share programs?  
What is the typical user of New Orleans bikeshare program?
What is the typical New Orleans bicyclist?
What sort of patterns of movement exist around certain neighborhoods and districts, at certain times?

**privacy?** 
are individuals able to be identified from their trip signature or within the dataset?
Do users know/care/expect that the bikes are tracked? 





**mini-summary of recent New Orleans Bike History**: 
New Orleans is consistently updating their bicycle networks and entities such as Bike Easy have helped advocate for expanded awareness and infrastructure to support the Complete Streets movement. 

Maps could help to explain these efforts to residents, and expand awareness of a variety of safety factors.  




### a content and requirements list, supported by:
- identification of anticipated thematic representation (e.g., dot map, choropleth, prop symbols, etc.)
- description of the anticipated user interaction (UI)
### wireframes, paper prototypes, or mockups
### a statement of ethics or map/data critique




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
- bike network users? tourist vs local? where do rides originate and end? can this be determined? 
- bikeshare area - sufficient?  how many bikes leave the area?  
- lotsa crowds, parades and festivals...how does Mardi Gras affect biking?



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

## resources
- [City of New Orleans Data Portal]()
- [Bike Easy NOLA](http://bikeeasy.org/)
- [Regional Planning Commission](norpc.org)
- [NOLA traffic camera citations 2008-2019](https://data.nola.gov/Public-Safety-and-Preparedness/Traffic-Camera-Citations/va3u-jspg)