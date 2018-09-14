# Really Epic Team 05 — Project 1 Proposal


## Project Title:   Econometric Property Investment Calculator (EPIC)

### Team Members: 
- Troy Bailey
- Seth Bitney
- Katarina Pin
- Valerie Wilmot
- Yuta Yamaguchi

### Project Description/Outline:  
We will analyze property values in the greater Austin area as they relate to potential influential factors using heat mapping as the primary visualization form.

### Research Questions to Answer: 
How are property values influenced by different factors such as commute, crime rates, school districts, population density, availability of healthcare resources, variety of restaurant choices, dog ownership, etc.?

### Data Sets to be Used: 
* Zillow
* OpenStreetMap
* City of Austin Census
* US Census Bureau
* School Digger
* Texas School Guide

## Data Acquisition and Cleanup
Started with 40,000 randomly generated coordinates with within a 20 mile radius of the Texas State Capital, then converted to physical addresses classified as residential homes (20,177).  From there, we dropped duplicates and ran addresses through the Zillow API module PyZillow to return values for zEstimate and square footage.  Properties without values were dropped, as well as properties with unreasonable values (e.g. $9M with 1 sqft) resulting in 8,530 unique properties.
![Image of workflow](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/dataDiagramCondensed.png)
We then collected commute times for each address based on census data, crime scores across the area evaluated, and school rating based on the nearest public school to each address. 

## Findings
Heat maps were created for each of the variables evaluated and are shown below.
#### Valuation
Property values were assesed based on value per square foot (zEstimate / square footage).  Results displayed as darker red indicating higher value per square foot.
![Image of value per square foot](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/valueScoreHeatmap.png)
#### Commute Score 
Commute score results displayed where darker blue indicates shorter commute times.
![Image of commute scores](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/commuteScoreHeatmap.png)
#### Safety Score 
Safety score results displayed where darker blue indicates safer areas.
![Image of safety scores](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/safetyScoreHeatmap.png)
#### School Rating 
School rating results displayed where darker blue indicates higher school rating.
![Image of school scores](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/schoolScoreHeatmap.png)

Using the following heat maps, we overlayed the maps to show interactions between valuation and the variables evaluated.
#### Value & Commute Score
![Image of value vs commute](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/valueVsCommute.png)

#### Value & Safety Score
![Image of value vs safety](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/valueVsSafety.png)

#### Value & School Rating
![Image of value vs school](https://github.com/vlarie/EPIC_team5/blob/master/Presentation/Heat%20Maps/valueVsSchools.png)

### Rough Breakdown of Tasks:
- [x] Define questions to ask
- [x] Task management system setup on Trello - Kat
- [x] Assign github owner - Valerie
- [x] Create documentation and setup files - Valerie
- [x] Research different datasets - Troy, Seth, Kat, Yuta, Valerie
- [x] Scheduling time for meetings
- [x] Exploration of data - Troy, Seth, Kat, Yuta, Valerie
- [x] Cleanup of data - Troy, Seth, Kat, Yuta, Valerie
- [x] Analysis of data - Troy, Seth, Kat, Yuta, Valerie
- [x] Create presentation with Google Slides - Kat & Valerie
- [x] Double check presentation requirements - Valerie
- [x] Double check presentation guidelines - Valerie


