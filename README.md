# Denver Traffic Accidents
### Causes, Correlations and Mitigating Factors
*video presentation here*
[Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZDFmOTQwZjctMTUyYS00YjNlLWE3ZmEtYWYwMzZmMTNlYzY2IiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9)
___
## Motivation
After witnessing nearly a dozen accidents at one intersection near my house and hearing myself and my neighbors say "This always happens here!"; I wanted to use my new analytics skill to investigate whether or not certain areas were more prone to accidents, if there were any common causes and what could be done to reduce accident numbers.
_____
### Data Used
- [Traffic Accidents - denvergov.org](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-traffic-accidents)
- [Traffic Signals - denvergov.org](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-traffic-signals)
- [Intelligent Traffic System Devices - denvergov.org](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-intelligent-traffic-system-devices)
- [Liquor Licenses - denvergov.org](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-liquor-licenses)
- [Denver Population - datacommons.org](https://datacommons.org/place/geoId/08031?category=Demographics#Population)

I wanted to use data around police traffic and pedestrian stops but [that data](https://www.denvergov.org/opendata/dataset/city-and-county-of-denver-intelligent-traffic-system-devices) was unavailable at the time of this project.
______
### Methodology
##### Cleaning and Manipulation
- Created a new column (offense_clean) to remove redundant text in the offense_id column.
- Replaced NAN number values with zeros where appropriate
- Created several columns to categorize data by month, year, day and season
- Merge with a zipcode table using geometry
- Used a function to determine minimum distance from traffic lights and cameras for each accident
___
##### Folder Structure and Descriptions

- /notebooks/ - 
    - ..Accidents EDA.ipynb - initial EDA and date manipulations
    - ..Main EDA.ipynb - majority of EDA done here
    - ..Liqour.ipynb - cleaning and manipulation of Liquor License dataset
    - ..Binning Distances.ipynb - creating distance bins for visualizations
- /images/ - images used in Dashboard
- /dashboards/ - Power BI Dashboard
____
### Conclusions
- Efforts to reduces pedestrian and cyclist accidents should continue.
    - This includes protected bike lanes, raised crosswalks and widened sidewalks
- Traffic lights and cameras do seem to have a positive impact on safety when placed in close proximity
- More DUI enforcement is needed, especially in key areas. 

